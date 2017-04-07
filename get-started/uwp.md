# <a name="get-started-with-microsoft-graph-in-a-universal-windows-10-app"></a>Начало работы с Microsoft Graph в универсальном приложении для Windows 10

> **Создаете приложения для корпоративных клиентов?** Ваше приложение может не работать, если корпоративный клиент включит функции корпоративной безопасности для мобильных устройств, например <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">условный доступ с устройств</a>. В этом случае у пользователей могут возникать ошибки, а вы не будете об этом знать. 

> Для поддержки **всех корпоративных клиентов** в **любых корпоративных сценариях** необходимо использовать конечную точку Azure AD и управлять приложениями с помощью [портала управления Azure](https://aka.ms/aadapplist). Дополнительные сведения см. в разделе [Выбор между конечными точками Azure AD и Azure AD версии 2.0](../authorization/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).

В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из [конечной точки Azure AD версии 2.0](https://developer.microsoft.com/en-us/graph/docs/authorization/converged_auth) и вызвать Microsoft Graph. В ней представлен разбор кода в [приложении Microsoft Graph Connect для универсальной платформы Windows (REST)](https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample) и [приложении Microsoft Graph Connect для универсальной платформы Windows (библиотека)](https://github.com/microsoftgraph/uwp-csharp-connect-sample), а также рассматриваются основные понятия, которые необходимо реализовать в приложении, использующем Microsoft Graph. В этой статье также описывается доступ к Microsoft Graph как с помощью необработанных вызовов REST, так и с помощью [клиентской библиотеки Microsoft Graph](http://www.nuget.org/packages/Microsoft.Graph/).

Вы можете скачать обе версии приложения, создание которого описывается в этом пошаговом руководстве, из следующих репозиториев GitHub:

* [Приложение Microsoft Graph Connect для UWP (REST)](https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample)
* [Приложение Microsoft Graph Connect для UWP (библиотека)](https://github.com/microsoftgraph/uwp-csharp-connect-sample)

**Не хотите создавать приложение?** С помощью [краткого руководства по Microsoft Graph](https://graph.microsoft.io/en-us/getting-started) вы сможете быстро приступить к работе.

## <a name="sample-user-interface"></a>Пользовательский интерфейс приложения

У этого приложения очень простой пользовательский интерфейс, состоящий из верхней панели команд, **кнопки подключения**, кнопки **отправки почты** и текстового поля, в которое автоматически подставляется адрес электронной почты вошедшего пользователя (его можно изменить).

Если пользователь не подключен, кнопка **отправки почты** неактивна:

![Экран, на котором кнопка подключения активна, а кнопка отправки почты неактивна](images/SignedOut.png)

Если пользователь подключен, на верхней панели команд отображается кнопка отключения:

![Экран с адресом электронной почты подключенного пользователя и активной кнопкой отправки почты](images/SignedIn.png)

Все строки пользовательского интерфейса хранятся в файле Resources.resw в папке Assets.

## <a name="prerequisites"></a>Необходимые условия

Чтобы приступить к работе, вам понадобится следующее: 

- [Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](http://dev.office.com/devprogram).
- Visual Studio 2015 
- [Начальный проект Microsoft Graph для UWP (библиотека)](https://github.com/microsoftgraph/uwp-csharp-connect-sample/tree/master/starter) или [начальный проект Microsoft Graph для UWP (REST)](https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/master/starter). Оба шаблона содержат пустые классы, в которые вы можете добавлять код. Они также содержат строки ресурсов. Чтобы скачать один или оба этих проекта, клонируйте и скачайте [приложение Microsoft Graph Connect для UWP (библиотека)](https://github.com/microsoftgraph/uwp-csharp-connect-sample) и/или [приложение Microsoft Graph Connect для UWP (REST)](https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample), а затем откройте решение в папке **starter**.


## <a name="register-the-app"></a>Регистрация приложения
 
1. Войдите на [портал регистрации приложений](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.
2. Выберите пункт **Добавить приложение**.
3. Введите имя приложения и выберите пункт **Создать приложение**.
    
    Откроется страница регистрации со свойствами приложения.
 
4. В разделе **Платформы** нажмите **Добавление платформы**.
5. Выберите **мобильную платформу**.
6. Скопируйте идентификатор клиента (идентификатор приложения) и URI перенаправления в буфер обмена. Эти значения потребуется ввести в примере приложения.

    Идентификатор приложения уникален. URI перенаправления — это уникальный универсальный код ресурса (URI), предоставляемый каждому приложению операционной системой Windows 10, чтобы гарантировать, что сообщения, отправленные на этот URI, отправляются только этому приложению. 

7. Нажмите кнопку **Сохранить**.

## <a name="configure-the-project"></a>Настройка проекта

1. Откройте файл решения для начального проекта в Visual Studio.
2. Откройте в проекте файл **App.xaml** и найдите узел `Application.Resources`. Замените временные идентификатор приложения и URI перенаправления соответствующими значениями для зарегистрированного приложения.


```xml
    <Application.Resources>
        <!-- Add your Client Id here. -->
        <x:String x:Key="ida:ClientID">ENTER_YOUR_CLIENT_ID</x:String>
        <!-- Add your Redirect URI here. -->
        <x:String x:Key="ida:ReturnUrl">ENTER_YOUR_REDIRECT_URI</x:String>
    </Application.Resources>
```

## <a name="install-the-microsoft-authentication-library-msal"></a>Установка библиотеки проверки подлинности (Майкрософт) — MSAL

[Библиотека проверки подлинности (Майкрософт)](https://www.nuget.org/packages/Microsoft.Identity.Client) содержит классы и методы, которые упрощают проверку подлинности пользователей через конечную точку Azure AD версии 2.0.

1. В обозревателе решений щелкните правой кнопкой мыши название проекта и выберите пункт **Управление пакетами NuGet...**
2. Нажмите кнопку "Обзор" и найдите файл Microsoft.Identity.Client.
3. Выберите последнюю версию библиотеки проверки подлинности (Майкрософт) и нажмите кнопку **Установить**.

## <a name="install-the-microsoft-graph-client-library"></a>Установка клиентской библиотеки Microsoft Graph

> **Примечание.** Если вы собираетесь использовать необработанные вызовы REST для доступа к Microsoft Graph, можете пропустить этот раздел.

1. В обозревателе решений щелкните правой кнопкой мыши название проекта и выберите пункт **Управление пакетами NuGet...**
2. Нажмите кнопку "Обзор" и найдите файл Microsoft.Graph.
3. Выберите последнюю версию клиентской библиотеки Microsoft Graph и нажмите кнопку **Установить**.

## <a name="create-the-authenticationhelpercs-class"></a>Создание класса AuthenticationHelper.cs

Откройте файл AuthenticationHelper.cs начального проекта. Этот файл содержит весь код проверки подлинности, а также дополнительную логику, которая сохраняет сведения о пользователях и выполняет принудительную проверку подлинности только при выходе пользователя из приложения. Этот класс содержит как минимум два метода: `GetTokenForUserAsync` и `Signout`. Если вы используете клиентскую библиотеку Microsoft Graph, вам потребуется добавить третий метод: `GetAuthenticatedClient`.

Метод ``GetTokenHelperAsync`` выполняется только во время проверки подлинности пользователя и каждый раз, когда приложение вызывает Microsoft Graph.

**Использование объявлений**

***Версия с использованием клиентской библиотеки***

Если вы используете клиентскую библиотеку Microsoft Graph, вам потребуются следующие объявления:

```c#
using System;
using System.Diagnostics;
using System.Net.Http.Headers;
using System.Threading.Tasks;
using Microsoft.Graph;
using Microsoft.Identity.Client;
```

***Версия с использованием REST***

Если вы используете необработанные вызовы REST для доступа к Microsoft Graph, вам потребуется добавить в класс AuthenticationHelper следующие объявления `using`:

```c#
using System;
using System.Threading.Tasks;
using Windows.Storage;
using Microsoft.Identity.Client;
```

**Поля класса**

Эти поля потребуются обеим версиям класса AuthenticationHelper:

```c#
// The Client ID is used by the application to uniquely identify itself to the Azure AD v2.0 endpoint.
static string clientId = App.Current.Resources["ida:ClientID"].ToString();
public static string[] Scopes = { "User.Read", "Mail.Send" };
public static PublicClientApplication IdentityClientApp = new PublicClientApplication(clientId);
public static string TokenForUser = null;
public static DateTimeOffset Expiration;
```

Обратите внимание, что в обеих версиях для проверки подлинности пользователя используется класс MSAL `PublicClientApplication`. В поле `Scopes` хранятся области разрешений Microsoft Graph, запрашиваемые приложением, когда пользователь проходит проверку подлинности. 

***Версия с использованием клиентской библиотеки***

Если вы используете клиентскую библиотеку, сохраните объект `GraphServicesClient` в виде поля, чтобы его не пришлось создавать несколько раз:

```c#
private static GraphServiceClient graphClient = null;
```

***Версия с использованием REST***

Если вы используете вызовы REST, вам потребуется хранить некоторые значения в параметрах роуминга приложения, чтобы хранить сведения о пользователе. (В другой версии эти сведения предоставляет клиентская библиотека.)

```c#
public static ApplicationDataContainer _settings = ApplicationData.Current.RoamingSettings;
```

**GetTokenForUserAsync**

***Версия с использованием клиентской библиотеки***

В методе `GetTokenForUserAsync` используются класс PublicClientApplicationClass и параметр ClientId, чтобы получить маркер доступа для пользователя. Если пользователь еще не прошел проверку подлинности, открывается пользовательский интерфейс проверки подлинности. Эту версию метода следует применять при использовании клиентской библиотеки.

```c#
        public static async Task<string> GetTokenForUserAsync()
        {
            AuthenticationResult authResult;
            try
            {
                authResult = await IdentityClientApp.AcquireTokenSilentAsync(Scopes);
                TokenForUser = authResult.Token;
            }

            catch (Exception)
            {
                if (TokenForUser == null || Expiration <= DateTimeOffset.UtcNow.AddMinutes(5))
                {
                    authResult = await IdentityClientApp.AcquireTokenAsync(Scopes);

                    TokenForUser = authResult.Token;
                    Expiration = authResult.ExpiresOn;
                }
            }

            return TokenForUser;
        }
```

***Версия с использованием REST***

Вариант метода `GetTokenForUserAsync` для REST выполняет немного больше действий, так как ему требуется хранить некоторые сведения о вошедшем пользователе.

```c#
        public static async Task<string> GetTokenForUserAsync()
        {
            AuthenticationResult authResult;
            try
            {
                authResult = await IdentityClientApp.AcquireTokenSilentAsync(Scopes);
                TokenForUser = authResult.Token;
                // save user ID in local storage
                _settings.Values["userID"] = authResult.User.UniqueId;
                _settings.Values["userEmail"] = authResult.User.DisplayableId;
                _settings.Values["userName"] = authResult.User.Name;
            }

            catch (Exception)
            {
                if (TokenForUser == null || Expiration <= DateTimeOffset.UtcNow.AddMinutes(5))
                {
                    authResult = await IdentityClientApp.AcquireTokenAsync(Scopes);

                    TokenForUser = authResult.Token;
                    Expiration = authResult.ExpiresOn;

                    // save user ID in local storage
                    _settings.Values["userID"] = authResult.User.UniqueId;
                    _settings.Values["userEmail"] = authResult.User.DisplayableId;
                    _settings.Values["userName"] = authResult.User.Name;
                }
            }

            return TokenForUser;
        }
```

**Выход**

В обеих версиях метод `Signout` выполняет выход из системы для всех пользователей, вошедших с помощью `PublicClientApplication` (в данном случае — только для одного пользователя), и обнуляет значение `TokenForUser`. Версия с использованием клиентской библиотеки также обнуляет сохраненное значение `GraphServicesClient`, а версия с использованием REST обнуляет значения, сохраненные в параметрах роуминга приложения.

***Версия с использованием клиентской библиотеки***

Это вариант метода `Signout` с использованием клиентской библиотеки.

```c#
        public static void SignOut()
        {
            foreach (var user in IdentityClientApp.Users)
            {
                user.SignOut();
            }
            graphClient = null;
            TokenForUser = null;

        }
``` 

***Версия с использованием REST***

Это вариант метода `Signout` с использованием REST.

```c#
        public static void SignOut()
        {
            foreach (var user in IdentityClientApp.Users)
            {
                user.SignOut();
            }

            TokenForUser = null;

            //Clear stored values from last authentication.
            _settings.Values["userID"] = null;
            _settings.Values["userEmail"] = null;
            _settings.Values["userName"] = null;

        }
```

**GetAuthenticatedClient (только для клиентской библиотеки)**

Наконец, если вы используете клиентскую библиотеку, вам потребуется метод, создающий `GraphServicesClient`. Этот метод создает клиент, использующий метод `GetTokenForUserAsync` для каждого вызова Microsoft Graph через клиент.

```c#
        public static GraphServiceClient GetAuthenticatedClient()
        {
            if (graphClient == null)
            {
                // Create Microsoft Graph client.
                try
                {
                    graphClient = new GraphServiceClient(
                        "https://graph.microsoft.com/v1.0",
                        new DelegateAuthenticationProvider(
                            async (requestMessage) =>
                            {
                                var token = await GetTokenForUserAsync();
                                requestMessage.Headers.Authorization = new AuthenticationHeaderValue("bearer", token);
                            }));
                    return graphClient;
                }

                catch (Exception ex)
                {
                    Debug.WriteLine("Could not create a graph client: " + ex.Message);
                }
            }

            return graphClient;
        }
```

## <a name="send-an-email-with-microsoft-graph"></a>Отправка электронного сообщения с помощью Microsoft Graph

Откройте файл MailHelper.cs начального проекта. Этот файл содержит код для создания и отправки электронного сообщения. Он состоит из одного метода (``ComposeAndSendMailAsync``), который создает и отправляет запрос POST конечной точке **https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail**. 

Метод ``ComposeAndSendMailAsync`` принимает три строковых значения — ``subject``, ``bodyContent`` и ``recipients``, которые передаются в него из файла MainPage.xaml.cs. Строки ``subject`` и ``bodyContent`` хранятся в файле Resources.resw вместе со всеми остальными строками пользовательского интерфейса. Строка ``recipients`` отражает значение из поля "Адрес" в интерфейсе приложения. 

**Версия с использованием REST**

В версии с использованием REST этот файл должен содержать следующие объявления `using`:

```c#
using System;
using System.Threading.Tasks;
```

Так как пользователь может указать несколько адресов, строку ``recipients`` необходимо разбить на набор объектов EmailAddress, которые затем можно передать в POST-тексте запроса:

```c#
            // Prepare the recipient list
            string[] splitter = { ";" };
            var splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            string recipientsJSON = null;

            int n = 0;
            foreach (string recipient in splitRecipientsString)
            {
                if ( n==0)
                recipientsJSON += "{'EmailAddress':{'Address':'" + recipient.Trim() + "'}}";
                else
                {
                    recipientsJSON += ", {'EmailAddress':{'Address':'" + recipient.Trim() + "'}}";
                }
                n++;
            }
```

Затем необходимо создать допустимый объект JSON Message и отправить его в конечную точку **me/microsoft.graph.SendMail** с помощью HTTP-запроса POST. Так как строка ``bodyContent`` — это документ HTML, запрос задает для параметра **ContentType** значение HTML. Обратите внимание на вызов ``AuthenticationHelper.GetTokenHelperAsync`` и убедитесь, что в запросе передается новый маркер доступа.

```c#
                HttpClient client = new HttpClient();
                var token = await AuthenticationHelper.GetTokenHelperAsync();
                client.DefaultRequestHeaders.Add("Authorization", "Bearer " + token);

                // Build contents of post body and convert to StringContent object.
                // Using line breaks for readability.
                string postBody = "{'Message':{" 
                    +  "'Body':{ " 
                    + "'Content': '" + bodyContent + "'," 
                    + "'ContentType':'HTML'}," 
                    + "'Subject':'" + subject + "'," 
                    + "'ToRecipients':[" + recipientsJSON +  "]}," 
                    + "'SaveToSentItems':true}";

                var emailBody = new StringContent(postBody, System.Text.Encoding.UTF8, "application/json");

                HttpResponseMessage response = await client.PostAsync(new Uri("https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail"), emailBody);

                if ( !response.IsSuccessStatusCode)
                {

                    throw new Exception("We could not send the message: " + response.StatusCode.ToString());
                }
```

Готовый класс должен выглядеть следующим образом:

```c#
    class MailHelper
    {
        /// <summary>
        /// Compose and send a new email.
        /// </summary>
        /// <param name="subject">The subject line of the email.</param>
        /// <param name="bodyContent">The body of the email.</param>
        /// <param name="recipients">A semicolon-separated list of email addresses.</param>
        /// <returns></returns>
        internal async Task ComposeAndSendMailAsync(string subject,
                                                            string bodyContent,
                                                            string recipients)
        {

            // Prepare the recipient list
            string[] splitter = { ";" };
            var splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            string recipientsJSON = null;

            int n = 0;
            foreach (string recipient in splitRecipientsString)
            {
                if ( n==0)
                recipientsJSON += "{'EmailAddress':{'Address':'" + recipient.Trim() + "'}}";
                else
                {
                    recipientsJSON += ", {'EmailAddress':{'Address':'" + recipient.Trim() + "'}}";
                }
                n++;
            }

            try
            {

                HttpClient client = new HttpClient();
                var token = await AuthenticationHelper.GetTokenForUserAsync();
                client.DefaultRequestHeaders.Add("Authorization", "Bearer " + token);

                // Build contents of post body and convert to StringContent object.
                // Using line breaks for readability.
                string postBody = "{'Message':{" 
                    +  "'Body':{ " 
                    + "'Content': '" + bodyContent + "'," 
                    + "'ContentType':'HTML'}," 
                    + "'Subject':'" + subject + "'," 
                    + "'ToRecipients':[" + recipientsJSON +  "]}," 
                    + "'SaveToSentItems':true}";

                var emailBody = new StringContent(postBody, System.Text.Encoding.UTF8, "application/json");

                HttpResponseMessage response = await client.PostAsync(new Uri("https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail"), emailBody);

                if ( !response.IsSuccessStatusCode)
                {

                    throw new Exception("We could not send the message: " + response.StatusCode.ToString());
                }


            }

            catch (Exception e)
            {
                throw new Exception("We could not send the message: " + e.Message);
            }
        }
    }
```

**Версия с использованием клиентской библиотеки**

В версии с использованием клиентской библиотеки этот файл должен содержать следующие объявления `using`:

```c#
using System;
using System.Collections.Generic;
using System.Threading.Tasks;
```

Код для отправки сообщения с использованием клиентской библиотеки во многом аналогичен коду с использованием вызовов REST. Вместо того чтобы создавать объекты JSON и передавать их непосредственно конечной точке **SendMail** с помощью HTTP-запроса POST, вы можете создать эквивалентные объекты, определенные в клиентской библиотеке, и передать полученный объект `Message` методу `SendMail` объекта `GraphServiceClient`. Клиент получает маркер доступа и передает запрос конечной точке **SendMail**.

Готовый класс должен выглядеть следующим образом:

```c#
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
                        Content = bodyContent,
                        ContentType = BodyType.Html,
                    },
                    Subject = subject,
                    ToRecipients = recipientList,
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
    }
``` 

##<a name="create-the-user-interface-in-mainpagexaml"></a>Создание пользовательского интерфейса в файле MainPage.xaml

Теперь, когда вы написали код, полностью выполняющий проверку подлинности пользователя и отправляющий сообщение через Microsoft Graph, остается создать простой интерфейс, описанный ниже. 

Файл MainPage.xaml начального проекта уже включает весь необходимый код XAML. Вам остается только добавить код интерфейса в файл MainPage.xaml.cs. Найдите этот файл в проекте и откройте его.

Этот файл уже содержит все объявления `using`, необходимые для обеих версий примера.

***Версия с использованием клиентской библиотеки***

Приложение, использующее клиентскую библиотеку, создает объект `GraphServiceClient`, когда пользователь проходит проверку подлинности. 

Добавьте этот код в пространство имен, чтобы завершить создание класса MainPage, использующего клиентскую библиотеку, в файле MainPage.xaml.cs:

```c#
    public sealed partial class MainPage : Page
    {
        private string _mailAddress;
        private string _displayName = null;
        private MailHelper _mailHelper = new MailHelper();

        public MainPage()
        {
            this.InitializeComponent();
        }

        protected override void OnNavigatedTo(NavigationEventArgs e)
        {
            // Developer code - if you haven't registered the app yet, we warn you. 
            if (!App.Current.Resources.ContainsKey("ida:ClientID"))
            {
                InfoText.Text = ResourceLoader.GetForCurrentView().GetString("NoClientIdMessage");
                ConnectButton.IsEnabled = false;
            }
            else
            {
                InfoText.Text = ResourceLoader.GetForCurrentView().GetString("ConnectPrompt");
                ConnectButton.IsEnabled = true;
            }
        }

        /// <summary>
        /// Signs in the current user.
        /// </summary>
        /// <returns></returns>
        public async Task<bool> SignInCurrentUserAsync()
        {
            var graphClient = AuthenticationHelper.GetAuthenticatedClient();

            if (graphClient != null)
            {
                var user = await graphClient.Me.Request().GetAsync();
                string userId = user.Id;
                _mailAddress = user.UserPrincipalName;
                _displayName = user.DisplayName;
                return true;
            }
            else
            {
                return false;
            }

        }


        private async void ConnectButton_Click(object sender, RoutedEventArgs e)
        {
            ProgressBar.Visibility = Visibility.Visible;
            if (await SignInCurrentUserAsync())
            { 
                InfoText.Text = "Hi " + _displayName + "," + Environment.NewLine + ResourceLoader.GetForCurrentView().GetString("SendMailPrompt");
                MailButton.IsEnabled = true;
                EmailAddressBox.IsEnabled = true;
                ConnectButton.Visibility = Visibility.Collapsed;
                DisconnectButton.Visibility = Visibility.Visible;
                EmailAddressBox.Text = _mailAddress;
            }
            else
            {
                InfoText.Text = ResourceLoader.GetForCurrentView().GetString("AuthenticationErrorMessage");
            }

            ProgressBar.Visibility = Visibility.Collapsed;
        }

        private async void MailButton_Click(object sender, RoutedEventArgs e)
        {
            _mailAddress = EmailAddressBox.Text;
            ProgressBar.Visibility = Visibility.Visible;
            MailStatus.Text = string.Empty;
            try
            {
                await _mailHelper.ComposeAndSendMailAsync(ResourceLoader.GetForCurrentView().GetString("MailSubject"), ComposePersonalizedMail(_displayName), _mailAddress);
                MailStatus.Text = string.Format(ResourceLoader.GetForCurrentView().GetString("SendMailSuccess"), _mailAddress);
            }
            catch (Exception)
            {
                MailStatus.Text = ResourceLoader.GetForCurrentView().GetString("MailErrorMessage");
            }
            finally
            {
                ProgressBar.Visibility = Visibility.Collapsed;
            }
            
        }

        // <summary>
        // Personalizes the email.
        // </summary>
        public static string ComposePersonalizedMail(string userName)
        {
            return String.Format(ResourceLoader.GetForCurrentView().GetString("MailContents"), userName);
        }

        private void Disconnect_Click(object sender, RoutedEventArgs e)
        {
            ProgressBar.Visibility = Visibility.Visible;
            AuthenticationHelper.SignOut();
            ProgressBar.Visibility = Visibility.Collapsed;
            MailButton.IsEnabled = false;
            EmailAddressBox.IsEnabled = false;
            ConnectButton.Visibility = Visibility.Visible;
            InfoText.Text = ResourceLoader.GetForCurrentView().GetString("ConnectPrompt");
            this._displayName = null;
            this._mailAddress = null;
        }
    }
```

***Версия с использованием REST***

Вариант этого класса с использованием REST во многом подобен варианту, использующему клиентскую библиотеку, но вызывает метод `GetTokenForUserAsync` напрямую, когда пользователь проходит проверку подлинности. Он также получает данные пользователя из параметров роуминга приложения. 

Добавьте этот код в пространство имен, чтобы завершить создание класса MainPage, использующего REST, в файле MainPage.xaml.cs:

```c#
    public sealed partial class MainPage : Page
    {
        private string _mailAddress;
        private string _displayName = null;
        private MailHelper _mailHelper = new MailHelper();
        public static ApplicationDataContainer _settings = ApplicationData.Current.RoamingSettings;

        public MainPage()
        {
            this.InitializeComponent();
        }

        protected override void OnNavigatedTo(NavigationEventArgs e)
        {
            // Developer code - if you haven't registered the app yet, we warn you. 
            if (!App.Current.Resources.ContainsKey("ida:ClientID"))
            {
                InfoText.Text = ResourceLoader.GetForCurrentView().GetString("NoClientIdMessage");
                ConnectButton.IsEnabled = false;
            }
            else
            {
                InfoText.Text = ResourceLoader.GetForCurrentView().GetString("ConnectPrompt");
                ConnectButton.IsEnabled = true;
            }
        }

        /// <summary>
        /// Signs in the current user.
        /// </summary>
        /// <returns></returns>
        public async Task<bool> SignInCurrentUserAsync()
        {
            var token = await AuthenticationHelper.GetTokenForUserAsync();

            if (token != null)
            {
                string userId = (string)_settings.Values["userID"];
                _mailAddress = (string)_settings.Values["userEmail"];
                _displayName = (string)_settings.Values["userName"];
                return true;
            }
            else
            {
                return false;
            }

        }


        private async void ConnectButton_Click(object sender, RoutedEventArgs e)
        {
            ProgressBar.Visibility = Visibility.Visible;
            if (await SignInCurrentUserAsync())
            { 
                InfoText.Text = "Hi " + _displayName + "," + Environment.NewLine + ResourceLoader.GetForCurrentView().GetString("SendMailPrompt");
                MailButton.IsEnabled = true;
                EmailAddressBox.IsEnabled = true;
                ConnectButton.Visibility = Visibility.Collapsed;
                DisconnectButton.Visibility = Visibility.Visible;
                EmailAddressBox.Text = _mailAddress;
            }
            else
            {
                InfoText.Text = ResourceLoader.GetForCurrentView().GetString("AuthenticationErrorMessage");
            }

            ProgressBar.Visibility = Visibility.Collapsed;
        }

        private async void MailButton_Click(object sender, RoutedEventArgs e)
        {
            _mailAddress = EmailAddressBox.Text;
            ProgressBar.Visibility = Visibility.Visible;
            MailStatus.Text = string.Empty;
            try
            {
                await _mailHelper.ComposeAndSendMailAsync(ResourceLoader.GetForCurrentView().GetString("MailSubject"), ComposePersonalizedMail(_displayName), _mailAddress);
                MailStatus.Text = string.Format(ResourceLoader.GetForCurrentView().GetString("SendMailSuccess"), _mailAddress);
            }
            catch (Exception)
            {
                MailStatus.Text = ResourceLoader.GetForCurrentView().GetString("MailErrorMessage");
            }
            finally
            {
                ProgressBar.Visibility = Visibility.Collapsed;
            }
            
        }

        // <summary>
        // Personalizes the email.
        // </summary>
        public static string ComposePersonalizedMail(string userName)
        {
            return String.Format(ResourceLoader.GetForCurrentView().GetString("MailContents"), userName);
        }

        private void Disconnect_Click(object sender, RoutedEventArgs e)
        {
            ProgressBar.Visibility = Visibility.Visible;
            AuthenticationHelper.SignOut();
            ProgressBar.Visibility = Visibility.Collapsed;
            MailButton.IsEnabled = false;
            EmailAddressBox.IsEnabled = false;
            ConnectButton.Visibility = Visibility.Visible;
            InfoText.Text = ResourceLoader.GetForCurrentView().GetString("ConnectPrompt");
            this._displayName = null;
            this._mailAddress = null;
        }
    }
```
 
Вы выполнили три действия, необходимых для взаимодействия с Microsoft Graph: регистрацию приложения, проверку подлинности пользователя и создание запроса. 

## <a name="run-the-app"></a>Запуск приложения
1. Нажмите клавишу F5 для сборки и запуска приложения. 

2. Войдите с помощью личной, рабочей или учебной учетной записи и предоставьте необходимые разрешения.

3. Нажмите кнопку **Отправить сообщение**. Под кнопкой появится сообщение, что отправка выполнена успешно.

## <a name="next-steps"></a>Дальнейшие действия
- Опробуйте REST API с помощью [песочницы Graph](https://graph.microsoft.io/graph-explorer).
- Найдите примеры распространенных операций как для REST, так и для пакета SDK, во [фрагментах кода Microsoft Graph для UWP (пакет SDK)](https://github.com/microsoftgraph/uwp-csharp-snippets-sample) и [фрагментах кода Microsoft Graph для UWP (REST)](https://github.com/microsoftgraph/uwp-csharp-snippets-rest-sample) или изучите другие [примеры UWP](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=uwp) на сайте GitHub.

## <a name="see-also"></a>См. также
- [Клиентская библиотека .NET Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [Протоколы Azure AD версии 2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Маркеры Azure AD версии 2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)

