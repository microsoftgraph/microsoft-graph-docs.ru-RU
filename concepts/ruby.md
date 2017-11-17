# <a name="get-started-with-microsoft-graph-in-a-ruby-on-rails-app"></a><span data-ttu-id="b5978-101">Начало работы с Microsoft Graph в приложении Ruby on Rails</span><span class="sxs-lookup"><span data-stu-id="b5978-101">Get started with Microsoft Graph in a Ruby on Rails app</span></span>

<span data-ttu-id="b5978-p101">В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из конечной точки Azure AD версии 2.0 и вызвать Microsoft Graph. В ней описывается создание [приложения Microsoft Graph Ruby on Rails Connect](https://github.com/microsoftgraph/ruby-connect-rest-sample) и рассматриваются основные понятия, которые необходимо реализовать для использования Microsoft Graph. Кроме того, в этой статье рассказывается, как получить доступ к Microsoft Graph с помощью прямых вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="b5978-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Microsoft Graph Ruby on Rails Connect Sample](https://github.com/microsoftgraph/ruby-connect-rest-sample) and explains the main concepts that you implement to use the Microsoft Graph. The article also describes how to access Microsoft Graph by using direct REST calls.</span></span>

<span data-ttu-id="b5978-105">Скачать вариант этого примера, использующий конечную точку Azure AD, можно на странице [приложения Microsoft Graph Ruby on Rails Connect](https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth).</span><span class="sxs-lookup"><span data-stu-id="b5978-105">To download a version of the Connect sample that uses the Azure AD endpoint, see [Microsoft Graph Ruby on Rails Connect Sample](https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth).</span></span>

<span data-ttu-id="b5978-106">На приведенном ниже рисунке показано создаваемое приложение.</span><span class="sxs-lookup"><span data-stu-id="b5978-106">The following image shows the app you'll create.</span></span> 

![Снимок экрана с приложением Microsoft Ruby on Rails Connect](./images/Microsoft-Graph-Ruby-Connect-UI.png)

<span data-ttu-id="b5978-p102">**Не хотите создавать приложение?** Вы можете быстро приступить к работе с помощью [краткого руководства по Microsoft Graph](https://graph.microsoft.io/en-us/getting-started) или скачать [пример Ruby REST Connect](https://github.com/microsoftgraph/ruby-connect-rest-sample), который рассматривается в этой статье.</span><span class="sxs-lookup"><span data-stu-id="b5978-p102">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/en-us/getting-started) to get up and running fast, or download the [Ruby REST Connect sample](https://github.com/microsoftgraph/ruby-connect-rest-sample) that this article is based on.</span></span>


## <a name="prerequisites"></a><span data-ttu-id="b5978-110">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b5978-110">Prerequisites</span></span>

<span data-ttu-id="b5978-111">Чтобы приступить к работе, вам понадобится следующее:</span><span class="sxs-lookup"><span data-stu-id="b5978-111">To get started, you'll need:</span></span> 

- <span data-ttu-id="b5978-112">Ruby 2.1 для запуска приложения на сервере разработки.</span><span class="sxs-lookup"><span data-stu-id="b5978-112">Ruby 2.1 to run the sample on a development server.</span></span>
- <span data-ttu-id="b5978-113">платформа Rails (пример протестирован на платформе Rails 4.2);</span><span class="sxs-lookup"><span data-stu-id="b5978-113">Rails framework (the sample has been tested on Rails 4.2).</span></span>
- <span data-ttu-id="b5978-114">диспетчер зависимостей Bundler;</span><span class="sxs-lookup"><span data-stu-id="b5978-114">Bundler dependency manager.</span></span>
- <span data-ttu-id="b5978-115">Интерфейс веб-сервера для Ruby (Rack).</span><span class="sxs-lookup"><span data-stu-id="b5978-115">Rack web server interface for Ruby.</span></span>
- <span data-ttu-id="b5978-116">[Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](http://dev.office.com/devprogram).</span><span class="sxs-lookup"><span data-stu-id="b5978-116">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
- <span data-ttu-id="b5978-p103">Начальный проект приложения Ruby on Rails, подключающегося с использованием Microsoft Graph. Скачайте [приложение Microsoft Graph Ruby on Rails Connect](https://github.com/microsoftgraph/ruby-connect-rest-sample). Начальный проект находится в папке _starter_.</span><span class="sxs-lookup"><span data-stu-id="b5978-p103">The Microsoft Graph Connect Starter Project for Ruby on Rails. Download the [Microsoft Graph Ruby on Rails Connect Sample](https://github.com/microsoftgraph/ruby-connect-rest-sample). The starter project is located in the _starter_ folder.</span></span>


## <a name="register-the-application"></a><span data-ttu-id="b5978-120">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="b5978-120">Register the application</span></span>

<span data-ttu-id="b5978-p104">Зарегистрируйте приложение на портале регистрации приложений (Майкрософт). При этом будут созданы идентификатор и секрет клиента, с помощью которых вы настроите приложение для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b5978-p104">Register an app on the Microsoft App Registration Portal. This generates the app ID and secret that you'll use to configure the app for authentication.</span></span>

1. <span data-ttu-id="b5978-123">Войдите на [портал регистрации приложений Майкрософт](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="b5978-123">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="b5978-124">Нажмите кнопку **Добавить приложение**.</span><span class="sxs-lookup"><span data-stu-id="b5978-124">Choose **Add an app**.</span></span>

3. <span data-ttu-id="b5978-125">Введите имя приложения и нажмите кнопку **Создать приложение**.</span><span class="sxs-lookup"><span data-stu-id="b5978-125">Enter a name for the app, and choose **Create application**.</span></span>

    <span data-ttu-id="b5978-126">Откроется страница регистрации со свойствами приложения.</span><span class="sxs-lookup"><span data-stu-id="b5978-126">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="b5978-p105">Скопируйте идентификатор приложения. Это уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="b5978-p105">Copy the application ID. This is the unique identifier for your app.</span></span>

5. <span data-ttu-id="b5978-p106">В разделе **Секреты приложения** нажмите кнопку **Создать новый пароль**. Скопируйте секрет приложения из диалогового окна **Новый пароль создан**.</span><span class="sxs-lookup"><span data-stu-id="b5978-p106">Under **Application Secrets**, choose **Generate New Password**. Copy the app secret from the **New password generated** dialog.</span></span>

    <span data-ttu-id="b5978-131">Идентификатор и секрет приложения используются для его настройки.</span><span class="sxs-lookup"><span data-stu-id="b5978-131">You'll use the application ID and app secret to configure the app.</span></span>

6. <span data-ttu-id="b5978-132">В разделе **Платформы** нажмите **Добавление платформы** > **Интернет**.</span><span class="sxs-lookup"><span data-stu-id="b5978-132">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="b5978-133">Установите флажок **Разрешить неявный поток** и введите URI перенаправления *http://localhost:3000/auth/microsoft_v2_auth/callback*.</span><span class="sxs-lookup"><span data-stu-id="b5978-133">Make sure the **Allow Implicit Flow** check box is selected, and enter *http://localhost:3000/auth/microsoft_v2_auth/callback* as the Redirect URI.</span></span>

    <span data-ttu-id="b5978-p107">Параметр "Разрешить неявный поток" включает гибридный поток OpenID Connect. Благодаря этому при проверке подлинности приложение может получить данные для входа (id_token) и артефакты (в данном случае — код авторизации), с помощью которых оно может получить маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="b5978-p107">The Allow Implicit Flow option enables the OpenID Connect hybrid flow. During authentication, this enables the app to receive both sign-in info (the id_token) and artifacts (in this case, an authorization code) that the app uses to obtain an access token.</span></span>

    <span data-ttu-id="b5978-136">URI перенаправления *http://localhost:3000/auth/microsoft_v2_auth/callback* — это значение, которое ПО промежуточного слоя OmniAuth использует после обработки запроса на проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="b5978-136">The redirect URI *http://localhost:3000/auth/microsoft_v2_auth/callback* is the value that the OmniAuth middleware is configured to use once it has processed the authentication request.</span></span>

8. <span data-ttu-id="b5978-137">Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="b5978-137">Choose **Save**.</span></span>

## <a name="configure-the-project"></a><span data-ttu-id="b5978-138">Настройка проекта</span><span class="sxs-lookup"><span data-stu-id="b5978-138">Configure the project</span></span>

1. <span data-ttu-id="b5978-p108">Скачайте или клонируйте [приложение Microsoft Graph Ruby on Rails Connect](https://github.com/microsoftgraph/ruby-connect-rest-sample). Откройте папку _starter_ в любом редакторе.</span><span class="sxs-lookup"><span data-stu-id="b5978-p108">Download or clone the [Microsoft Graph Ruby on Rails Connect Sample](https://github.com/microsoftgraph/ruby-connect-rest-sample). Open the _starter_ folder in the editor of your choice.</span></span>
1. <span data-ttu-id="b5978-141">Если у вас еще нет Bundler и Rack, их можно установить с помощью приведенной ниже команды.</span><span class="sxs-lookup"><span data-stu-id="b5978-141">If you don't already have bundler and rack, you can install them with the following command.</span></span>

    ```
    gem install bundler rack
    ```
2. <span data-ttu-id="b5978-142">В файле config/environment.rb выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="b5978-142">In the config/environment.rb file, do the following:</span></span>
    - <span data-ttu-id="b5978-143">Замените текст *ENTER_YOUR_CLIENT_ID* на идентификатор клиента для зарегистрированного приложения.</span><span class="sxs-lookup"><span data-stu-id="b5978-143">Replace *ENTER_YOUR_CLIENT_ID* with the client ID of your registered  application.</span></span>
    - <span data-ttu-id="b5978-144">Замените текст *ENTER_YOUR_SECRET* на ключ для зарегистрированного приложения.</span><span class="sxs-lookup"><span data-stu-id="b5978-144">Replace *ENTER_YOUR_SECRET* with the key of your registered application.</span></span>

3. <span data-ttu-id="b5978-145">Установите приложение Rails и зависимости с помощью приведенной ниже команды.</span><span class="sxs-lookup"><span data-stu-id="b5978-145">Install the Rails application and dependencies with the following command.</span></span>

    ```
    bundle install
    ```

## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="b5978-146">Проверка подлинности пользователя и получение маркера доступа</span><span class="sxs-lookup"><span data-stu-id="b5978-146">Authenticate the user and get an access token</span></span>

<span data-ttu-id="b5978-p109">В этом приложении используется поток предоставления кода авторизации с делегированным удостоверением пользователя. В веб-приложении для этого потока требуются идентификатор, секрет и URI перенаправления зарегистрированного приложения.</span><span class="sxs-lookup"><span data-stu-id="b5978-p109">This app uses the authorization code grant flow with a delegated user identity. For a web application, the flow requires the application ID, secret, and redirect URI from the registered app.</span></span> 

<span data-ttu-id="b5978-149">Поток проверки подлинности можно разделить на следующие основные этапы:</span><span class="sxs-lookup"><span data-stu-id="b5978-149">The auth flow can be broken down into these basic steps:</span></span>

1. <span data-ttu-id="b5978-150">Перенаправление пользователя для проверки подлинности и согласия</span><span class="sxs-lookup"><span data-stu-id="b5978-150">Redirect the user for authentication and consent</span></span>
2. <span data-ttu-id="b5978-151">Получение кода авторизации</span><span class="sxs-lookup"><span data-stu-id="b5978-151">Get an authorization code</span></span>
3. <span data-ttu-id="b5978-152">Обмен кода авторизации на маркер доступа</span><span class="sxs-lookup"><span data-stu-id="b5978-152">Redeem the authorization code for an access token</span></span>

><span data-ttu-id="b5978-153">Дополнительные сведения об этом потоке проверки подлинности см. в разделе [Из веб-приложения в веб-интерфейс API](https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api) и примере [Интеграция удостоверения Майкрософт и Microsoft Graph в веб-приложения с помощью OpenID Connect](https://azure.microsoft.com/en-us/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/) в документации по Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b5978-153">For more information about this auth flow, see [Web application to web API](https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api) and  [Integrate Microsoft identity and the Microsoft Graph into a web application using OpenID Connect](https://azure.microsoft.com/en-us/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/) in the Azure AD documentation.</span></span>

<span data-ttu-id="b5978-154">Мы будем использовать три элемента ПО промежуточного слоя [Rack](http://rack.github.io/), чтобы приложение поддерживало проверку подлинности с помощью Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="b5978-154">We'll be using a stack of three pieces of [Rack](http://rack.github.io/) middleware to enable the app to authenticate against the Microsoft Graph:</span></span>

- <span data-ttu-id="b5978-155">[OmniAuth](https://rubygems.org/gems/omniauth), обобщенная платформа Rack для проверки подлинности с использованием нескольких поставщиков.</span><span class="sxs-lookup"><span data-stu-id="b5978-155">[OmniAuth](https://rubygems.org/gems/omniauth), a generalized Rack framework for multiple-provider authentication.</span></span>
- <span data-ttu-id="b5978-156">[Omniauth-oauth2](https://rubygems.org/gems/omniauth-oauth2), абстрактная стратегия OAuth2 для OmniAuth.</span><span class="sxs-lookup"><span data-stu-id="b5978-156">[Omniauth-oauth2](https://rubygems.org/gems/omniauth-oauth2), an abstract OAuth2 strategy for OmniAuth.</span></span> 
- <span data-ttu-id="b5978-p110">omniauth-microsoft_v2_auth, стратегия OmniAuth, настраивающая Omniauth-oauth2 для явной проверки подлинности с использованием конечной точки Azure AD версии 2.0. Этот проект включен в пример кода.</span><span class="sxs-lookup"><span data-stu-id="b5978-p110">omniauth-microsoft_v2_auth, an OmniAuth strategy that customizes Omniauth-oauth2 to specifically provide authentication against the Azure AD v2.0 endpoint. This project is included in the code sample.</span></span>

### <a name="specify-gem-dependencies-for-authentication"></a><span data-ttu-id="b5978-159">Указание необходимых gem-пакетов для проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b5978-159">Specify gem dependencies for authentication</span></span>

<span data-ttu-id="b5978-160">В Gemfile раскомментируйте перечисленные ниже gem-пакеты, чтобы добавить их в качестве зависимостей.</span><span class="sxs-lookup"><span data-stu-id="b5978-160">In Gemfile, uncomment the following gems to add them as dependencies.</span></span>

    ```
    gem 'omniauth'
    gem 'omniauth-oauth2'
    gem 'omniauth-microsoft_v2_auth', path: './omniauth-microsoft_v2_auth'
    ```

<span data-ttu-id="b5978-161">Обратите внимание, что стратегия `omniauth-microsoft_v2_auth` включена в проект приложения и будет установлена из указанного пути.</span><span class="sxs-lookup"><span data-stu-id="b5978-161">Note that `omniauth-microsoft_v2_auth` is included in the app project, and will be installed from the path specified.</span></span> 

### <a name="configure-the-authentication-middleware"></a><span data-ttu-id="b5978-162">Настройка ПО промежуточного слоя для проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b5978-162">Configure the authentication middleware</span></span>

<span data-ttu-id="b5978-163">В файле `config/initializers/omniauth-microsoft_v2_auth.rb` раскомментируйте приведенные ниже строки.</span><span class="sxs-lookup"><span data-stu-id="b5978-163">In `config/initializers/omniauth-microsoft_v2_auth.rb`, uncomment the following lines.</span></span>

    ```
    Rails.application.config.middleware.use OmniAuth::Builder do
      provider :microsoft_v2_auth,
      ENV['CLIENT_ID'],
      ENV['CLIENT_SECRET'],
      :scope => ENV['SCOPE']
    end
    ```
<span data-ttu-id="b5978-p111">Это необходимо для настройки ПО промежуточного слоя OmniAuth, в частности для указания идентификатора и секрета приложения, а также запрашиваемых областей разрешений. Это значения, которые вы указали ранее в файле `config/environment.rb`.</span><span class="sxs-lookup"><span data-stu-id="b5978-p111">This configures the OmniAuth middleware, including specifying the app ID and app secret to use, as well as the scopes to request for the user. These are the values you specified earlier in `config/environment.rb`.</span></span>

### <a name="specify-routes-for-authentication"></a><span data-ttu-id="b5978-166">Указание маршрутов для проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b5978-166">Specify routes for authentication</span></span>

<span data-ttu-id="b5978-p112">Теперь нам необходимо указать два маршрута для потока проверки подлинности. Первый маршрут пересылает запрос проверки подлинности в ПО промежуточного слоя OmniAuth, а второй задает расположение в приложении для перенаправления OmniAuth после проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b5978-p112">Now we need to specify two routes necessary for the authentication flow. The first route forwards the authentication request to the OmniAuth middleware, and the second specifies the location in the app to which OmniAuth should redirect once authentication has occurred.</span></span>

<span data-ttu-id="b5978-169">В файле `config/routes.rb` раскомментируйте указанную ниже директиву маршрута.</span><span class="sxs-lookup"><span data-stu-id="b5978-169">In `config/routes.rb`, uncomment the following route directive.</span></span>

    get '/login', to: 'pages#login'

<span data-ttu-id="b5978-170">При этом запросы на вход направляются методу `login` контроллера страниц, который, в свою очередь, перенаправляет запрос в ПО промежуточного слоя omniauth-microsoft_v2_auth.</span><span class="sxs-lookup"><span data-stu-id="b5978-170">This directs login requests to the pages controller's `login` method, which in turn redirects the request to the omniauth-microsoft_v2_auth middleware.</span></span>

    def login
        redirect_to '/auth/microsoft_v2_auth'
    end

<span data-ttu-id="b5978-p113">Затем необходимо указать, на какую страницу приложения будет переходить OmniAuth после проверки подлинности. Раскомментируйте приведенный ниже маршрут.</span><span class="sxs-lookup"><span data-stu-id="b5978-p113">Next, we need to specify where in the app OmniAuth should redirect once authentication has occurred. Uncomment the following route.</span></span>

    match '/auth/:provider/callback', to: 'pages#callback', via: [:get, :post]

<span data-ttu-id="b5978-p114">Завершив проверку подлинности пользователя, OmniAuth вызывает URL-адрес перенаправления, указанный при регистрации приложения (в данном случае — *http://localhost:3000/auth/microsoft_v2_auth/callback*). Приведенный выше шаблон маршрута соответствует этому URL-адресу, поэтому запрос направляется методу `callback` контроллера страниц.</span><span class="sxs-lookup"><span data-stu-id="b5978-p114">When OmniAuth has finished authenticating the user, it calls the redirect URL specified in the app registration; in this case, *http://localhost:3000/auth/microsoft_v2_auth/callback*. The route pattern above matches that URL and so routes the request to the page controller's `callback` method.</span></span>

### <a name="get-an-access-token"></a><span data-ttu-id="b5978-175">Получение маркера доступа</span><span class="sxs-lookup"><span data-stu-id="b5978-175">Get an access token</span></span>

<span data-ttu-id="b5978-176">Теперь мы добавим код, который запускает проверку подлинности и получает маркер доступа, когда пользователь выполнит вход.</span><span class="sxs-lookup"><span data-stu-id="b5978-176">Next, we'll add the code that actually starts the authentication process, and retrieves the access token once the user has successfully signed in.</span></span>

<span data-ttu-id="b5978-p115">Изучите `app/views/pages/index.html.erb`, представление для корневого каталога сайта. Это представление содержит одну кнопку, с помощью которой пользователь может выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="b5978-p115">Take a look at `app/views/pages/index.html.erb`, the view for the site root. The view includes a single button, which enables users to sign in.</span></span>

    <button class="ms-Button" onclick="window.location.href = '/login'">
        <span class="ms-Button-label"><%= t('connect_button') %></span>
    </button>

<span data-ttu-id="b5978-p116">Как показано выше, метод входа выполняет перенаправление в ПО промежуточного слоя OmniAuth, для которого настроены идентификатор и секрет клиента, а также запрашиваемые области разрешений. После успешной проверки подлинности пользователя OmniAuth возвращает приложению хэш с маркером доступа и другими сведениями о пользователе.</span><span class="sxs-lookup"><span data-stu-id="b5978-p116">As shown earlier, the login method redirects to the OmniAuth middleware, which has been configured with the app ID and app secret, as well as the scopes to request for the user. Once the user is successfully authenticated, OmniAuth returns a hash with the access token and other user information to the app.</span></span>

<span data-ttu-id="b5978-181">Теперь добавим код для обработки обратного вызова OmniAuth и получения сведений из хэша.</span><span class="sxs-lookup"><span data-stu-id="b5978-181">Now let's add code to handle the OmniAuth callback, and retrieve information from that hash.</span></span> 

<span data-ttu-id="b5978-182">В файле `app/controllers/pages_controller.rb` замените пустой метод `callback` приведенным ниже кодом.</span><span class="sxs-lookup"><span data-stu-id="b5978-182">In `app/controllers/pages_controller.rb`, replace the empty `callback` method with the following code.</span></span>

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

<span data-ttu-id="b5978-183">Этот метод извлекает хэш проверки подлинности, а затем сохраняет маркер доступа, имя пользователя и электронный адрес в текущем сеансе.</span><span class="sxs-lookup"><span data-stu-id="b5978-183">This method retrieves the authentication hash, and then stores the access token, user name, and email in the current session.</span></span>

> <span data-ttu-id="b5978-p117">**Примечание.** Простые процедуры проверки подлинности и обработки маркеров в этом проекте представлены исключительно в качестве примера. Скорее всего, в рабочем приложении вы реализуете более надежную процедуру проверки подлинности, включающую безопасную обработку и обновление маркеров.</span><span class="sxs-lookup"><span data-stu-id="b5978-p117">**Note:** The simple authentication  and token handling in this project is presented for illustrative purposes only. In a production app, you would likely construct a more robust way of handling authentication, including secure token handling and token refresh.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="b5978-186">Вызов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b5978-186">Call Microsoft Graph</span></span>

<span data-ttu-id="b5978-187">Теперь вы готовы добавить код для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b5978-187">Now you're ready to add code to call Microsoft Graph.</span></span> 

<span data-ttu-id="b5978-p118">Представление, отображаемое с помощью метода `callback` (`app/views/pages/callback.html.erb`) содержит простую форму с одной кнопкой. Форма отправляет данные в `send_mail` и содержит один параметр — электронный адрес получателя.</span><span class="sxs-lookup"><span data-stu-id="b5978-p118">The view rendered by the `callback` method (`app/views/pages/callback.html.erb`) includes a simple form with a single button. The form posts to  `send_mail`, and includes a single parameter, the email address of the intended recipient.</span></span>
    
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

<span data-ttu-id="b5978-190">В файле `app/controllers/pages_controller.rb` замените пустой метод `send_mail` приведенным ниже кодом.</span><span class="sxs-lookup"><span data-stu-id="b5978-190">In `app/controllers/pages_controller.rb`, replace the empty `send_mail` method with the following code.</span></span>

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

<span data-ttu-id="b5978-191">Этот код создает HTTP-запрос, форматирует электронное сообщение, а затем вызывает Microsoft Graph для отправки сообщения.</span><span class="sxs-lookup"><span data-stu-id="b5978-191">This code constructs the HTTP request, formats the email, and then calls Microsoft Graph to send the email.</span></span>

<span data-ttu-id="b5978-p119">Чтобы создать сообщение, код извлекает имя пользователя из маркера сеанса и электронный адрес получателя из параметров, переданных формой. Затем код считывает текст сообщения из включенного в проект шаблона, интерполирует имя пользователя и электронный адрес и добавляет текст сообщения в текст HTTP-запроса.</span><span class="sxs-lookup"><span data-stu-id="b5978-p119">To create the email, the code pulls the user name from the session token and the recipient email address from the parameters passed from the form. The code then reads the email body from a template included in the project, interpolates the user name and email address, and attaches the email text as the HTTP request body.</span></span>

<span data-ttu-id="b5978-194">Чтобы отправить сообщение, код создает HTTP-запрос, добавляет маркер доступа в качестве заголовка авторизации, а затем отправляет запрос конечной точке отправки почты.</span><span class="sxs-lookup"><span data-stu-id="b5978-194">To send the email, the code constructs the HTTP request, attaches the access token as an authorization header, and then posts the request to the send email endpoint.</span></span>

<span data-ttu-id="b5978-195">Наконец, код использует возвращенный код HTTP-ответа, чтобы сообщить пользователю, было ли сообщение успешно отправлено.</span><span class="sxs-lookup"><span data-stu-id="b5978-195">Finally, the code uses the HTTP response code returned to notify the user whether or not the email was successful.</span></span>

## <a name="run-the-app"></a><span data-ttu-id="b5978-196">Запуск приложения</span><span class="sxs-lookup"><span data-stu-id="b5978-196">Run the app</span></span>

1. <span data-ttu-id="b5978-197">Установите приложение Rails и зависимости с помощью приведенной ниже команды.</span><span class="sxs-lookup"><span data-stu-id="b5978-197">Install the Rails application and dependencies with the following command.</span></span>

    ```
    bundle install
    ```
2. <span data-ttu-id="b5978-198">Чтобы запустить приложение Rails, введите приведенную ниже команду.</span><span class="sxs-lookup"><span data-stu-id="b5978-198">To start the Rails application, type the following command.</span></span>

    ```
    rackup -p 3000
    ```
3. <span data-ttu-id="b5978-199">Введите адрес `http://localhost:3000` в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="b5978-199">Go to `http://localhost:3000` in your web browser.</span></span>

## <a name="see-also"></a><span data-ttu-id="b5978-200">См. также</span><span class="sxs-lookup"><span data-stu-id="b5978-200">See also</span></span>
- <span data-ttu-id="b5978-201">Попробуйте REST API, используя [песочницу Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="b5978-201">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="b5978-202">Просмотрите другие [примеры Microsoft Graph](https://github.com/microsoftgraph) на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="b5978-202">Explore our other [Microsoft Graph samples](https://github.com/microsoftgraph) on GitHub.</span></span>


