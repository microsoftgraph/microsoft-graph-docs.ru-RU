# <a name="get-started-with-microsoft-graph-in-a-ruby-on-rails-app"></a>Начало работы с Microsoft Graph в приложении Ruby on Rails

В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из конечной точки Azure AD версии 2.0 и вызвать Microsoft Graph. В ней описывается создание [приложения Microsoft Graph Ruby on Rails Connect](https://github.com/microsoftgraph/ruby-connect-rest-sample) и рассматриваются основные понятия, которые необходимо реализовать для использования Microsoft Graph. Кроме того, в этой статье рассказывается, как получить доступ к Microsoft Graph с помощью прямых вызовов REST.

Скачать вариант этого примера, использующий конечную точку Azure AD, можно на странице [приложения Microsoft Graph Ruby on Rails Connect](https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth).

На приведенном ниже рисунке показано создаваемое приложение. 

![Снимок экрана с приложением Microsoft Ruby on Rails Connect](./images/Microsoft-Graph-Ruby-Connect-UI.png)

**Не хотите создавать приложение?** Вы можете быстро приступить к работе с помощью [краткого руководства по Microsoft Graph](https://graph.microsoft.io/en-us/getting-started) или скачать [пример Ruby REST Connect](https://github.com/microsoftgraph/ruby-connect-rest-sample), который рассматривается в этой статье.


## <a name="prerequisites"></a>Необходимые компоненты

Чтобы приступить к работе, вам понадобится следующее: 

- Ruby 2.1 для запуска приложения на сервере разработки.
- платформа Rails (пример протестирован на платформе Rails 4.2);
- диспетчер зависимостей Bundler;
- Интерфейс веб-сервера для Ruby (Rack).
- [Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](http://dev.office.com/devprogram).
- Начальный проект приложения Ruby on Rails, подключающегося с использованием Microsoft Graph. Скачайте [приложение Microsoft Graph Ruby on Rails Connect](https://github.com/microsoftgraph/ruby-connect-rest-sample). Начальный проект находится в папке _starter_.


## <a name="register-the-application"></a>Регистрация приложения

Зарегистрируйте приложение на портале регистрации приложений (Майкрософт). При этом будут созданы идентификатор и секрет клиента, с помощью которых вы настроите приложение для проверки подлинности.

1. Войдите на [портал регистрации приложений Майкрософт](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.

2. Нажмите кнопку **Добавить приложение**.

3. Введите имя приложения и нажмите кнопку **Создать приложение**.

    Откроется страница регистрации со свойствами приложения.

4. Скопируйте идентификатор приложения. Это уникальный идентификатор приложения.

5. В разделе **Секреты приложения** нажмите кнопку **Создать новый пароль**. Скопируйте секрет приложения из диалогового окна **Новый пароль создан**.

    Идентификатор и секрет приложения используются для его настройки.

6. В разделе **Платформы** нажмите **Добавление платформы** > **Интернет**.

7. Установите флажок **Разрешить неявный поток** и введите URI перенаправления *http://localhost:3000/auth/microsoft_v2_auth/callback*.

    Параметр "Разрешить неявный поток" включает гибридный поток OpenID Connect. Благодаря этому при проверке подлинности приложение может получить данные для входа (id_token) и артефакты (в данном случае — код авторизации), с помощью которых оно может получить маркер доступа.

    URI перенаправления *http://localhost:3000/auth/microsoft_v2_auth/callback* — это значение, которое ПО промежуточного слоя OmniAuth использует после обработки запроса на проверку подлинности.

8. Нажмите кнопку **Сохранить**.

## <a name="configure-the-project"></a>Настройка проекта

1. Скачайте или клонируйте [приложение Microsoft Graph Ruby on Rails Connect](https://github.com/microsoftgraph/ruby-connect-rest-sample). Откройте папку _starter_ в любом редакторе.
1. Если у вас еще нет Bundler и Rack, их можно установить с помощью приведенной ниже команды.

    ```
    gem install bundler rack
    ```
2. В файле config/environment.rb выполните указанные ниже действия.
    - Замените текст *ENTER_YOUR_CLIENT_ID* на идентификатор клиента для зарегистрированного приложения.
    - Замените текст *ENTER_YOUR_SECRET* на ключ для зарегистрированного приложения.

3. Установите приложение Rails и зависимости с помощью приведенной ниже команды.

    ```
    bundle install
    ```

## <a name="authenticate-the-user-and-get-an-access-token"></a>Проверка подлинности пользователя и получение маркера доступа

В этом приложении используется поток предоставления кода авторизации с делегированным удостоверением пользователя. В веб-приложении для этого потока требуются идентификатор, секрет и URI перенаправления зарегистрированного приложения. 

Поток проверки подлинности можно разделить на следующие основные этапы:

1. Перенаправление пользователя для проверки подлинности и согласия
2. Получение кода авторизации
3. Обмен кода авторизации на маркер доступа

>Дополнительные сведения об этом потоке проверки подлинности см. в разделе [Из веб-приложения в веб-интерфейс API](https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api) и примере [Интеграция удостоверения Майкрософт и Microsoft Graph в веб-приложения с помощью OpenID Connect](https://azure.microsoft.com/en-us/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/) в документации по Azure AD.

Мы будем использовать три элемента ПО промежуточного слоя [Rack](http://rack.github.io/), чтобы приложение поддерживало проверку подлинности с помощью Microsoft Graph:

- [OmniAuth](https://rubygems.org/gems/omniauth), обобщенная платформа Rack для проверки подлинности с использованием нескольких поставщиков.
- [Omniauth-oauth2](https://rubygems.org/gems/omniauth-oauth2), абстрактная стратегия OAuth2 для OmniAuth. 
- omniauth-microsoft_v2_auth, стратегия OmniAuth, настраивающая Omniauth-oauth2 для явной проверки подлинности с использованием конечной точки Azure AD версии 2.0. Этот проект включен в пример кода.

### <a name="specify-gem-dependencies-for-authentication"></a>Указание необходимых gem-пакетов для проверки подлинности

В Gemfile раскомментируйте перечисленные ниже gem-пакеты, чтобы добавить их в качестве зависимостей.

    ```
    gem 'omniauth'
    gem 'omniauth-oauth2'
    gem 'omniauth-microsoft_v2_auth', path: './omniauth-microsoft_v2_auth'
    ```

Обратите внимание, что стратегия `omniauth-microsoft_v2_auth` включена в проект приложения и будет установлена из указанного пути. 

### <a name="configure-the-authentication-middleware"></a>Настройка ПО промежуточного слоя для проверки подлинности

В файле `config/initializers/omniauth-microsoft_v2_auth.rb` раскомментируйте приведенные ниже строки.

    ```
    Rails.application.config.middleware.use OmniAuth::Builder do
      provider :microsoft_v2_auth,
      ENV['CLIENT_ID'],
      ENV['CLIENT_SECRET'],
      :scope => ENV['SCOPE']
    end
    ```
Это необходимо для настройки ПО промежуточного слоя OmniAuth, в частности для указания идентификатора и секрета приложения, а также запрашиваемых областей разрешений. Это значения, которые вы указали ранее в файле `config/environment.rb`.

### <a name="specify-routes-for-authentication"></a>Указание маршрутов для проверки подлинности

Теперь нам необходимо указать два маршрута для потока проверки подлинности. Первый маршрут пересылает запрос проверки подлинности в ПО промежуточного слоя OmniAuth, а второй задает расположение в приложении для перенаправления OmniAuth после проверки подлинности.

В файле `config/routes.rb` раскомментируйте указанную ниже директиву маршрута.

    get '/login', to: 'pages#login'

При этом запросы на вход направляются методу `login` контроллера страниц, который, в свою очередь, перенаправляет запрос в ПО промежуточного слоя omniauth-microsoft_v2_auth.

    def login
        redirect_to '/auth/microsoft_v2_auth'
    end

Затем необходимо указать, на какую страницу приложения будет переходить OmniAuth после проверки подлинности. Раскомментируйте приведенный ниже маршрут.

    match '/auth/:provider/callback', to: 'pages#callback', via: [:get, :post]

Завершив проверку подлинности пользователя, OmniAuth вызывает URL-адрес перенаправления, указанный при регистрации приложения (в данном случае — *http://localhost:3000/auth/microsoft_v2_auth/callback*). Приведенный выше шаблон маршрута соответствует этому URL-адресу, поэтому запрос направляется методу `callback` контроллера страниц.

### <a name="get-an-access-token"></a>Получение маркера доступа

Теперь мы добавим код, который запускает проверку подлинности и получает маркер доступа, когда пользователь выполнит вход.

Изучите `app/views/pages/index.html.erb`, представление для корневого каталога сайта. Это представление содержит одну кнопку, с помощью которой пользователь может выполнить вход.

    <button class="ms-Button" onclick="window.location.href = '/login'">
        <span class="ms-Button-label"><%= t('connect_button') %></span>
    </button>

Как показано выше, метод входа выполняет перенаправление в ПО промежуточного слоя OmniAuth, для которого настроены идентификатор и секрет клиента, а также запрашиваемые области разрешений. После успешной проверки подлинности пользователя OmniAuth возвращает приложению хэш с маркером доступа и другими сведениями о пользователе.

Теперь добавим код для обработки обратного вызова OmniAuth и получения сведений из хэша. 

В файле `app/controllers/pages_controller.rb` замените пустой метод `callback` приведенным ниже кодом.

    ```
    def callback
        # Access the authentication hash for omniauth
        # and extract the auth token, user name, and email
        data = request.env['omniauth.auth']
    
        @email = data[:extra][:raw_info][:userPrincipalName]
        @name = data[:extra][:raw_info][:displayName]

        # Associate token/user values to the session
        session[:access_token] = data['credentials']['token']
        session[:name] = @name
        session[:email] = @email
        
        # Debug logging
        logger.info "Name: #{@name}"
        logger.info "Email: #{@email}"
        logger.info "[callback] - Access token: #{session[:access_token]}"
    end

    ```

Этот метод извлекает хэш проверки подлинности, а затем сохраняет маркер доступа, имя пользователя и электронный адрес в текущем сеансе.

> **Примечание.** Простые процедуры проверки подлинности и обработки маркеров в этом проекте представлены исключительно в качестве примера. Скорее всего, в рабочем приложении вы реализуете более надежную процедуру проверки подлинности, включающую безопасную обработку и обновление маркеров.

## <a name="call-microsoft-graph"></a>Вызов Microsoft Graph

Теперь вы готовы добавить код для вызова Microsoft Graph. 

Представление, отображаемое с помощью метода `callback` (`app/views/pages/callback.html.erb`) содержит простую форму с одной кнопкой. Форма отправляет данные в `send_mail` и содержит один параметр — электронный адрес получателя.
    
    ``` 
    <form action="../../send_mail" method="post">
      <div class="ms-Grid-col ms-u-mdPush1 ms-u-md9 ms-u-lgPush1 ms-u-lg6">
        ...
            <div class="ms-TextField">
               <input class="ms-TextField-field" name="specified_email" value="<%= @email %>">
            </div>
            <button class="ms-Button">
            <span class="ms-Button-label"><i class="ms-Icon ms-Icon--mail" aria-hidden="true"></i><%= t('send_mail_button') %></span>
            </button> 
        ...
    ```

В файле `app/controllers/pages_controller.rb` замените пустой метод `send_mail` приведенным ниже кодом.

    ```
    def send_mail
        logger.debug "[send_mail] - Access token: #{session[:access_token]}"
        
        # Used in the template
        @name = session[:name]
        @email = params[:specified_email]
        @recipient = params[:specified_email]
        @mail_sent = false
        
        send_mail_endpoint = URI("#{GRAPH_RESOURCE}#{SENDMAIL_ENDPOINT}")
        content_type = CONTENT_TYPE
        http = Net::HTTP.new(send_mail_endpoint.host, send_mail_endpoint.port)
        http.use_ssl = true
        
        # If you want to use a sniffer tool, like Fiddler, to see the request
        # you might need to add this line to tell the engine not to verify the
        # certificate or you might see a "certificate verify failed" error
        # http.verify_mode = OpenSSL::SSL::VERIFY_NONE
        
        email_body = File.read('app/assets/MailTemplate.html')
        email_body.sub! '{given_name}', @name
        email_subject = t('email_subject')
        
        logger.debug email_body
    
        email_message = "{
            Message: {
            Subject: '#{email_subject}',
            Body: {
                ContentType: 'HTML',
                Content: '#{email_body}'
            },
            ToRecipients: [
                {
                    EmailAddress: {
                        Address: '#{@recipient}'
                    }
                }
            ]
            },
            SaveToSentItems: true
            }"
            
        response = http.post(
            SENDMAIL_ENDPOINT,
            email_message,
            'Authorization' => "Bearer #{session[:access_token]}",
            'Content-Type' => content_type
        )
        
        logger.debug "Code: #{response.code}"
        logger.debug "Message: #{response.message}"
        
        # The send mail endpoint returns a 202 - Accepted code on success
        if response.code == '202'
            @mail_sent = true
        else
            @mail_sent = false
            flash[:httpError] = "#{response.code} - #{response.message}"
        end
        
        render 'callback'
    end
    ```

Этот код создает HTTP-запрос, форматирует электронное сообщение, а затем вызывает Microsoft Graph для отправки сообщения.

Чтобы создать сообщение, код извлекает имя пользователя из маркера сеанса и электронный адрес получателя из параметров, переданных формой. Затем код считывает текст сообщения из включенного в проект шаблона, интерполирует имя пользователя и электронный адрес и добавляет текст сообщения в текст HTTP-запроса.

Чтобы отправить сообщение, код создает HTTP-запрос, добавляет маркер доступа в качестве заголовка авторизации, а затем отправляет запрос конечной точке отправки почты.

Наконец, код использует возвращенный код HTTP-ответа, чтобы сообщить пользователю, было ли сообщение успешно отправлено.

## <a name="run-the-app"></a>Запуск приложения

1. Установите приложение Rails и зависимости с помощью приведенной ниже команды.

    ```
    bundle install
    ```
2. Чтобы запустить приложение Rails, введите приведенную ниже команду.

    ```
    rackup -p 3000
    ```
3. Введите адрес `http://localhost:3000` в веб-браузере.

## <a name="see-also"></a>См. также
- Попробуйте REST API, используя [песочницу Graph](https://graph.microsoft.io/graph-explorer).
- Просмотрите другие [примеры Microsoft Graph](https://github.com/microsoftgraph) на сайте GitHub.


