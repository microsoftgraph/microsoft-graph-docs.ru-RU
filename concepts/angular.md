# <a name="get-started-with-microsoft-graph-in-an-angularjs-app"></a>Начало работы с Microsoft Graph в приложении AngularJS

В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из конечной точки Azure AD версии 2.0 и вызвать Microsoft Graph. В ней рассматривается создание [приложения Microsoft Connect для AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample) и объясняются основные понятия, которые необходимо реализовать для использования Microsoft Graph. В этой статье также описывается, как получить доступ к Microsoft Graph с помощью [пакета SDK Microsoft Graph для JavaScript](https://github.com/microsoftgraph/msgraph-sdk-javascript) или необработанных вызовов REST.

На приведенном ниже рисунке показано создаваемое приложение. 

![Веб-приложение после входа с кнопкой "Отправить сообщение"](./images/angular-connect-sample.png)


**Не хотите создавать приложение?** С помощью [краткого руководства по Microsoft Graph](https://graph.microsoft.io/ru-RU/getting-started) вы сможете быстро приступить к работе.

Скачать вариант этого примера, использующий конечную точку Azure AD, можно на странице [приложения Microsoft Graph Connect для AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample/releases/tag/last_v1_auth).


## <a name="prerequisites"></a>Необходимые условия

Чтобы приступить к работе, вам понадобится следующее: 

- [Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](https://docs.microsoft.com/ru-RU/office/developer-program/office-365-developer-program-faq#account-types).
- [Node.js с npm](https://nodejs.org/en/download/).
- [Bower](https://bower.io).
- [Приложение Microsoft Graph Connect для AngularJS](https://github.com/microsoftgraph/angular-connect-sample). Вы будете использовать папку **starter-project** в примерах файлов для этого пошагового руководства.

## <a name="register-the-application"></a>Регистрация приложения
Зарегистрируйте приложение на портале регистрации приложений (Майкрософт). При этом будут созданы идентификатор и пароль приложения, которые понадобятся при его настройке в Visual Studio.

1. Войдите на [портал регистрации приложений Майкрософт](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.

2. Нажмите кнопку **Добавить приложение**.

3. Введите имя приложения и нажмите кнопку **Создать приложение**. 
    
    Откроется страница регистрации со свойствами приложения.

4. Скопируйте идентификатор приложения. Это уникальный идентификатор приложения, который используется для его настройки.

5. В разделе **Платформы** выберите **Добавление платформы** > **Веб**.

6. Убедитесь, что установлен флажок **Разрешить неявный поток**, и введите *http://localhost:8080* в качестве URI перенаправления. 

7. Нажмите кнопку **Сохранить**.


## <a name="configure-the-project"></a>Настройка проекта
1. Откройте папку **starter-project** с файлами примера.
2. Откройте командную строку и выполните приведенные ниже команды в корневом каталоге начального проекта. При этом устанавливаются зависимости проекта.

        npm install  
        bower install
    
3. В файлах начального проекта перейдите к папке **public/scripts** и откройте файл config.js.
4. В поле **clientID** замените текст **ENTER_YOUR_CLIENT_ID** на скопированный идентификатор приложения.

## <a name="call-microsoft-graph-with-the-sdk"></a>Вызовы Microsoft Graph с помощью пакета SDK
Приложение вызывает Microsoft Graph, чтобы получить данные пользователя и отправить электронное сообщение от его имени. Такие вызовы отправляются из MainController в ответ на события пользовательского интерфейса.

Откройте файл app.js и добавьте в его конец следующий код. Этот код инициализирует пакет SDK.

    var authToken;
    var graphClient = MicrosoftGraph.Client.init({
        authProvider: function(done) {
        if (typeof authToken === "undefined") {
          done({err: "No auth token"})
        } else {
          done(null, authToken); //first parameter takes an error if you can't get an access token
        }
        }
    });

### <a name="using-the-sdk"></a>Использование пакета SDK
1. В файле graphHelper.js замените строку *// Get the profile of the current user* на приведенный ниже код. Этот код настраивает и отправляет запрос GET конечной точке */me*, а затем обрабатывает ответ.

        // Get the profile of the current user.
        me: function me() {
          return graphClient.api('/me').get();
        },
  
2. Замените строку *// Send an email on behalf of the current user* на приведенный ниже код. Этот код настраивает и отправляет запрос POST конечной точке */me/sendMail*, а затем обрабатывает ответ.

        // Send an email on behalf of the current user.
        sendMail: function sendMail(email) {
          return graphClient.api('/me/sendMail').post({ 'message' : email, 'saveToSentItems': true });
        }

3. В папке **public/controllers** откройте файл mainController.js.

4. Замените строку *// Set the default headers and user properties* на приведенный ниже код. Этот код добавляет маркер доступа к HTTP-запросу, вызывает **GraphHelper.me**, чтобы получить профиль текущего пользователя, и обрабатывает ответ.

        // Set the default headers and user properties.
        function processAuth() {

        // let the authProvider access the access token
        authToken = localStorage.token;

        if (localStorage.getItem('user') === null) {

          // Get the profile of the current user.
          GraphHelper.me().then(function(user) {

            // Save the user to localStorage.
            localStorage.setItem('user', angular.toJson(user));

            vm.displayName = user.displayName;
            vm.emailAddress = user.mail || user.userPrincipalName;
          });
        } else {
          let user = angular.fromJson(localStorage.user);

          vm.displayName = user.displayName;
          vm.emailAddress = user.mail || user.userPrincipalName;
        }

        }

5. Замените строку *// Send an email on behalf of the current user* на приведенный ниже код. Этот код создает электронное сообщение, вызывает метод **GraphHelper.sendMail** и обрабатывает ответ.

        // Send an email on behalf of the current user.
        function sendMail() {

          authToken = localStorage.token;       

          // Build the HTTP request payload (the Message object).
          var email = {
          Subject: 'Welcome to Microsoft Graph development with Angular and the Microsoft Graph Connect sample',
          Body: {
            ContentType: 'HTML',
            Content: getEmailContent()
          },
          ToRecipients: [
            {
              EmailAddress: {
            Address: vm.emailAddress
              }
            }
          ]
          };

          // Save email address so it doesn't get lost with two way data binding.
          vm.emailAddressSent = vm.emailAddress;
          GraphHelper.sendMail(email)
        .then(function (response) {
          $log.debug('HTTP request to the Microsoft Graph API returned successfully.', response);
          vm.requestSuccess = true;
          vm.requestFinished = true;
          $scope.$apply();
        }, function (error) {
          $log.error('HTTP request to the Microsoft Graph API failed.');
          vm.requestSuccess = false;
          vm.requestFinished = true;
          $scope.$apply();
        });

        };

6. Сохраните все изменения.

## <a name="run-the-app"></a>Запуск приложения

1. Откройте командную строку и выполните приведенную ниже команду в корневом каталоге начального проекта.

        npm start

2. Введите в браузере адрес *http://localhost:8080* и нажмите кнопку **Подключиться**.

3. Выполните вход и предоставьте запрашиваемые разрешения. 

4. При необходимости измените электронный адрес получателя и нажмите кнопку **Отправить сообщение**. Под кнопкой появится сообщение, что отправка выполнена успешно. 

## <a name="next-steps"></a>Дальнейшие действия
- Попробуйте REST API, используя [песочницу Graph](https://developer.microsoft.com/graph/graph-explorer).
- Просмотрите другие [примеры AngularJS](https://github.com/search?utf8=%E2%9C%93&q=angular+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) на сайте GitHub.


## <a name="see-also"></a>См. также
- [Протоколы Azure AD версии 2.0](https://azure.microsoft.com/ru-RU/documentation/articles/active-directory-v2-protocols/)
- [Маркеры Azure AD версии 2.0](https://azure.microsoft.com/ru-RU/documentation/articles/active-directory-v2-tokens/)
