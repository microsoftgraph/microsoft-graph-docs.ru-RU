# <a name="get-started-with-microsoft-graph-in-an-ios-app"></a><span data-ttu-id="ec4ee-101">Начало работы с Microsoft Graph в приложении для iOS</span><span class="sxs-lookup"><span data-stu-id="ec4ee-101">Get started with Microsoft Graph in an iOS App</span></span>

> <span data-ttu-id="ec4ee-p101">**Создаете приложения для корпоративных клиентов?** Ваше приложение может не работать, если корпоративный клиент включит функции корпоративной безопасности для мобильных устройств, например <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">условный доступ с устройств</a>. В этом случае у пользователей могут возникать ошибки, а вы не будете об этом знать.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="ec4ee-p102">Для поддержки **всех корпоративных клиентов** в **любых корпоративных сценариях** необходимо использовать конечную точку Azure AD и управлять приложениями с помощью [портала управления Azure](https://aka.ms/aadapplist). Дополнительные сведения см. в разделе [Выбор между конечными точками Azure AD и Azure AD версии 2.0](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure Management Portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="ec4ee-p103">В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из [конечной точки Azure AD версии 2.0](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) и вызвать Microsoft Graph. В ней представлен разбор кода [приложения Office 365 Connect для iOS (пакет SDK)](https://github.com/microsoftgraph/ios-objectivec-connect-sample) и рассматриваются основные понятия, которые необходимо реализовать в приложении, использующем Microsoft Graph. Кроме того, в ней описывается доступ к Microsoft Graph с помощью [пакета SDK Microsoft Graph для iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (SDK)](https://github.com/microsoftgraph/ios-objectivec-connect-sample) to explain the main concepts that you have to implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using the [Microsoft Graph SDK for iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).</span></span>

<span data-ttu-id="ec4ee-110">Вы можете скачать подходящую вам версию приложения из следующего репозитория GitHub:</span><span class="sxs-lookup"><span data-stu-id="ec4ee-110">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="ec4ee-111">Приложение Office 365 Connect для iOS, использующее пакет SDK Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ec4ee-111">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-objectivec-connect-sample)

<span data-ttu-id="ec4ee-112">На приведенном ниже рисунке показано создаваемое приложение.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-112">The following image shows the app you'll create.</span></span>

