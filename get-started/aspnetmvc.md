# <a name="get-started-with-microsoft-graph-in-an-aspnet-46-mvc-app"></a>Начало работы с Microsoft Graph в приложении ASP.NET 4.6 MVC

В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из конечной точки Azure AD версии 2.0 и вызвать Microsoft Graph. В ней рассматривается создание [примера приложения Microsoft Graph Connect для ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample) и объясняются основные понятия, которые необходимо реализовать для использования Microsoft Graph.

На приведенном ниже рисунке показано создаваемое приложение. 

![Веб-приложение с кнопками "Получить адрес электронной почты" и "Отправить по электронной почте"](images/aspnet-connect-sample.png "Веб-приложение с кнопками "Получить адрес электронной почты" и "Отправить по электронной почте"")

[Конечная точка Azure AD версии 2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-appmodel-v2-overview) позволяет пользователям входить с учетной записью Майкрософт (MSA), с рабочей или учебной учетной записью. Приложение использует [ПО промежуточного слоя OpenID Connect OWIN для ASP.Net](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/) и [библиотеку проверки подлинности Майкрософт (MSAL) для .NET](https://www.nuget.org/packages/Microsoft.Identity.Client) для входа в систему и управления маркером.

**Не хотите создавать приложение?** Воспользуйтесь [кратким руководством по Microsoft Graph](https://developer.microsoft.com/en-us/graph/quick-start) для быстрого начала работы. Обратите внимание, что у нас также есть [REST-версия этого приложения](https://github.com/microsoftgraph/aspnet-connect-rest-sample).

## <a name="prerequisites"></a>Необходимые условия

Чтобы приступить к работе, вам понадобится следующее: 

- [Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](http://dev.office.com/devprogram).
- Visual Studio 2015 
- [Пример приложения, подключающегося с использованием Microsoft Graph, для ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample). Используйте папку **starter-project** с файлами примера.


## <a name="register-the-application"></a>Регистрация приложения

На этом этапе зарегистрируйте приложение на портале регистрации приложений Майкрософт. При этом будут созданы идентификатор и пароль приложения, которые понадобятся при его настройке в Visual Studio.

1. Войдите на [портал регистрации приложений Майкрософт](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.

2. Нажмите кнопку **Добавить приложение**.

3. Введите имя приложения и нажмите кнопку **Создать приложение**. 
    
    Откроется страница регистрации со свойствами приложения.

4. Скопируйте идентификатор приложения. Это уникальный идентификатор приложения. 

5. В разделе **Секреты приложения** нажмите кнопку **Создать новый пароль**. Скопируйте пароль из диалогового окна **Новый пароль создан**.

    Идентификатор и пароль приложения используются для его настройки. 

6. В разделе **Платформы** нажмите **Добавление платформы** > **Интернет**.

7. Убедитесь, что установлен флажок **Разрешить неявный поток** и введите универсальный код ресурса (URI) перенаправления *http://localhost:55065/*. 

    Параметр **Разрешить неявный поток** включает гибридный поток OpenID Connect. Благодаря этому при проверке подлинности приложение может получить данные для входа (**id_token**) и артефакты (в данном случае — код авторизации), с помощью которых оно может получить маркер доступа.

8. Нажмите кнопку **Сохранить**.

### <a name="configure-the-project"></a>Настройка проекта

1. Откройте файл решения для начального проекта в Visual Studio.

2. Откройте файл web.config проекта.

3. Найдите клавиши настройки приложения в элементе **appSettings**. Замените значения заполнителей ENTER_YOUR_CLIENT_ID и ENTER_YOUR_SECRET значениями, которые вы только что скопировали.

URI перенаправления выступает в роли URL-адреса зарегистрированного проекта. Запрошенные [области разрешений](https://developer.microsoft.com/en-us/graph/docs/concepts/permission_scopes) позволяют приложению получить данные профилей пользователей и отправить сообщение электронной почты.


## <a name="authenticate-the-user-and-get-an-access-token"></a>Проверка подлинности пользователя и получение маркера доступа

На этом этапе вы добавите код для входа и управления маркером. Но для начала подробнее рассмотрим поток проверки подлинности.

В этом приложении используется поток предоставления кода авторизации с делегированным удостоверением пользователя. В веб-приложении для этого потока требуются идентификатор, пароль и URI перенаправления зарегистрированного приложения. 

Поток проверки подлинности можно разделить на следующие основные этапы.

1. Перенаправление пользователя для проверки подлинности и согласия
2. Получение кода авторизации
3. Обмен кода авторизации на маркер доступа
4. Использование маркера обновления для получения нового маркера доступа по истечении срока действия текущего

Приложение использует [ПО промежуточного слоя OpenID Connect OWIN для ASP.Net](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/) и [библиотеку проверки подлинности Майкрософт (MSAL) для .NET](https://www.nuget.org/packages/Microsoft.Identity.Client) для входа в систему и управления маркером. Они обрабатывают большинство задач проверки подлинности.
    
В начальном проекте уже объявлены указанные ниже зависимости ПО промежуточного слоя MSAL NuGet.

  - Microsoft.Owin.Security.OpenIdConnect
  - Microsoft.Owin.Security.Cookies
  - Microsoft.Owin.Host.SystemWeb
  - Microsoft.Identity.Client

Теперь вернемся к созданию приложения.

1. В папке **App_Start** откройте файл Startup.Auth.cs. 

1. Замените метод **ConfigureAuth** указанным ниже кодом. Таким образом, вы зададите координаты для связи с Azure AD и установите проверку подлинности на основе файлов cookie, которые использует ПО промежуточного слоя OpenID Connect.

        public void ConfigureAuth(IAppBuilder app)
        {
            app.SetDefaultSignInAsAuthenticationType(CookieAuthenticationDefaults.AuthenticationType);

            app.UseCookieAuthentication(new CookieAuthenticationOptions());

            app.UseOpenIdConnectAuthentication(
                new OpenIdConnectAuthenticationOptions
                {

                    // The `Authority` represents the Microsoft v2.0 authentication and authorization service.
                    // The `Scope` describes the permissions that your app will need. See https://azure.microsoft.com/documentation/articles/active-directory-v2-scopes/                    
                    ClientId = appId,
                    Authority = "https://login.microsoftonline.com/common/v2.0",
                    PostLogoutRedirectUri = redirectUri,
                    RedirectUri = redirectUri,
                    Scope = "openid email profile offline_access " + graphScopes,
                    TokenValidationParameters = new TokenValidationParameters
                    {
                        ValidateIssuer = false,
                        // In a real application you would use IssuerValidator for additional checks, 
                        // like making sure the user's organization has signed up for your app.
                        //     IssuerValidator = (issuer, token, tvp) =>
                        //     {
                        //         if (MyCustomTenantValidation(issuer)) 
                        //             return issuer;
                        //         else
                        //             throw new SecurityTokenInvalidIssuerException("Invalid issuer");
                        //     },
                    },
                    Notifications = new OpenIdConnectAuthenticationNotifications
                    {
                        AuthorizationCodeReceived = async (context) =>
                        {
                            var code = context.Code;
                            string signedInUserID = context.AuthenticationTicket.Identity.FindFirst(ClaimTypes.NameIdentifier).Value;
                            ConfidentialClientApplication cca = new ConfidentialClientApplication(
                                appId, 
                                redirectUri,
                                new ClientCredential(appSecret),
                                new SessionTokenCache(signedInUserID, context.OwinContext.Environment["System.Web.HttpContextBase"] as HttpContextBase));
                                string[] scopes = graphScopes.Split(new char[] { ' ' });

                            AuthenticationResult result = await cca.AcquireTokenByAuthorizationCodeAsync(scopes, code);
                        },
                        AuthenticationFailed = (context) =>
                        {
                            context.HandleResponse();
                            context.Response.Redirect("/Error?message=" + context.Exception.Message);
                            return Task.FromResult(0);
                        }
                    }
                });
        }
  
  Класс OWIN Startup (определенный в Startup.cs) вызывает метод **ConfigureAuth** при запуске приложения, а это, в свою очередь, вызывает **app.UseOpenIdConnectAuthentication** для инициализации ПО промежуточного слоя для входа и первоначального запроса маркера. Приложение запрашивает следующие области разрешений:

  - **openid**, **email**, **profile** для входа
  - **offline\_access** (требуется для получения маркера обновления), **User.Read**, **Mail.Send** для приобретения маркера
  
  Объект MSAL **ConfidentialClientApplication** представляет приложение и обрабатывает задачи управления маркером. Он инициализируется с помощью **SessionTokenCache** (пример применения кэша маркера определен в TokenStorage/SessionTokenCache.cs), где хранятся данные маркера Кэш сохраняет маркеры в текущем сеансе HTTP на основе идентификатора пользователя, но рабочее приложение, скорее всего, будет использовать более долговременное хранилище.

Теперь добавим код для примера поставщика проверки подлинности, который разработан таким образом, чтобы его было легко заменить вашим настраиваемым поставщиком проверки подлинности. Классы интерфейса и поставщика уже добавлены в проект.

1. В папке **Helpers** откройте файл SampleAuthProvider.cs.

1. Замените метод **GetUserAccessTokenAsync** следующим кодом, в котором используется MSAL для получения маркера доступа.

        // Get an access token. First tries to get the token from the token cache.
        public async Task<string> GetUserAccessTokenAsync()
        {
            string signedInUserID = ClaimsPrincipal.Current.FindFirst(ClaimTypes.NameIdentifier).Value;
            tokenCache = new SessionTokenCache(
                signedInUserID, 
                HttpContext.Current.GetOwinContext().Environment["System.Web.HttpContextBase"] as HttpContextBase);
            //var cachedItems = tokenCache.ReadItems(appId); // see what's in the cache

            ConfidentialClientApplication cca = new ConfidentialClientApplication(
                appId, 
                redirectUri,
                new ClientCredential(appSecret), 
                tokenCache);

            try
            {
                AuthenticationResult result = await cca.AcquireTokenSilentAsync(scopes.Split(new char[] { ' ' }));
                return result.Token;
            }

            // Unable to retrieve the access token silently.
            catch (MsalSilentTokenAcquisitionException)
            {
                HttpContext.Current.Request.GetOwinContext().Authentication.Challenge(
                    new AuthenticationProperties() { RedirectUri = "/" },
                    OpenIdConnectAuthenticationDefaults.AuthenticationType);

                throw new Exception(Resource.Error_AuthChallengeNeeded);
            }
        }

  MSAL проверяет кэш на наличие совпадающего маркера доступа, срок действия которого не истек и не подходит к концу. Если не удается найти действующий маркер, он использует маркер обновления (при наличии действующего маркера) для получения нового маркера доступа. Если не удается получить новый маркер доступа автоматически, MSAL вызывает исключение **MsalSilentTokenAcquisitionException**, указывая, что требуется действие пользователя. 

Далее добавьте код для обработки входа и выхода из пользовательского интерфейса.

1. В папке **Controllers** откройте файл AccountController.cs.  

1. Добавьте следующие методы в класс **AccountController**. Метод **SignIn** подает сигнал ПО промежуточного слоя, что следует отправить запрос о проверке подлинности в Azure AD.

        public void SignIn()
        {
            if (!Request.IsAuthenticated)
            {
                // Signal OWIN to send an authorization request to Azure.
                HttpContext.GetOwinContext().Authentication.Challenge(
                    new AuthenticationProperties { RedirectUri = "/" },
                    OpenIdConnectAuthenticationDefaults.AuthenticationType);
            }
        }

        // Here we just clear the token cache, sign out the GraphServiceClient, and end the session with the web app.  
        public void SignOut()
        {
            if (Request.IsAuthenticated)
            {
                // Get the user's token cache and clear it.
                string userObjectId = ClaimsPrincipal.Current.FindFirst(ClaimTypes.NameIdentifier).Value;

                SessionTokenCache tokenCache = new SessionTokenCache(userObjectId, HttpContext);
                tokenCache.Clear(userObjectId);
            }

            //SDKHelper.SignOutClient();

            // Send an OpenID Connect sign-out request. 
            HttpContext.GetOwinContext().Authentication.SignOut(
            CookieAuthenticationDefaults.AuthenticationType);
            Response.Redirect("/");
        }

Теперь вы готовы добавить код для вызова Microsoft Graph. 

## <a name="call-microsoft-graph"></a>Вызов Microsoft Graph

На этом шаге вы рассмотрите классы **SDKHelper**, **GraphService** и **HomeController**. 

 - Класс **SDKHelper** инициализирует экземпляр **GraphServiceClient** из библиотеки перед каждым вызовом Microsoft Graph. В этом случае маркер доступа добавляется в запрос. 
 - Класс **GraphService** создает и отправляет запросы в Microsoft Graph с помощью библиотеки и обрабатывает отклики.
 - Класс **HomeController** содержит действия, которые отправляют вызовы в библиотеку в ответ на события пользовательского интерфейса.

В начальном проекте уже объявлена зависимость для пакета NuGet клиентской библиотеки .NET для Microsoft Graph:  *Microsoft.Graph*.

1. Щелкните правой кнопкой мыши папку **Helpers** и выберите пункт **Add** > **Class**. 

1. Присвойте имя новому классу *SDKHelper* и нажмите кнопку **Добавить**.

1. Замените содержимое приведенным ниже кодом.

        using System.Net.Http.Headers;
        using Microsoft.Graph;

        namespace Microsoft_Graph_SDK_ASPNET_Connect.Helpers
        {
            public class SDKHelper
            {   
                private static GraphServiceClient graphClient = null;

                // Get an authenticated Microsoft Graph Service client.
                public static GraphServiceClient GetAuthenticatedClient()
                {
                    GraphServiceClient graphClient = new GraphServiceClient(
                        new DelegateAuthenticationProvider(
                            async (requestMessage) =>
                            {
                                string accessToken = await SampleAuthProvider.Instance.GetUserAccessTokenAsync();

                                // Append the access token to the request.
                                requestMessage.Headers.Authorization = new AuthenticationHeaderValue("bearer", accessToken);
                            }));
                    return graphClient;
                }

                public static void SignOutClient()
                {
                    graphClient = null;
                }
            }
        }

  Обратите внимание на вызов поставщика **SampleAuthProvider** для получения маркера при инициализации клиента.

1. В папке **Models** откройте файл GraphService.cs. Служба использует библиотеку для взаимодействия с Microsoft Graph.

1. Добавьте следующий оператор **using**.

        using Microsoft.Graph;

1. Замените часть кода *// GetMyEmailAddress* следующим методом. Таким образом будет получен электронный адрес текущего пользователя. 

        // Get the current user's email address from their profile.
        public async Task<string> GetMyEmailAddress(GraphServiceClient graphClient)
        {

            // Get the current user. 
            // The app only needs the user's email address, so select the mail and userPrincipalName properties.
            // If the mail property isn't defined, userPrincipalName should map to the email for all account types. 
            User me = await graphClient.Me.Request().Select("mail,userPrincipalName").GetAsync();
            return me.Mail ?? me.UserPrincipalName;
        }

  Обратите внимание на сегмент **Select**, который требует, чтобы возвращались только элементы **mail** и **userPrinicipalName**. Можно использовать сегменты **Select** и **Filter**, чтобы уменьшить размер полезных данных отклика.

1. Замените часть кода *// SendEmail* следующими методами для создания и отправки сообщения электронной почты.

        public async Task<Message> BuildEmailMessage(GraphServiceClient graphClient, string recipients, string subject)
        {

            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync(graphClient);


            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if ( photoStream == null)
            {
                photoStream = System.IO.File.OpenRead(System.Web.Hosting.HostingEnvironment.MapPath("/Content/test.jpg"));
            }

            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDrive(graphClient, photoStreamMS.ToArray());

            MessageAttachmentsCollectionPage attachments = new MessageAttachmentsCollectionPage();
            attachments.Add(new FileAttachment
            {
                ODataType = "#microsoft.graph.fileAttachment",
                ContentBytes = photoStreamMS.ToArray(),
                ContentType = "image/png",
                Name = "me.png"
            });

            Permission sharingLink = await GetSharingLinkAsync(graphClient, photoFile.Id);

            // Add the sharing link to the email body.
            string bodyContent = string.Format(Resource.Graph_SendMail_Body_Content, sharingLink.Link.WebUrl);

            // Prepare the recipient list.
            string[] splitter = { ";" };
            string[] splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            List<Recipient> recipientList = new List<Recipient>();
            foreach (string recipient in splitRecipientsString)
            {
                recipientList.Add(new Recipient
                {
                    EmailAddress = new EmailAddress
                    {
                        Address = recipient.Trim()
                    }
                });
            }

            // Build the email message.
            Message email = new Message
            {
                Body = new ItemBody
                {
                    Content = bodyContent,
                    ContentType = BodyType.Html,
                },
                Subject = subject,
                ToRecipients = recipientList,
                Attachments = attachments
            };
            return email;
        }

        // Gets the stream content of the signed-in user's photo. 
        // This snippet doesn't work with consumer accounts.
        public async Task<Stream> GetCurrentUserPhotoStreamAsync(GraphServiceClient graphClient)
        {
            Stream currentUserPhotoStream = null;

            try
            {
                currentUserPhotoStream = await graphClient.Me.Photo.Content.Request().GetAsync();

            }

            // If the user account is MSA (not work or school), the service will throw an exception.
            catch (ServiceException)
            {
                return null;
            }

            return currentUserPhotoStream;

        }

        // Uploads the specified file to the user's root OneDrive directory.
        public async Task<DriveItem> UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
        {
            DriveItem uploadedFile = null;

            try
            {
                MemoryStream fileStream = new MemoryStream(file);
                uploadedFile = await graphClient.Me.Drive.Root.ItemWithPath("me.png").Content.Request().PutAsync<DriveItem>(fileStream);

            }


            catch (ServiceException)
            {
                return null;
            }

            return uploadedFile;
        }

        public static async Task<Permission> GetSharingLinkAsync(GraphServiceClient graphClient, string Id)
        {
            Permission permission = null;

            try
            {
                permission = await graphClient.Me.Drive.Items[Id].CreateLink("view").Request().PostAsync();
            }

            catch (ServiceException)
            {
                return null;
            }

            return permission;
        }

1. В папке **Controllers** откройте файл HomeController.cs.

1. Добавьте следующий оператор **using**.

        using Microsoft.Graph;
  
1. Замените часть кода *// Controller actions* следующими действиями.

        [Authorize]
        // Get the current user's email address from their profile.
        public async Task<ActionResult> GetMyEmailAddress()
        {
            try
            {

                // Initialize the GraphServiceClient.
                GraphServiceClient graphClient = SDKHelper.GetAuthenticatedClient();

                // Get the current user's email address. 
                ViewBag.Email = await graphService.GetMyEmailAddress(graphClient);
                return View("Graph");
            }
            catch (ServiceException se)
            {
                if (se.Error.Message == Resource.Error_AuthChallengeNeeded) return new EmptyResult();
                return RedirectToAction("Index", "Error", new { message = Resource.Error_Message + Request.RawUrl + ": " + se.Error.Message });
            }
        }

        [Authorize]
        // Send mail on behalf of the current user.
        public async Task<ActionResult> SendEmail()
        {
            if (string.IsNullOrEmpty(Request.Form["email-address"]))
            {
                ViewBag.Message = Resource.Graph_SendMail_Message_GetEmailFirst;
                return View("Graph");
            }

            // Build the email message.
            Message message = await graphService.BuildEmailMessage(graphClient, Request.Form["recipients"], Request.Form["subject"]);
            try
            {

                // Initialize the GraphServiceClient.
                GraphServiceClient graphClient = SDKHelper.GetAuthenticatedClient();

                // Send the email.
                await graphService.SendEmail(graphClient, message);

                // Reset the current user's email address and the status to display when the page reloads.
                ViewBag.Email = Request.Form["email-address"];
                ViewBag.Message = Resource.Graph_SendMail_Success_Result;
                return View("Graph");
            }
            catch (ServiceException se)
            {
                if (se.Error.Message == Resource.Error_AuthChallengeNeeded) return new EmptyResult();
                return RedirectToAction("Index", "Error", new { message = Resource.Error_Message + Request.RawUrl + ": " + se.Error.Message });
           }
        }

Теперь измените исключение, которое возвращает поставщик проверки подлинности, если требуется действие пользователя.

1. В папке **Helpers** откройте файл SampleAuthProvider.cs.

1. Добавьте следующий оператор **using**.

        using Microsoft.Graph;
  
1. В блоке **catch** метода **GetUserAccessTokenAsync** измените возвращаемое исключение, как показано ниже.

        throw new ServiceException(
            new Error
            {
                Code = GraphErrorCode.AuthenticationFailure.ToString(),
                Message = Resource.Error_AuthChallengeNeeded,
            });

Наконец, добавьте вызов для выхода клиента. 

1. В папке **Controllers** откройте файл AccountController.cs. 

1. Раскомментируйте приведенную ниже строку.

        SDKHelper.SignOutClient();

Теперь вы готовы к [запуску приложения](#run-the-app).

## <a name="run-the-app"></a>Запуск приложения
1. Нажмите клавишу F5 для сборки и запуска приложения. 

2. Войдите с помощью личной, рабочей или учебной учетной записи и предоставьте необходимые разрешения.

3. Нажмите кнопку **Получить адрес электронной почты**. После завершения операции на странице отобразится адрес электронной почты пользователя, который вошел в систему.

4. При необходимости измените список получателей и тему сообщения электронной почты, а затем нажмите кнопку **Отправить сообщение**. Под кнопкой отобразится сообщение об успешной отправке почты.


## <a name="next-steps"></a>Дальнейшие действия
- Попробуйте REST API, используя [песочницу Graph](https://graph.microsoft.io/graph-explorer).
- Вы можете найти примеры распространенных операций в [примере приложения Snippets Microsoft Graph для ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-snippets-sample) и других [примерах ASP.NET](http://aka.ms/aspnetgraphsamples) на сайте GitHub.

## <a name="see-also"></a>См. также
- [Клиентская библиотека .NET Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [Сценарий проверки подлинности веб-приложения для веб-API](https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api)
- [Интеграция идентификатора Майкрософт и Microsoft Graph в веб-приложении с помощью OpenID Connect](https://azure.microsoft.com/en-us/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/)
- [Протоколы Azure AD версии 2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Маркеры Azure AD версии 2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
