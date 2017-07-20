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

        // Send an email message from the current user.
        public async Task SendEmail(GraphServiceClient graphClient, Message message)
        {
            await graphClient.Me.SendMail(message, true).Request().PostAsync();
        }

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
  
1. Замените часть кода *// Controller actions* указанными ниже действиями.

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

            try
            {

                // Initialize the GraphServiceClient.
                GraphServiceClient graphClient = SDKHelper.GetAuthenticatedClient();

                // Build the email message.
                Message message = await graphService.BuildEmailMessage(graphClient, Request.Form["recipients"], Request.Form["subject"]);

                // Send the email.
                await graphService.SendEmail(graphClient, message);

                // Reset the current user's email address and the status to display when the page reloads.
                ViewBag.Email = Request.Form["email-address"];
                ViewBag.Message = Resource.Graph_SendMail_Success_Result;
                return View("Graph");
            }
            catch (ServiceException se)
            {
                if (se.Error.Code == Resource.Error_AuthChallengeNeeded) return new EmptyResult();
                return RedirectToAction("Index", "Error", new { message = Resource.Error_Message + Request.RawUrl + ": " + se.Error.Message });
            }
        }

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
- [Получение маркеров доступа для вызова Microsoft Graph](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [Получение доступа от имени пользователя](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [Получение доступа без пользователя](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)