![В пошаговом руководстве по этому примеру показаны подключение и отправка электронного сообщения в приложении](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="ec4ee-114">Рабочий процесс состоит из подключения к Microsoft Graph, проверки подлинности, входа с помощью рабочей или личной учетной записи и отправки сообщения получателю.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-114">The workflow will be to connect/authenticate to Microsoft Graph, sign in with your work or personal account, and finally send a mail to a recipient.</span></span>

<span data-ttu-id="ec4ee-p104">**Не хотите создавать приложение?** С помощью [краткого руководства по Microsoft Graph](https://graph.microsoft.io/en-us/getting-started) вы сможете быстро приступить к работе.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/en-us/getting-started) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec4ee-117">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ec4ee-117">Prerequisites</span></span>

<span data-ttu-id="ec4ee-118">Чтобы приступить к работе, вам понадобится следующее:</span><span class="sxs-lookup"><span data-stu-id="ec4ee-118">To get started, you'll need:</span></span> 

* <span data-ttu-id="ec4ee-119">[Xcode](https://developer.apple.com/xcode/downloads/) от Apple.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-119">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="ec4ee-120">Установка [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) в качестве диспетчера зависимостей.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-120">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="ec4ee-121">[Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](http://dev.office.com/devprogram).</span><span class="sxs-lookup"><span data-stu-id="ec4ee-121">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
* <span data-ttu-id="ec4ee-p105">[Начальный проект Microsoft Graph для iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample). Этот шаблон содержит классы, в которые вы можете добавлять код. Чтобы получить этот проект, клонируйте или скачайте пример проекта из этого расположения и используйте рабочую область в папке **starter-project** (**O365-iOS-Microsoft-Graph-SDK.xcworkspace**).</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p105">The [Microsoft Graph Starter Project for iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample). This template contains classes that you'll add code to. To get this project, clone or download the sample project from this location, and you'll work with the workspace inside the **starter-project** folder (**O365-iOS-Microsoft-Graph-SDK.xcworkspace**).</span></span>

## <a name="register-the-app"></a><span data-ttu-id="ec4ee-125">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="ec4ee-125">Register the app</span></span>
 
1. <span data-ttu-id="ec4ee-126">Войдите на [портал регистрации приложений](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-126">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="ec4ee-127">Выберите пункт **Добавить приложение**.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-127">Select **Add an app**.</span></span>
3. <span data-ttu-id="ec4ee-128">Введите имя приложения и выберите пункт **Создать приложение**.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-128">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="ec4ee-129">Откроется страница регистрации со свойствами приложения.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-129">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="ec4ee-130">В разделе **Платформы** нажмите **Добавление платформы**.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-130">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="ec4ee-131">Выберите **мобильную платформу**.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-131">Select **Mobile platform**.</span></span>
6. <span data-ttu-id="ec4ee-p106">Скопируйте идентификатор клиента в буфер обмена. Это значение потребуется ввести в примере приложения.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p106">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="ec4ee-134">Идентификатор приложения является уникальным.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-134">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="ec4ee-135">Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-135">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="ec4ee-136">Импорт зависимостей проекта</span><span class="sxs-lookup"><span data-stu-id="ec4ee-136">Importing the project dependencies</span></span>

1. <span data-ttu-id="ec4ee-p107">Клонируйте этот репозиторий, [Приложение Office 365 Connect для iOS, использующее пакета SDK Microsoft Graph](https://github.com/microsoftgraph/ios-objectivec-connect-sample). **Помните, что вы будете использовать пример из папки starter-project, а не из корневого каталога проекта.**</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p107">Clone this repository, [Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-objectivec-connect-sample). **Remember you will use the sample in the starter-project folder and not the sample at the root of the project.**</span></span>
2. <span data-ttu-id="ec4ee-p108">Импортируйте зависимости пакета SDK Microsoft Graph и проверки подлинности с помощью CocoaPods. Этот пример приложения уже содержит файл, который добавит компоненты pod в проект. Перейдите к папке **starter-project** в приложении **Терминал**, а затем из приложения **Терминал** выполните следующую команду:</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p108">Use CocoaPods to import the Microsoft Graph SDK and authentication dependencies. This sample app already contains a podfile that will get the pods into the project. Navigate to the folder **starter-project** in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="ec4ee-p109">Вы получите подтверждение импорта компонентов pod в проект. Дополнительные сведения см. в статье [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html).</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p109">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="ec4ee-144">Включение общего доступа к цепочке ключей</span><span class="sxs-lookup"><span data-stu-id="ec4ee-144">Enable keychain sharing</span></span>
 
<span data-ttu-id="ec4ee-p110">Для Xcode 8 необходимо добавить группу цепочки ключей. В противном случае приложению не удастся получить доступ к цепочке ключей. Чтобы добавить группу цепочки ключей:</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p110">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="ec4ee-p111">На панели управления проектом в Xcode выберите нужный проект (клавиши ⌘+1).</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p111">Select the project on the project manager panel in Xcode. (⌘ + 1).</span></span>
 
2. <span data-ttu-id="ec4ee-149">Выберите проект **O365-iOS-Microsoft-Graph-SDK**.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-149">Select **O365-iOS-Microsoft-Graph-SDK**.</span></span>
 
3. <span data-ttu-id="ec4ee-150">На вкладке "Возможности" включите **общий доступ к цепочке ключей**.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-150">On the Capabilities tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="ec4ee-151">Добавьте адрес **com.microsoft.O365-iOS-Microsoft-Graph-SDK** в группы цепочек ключей.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-151">Add **com.microsoft.O365-iOS-Microsoft-Graph-SDK** to the Keychain Groups.</span></span>
 

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="ec4ee-152">Проверка подлинности с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ec4ee-152">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="ec4ee-p112">Чтобы вернуться к рабочему процессу пользовательского интерфейса, приложение должно выполнить проверку подлинности пользователя, после чего оно сможет отправить сообщение указанному пользователю. Чтобы отправлять запросы службе Microsoft Graph, необходимо указать поставщика проверки подлинности, который способен проверять подлинность HTTPS-запросов с помощью соответствующего маркера носителя OAuth 2.0. Пример проекта содержит готовый класс проверки подлинности с именем **AuthenticationProvider.m.** Мы добавим функцию, которая запрашивает (и получает) маркер доступа для вызова API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p112">To revisit the UI workflow, the app is going to have the user authenticate, and then they'll have the ability to send a mail to a specified user. To make requests against the Microsoft Graph service, an authentication provider must be supplied which is capable of authenticating HTTPS requests with an appropriate OAuth 2.0 bearer token. In the sample project there's an authentication class already stubbed out called **AuthenticationProvider.m.** We will add a function to request, and acquire, an access token for calling the Microsoft Graph API.</span></span> 

1. <span data-ttu-id="ec4ee-p113">Откройте рабочую область проекта Xcode (**O365-iOS-Microsoft-Graph-SDK.xcworkspace**) в папке **starter-project**, перейдите к папке **Authentication** и откройте файл **AuthenticationProvider.m.** Добавьте в этот класс приведенный ниже код.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p113">Open the Xcode project workspace (**O365-iOS-Microsoft-Graph-SDK.xcworkspace**) in the **starter-project** folder, and navigate to the **Authentication** folder and open the file **AuthenticationProvider.m.** Add the following code to that class.</span></span>

        -(void) connectToGraphWithClientId:(NSString *)clientId scopes:(NSArray *)scopes completion:(void (^)   (NSError *))completion{
            [NXOAuth2AuthenticationProvider setClientId:kClientId
                                              scopes:scopes];
    
    
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

2. <span data-ttu-id="ec4ee-p114">Затем добавьте метод в файл заголовка. Откройте файл **AuthenticationProvider.h** и добавьте в класс приведенный ниже код.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p114">Next add the method to the header file. Open the file **AuthenticationProvider.h** and add the following code to this class.</span></span>

        -(void) connectToGraphWithClientId:(NSString *)clientId
                            scopes:(NSArray *)scopes
                        completion:(void (^)(NSError *error))completion;



2. <span data-ttu-id="ec4ee-p115">Наконец, мы вызовем этот метод из файла **ConnectViewController.m**. Этот контроллер является представлением по умолчанию для приложения и содержит одну кнопку с надписью **Connect** (Подключиться), при нажатии который запускается проверка подлинности. Этот метод принимает два параметра: **идентификатор клиента** и **разрешения**. Далее в этой статье мы подробнее рассмотрим их. Добавьте представленное ниже действие в файл **ConnectViewController.m**.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p115">Finally we'll call this method from **ConnectViewController.m**. This controller is the default view that the app loads, and there is a single button named **Connect** that the user will tap that will initiate the authentication process. This method takes in two parameters, the **Client ID** and **scopes**, we'll discuss these in more detail below. Add the following action to **ConnectViewController.m**.</span></span>

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

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="ec4ee-165">Отправка электронного сообщения с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ec4ee-165">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="ec4ee-p116">Когда в приложении будет настроена проверка подлинности, необходимо отправить пользователю сообщение с помощью API Microsoft Graph. По умолчанию получателем будет вошедший пользователь, но вы можете указать любой адрес. Соответствующий код находится в папке **Controllers**, в классе **SendMailViewController.m.** Вы заметите, что здесь имеется другой код для пользовательского интерфейса, а также вспомогательный метод для получения данных профиля пользователя из службы Microsoft Graph. Мы сосредоточимся на методах для создания и отправки электронного сообщения.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p116">After configuring the project to be able to authenticate, the next tasks are sending a mail to a user using the Microsoft Graph API. By default the logged in user will be the recipient, but you have the ability to change it to any other recipient. The code we'll work with here is located in the **Controllers** folder and in the class **SendMailViewController.m.** You'll see that there is other code represented here for the UI, and a helper method to retrieve user profile information from the Microsoft Graph service. We'll concentrate on the methods for creating a mail message and sending that message.</span></span>

1. <span data-ttu-id="ec4ee-p117">Откройте файл **SendMailViewController.m.** из папки Controllers и добавьте в класс следующий вспомогательный метод:</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p117">Open **SendMailViewController.m.** in the Controllers folder and add the following helper method to the class:</span></span>

        // Create a sample test message to send to specified user account
        -(MSGraphMessage*) getSampleMessage{
            MSGraphMessage *message = [[MSGraphMessage alloc]init];
            MSGraphRecipient *toRecipient = [[MSGraphRecipient alloc]init];
            MSGraphEmailAddress *email = [[MSGraphEmailAddress alloc]init];
    
            email.address = self.emailAddress;
            toRecipient.emailAddress = email;
    
            NSMutableArray *toRecipients = [[NSMutableArray alloc]init];
            [toRecipients addObject:toRecipient];
    
            message.subject = NSLocalizedString(@"MAIL_SUBJECT", comment: "");
    
            MSGraphItemBody *emailBody = [[MSGraphItemBody alloc]init];
            NSString *htmlContentPath = [[NSBundle mainBundle] pathForResource:@"EmailBody" ofType:@"html"];
            NSString *htmlContentString = [NSString stringWithContentsOfFile:htmlContentPath encoding:NSUTF8StringEncoding error:nil];
    
            emailBody.content = htmlContentString;
            emailBody.contentType = [MSGraphBodyType html];
            message.body = emailBody;
    
            message.toRecipients = toRecipients;
    
            return message;
    
        }


2. <span data-ttu-id="ec4ee-p118">Откройте файл **SendMailViewController.m.** Добавьте в класс приведенный ниже метод отправки почты.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p118">Open **SendMailViewController.m.** Add the following send mail method to the class.</span></span>  

        //Send mail to the specified user in the email text field
        -(void) sendMail {   
            MSGraphMessage *message = [self getSampleMessage];
            MSGraphUserSendMailRequestBuilder *requestBuilder = [[self.graphClient me]sendMailWithMessage:message saveToSentItems:true];
            NSLog(@"%@", requestBuilder);
            MSGraphUserSendMailRequest *mailRequest = [requestBuilder request];
            [mailRequest executeWithCompletion:^(NSDictionary *response, NSError *error) {
                if(!error){
                    NSLog(@"response %@", response);
                    NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
            
                    dispatch_async(dispatch_get_main_queue(), ^{
                        self.statusTextView.text = NSLocalizedString(@"SEND_SUCCESS", comment: "");
                });
            }
            else {
                NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
                self.statusTextView.text = NSLocalizedString(@"SEND_FAILURE", comment: "");
                }
            }];
    
        }

<span data-ttu-id="ec4ee-p119">Поэтому для демонстрации метод **getSampleMessage** создает черновик сообщения HTML. Затем следующий метод, **sendMail**, выполняет запрос на отправку этого сообщения. И снова получателем по умолчанию будет вошедший пользователь.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p119">So **getSampleMessage** creates a draft HTML sample mail to use for demo purposes. The next method, **sendMail**, then takes that message and executes the request to send it. Again the default recipient is the signed-in user.</span></span>


## <a name="run-the-app"></a><span data-ttu-id="ec4ee-178">Запуск приложения</span><span class="sxs-lookup"><span data-stu-id="ec4ee-178">Run the app</span></span>
1. <span data-ttu-id="ec4ee-p120">Прежде чем запускать пример, необходимо указать идентификатор клиента, полученный во время регистрации (раздел **Регистрация приложения**). Откройте файл **AuthenticationConstants.m** в папке **Application**. Вы увидите, что в начало файла можно добавить идентификатор клиента, скопированный в ходе регистрации.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p120">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.** Open **AuthenticationConstants.m** under the **Application** folder. You'll see that the ClientID from the registration process can be added to the top of the file.:</span></span>  

        // You will set your application's clientId
        NSString * const kClientId    = @"ENTER_CLIENT_ID_HERE";
        NSString * const kScopes = @"https://graph.microsoft.com/Mail.Send, https://graph.microsoft.com/User.Read, offline_access";
<span data-ttu-id="ec4ee-p121">Примечание. Вы заметите, что для этого проекта настроены следующие разрешения: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. Эти разрешения необходимы для правильной работы приложения, в частности отправки сообщения в учетную запись почты и получения данных профиля (отображаемое имя, адрес электронной почты).</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p121">Note: You'll notice that the following permission scopes have been configured for this project: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address) require these permissions for the app to run properly.</span></span>

2. <span data-ttu-id="ec4ee-184">Запустите приложение, нажмите кнопку **Connect** (Подключиться), войдите с помощью рабочей или учебной учетной записи и предоставьте запрашиваемые разрешения.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-184">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="ec4ee-p122">Нажмите кнопку **Отправить сообщение**. Под кнопкой появится сообщение, что отправка выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="ec4ee-p122">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ec4ee-187">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="ec4ee-187">Next steps</span></span>
- <span data-ttu-id="ec4ee-188">Попробуйте REST API, используя [песочницу Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="ec4ee-188">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="ec4ee-189">Примеры распространенных операций REST и SDK вы найдете во [фрагментах кода на языке Objective C с использованием Microsoft Graph для iOS](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span><span class="sxs-lookup"><span data-stu-id="ec4ee-189">Find examples of common operations for both REST and SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="ec4ee-190">См. также</span><span class="sxs-lookup"><span data-stu-id="ec4ee-190">See also</span></span>
- [<span data-ttu-id="ec4ee-191">Microsoft Graph SDK для iOS</span><span class="sxs-lookup"><span data-stu-id="ec4ee-191">Microsoft Graph SDK for iOS</span></span>](https://github.com/microsoftgraph/msgraph-sdk-ios)
- [<span data-ttu-id="ec4ee-192">Протоколы Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="ec4ee-192">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="ec4ee-193">Маркеры Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="ec4ee-193">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
