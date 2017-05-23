# <a name="get-started-with-microsoft-graph-in-a-xamarin-forms-app"></a>Начало работы с Microsoft Graph в приложении на базе Xamarin.Forms

> **Создаете приложения для корпоративных клиентов?** Ваше приложение может не работать, если корпоративный клиент включит функции корпоративной безопасности для мобильных устройств, например <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">условный доступ с устройств</a>. В этом случае у пользователей могут возникать ошибки, а вы не будете об этом знать. 

В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из [конечной точки Azure AD версии 2.0](https://developer.microsoft.com/graph/docs/concepts/converged_auth) и вызвать Microsoft Graph. В ней представлен разбор кода [приложения Microsoft Graph Connect для Xamarin.Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) и рассматриваются основные понятия, которые необходимо реализовать в приложении, использующем Microsoft Graph. В этой статье также описывается доступ к Microsoft Graph с помощью [клиентской библиотеки Microsoft Graph](http://www.nuget.org/packages/Microsoft.Graph/).

Вы создадите такое приложение.

| UWP | Android | iOS |
| --- | ------- | ----|
| <img src="images/UWP.png" alt="Connect sample on UWP" width="100%" /> | <img src="images/Droid.png" alt="Connect sample on Android" width="100%" /> | <img src="images/iOS.png" alt="Connect sample on iOS" width="100%" /> |

**Не хотите создавать приложение?** Вы можете быстро приступить к работе с помощью [краткого руководства по Microsoft Graph](https://developer.microsoft.com/graph/quick-start) или скачать [приложение Microsoft Graph Connect для Xamarin.Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample), которое рассматривается в этой статье.

## <a name="prerequisites"></a>Необходимые компоненты

Чтобы приступить к работе, вам понадобится следующее: 

- [Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](http://dev.office.com/devprogram).
- Visual Studio 2015. 
- [Xamarin для Visual Studio](https://www.xamarin.com/visual-studio).
- Windows 10 ([с включенным режимом разработки](https://msdn.microsoft.com/library/windows/apps/xaml/dn706236.aspx)).
- [Начальный проект Microsoft Graph Connect для Xamarin.Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample/tree/master/starter). Этот шаблон содержит несколько классов, в которые вы можете добавлять код. В нем также есть полные представления и строки ресурсов. Чтобы получить этот проект, клонируйте или скачайте [приложение Microsoft Graph Connect для Xamarin.Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) и откройте решение **XamarinConnect** в папке **starter**. 

Чтобы выполнить проект iOS в этом примере, вам потребуются следующие компоненты:

- Последний пакет SDK для iOS
- Последняя версия Xcode
- Mac OS X Sierra (10.12) и более поздней версии 
- [Xamarin.iOS](https://developer.xamarin.com/guides/ios/getting_started/installation/mac/)
- [Агент Xamarin Mac, подключенный к Visual Studio](https://developer.xamarin.com/guides/ios/getting_started/installation/windows/connecting-to-mac/)


## <a name="register-the-app"></a>Регистрация приложения
 
1. Войдите на [портал регистрации приложений](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.
2. Выберите пункт **Добавить приложение**.
3. Введите имя приложения и выберите пункт **Создать приложение**.
    
    Откроется страница регистрации со свойствами приложения.
 
4. В разделе **Платформы** выберите **Добавление платформы**.
5. Выберите **Собственное приложение**.
6. Скопируйте идентификатор приложения. Вам потребуется ввести это значение в примере приложения.

    Идентификатор приложения уникален. URI перенаправления — это уникальный универсальный код ресурса (URI), предоставляемый каждому приложению операционной системой Windows 10, чтобы гарантировать, что сообщения, отправленные на этот URI, отправляются только этому приложению. 

7. Нажмите кнопку **Сохранить**.

## <a name="configure-the-project"></a>Настройка проекта

1. Откройте файл решения для начального проекта в Visual Studio.
2. Откройте файл **App.cs** в проекте **XamarinConnect (Portable)** и найдите поле `ClientId`. Замените временное значение идентификатором зарегистрированного приложения.

```
public static string ClientID = "ENTER_YOUR_CLIENT_ID";
public static string[] Scopes = { "User.Read", "Mail.Send", "Files.ReadWrite" };
```
В значении `Scopes` хранятся области разрешений Microsoft Graph, запрашиваемые приложением, когда пользователь проходит проверку подлинности. Обратите внимание, что конструктор класса `App` использует значение ClientID для создания экземпляра класса MSAL `PublicClientApplication`. Этот класс потребуется позже для проверки подлинности пользователя.

```
IdentityClientApp = new PublicClientApplication(ClientID);
```

## <a name="send-an-email-with-microsoft-graph"></a>Отправка электронного письма с помощью Microsoft Graph

Откройте файл MailHelper.cs начального проекта. Этот файл содержит код для создания и отправки электронного сообщения. Он состоит из одного метода (``ComposeAndSendMailAsync``), который создает и отправляет запрос POST конечной точке **https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail**. 

Метод ``ComposeAndSendMailAsync`` принимает три строковых значения — ``subject``, ``bodyContent`` и ``recipients``, которые передаются ему посредством файла MainPage.xaml.cs. Строки ``subject`` и ``bodyContent`` хранятся в файле AppResources.resx вместе со всеми остальными строками пользовательского интерфейса. Строка ``recipients`` принимает значения из поля адреса в интерфейсе приложения. 

**Использование объявлений**

Убедитесь, что вверху файла есть указанные ниже объявления.

```
using System;
using System.Collections.Generic;
using System.Linq;
using System.Reflection;
using System.Threading.Tasks;
using Microsoft.Graph;
```

Первая задача в методе ``ComposeAndSendMailAsync`` — получение фотографии текущего пользователя из Microsoft Graph. В этой строке выполняется вызов усеченного метода `GetCurrentUserPhotoStreamAsync`:

```
            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync();
```

Полностью метод `GetCurrentUserPhotoStreamAsync` выглядит так:

```
        // Gets the stream content of the signed-in user's photo. 
        // This snippet doesn't work with consumer accounts.
        public async Task<Stream> GetCurrentUserPhotoStreamAsync()
        {
            Stream currentUserPhotoStream = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                currentUserPhotoStream = await graphClient.Me.Photo.Content.Request().GetAsync();

            }

            // If the user account is MSA (not work or school), the service will throw an exception.
            catch (ServiceException)
            {
                return null;
            }

            return currentUserPhotoStream;

        }
```

Если у пользователя нет фотографии, то эта логика получает другой файл изображения, включенный в проект:

```
            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if (photoStream == null)
            {
                var assembly = typeof(MailHelper).GetTypeInfo().Assembly;
                photoStream = assembly.GetManifestResourceStream("XamarinConnect.test.jpg");
            }
```

Теперь, когда у нас есть поток изображений, мы можем отправить файл в OneDrive, вызвав усеченный метод `UploadFileToOneDriveAsync`:

```
            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDriveAsync(photoStreamMS.ToArray());
```

Полностью метод `UploadFileToOneDriveAsync` выглядит так:

```
        // Uploads the specified file to the user's root OneDrive directory.
        public async Task<DriveItem> UploadFileToOneDriveAsync(byte[] file)
        {
            DriveItem uploadedFile = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                MemoryStream fileStream = new MemoryStream(file);
                uploadedFile = await graphClient.Me.Drive.Root.ItemWithPath("me.png").Content.Request().PutAsync<DriveItem>(fileStream);

            }


            catch (ServiceException)
            {
                return null;
            }

            return uploadedFile;
        }
```

Кроме того, мы можем использовать этот поток для создания объекта `MessageAttachmentsCollectionPage`, который можно передать вместе с сообщением:

```
            MessageAttachmentsCollectionPage attachments = new MessageAttachmentsCollectionPage();
            attachments.Add(new FileAttachment
            {
                ODataType = "#microsoft.graph.fileAttachment",
                ContentBytes = photoStreamMS.ToArray(),
                ContentType = "image/png",
                Name = "me.png"
            });
```

Мы можем получить ссылку для общего доступа к недавно добавленному в OneDrive файлу, вызвав усеченный метод `GetSharingLinkAsync`. Строка `bodyContent` содержит заполнитель для этой ссылки:

```
            // Get the sharing link and insert it into the message body.
            Permission sharingLink = await GetSharingLinkAsync(photoFile.Id);
            string bodyContentWithSharingLink = String.Format(bodyContent, sharingLink.Link.WebUrl);
```

Полностью метод `GetSharingLinkAsync` выглядит так:

```
        public static async Task<Permission> GetSharingLinkAsync(string Id)
        {
            Permission permission = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                permission = await graphClient.Me.Drive.Items[Id].CreateLink("view").Request().PostAsync();
            }

            catch (ServiceException)
            {
                return null;
            }

            return permission;
        }
```

Так как пользователь может указать несколько адресов, строку ``recipients`` необходимо разбить на несколько объектов `EmailAddress`, используемых для создания списка объектов `Recipients`, которые затем можно передать в теле POST-запроса:

```
            // Prepare the recipient list
            string[] splitter = { ";" };
            var splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            List<Recipient> recipientList = new List<Recipient>();

            foreach (string recipient in splitRecipientsString)
            {
                recipientList.Add(new Recipient { EmailAddress = new EmailAddress { Address = recipient.Trim() } });
            }
```

В конце необходимо создать объект `Message` и отправить его в конечную точку **me/microsoft.graph.SendMail** с помощью `GraphServiceClient`. Так как строка ``bodyContent`` представляет собой документ HTML, запрос задает для параметра **ContentType** значение HTML.

```
            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();

                var email = new Message
                {
                    Body = new ItemBody
                    {
                        Content = bodyContentWithSharingLink,
                        ContentType = BodyType.Html,
                    },
                    Subject = subject,
                    ToRecipients = recipientList,
                    Attachments = attachments
                };

                try
                {
                    await graphClient.Me.SendMail(email, true).Request().PostAsync();
                }
                catch (ServiceException exception)
                {
                    throw new Exception("We could not send the message: " + exception.Error == null ? "No error message returned." : exception.Error.Message);
                }


            }

            catch (Exception e)
            {
                throw new Exception("We could not send the message: " + e.Message);
            }
```

Готовый класс должен выглядеть следующим образом:

```
    public class MailHelper
    {
        /// <summary>
        /// Compose and send a new email.
        /// </summary>
        /// <param name="subject">The subject line of the email.</param>
        /// <param name="bodyContent">The body of the email.</param>
        /// <param name="recipients">A semicolon-separated list of email addresses.</param>
        /// <returns></returns>
        public async Task ComposeAndSendMailAsync(string subject,
                                                            string bodyContent,
                                                            string recipients)
        {

            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync();


            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if (photoStream == null)
            {
                var assembly = typeof(MailHelper).GetTypeInfo().Assembly;
                photoStream = assembly.GetManifestResourceStream("XamarinConnect.test.jpg");
            }

            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDriveAsync(photoStreamMS.ToArray());

            MessageAttachmentsCollectionPage attachments = new MessageAttachmentsCollectionPage();
            attachments.Add(new FileAttachment
            {
                ODataType = "#microsoft.graph.fileAttachment",
                ContentBytes = photoStreamMS.ToArray(),
                ContentType = "image/png",
                Name = "me.png"
            });

            // Get the sharing link and insert it into the message body.
            Permission sharingLink = await GetSharingLinkAsync(photoFile.Id);
            string bodyContentWithSharingLink = String.Format(bodyContent, sharingLink.Link.WebUrl);


            // Prepare the recipient list
            string[] splitter = { ";" };
            var splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            List<Recipient> recipientList = new List<Recipient>();

            foreach (string recipient in splitRecipientsString)
            {
                recipientList.Add(new Recipient { EmailAddress = new EmailAddress { Address = recipient.Trim() } });
            }

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();

                var email = new Message
                {
                    Body = new ItemBody
                    {
                        Content = bodyContentWithSharingLink,
                        ContentType = BodyType.Html,
                    },
                    Subject = subject,
                    ToRecipients = recipientList,
                    Attachments = attachments
                };

                try
                {
                    await graphClient.Me.SendMail(email, true).Request().PostAsync();
                }
                catch (ServiceException exception)
                {
                    throw new Exception("We could not send the message: " + exception.Error == null ? "No error message returned." : exception.Error.Message);
                }


            }

            catch (Exception e)
            {
                throw new Exception("We could not send the message: " + e.Message);
            }
        }

        // Gets the stream content of the signed-in user's photo. 
        // This snippet doesn't work with consumer accounts.
        public async Task<Stream> GetCurrentUserPhotoStreamAsync()
        {
            Stream currentUserPhotoStream = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
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
        public async Task<DriveItem> UploadFileToOneDriveAsync(byte[] file)
        {
            DriveItem uploadedFile = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                MemoryStream fileStream = new MemoryStream(file);
                uploadedFile = await graphClient.Me.Drive.Root.ItemWithPath("me.png").Content.Request().PutAsync<DriveItem>(fileStream);

            }


            catch (ServiceException)
            {
                return null;
            }

            return uploadedFile;
        }

        public static async Task<Permission> GetSharingLinkAsync(string Id)
        {
            Permission permission = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                permission = await graphClient.Me.Drive.Items[Id].CreateLink("view").Request().PostAsync();
            }

            catch (ServiceException)
            {
                return null;
            }

            return permission;
        }


    }
}
``` 

Вы выполнили три действия, необходимых для взаимодействия с Microsoft Graph: регистрацию приложения, проверку подлинности пользователя и создание запроса. 

## <a name="run-the-app"></a>Запуск приложения
1. Выберите проект, который нужно запустить. Если выбрать универсальную платформу Windows, пример можно запустить на локальном компьютере. Чтобы запустить проект iOS, вам потребуется подключиться к [компьютеру Mac, на котором установлены средства Xamarin](https://developer.xamarin.com/guides/ios/getting_started/installation/windows/connecting-to-mac/). (Вы также можете открыть это решение в Xamarin Studio на компьютере Mac и запустить пример прямо оттуда.) Чтобы запустить проект для Android, вы можете использовать [эмулятор Visual Studio для Android](https://www.visualstudio.com/features/msft-android-emulator-vs.aspx). 

    ![](images/SelectProject.png "Select project in Visual Studio")

2. Нажмите клавишу F5 для сборки и отладки. Запустите решение и войдите в систему с помощью личной, рабочей или учебной учетной записи.
    > **Примечание.** Возможно, потребуется открыть диспетчер конфигурации сборки и убедиться, что для проекта UWP выбраны этапы сборки и развертывания. 

3. Войдите с помощью личной, рабочей или учебной учетной записи и предоставьте необходимые разрешения.

4. Нажмите кнопку **Отправить сообщение**. После отправки письма отобразится сообщение об успешном выполнении этой операции. Это письмо включает фотографию в виде вложения, а также ссылку для общего доступа к добавленному в OneDrive файлу.

## <a name="next-steps"></a>Дальнейшие действия
- Попробуйте REST API, используя [песочницу Graph](https://graph.microsoft.io/graph-explorer).
- Вы можете найти примеры распространенных операций в [библиотеке фрагментов кода с использованием пакеты SDK Microsoft Graph для Xamarin.Forms](https://github.com/microsoftgraph/xamarin-csharp-snippets-sample) или изучить другие [примеры для Xamarin](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=xamarin) на сайте GitHub.

## <a name="see-also"></a>См. также
- [Клиентская библиотека .NET Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [Протоколы Azure AD версии 2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Маркеры Azure AD версии 2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
