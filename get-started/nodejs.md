# <a name="get-started-with-microsoft-graph-in-a-nodejs-app"></a>Начало работы с Microsoft Graph в приложении Node.js

В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из конечной точки Azure AD версии 2.0 и вызвать Microsoft Graph. В ней рассматривается создание [приложения Microsoft Connect для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) и объясняются основные понятия, которые необходимо реализовать для использования Microsoft Graph. В этой статье рассказывается, как получить доступ к API Microsoft Graph с помощью необработанных вызовов REST.

На приведенном ниже рисунке показано создаваемое приложение. 

![Веб-приложение после входа с кнопкой "Отправить сообщение"](./images/web-screenshot.png)


**Не хотите создавать приложение?** С помощью [краткого руководства по Microsoft Graph](https://graph.microsoft.io/en-us/getting-started) вы сможете быстро приступить к работе.

Скачать вариант этого примера, использующий конечную точку Azure AD, можно на странице [приложения Microsoft Graph Connect для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample/releases/tag/last_v1_auth).


## <a name="prerequisites"></a>Необходимые условия

Чтобы приступить к работе, вам понадобится следующее: 

- [Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](http://dev.office.com/devprogram).
- [Node.js с npm](https://nodejs.org/en/download/). 
- [Приложение Microsoft Connect для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample). Вы будете использовать папку **starter-project** в примерах файлов для этого пошагового руководства.

## <a name="register-the-application"></a>Регистрация приложения
Зарегистрируйте приложение на портале регистрации приложений (Майкрософт). При этом будут созданы идентификатор и пароль приложения, которые понадобятся при его настройке в Visual Studio.

1. Войдите на [портал регистрации приложений Майкрософт](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.

2. Нажмите кнопку **Добавить приложение**.

3. Введите имя приложения и нажмите кнопку **Создать приложение**. 
    
    Откроется страница регистрации со свойствами приложения.

4. Скопируйте идентификатор приложения. Это уникальный идентификатор приложения. 

5. В разделе **Секреты приложения** нажмите кнопку **Создать новый пароль**. Скопируйте пароль из диалогового окна **Новый пароль создан**.

    Идентификатор и пароль (секрет) приложения используются для его настройки. 

6. В разделе **Платформы** нажмите **Добавление платформы** > **Интернет**.

7. Введите URI перенаправления *http://localhost:3000/login*. 

8. Нажмите кнопку **Сохранить**.


## <a name="configure-the-project"></a>Настройка проекта
1. Откройте папку **starter-project** с файлами примера.

1. Откройте командную строку и выполните приведенную ниже команду в корневом каталоге начального проекта. При этом устанавливаются зависимости проекта.

        npm install

1. Откройте в начальном проекте файл authHelper.js.


1. В поле **credentials** замените строки **ENTER\_YOUR\_CLIENT\_ID** и **ENTER\_YOUR\_SECRET** скопированными только что значениями.

  
## <a name="authenticate-the-user-and-get-an-access-token"></a>Проверка подлинности пользователя и получение маркера доступа
На этом этапе вы добавите код для входа и управления маркером. Но для начала подробнее рассмотрим поток проверки подлинности.

В этом приложении используется поток предоставления кода авторизации с делегированным удостоверением пользователя. В веб-приложении для этого потока требуются идентификатор, секрет и URI перенаправления зарегистрированного приложения. 

Поток проверки подлинности можно разделить на следующие основные этапы:

1. Перенаправление пользователя для проверки подлинности и согласия
2. Получение кода авторизации
3. Обмен кода авторизации на маркер доступа
4. Использование маркера обновления для получения нового маркера доступа по истечении срока действия текущего

В приложении используется ПО промежуточного слоя [oauth](https://www.npmjs.com/package/oauth) для проверки подлинности и получения маркеров. С помощью ПО промежуточного слоя [cookie-parser](https://www.npmjs.com/package/cookie-parser) приложение кэширует сведения о маркере в файлах cookie. Код, используемый для хранения сведений о маркере и доступа к ним, находится в контроллере index.js.
    
   >**Важно!** Простые процедуры проверки подлинности и обработки маркеров в этом проекте представлены исключительно в качестве примера. В рабочем приложении следует реализовать более надежную процедуру проверки подлинности, включающую утверждение и безопасную обработку маркеров.

Теперь вернемся к созданию приложения.

1. В файле authHelper.js замените функцию *getTokenFromCode* приведенным ниже кодом. Этот код получает маркер доступа с помощью кода авторизации.

        function getTokenFromCode(code, callback) {
            var OAuth2 = OAuth.OAuth2;
            var oauth2 = new OAuth2(
                credentials.client_id,
                credentials.client_secret,
                credentials.authority,
                credentials.authorize_endpoint,
                credentials.token_endpoint
            );

            oauth2.getOAuthAccessToken(
                code,
                {
                    grant_type: 'authorization_code',
                    redirect_uri: credentials.redirect_uri,
                    response_mode: 'form_post',
                    nonce: uuid.v4(),
                    state: 'abcd'
                },
                function (e, accessToken, refreshToken) {
                    callback(e, accessToken, refreshToken);
                }
            );
        }

1. Замените функцию **getTokenFromRefreshToken** приведенным ниже кодом. Этот код получает маркер доступа с помощью маркера обновления.

        function getTokenFromRefreshToken(refreshToken, callback) {
            var OAuth2 = OAuth.OAuth2;
            var oauth2 = new OAuth2(
                credentials.client_id,
                credentials.client_secret,
                credentials.authority,
                credentials.authorize_endpoint,
                credentials.token_endpoint
            );

            oauth2.getOAuthAccessToken(
                refreshToken,
                {
                    grant_type: 'refresh_token',
                    redirect_uri: credentials.redirect_uri,
                    response_mode: 'form_post',
                    nonce: uuid.v4(),
                    state: 'abcd'
                },
                function (e, accessToken) {
                    callback(e, accessToken);
                }
            );
        }

Теперь вы готовы добавить код для вызова Microsoft Graph. 

## <a name="call-microsoft-graph"></a>Вызов Microsoft Graph
Приложение вызывает Microsoft Graph, чтобы получить данные пользователя и отправить электронное сообщение от его имени. Такие вызовы отправляются из контроллера index.js в ответ на события пользовательского интерфейса.

1. Откройте файл requestUtil.js.

1. Замените функцию **getUserData** приведенным ниже кодом. Этот код настраивает и отправляет запрос GET конечной точке */me*, а затем обрабатывает ответ.

        function getUserData(accessToken, callback) {
            var options = {
                host: 'graph.microsoft.com',
                path: '/v1.0/me',
                method: 'GET',
                headers: {
                    'Content-Type': 'application/json',
                    Accept: 'application/json',
                    Authorization: 'Bearer ' + accessToken
                }
            };

            https.get(options, function (response) {
                var body = '';
                response.on('data', function (d) {
                    body += d;
                });
                response.on('end', function () {
                    var error;
                    if (response.statusCode === 200) {
                        callback(null, JSON.parse(body));
                    } else {
                        error = new Error();
                        error.code = response.statusCode;
                        error.message = response.statusMessage;
                        // The error body sometimes includes an empty space
                        // before the first character, remove it or it causes an error.
                        body = body.trim();
                        error.innerError = JSON.parse(body).error;
                        callback(error, null);
                    }
                });
            }).on('error', function (e) {
                callback(e, null);
            });
        }

1. Замените функцию **postSendMail** приведенным ниже кодом. Этот код настраивает и отправляет запрос POST конечной точке */me/sendMail*, а затем обрабатывает ответ.

        function postSendMail(accessToken, mailBody, callback) {
            var outHeaders = {
                'Content-Type': 'application/json',
                Authorization: 'Bearer ' + accessToken,
                'Content-Length': mailBody.length
            };
            var options = {
                host: 'graph.microsoft.com',
                path: '/v1.0/me/sendMail',
                method: 'POST',
                headers: outHeaders
            };

            // Set up the request
            var post = https.request(options, function (response) {
                var body = '';
                response.on('data', function (d) {
                    body += d;
                });
                response.on('end', function () {
                    var error;
                    if (response.statusCode === 202) {
                        callback(null);
                    } else {
                        error = new Error();
                        error.code = response.statusCode;
                        error.message = response.statusMessage;
                        // The error body sometimes includes an empty space
                        // before the first character, remove it or it causes an error.
                        body = body.trim();
                        error.innerError = JSON.parse(body).error;
                        // Note: If you receive a 500 - Internal Server Error
                        // while using a Microsoft account (outlook.com, hotmail.com or live.com),
                        // it's possible that your account has not been migrated to support this flow.
                        // Check the inner error object for code 'ErrorInternalServerTransientError'.
                        // You can try using a newly created Microsoft account or contact support.
                        callback(error);
                    }
                });
            });
            
            // write the outbound data to it
            post.write(mailBody);
            // we're done!
            post.end();

            post.on('error', function (e) {
                callback(e);
            });
        }
  
1. Откройте файл emailer.js.

1. Замените функцию **wrapEmail** приведенным ниже кодом. Этот код создает полезные данные, представляющие отправляемое сообщение.

        function wrapEmail(content, recipient) {
            var emailAsPayload = {
                Message: {
                    Subject: 'Welcome to Office 365 development with Node.js and the Office 365 Connect sample',
                    Body: {
                        ContentType: 'HTML',
                        Content: content
                    },
                    ToRecipients: [
                        {
                            EmailAddress: {
                                Address: recipient
                            }
                        }
                    ]
                },
                SaveToSentItems: true
            };
            return emailAsPayload;
        }

## <a name="run-the-app"></a>Запуск приложения

1. Откройте командную строку и выполните приведенную ниже команду в корневом каталоге начального проекта.


        npm start

1. Введите в браузере адрес *http://localhost:3000* и нажмите кнопку **Подключиться к Office 365**.

1. Выполните вход и предоставьте запрашиваемые разрешения. 

1. При необходимости измените электронный адрес получателя и нажмите кнопку **Отправить сообщение**. Под кнопкой появится сообщение, что отправка выполнена успешно. 

## <a name="next-steps"></a>Дальнейшие действия
- Попробуйте REST API, используя [песочницу Graph](https://graph.microsoft.io/graph-explorer).
- Просмотрите другие [примеры Node.js](https://github.com/search?utf8=%E2%9C%93&q=node+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) на сайте GitHub.


## <a name="see-also"></a>См. также
- [Протоколы Azure AD версии 2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Маркеры Azure AD версии 2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)