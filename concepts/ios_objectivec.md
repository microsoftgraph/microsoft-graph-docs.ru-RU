# <a name="get-started-with-microsoft-graph-in-an-objectve-c-ios-app"></a><span data-ttu-id="7538c-101">Начало работы с Microsoft Graph в приложении для iOS на языке Objectve C</span><span class="sxs-lookup"><span data-stu-id="7538c-101">Get started with Microsoft Graph in an Objectve C iOS App</span></span>

> <span data-ttu-id="7538c-p101">**Создаете приложения для корпоративных клиентов?** Ваше приложение может не работать, если корпоративный клиент включит функции корпоративной безопасности для мобильных устройств, например <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">условный доступ с устройств</a>. В этом случае у пользователей могут возникать ошибки, а вы не будете об этом знать.</span><span class="sxs-lookup"><span data-stu-id="7538c-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="7538c-p102">Для поддержки **всех корпоративных клиентов** в **любых корпоративных сценариях** необходимо использовать конечную точку Azure AD и управлять приложениями с помощью [портала Azure](https://aka.ms/aadapplist). Дополнительные сведения см. в разделе [Выбор между конечными точками Azure AD и Azure AD версии 2.0](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span><span class="sxs-lookup"><span data-stu-id="7538c-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure Management Portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="7538c-p103">В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из [конечной точки Azure AD версии 2.0](https://developer.microsoft.com/ru-RU/graph/docs/concepts/converged_auth) и вызвать Microsoft Graph. В ней представлен разбор кода [приложения Office 365 Connect для iOS (пакет SDK)](https://github.com/microsoftgraph/ios-objectivec-connect-sample) и рассматриваются основные понятия, которые необходимо реализовать в приложении, использующем Microsoft Graph. Кроме того, в ней описывается доступ к Microsoft Graph с помощью [пакета SDK Microsoft Graph для iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).</span><span class="sxs-lookup"><span data-stu-id="7538c-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/ru-RU/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (SDK)](https://github.com/microsoftgraph/ios-objectivec-connect-sample) to explain the main concepts that you have to implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using the [Microsoft Graph SDK for iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).</span></span>

<span data-ttu-id="7538c-110">Вы можете скачать подходящую вам версию приложения из следующего репозитория GitHub:</span><span class="sxs-lookup"><span data-stu-id="7538c-110">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="7538c-111">Приложение Office 365 Connect для iOS, использующее пакет SDK Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7538c-111">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-objectivec-connect-sample)

<span data-ttu-id="7538c-112">На приведенном ниже рисунке показано создаваемое приложение.</span><span class="sxs-lookup"><span data-stu-id="7538c-112">The following image shows the app you'll create.</span></span>

![В пошаговом руководстве по этому примеру показаны подключение и отправка электронного сообщения в приложении](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="7538c-114">Рабочий процесс состоит из подключения к Microsoft Graph, проверки подлинности, входа с помощью рабочей или личной учетной записи и отправки сообщения получателю.</span><span class="sxs-lookup"><span data-stu-id="7538c-114">The workflow will be to connect/authenticate to Microsoft Graph, sign in with your work or personal account, and finally send a mail to a recipient.</span></span>

<span data-ttu-id="7538c-p104">**Не хотите создавать приложение?** С помощью [краткого руководства по Microsoft Graph](https://graph.microsoft.io/ru-RU/getting-started) вы сможете быстро приступить к работе.</span><span class="sxs-lookup"><span data-stu-id="7538c-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/ru-RU/getting-started) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7538c-117">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7538c-117">Prerequisites</span></span>

<span data-ttu-id="7538c-118">Чтобы приступить к работе, вам понадобится следующее:</span><span class="sxs-lookup"><span data-stu-id="7538c-118">To get started, you'll need:</span></span> 

* <span data-ttu-id="7538c-119">[Xcode](https://developer.apple.com/xcode/downloads/) от Apple.</span><span class="sxs-lookup"><span data-stu-id="7538c-119">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="7538c-120">Установка [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) в качестве диспетчера зависимостей.</span><span class="sxs-lookup"><span data-stu-id="7538c-120">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="7538c-121">[Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](http://dev.office.com/devprogram).</span><span class="sxs-lookup"><span data-stu-id="7538c-121">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
* <span data-ttu-id="7538c-122">[Начальный проект Microsoft Graph для iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span><span class="sxs-lookup"><span data-stu-id="7538c-122">The [Microsoft Graph Starter Project for iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> <span data-ttu-id="7538c-123">Этот шаблон содержит классы, в которые вы можете добавлять код.</span><span class="sxs-lookup"><span data-stu-id="7538c-123">This template contains classes that you'll add code to.</span></span> <span data-ttu-id="7538c-124">Чтобы получить этот проект, клонируйте или скачайте пример проекта из этого расположения и используйте рабочую область в папке **starter-project** (**ios-objectivec-connect-sample.xcworkspace**).</span><span class="sxs-lookup"><span data-stu-id="7538c-124">To get this project, clone or download the sample project from this location, and you'll work with the workspace inside the **starter-project** folder (**ios-objectivec-connect-sample.xcworkspace**).</span></span>

## <a name="register-the-app"></a><span data-ttu-id="7538c-125">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="7538c-125">Register the app</span></span>
 
1. <span data-ttu-id="7538c-126">Войдите на [портал регистрации приложений](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="7538c-126">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="7538c-127">Выберите пункт **Добавить приложение**.</span><span class="sxs-lookup"><span data-stu-id="7538c-127">Select **Add an app**.</span></span>
3. <span data-ttu-id="7538c-128">Введите имя приложения и выберите пункт **Создать приложение**.</span><span class="sxs-lookup"><span data-stu-id="7538c-128">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="7538c-129">Откроется страница регистрации со свойствами приложения.</span><span class="sxs-lookup"><span data-stu-id="7538c-129">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="7538c-130">В разделе **Платформы** нажмите **Добавление платформы**.</span><span class="sxs-lookup"><span data-stu-id="7538c-130">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="7538c-131">Выберите пункт **Собственная платформа**.</span><span class="sxs-lookup"><span data-stu-id="7538c-131">Select **Native platform**.</span></span>
6. <span data-ttu-id="7538c-p106">Скопируйте идентификатор клиента в буфер обмена. Это значение потребуется ввести в примере приложения.</span><span class="sxs-lookup"><span data-stu-id="7538c-p106">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="7538c-134">Идентификатор приложения является уникальным.</span><span class="sxs-lookup"><span data-stu-id="7538c-134">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="7538c-135">Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="7538c-135">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="7538c-136">Импорт зависимостей проекта</span><span class="sxs-lookup"><span data-stu-id="7538c-136">Importing the project dependencies</span></span>

1. <span data-ttu-id="7538c-137">Клонируйте этот репозиторий, [Приложение Office 365 Connect для iOS, использующее пакет SDK Microsoft Graph](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span><span class="sxs-lookup"><span data-stu-id="7538c-137">Clone this repository, [Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> 
><span data-ttu-id="7538c-138">ВАЖНО! Используйте пример из папки starter-project, а не из корневого каталога проекта.</span><span class="sxs-lookup"><span data-stu-id="7538c-138">IMPORTANT: Use the sample in the starter-project folder and not the sample at the root of the project.</span></span>

2. <span data-ttu-id="7538c-p107">Импортируйте зависимости пакета SDK Microsoft Graph и проверки подлинности с помощью CocoaPods. Этот пример приложения уже содержит файл, который добавит компоненты pod в проект. Перейдите к папке **starter-project** в приложении **Терминал**, а затем из приложения **Терминал** выполните следующую команду:</span><span class="sxs-lookup"><span data-stu-id="7538c-p107">Use CocoaPods to import the Microsoft Graph SDK and authentication dependencies. This sample app already contains a podfile that will get the pods into the project. Navigate to the folder **starter-project** in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="7538c-p108">Вы получите подтверждение импорта компонентов pod в проект. Дополнительные сведения см. в статье [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html).</span><span class="sxs-lookup"><span data-stu-id="7538c-p108">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="7538c-144">Включение общего доступа к цепочке ключей</span><span class="sxs-lookup"><span data-stu-id="7538c-144">Enable keychain sharing</span></span>
 
<span data-ttu-id="7538c-p109">Для Xcode 8 необходимо добавить группу цепочки ключей. В противном случае приложению не удастся получить доступ к цепочке ключей. Чтобы добавить группу цепочки ключей:</span><span class="sxs-lookup"><span data-stu-id="7538c-p109">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="7538c-p110">На панели управления проектом в Xcode выберите нужный проект (клавиши ⌘+1).</span><span class="sxs-lookup"><span data-stu-id="7538c-p110">Select the project on the project manager panel in Xcode. (⌘ + 1).</span></span>
 
2. <span data-ttu-id="7538c-149">Выберите **iOS-ObjectiveC-Connect-Sample**.</span><span class="sxs-lookup"><span data-stu-id="7538c-149">Select **iOS-ObjectiveC-Connect-Sample**.</span></span>
 
3. <span data-ttu-id="7538c-150">На вкладке "Возможности" включите **общий доступ к цепочке ключей**.</span><span class="sxs-lookup"><span data-stu-id="7538c-150">On the Capabilities tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="7538c-151">Добавьте **com.microsoft.ios-objectivec-connect-sample** в группы цепочек ключей.</span><span class="sxs-lookup"><span data-stu-id="7538c-151">Add **com.microsoft.ios-objectivec-connect-sample** to the Keychain Groups.</span></span>
 

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="7538c-152">Проверка подлинности с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7538c-152">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="7538c-p111">Чтобы вернуться к рабочему процессу пользовательского интерфейса, приложение должно выполнить проверку подлинности пользователя, после чего оно сможет отправить сообщение указанному пользователю. Чтобы отправлять запросы службе Microsoft Graph, необходимо указать поставщика проверки подлинности, который способен проверять подлинность HTTPS-запросов с помощью соответствующего маркера носителя OAuth 2.0. Пример проекта содержит готовый класс проверки подлинности с именем **AuthenticationProvider.m.** Мы добавим функцию, которая запрашивает (и получает) маркер доступа для вызова API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7538c-p111">To revisit the UI workflow, the app is going to have the user authenticate, and then they'll have the ability to send a mail to a specified user. To make requests against the Microsoft Graph service, an authentication provider must be supplied which is capable of authenticating HTTPS requests with an appropriate OAuth 2.0 bearer token. In the sample project there's an authentication class already stubbed out called **AuthenticationProvider.m.** We will add a function to request, and acquire, an access token for calling the Microsoft Graph API.</span></span> 

1. <span data-ttu-id="7538c-157">Откройте рабочую область проекта Xcode (**iOS-ObjectiveC-Connect-Sample.xcworkspace**) в папке **starter-project**, перейдите к папке **Authentication** и откройте файл **AuthenticationProvider.m.**</span><span class="sxs-lookup"><span data-stu-id="7538c-157">Open the Xcode project workspace (**iOS-ObjectiveC-Connect-Sample.xcworkspace**) in the **starter-project** folder, and navigate to the **Authentication** folder and open the file **AuthenticationProvider.m.**</span></span> <span data-ttu-id="7538c-158">Добавьте в этот класс приведенный ниже код.</span><span class="sxs-lookup"><span data-stu-id="7538c-158">Add the following code to that class.</span></span>

```objectivec
   -(void) connectToGraphWithClientId:(NSString *)clientId scopes:(NSArray *)scopes completion:(void (^)    (NSError *))completion{
      [NXOAuth2AuthenticationProvider setClientId:kClientId scopes:scopes];
      /**
      Obtains access token by performing login with UI, where viewController specifies the parent view controller.
      @param viewController The view controller to present the UI on.
      @param completionHandler The completion handler to be called when the authentication has completed.
      error should be non nil if there was no error, and should contain any error(s) that occurred.
      */

      if ([[NXOAuth2AuthenticationProvider sharedAuthProvider] loginSilent]) {
         completion(nil);
      }
      else {
         [[NXOAuth2AuthenticationProvider sharedAuthProvider] loginWithViewController:nil completion:^(NSError *error) {
            if (!error) {
               NSLog(@"Authentication successful.");
               completion(nil);
            }
            else {
               NSLog(@"Authentication failed - %@", error.localizedDescription);
               completion(error);
            }
         }];
      }
   }
```     

2. <span data-ttu-id="7538c-p113">Затем добавьте метод в файл заголовка. Откройте файл **AuthenticationProvider.h** и добавьте в класс приведенный ниже код.</span><span class="sxs-lookup"><span data-stu-id="7538c-p113">Next add the method to the header file. Open the file **AuthenticationProvider.h** and add the following code to this class.</span></span>
   ```objectivec
   -(void) connectToGraphWithClientId:(NSString *)clientId
                               scopes:(NSArray *)scopes
                           completion:(void (^)(NSError *error))completion;
   ```

2. <span data-ttu-id="7538c-p114">Наконец, мы вызовем этот метод из файла **ConnectViewController.m**. Этот контроллер является представлением по умолчанию для приложения и содержит одну кнопку с надписью **Connect** (Подключиться), при нажатии который запускается проверка подлинности. Этот метод принимает два параметра: **идентификатор клиента** и **разрешения**. Далее в этой статье мы подробнее рассмотрим их. Добавьте представленное ниже действие в файл **ConnectViewController.m**.</span><span class="sxs-lookup"><span data-stu-id="7538c-p114">Finally we'll call this method from **ConnectViewController.m**. This controller is the default view that the app loads, and there is a single button named **Connect** that the user will tap that will initiate the authentication process. This method takes in two parameters, the **Client ID** and **scopes**, we'll discuss these in more detail below. Add the following action to **ConnectViewController.m**.</span></span>

```objectivec
- (IBAction)connectTapped:(id)sender {
   [self showLoadingUI:YES];
   NSArray *scopes = [kScopes componentsSeparatedByString:@","];
   [self.authProvider connectToGraphWithClientId:kClientId scopes:scopes completion:^(NSError *error) {
   if (!error) {
      [self performSegueWithIdentifier:@"showSendMail" sender:nil];
      [self showLoadingUI:NO];
      NSLog(@"Authentication successful.");
   }
   else{
      NSLog(NSLocalizedString(@"CHECK_LOG_ERROR", error.localizedDescription));
      [self showLoadingUI:NO];
   };
  }];
}
```     

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="7538c-165">Отправка электронного сообщения с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7538c-165">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="7538c-p115">Когда в приложении будет настроена проверка подлинности, необходимо отправить пользователю сообщение с помощью API Microsoft Graph. По умолчанию получателем будет вошедший пользователь, но вы можете указать любой адрес. Соответствующий код находится в папке **Controllers**, в классе **SendMailViewController.m.** Вы заметите, что здесь имеется другой код для пользовательского интерфейса, а также вспомогательный метод для получения данных профиля пользователя из службы Microsoft Graph. Мы сосредоточимся на методах для создания и отправки электронного сообщения.</span><span class="sxs-lookup"><span data-stu-id="7538c-p115">After configuring the project to be able to authenticate, the next tasks are sending a mail to a user using the Microsoft Graph API. By default the logged in user will be the recipient, but you have the ability to change it to any other recipient. The code we'll work with here is located in the **Controllers** folder and in the class **SendMailViewController.m.** You'll see that there is other code represented here for the UI, and a helper method to retrieve user profile information from the Microsoft Graph service. We'll concentrate on the methods for creating a mail message and sending that message.</span></span>

1. <span data-ttu-id="7538c-171">Откройте файл **SendMailViewController.m.** из папки Controllers и добавьте следующий код в метод **viewDidLoad** после строки `self.graphClient = [MSGraphClient client]`:</span><span class="sxs-lookup"><span data-stu-id="7538c-171">Open **SendMailViewController.m** in the Controllers folder and add the following code to the **viewDidLoad** method, after `self.graphClient = [MSGraphClient client]`</span></span>
   ```objectivec
       [self getUserInfo:(self.emailAddress) completion:^( NSError *error) {
        if (!error) {
            [self getUserPicture:(self.emailAddress)  completion:^(UIImage *image, NSError *error) {
                if (!error) {
                    self.userPicture = image;
                } else {
                    //get the test image out of the project resources
                    self.userPicture = [UIImage imageNamed:(@"test.png")];
                }
                [self uploadPictureToOneDrive:(self.userPicture) completion:^(NSString *webUrl, NSError *error) {
                    if (!error) {
                        self.pictureWebUrl = webUrl;
                        dispatch_async(dispatch_get_main_queue(), ^{
                            self.sendMailButton.enabled = true;
                        });
                    } else {
                        dispatch_async(dispatch_get_main_queue(), ^{
                            NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
                            self.statusTextView.text = NSLocalizedString(@"PICTURE_UPLOAD_FAILURE", comment: "");
                        });
                    }
                }];
            }];
        }
    }];
   ```

1. <span data-ttu-id="7538c-172">Откройте файл **SendMailViewController.m**</span><span class="sxs-lookup"><span data-stu-id="7538c-172">Open **SendMailViewController.m.**</span></span> <span data-ttu-id="7538c-173">из папки Controllers и добавьте в класс следующий вспомогательный метод:</span><span class="sxs-lookup"><span data-stu-id="7538c-173">in the Controllers folder and add the following helper method to the class</span></span>
```objectivec
  //Create a sample test message to send to specified user account
  -(MSGraphMessage*) getSampleMessage{
      MSGraphMessage *message = [[MSGraphMessage alloc]init];
      MSGraphRecipient *toRecipient = [[MSGraphRecipient alloc]init];
      MSGraphEmailAddress *email = [[MSGraphEmailAddress alloc]init];
    
      //need to get email text field for send to!
    
      email.address = self.emailAddress;
      toRecipient.emailAddress = email;
    
      NSMutableArray *toRecipients = [[NSMutableArray alloc]init];
      [toRecipients addObject:toRecipient];
    
      message.subject = NSLocalizedString(@"MAIL_SUBJECT", comment: "");
    
      MSGraphItemBody *emailBody = [[MSGraphItemBody alloc]init];
      NSString *htmlContentPath = [[NSBundle mainBundle] pathForResource:@"EmailBody" ofType:@"html"];
      NSString *htmlContentString = [NSString stringWithContentsOfFile:htmlContentPath encoding:NSUTF8StringEncoding error:nil];
    
      emailBody.content = htmlContentString;
      NSString *replaceString = @"a href=";
      replaceString = [replaceString stringByAppendingString:(self.pictureWebUrl)];
      emailBody.content = [emailBody.content stringByReplacingOccurrencesOfString:(@"a href=%s") withString:(replaceString)];
      emailBody.contentType = [MSGraphBodyType html];
      message.body = emailBody;
    
      message.toRecipients = toRecipients;
    
      MSGraphFileAttachment *fileAttachment= [[MSGraphFileAttachment alloc]init];
      fileAttachment.oDataType = @"#microsoft.graph.fileAttachment";
      fileAttachment.contentType = @"image/png";
    
      NSString *decodedString = [UIImagePNGRepresentation(self.userPicture) base64EncodedStringWithOptions:NSDataBase64EncodingEndLineWithCarriageReturn];
    
      fileAttachment.contentBytes = decodedString;
      fileAttachment.name = @"me.png";
      message.attachments = [message.attachments arrayByAddingObject:(fileAttachment)];
      return message;
    
    }
```
3. <span data-ttu-id="7538c-174">Откройте файл **SendMailViewController.m.** Добавьте в класс приведенный ниже метод.</span><span class="sxs-lookup"><span data-stu-id="7538c-174">Open **SendMailViewController.m** Add the following method to the class.</span></span>
<span data-ttu-id="7538c-175">Метод **uploadPictureToOneDrive** отправляет аватар [пользователя](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user) из данных ресурса [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user) и возвращает URL-адрес совместного доступа, внедренный в текст электронного сообщения, отправленного приложением.</span><span class="sxs-lookup"><span data-stu-id="7538c-175">**uploadPictureToOneDrive** uploads the [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user)'s profile picture from their [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user) information and returns the web sharing Url to be embedded in the body of the email that is sent by the sample.</span></span>

  ```objectivec
  -(void) uploadPictureToOneDrive: (UIImage *) image completion:(void(^) (NSString*, NSError*))completionBlock{
    
    NSData *data = UIImagePNGRepresentation(image);
    [[[[[[[self.graphClient me]
          drive]
         root]
        children]
       driveItem:(@"me.png")]
      contentRequest]
     uploadFromData:(data) completion:^(MSGraphDriveItem *response, NSError *error) {
         
         if (!error) {
             NSString *webUrl = response.webUrl;
             completionBlock(webUrl, error);
         } else {
             dispatch_async(dispatch_get_main_queue(), ^{
                 self.statusTextView.text =  NSLocalizedString(@"USER_GET_PICTURE_FAILURE", comment: "");
                 NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
             });
         }
     }];
    }
  ```
4. <span data-ttu-id="7538c-176">Откройте файл **SendMailViewController.m** и добавьте в класс приведенный ниже метод.</span><span class="sxs-lookup"><span data-stu-id="7538c-176">Open **SendMailViewController.m** and add the following method to the class.</span></span> 
<span data-ttu-id="7538c-177">Метод **getUserPicture** возвращает аватар [пользователя](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user), если он доступен.</span><span class="sxs-lookup"><span data-stu-id="7538c-177">**getUserPicture** returns the [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user)'s profile picture if it is available.</span></span>
   ```objectivec
   -(void) getUserPicture: (NSString *)url completion:(void(^) (UIImage*, NSError*))completionBlock {
    
    [[[self.graphClient me] photoValue] downloadWithCompletion:^(NSURL *location, NSURLResponse *response, NSError *error) {
        //code
        if (!error) {
            NSData *data = [NSData dataWithContentsOfURL:location];
            UIImage *img = [[UIImage alloc] initWithData:data];
            completionBlock(img, error);
        } else{
            completionBlock(nil, error);

        }
    }];
    }

   ```
3. <span data-ttu-id="7538c-178">Откройте файл **SendMailViewcontroller.m** и добавьте в класс приведенный ниже метод.</span><span class="sxs-lookup"><span data-stu-id="7538c-178">Open **SendMailViewcontroller.m** and add the following method to the class.</span></span>
<span data-ttu-id="7538c-179">Этот метод получает ресурс [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user), который представляет пользователя, прошедшего проверку подлинности, и кэширует поля, необходимые для получения аватара пользователя и отправки электронного сообщения.</span><span class="sxs-lookup"><span data-stu-id="7538c-179">This method gets the [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user) resource representing the authenticated user and caches the fields necessary to get the user's profile picture and send an email.</span></span>
   ```objectivec
   //Retrieve the logged in user's display name and email address
   -(void) getUserInfo: (NSString *)url completion:(void(^) ( NSError*))completionBlock{
    
    [[[self.graphClient me]request]getWithCompletion:^(MSGraphUser *response, NSError *error) {
        if(!error){
            dispatch_async(dispatch_get_main_queue(), ^{
                self.emailAddress = response.userPrincipalName;
                self.emailTextField.text = self.emailAddress;
                self.headerLabel.text = [NSString stringWithFormat:(NSLocalizedString(@"HI_USER", comment "")), response.displayName];
                self.statusTextView.text =  NSLocalizedString(@"USER_INFO_LOAD_SUCCESS", comment: "");
            });

            completionBlock(nil);
        }
        else{
            dispatch_async(dispatch_get_main_queue(), ^{
                self.statusTextView.text =  NSLocalizedString(@"USER_INFO_LOAD_FAILURE", comment: "");
                NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
            });
            completionBlock(error);
        }
    }];
    
   }

   ```
3. <span data-ttu-id="7538c-180">Откройте файл **SendMailViewController.m.** Добавьте в класс приведенный ниже метод отправки почты.</span><span class="sxs-lookup"><span data-stu-id="7538c-180">Open **SendMailViewController.m** Add the following send mail method to the class.</span></span>
<span data-ttu-id="7538c-181">Для демонстрации метод **getSampleMessage** создает черновик сообщения HTML.</span><span class="sxs-lookup"><span data-stu-id="7538c-181">**getSampleMessage** creates a draft HTML sample mail to use for demo purposes.</span></span> <span data-ttu-id="7538c-182">Затем следующий метод, **sendMail**, выполняет запрос на отправку этого сообщения.</span><span class="sxs-lookup"><span data-stu-id="7538c-182">The next method, **sendMail**, then takes that message and executes the request to send it.</span></span> <span data-ttu-id="7538c-183">И снова получателем по умолчанию будет вошедший пользователь.</span><span class="sxs-lookup"><span data-stu-id="7538c-183">Again the default recipient is the signed-in user.</span></span>


  ```objectivec
   //Send mail to the specified user in the email text field
   -(void) sendMail {
    MSGraphMessage *message = [self getSampleMessage];
    MSGraphUserSendMailRequestBuilder *requestBuilder = [[self.graphClient me]sendMailWithMessage:message saveToSentItems:true];
    NSLog(@"%@", requestBuilder);
    MSGraphUserSendMailRequest *mailRequest = [requestBuilder request];
    [mailRequest executeWithCompletion:^(NSDictionary *response, NSError *error) {
        if(!error){
            NSLog(@"response %@", response);
             dispatch_async(dispatch_get_main_queue(), ^{
                self.statusTextView.text = NSLocalizedString(@"SEND_SUCCESS", comment: "");
                self.descriptionLabel.text = @"Check your inbox. You have a new message :)";
            });
        }
        else {
            dispatch_async(dispatch_get_main_queue(), ^{
                NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
                self.statusTextView.text = NSLocalizedString(@"SEND_FAILURE", comment: "");
            });
        }
    }];
   }
   ```



## <a name="run-the-app"></a><span data-ttu-id="7538c-184">Запуск приложения</span><span class="sxs-lookup"><span data-stu-id="7538c-184">Run the app</span></span>
1. <span data-ttu-id="7538c-p121">Прежде чем запускать пример, необходимо указать идентификатор клиента, полученный во время регистрации (раздел **Регистрация приложения**). Откройте файл **AuthenticationConstants.m** в папке **Application**. Вы увидите, что в начало файла можно добавить идентификатор клиента, скопированный в ходе регистрации.</span><span class="sxs-lookup"><span data-stu-id="7538c-p121">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.** Open **AuthenticationConstants.m** under the **Application** folder. You'll see that the ClientID from the registration process can be added to the top of the file.:</span></span>  
   ```objectivec
   // You will set your application's clientId
   NSString * const kClientId    = @"ENTER_YOUR_CLIENT_ID";
   NSString * const kScopes = @"https://graph.microsoft.com/User.Read, https://graph.microsoft.com/Mail.ReadWrite, https://graph.microsoft.com/Mail.Send, https://graph.microsoft.com/Files.ReadWrite";
   ```      

><span data-ttu-id="7538c-p122">Примечание. Вы заметите, что для этого проекта настроены следующие разрешения: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. Эти разрешения необходимы для правильной работы приложения, в частности отправки сообщения в учетную запись почты и получения данных профиля (отображаемое имя, адрес электронной почты).</span><span class="sxs-lookup"><span data-stu-id="7538c-p122">Note: You'll notice that the following permission scopes have been configured for this project: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address) require these permissions for the app to run properly.</span></span>

2. <span data-ttu-id="7538c-190">Запустите приложение, нажмите кнопку **Connect** (Подключиться), войдите с помощью рабочей или учебной учетной записи и предоставьте запрашиваемые разрешения.</span><span class="sxs-lookup"><span data-stu-id="7538c-190">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="7538c-p123">Нажмите кнопку **Отправить сообщение**. Под кнопкой появится сообщение, что отправка выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="7538c-p123">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7538c-193">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="7538c-193">Next steps</span></span>
- <span data-ttu-id="7538c-194">Попробуйте REST API, используя [песочницу Graph](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="7538c-194">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="7538c-195">Примеры распространенных операций REST и SDK вы найдете во [фрагментах кода на языке Objective C с использованием Microsoft Graph для iOS](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span><span class="sxs-lookup"><span data-stu-id="7538c-195">Find examples of common operations for both REST and SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="7538c-196">См. также</span><span class="sxs-lookup"><span data-stu-id="7538c-196">See also</span></span>
- [<span data-ttu-id="7538c-197">Microsoft Graph SDK для iOS</span><span class="sxs-lookup"><span data-stu-id="7538c-197">Microsoft Graph SDK for iOS</span></span>](https://github.com/microsoftgraph/msgraph-sdk-ios)
- [<span data-ttu-id="7538c-198">Протоколы Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="7538c-198">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/ru-RU/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="7538c-199">Маркеры Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="7538c-199">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/ru-RU/documentation/articles/active-directory-v2-tokens/)
