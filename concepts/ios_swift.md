# <a name="get-started-with-microsoft-graph-in-a-swift-ios-app"></a><span data-ttu-id="1d63d-101">Начало работы с Microsoft Graph в приложении Swift для iOS</span><span class="sxs-lookup"><span data-stu-id="1d63d-101">Get started with Microsoft Graph in a Swift iOS App</span></span>

> <span data-ttu-id="1d63d-p101">**Создаете приложения для корпоративных клиентов?** Ваше приложение может не работать, если корпоративный клиент включит функции корпоративной безопасности для мобильных устройств, например <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">условный доступ с устройств</a>. В этом случае у пользователей могут возникать ошибки, а вы не будете об этом знать.</span><span class="sxs-lookup"><span data-stu-id="1d63d-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="1d63d-p102">Для поддержки **всех корпоративных клиентов** в **любых корпоративных сценариях** необходимо использовать конечную точку Azure AD и управлять приложениями с помощью [портала управления Azure](https://aka.ms/aadapplist). Дополнительные сведения см. в разделе [Выбор между конечными точками Azure AD и Azure AD версии 2.0](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span><span class="sxs-lookup"><span data-stu-id="1d63d-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure Management Portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="1d63d-p103">В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из [конечной точки Azure AD версии 2.0](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) и вызвать Microsoft Graph. В ней представлен разбор кода [приложения Office 365 Connect для iOS (пакет SDK)](https://github.com/microsoftgraph/ios-swift-connect-sample) и рассматриваются основные понятия, которые необходимо реализовать в приложении, использующем Microsoft Graph. Кроме того, в ней описывается доступ к Microsoft Graph с помощью [пакета SDK Microsoft Graph для iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).</span><span class="sxs-lookup"><span data-stu-id="1d63d-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (SDK)](https://github.com/microsoftgraph/ios-swift-connect-sample) to explain the main concepts that you have to implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using the [Microsoft Graph SDK for iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).</span></span>

<span data-ttu-id="1d63d-110">Вы можете скачать подходящую вам версию приложения из следующего репозитория GitHub:</span><span class="sxs-lookup"><span data-stu-id="1d63d-110">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="1d63d-111">Приложение Office 365 Connect для iOS, использующее пакет SDK Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1d63d-111">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-objectivec-connect-sample)

<span data-ttu-id="1d63d-112">На приведенном ниже рисунке показано создаваемое приложение.</span><span class="sxs-lookup"><span data-stu-id="1d63d-112">The following image shows the app you'll create.</span></span>

![В пошаговом руководстве по этому примеру показаны подключение и отправка электронного сообщения в приложении](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="1d63d-114">Рабочий процесс состоит из подключения к Microsoft Graph, проверки подлинности, входа с помощью рабочей или личной учетной записи и отправки сообщения получателю.</span><span class="sxs-lookup"><span data-stu-id="1d63d-114">The workflow will be to connect/authenticate to Microsoft Graph, sign in with your work or personal account, and finally send a mail to a recipient.</span></span>

<span data-ttu-id="1d63d-p104">**Не хотите создавать приложение?** С помощью [краткого руководства по Microsoft Graph](https://graph.microsoft.io/en-us/getting-started) вы сможете быстро приступить к работе.</span><span class="sxs-lookup"><span data-stu-id="1d63d-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/en-us/getting-started) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d63d-117">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1d63d-117">Prerequisites</span></span>

<span data-ttu-id="1d63d-118">Чтобы приступить к работе, вам понадобится следующее:</span><span class="sxs-lookup"><span data-stu-id="1d63d-118">To get started, you'll need:</span></span> 

* <span data-ttu-id="1d63d-119">[Xcode](https://developer.apple.com/xcode/downloads/) от Apple.</span><span class="sxs-lookup"><span data-stu-id="1d63d-119">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="1d63d-120">Установка [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) в качестве диспетчера зависимостей.</span><span class="sxs-lookup"><span data-stu-id="1d63d-120">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="1d63d-121">[Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](http://dev.office.com/devprogram).</span><span class="sxs-lookup"><span data-stu-id="1d63d-121">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
* <span data-ttu-id="1d63d-122">[Начальный проект Microsoft Graph для iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span><span class="sxs-lookup"><span data-stu-id="1d63d-122">The [Microsoft Graph Starter Project for iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> <span data-ttu-id="1d63d-123">Этот шаблон содержит классы, в которые вы можете добавлять код.</span><span class="sxs-lookup"><span data-stu-id="1d63d-123">This template contains classes that you'll add code to.</span></span> <span data-ttu-id="1d63d-124">Чтобы получить этот проект, клонируйте или скачайте пример проекта из этого расположения и используйте рабочую область в папке **starter-project** (**ios-objectivec-connect-sample.xcworkspace**).</span><span class="sxs-lookup"><span data-stu-id="1d63d-124">To get this project, clone or download the sample project from this location, and you'll work with the workspace inside the **starter-project** folder (**ios-objectivec-connect-sample.xcworkspace**).</span></span>

## <a name="register-the-app"></a><span data-ttu-id="1d63d-125">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="1d63d-125">Register the app</span></span>
 
1. <span data-ttu-id="1d63d-126">Войдите на [портал регистрации приложений](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="1d63d-126">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="1d63d-127">Выберите пункт **Добавить приложение**.</span><span class="sxs-lookup"><span data-stu-id="1d63d-127">Select **Add an app**.</span></span>
3. <span data-ttu-id="1d63d-128">Введите имя приложения и выберите пункт **Создать приложение**.</span><span class="sxs-lookup"><span data-stu-id="1d63d-128">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="1d63d-129">Откроется страница регистрации со свойствами приложения.</span><span class="sxs-lookup"><span data-stu-id="1d63d-129">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="1d63d-130">В разделе **Платформы** нажмите **Добавление платформы**.</span><span class="sxs-lookup"><span data-stu-id="1d63d-130">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="1d63d-131">Выберите пункт **Собственная платформа**.</span><span class="sxs-lookup"><span data-stu-id="1d63d-131">Select **Native platform**.</span></span>
6. <span data-ttu-id="1d63d-p106">Скопируйте идентификатор клиента в буфер обмена. Это значение потребуется ввести в примере приложения.</span><span class="sxs-lookup"><span data-stu-id="1d63d-p106">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="1d63d-134">Идентификатор приложения является уникальным.</span><span class="sxs-lookup"><span data-stu-id="1d63d-134">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="1d63d-135">Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="1d63d-135">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="1d63d-136">Импорт зависимостей проекта</span><span class="sxs-lookup"><span data-stu-id="1d63d-136">Importing the project dependencies</span></span>

1. <span data-ttu-id="1d63d-137">Клонируйте этот репозиторий, [Приложение Office 365 Connect для iOS, использующее пакет SDK Microsoft Graph](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span><span class="sxs-lookup"><span data-stu-id="1d63d-137">Clone this repository, [Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> 
><span data-ttu-id="1d63d-138">ВАЖНО! Используйте пример из папки starter-project, а не из корневого каталога проекта.</span><span class="sxs-lookup"><span data-stu-id="1d63d-138">IMPORTANT: Use the sample in the starter-project folder and not the sample at the root of the project.</span></span>

2. <span data-ttu-id="1d63d-p107">Импортируйте зависимости пакета SDK Microsoft Graph и проверки подлинности с помощью CocoaPods. Этот пример приложения уже содержит файл, который добавит компоненты pod в проект. Перейдите к папке **starter-project** в приложении **Терминал**, а затем из приложения **Терминал** выполните следующую команду:</span><span class="sxs-lookup"><span data-stu-id="1d63d-p107">Use CocoaPods to import the Microsoft Graph SDK and authentication dependencies. This sample app already contains a podfile that will get the pods into the project. Navigate to the folder **starter-project** in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="1d63d-p108">Вы получите подтверждение импорта компонентов pod в проект. Дополнительные сведения см. в статье [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html).</span><span class="sxs-lookup"><span data-stu-id="1d63d-p108">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="1d63d-144">Включение общего доступа к цепочке ключей</span><span class="sxs-lookup"><span data-stu-id="1d63d-144">Enable keychain sharing</span></span>
 
<span data-ttu-id="1d63d-p109">Для Xcode 8 необходимо добавить группу цепочки ключей. В противном случае приложению не удастся получить доступ к цепочке ключей. Чтобы добавить группу цепочки ключей:</span><span class="sxs-lookup"><span data-stu-id="1d63d-p109">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="1d63d-p110">На панели управления проектом в Xcode выберите нужный проект (клавиши ⌘+1).</span><span class="sxs-lookup"><span data-stu-id="1d63d-p110">Select the project on the project manager panel in Xcode. (⌘ + 1).</span></span>
 
2. <span data-ttu-id="1d63d-149">Выберите **iOS-ObjectiveC-Connect-Sample**.</span><span class="sxs-lookup"><span data-stu-id="1d63d-149">Select **iOS-ObjectiveC-Connect-Sample**.</span></span>
 
3. <span data-ttu-id="1d63d-150">На вкладке "Возможности" включите **общий доступ к цепочке ключей**.</span><span class="sxs-lookup"><span data-stu-id="1d63d-150">On the Capabilities tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="1d63d-151">Добавьте **com.microsoft.ios-objectivec-connect-sample** в группы цепочек ключей.</span><span class="sxs-lookup"><span data-stu-id="1d63d-151">Add **com.microsoft.ios-objectivec-connect-sample** to the Keychain Groups.</span></span>

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="1d63d-152">Проверка подлинности с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1d63d-152">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="1d63d-153">Чтобы вернуться к рабочему процессу пользовательского интерфейса, приложение должно выполнить проверку подлинности пользователя, после чего оно сможет отправить сообщение указанному пользователю.</span><span class="sxs-lookup"><span data-stu-id="1d63d-153">To revisit the UI workflow, the app is going to have the user authenticate, and then they'll have the ability to send a mail to a specified user.</span></span> <span data-ttu-id="1d63d-154">Чтобы отправлять запросы службе Microsoft Graph, необходимо указать поставщика проверки подлинности, который способен выполнять аутентификацию HTTPS-запросов с помощью соответствующего токена носителя OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="1d63d-154">To make requests against the Microsoft Graph service, an authentication provider must be supplied which is capable of authenticating HTTPS requests with an appropriate OAuth 2.0 bearer token.</span></span> <span data-ttu-id="1d63d-155">Пример проекта содержит готовую структуру проверки подлинности с именем **Authentication.swift.**</span><span class="sxs-lookup"><span data-stu-id="1d63d-155">In the sample project there's an authentication structure already stubbed out called **Authentication.swift.**</span></span> <span data-ttu-id="1d63d-156">Мы добавим функцию, которая запрашивает (и получает) маркер доступа для вызова API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d63d-156">We will add a function to request, and acquire, an access token for calling the Microsoft Graph API.</span></span> 

1. <span data-ttu-id="1d63d-157">Откройте рабочую область проекта Xcode (**Graph-iOS-Swift-Connect.xcworkspace**) и откройте файл расширения структуры **Authentication.swift**. Найдите в этом расширении приведенный ниже код.</span><span class="sxs-lookup"><span data-stu-id="1d63d-157">Open the Xcode project workspace (**Graph-iOS-Swift-Connect.xcworkspace**), and open the structure extension file **Authentication.swift** Find the following code in that extension.</span></span>


  ```swift
     /**
     Authenticates to Microsoft Graph. 
     If a user has previously signed in before and not disconnected, silent log in
     will take place. 
     If not, authentication will ask for credentials
     */
    func connectToGraph(withClientId clientId: String,
                                     scopes: [String],
                                     completion:@escaping (_ error: MSGraphError?) -> Void) {
    
        // Set client ID
        NXOAuth2AuthenticationProvider.setClientId(clientId, scopes: scopes)
        
        // Try silent log in. This will attempt to sign in if there is a previous successful
        // sign in user information.
        if NXOAuth2AuthenticationProvider.sharedAuth().loginSilent() == true {
            completion(nil)
        }
        // Otherwise, present log in controller.
        else {
            NXOAuth2AuthenticationProvider.sharedAuth()
                .login(with: nil) { (error: Error?) in
                    
                    if let nserror = error {
                        completion(MSGraphError.nsErrorType(error: nserror as NSError))
                    }
                    else {
                        completion(nil)
                    }
            }
        }
    }
  ```


2. <span data-ttu-id="1d63d-158">Мы вызовем этот метод из файла **ConnectViewController.swift**.</span><span class="sxs-lookup"><span data-stu-id="1d63d-158">We'll call this method from **ConnectViewController.swift**.</span></span> <span data-ttu-id="1d63d-159">Этот контроллер является представлением по умолчанию для приложения и содержит одну кнопку с надписью **Connect** (Подключиться), при нажатии который запускается проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="1d63d-159">This controller is the default view that the app loads, and there is a single button named **Connect** that the user will tap that will initiate the authentication process.</span></span> <span data-ttu-id="1d63d-160">Этот метод принимает один параметр, **scopes**. Мы подробнее рассмотрим области далее в этой статье.</span><span class="sxs-lookup"><span data-stu-id="1d63d-160">This method takes in one parameter, the **scopes**, we'll discuss scopes in more detail below.</span></span> <span data-ttu-id="1d63d-161">Добавьте приведенное ниже действие в файл **ConnectViewController.swift**.</span><span class="sxs-lookup"><span data-stu-id="1d63d-161">Add the following action to **ConnectViewController.swift**.</span></span>

  ```swift
  // MARK: Authentication
  private extension ConnectViewController {
    func authenticate() {
        loadingUI(show: true)
        
        let clientId = ApplicationConstants.clientId
        let scopes = ApplicationConstants.scopes
        
        authentication.connectToGraph(withClientId: clientId, scopes: scopes) {
            (error) in
            
            defer {self.loadingUI(show: false)}
            
            if let graphError = error {
                switch graphError {
                case .nsErrorType(let nsError):
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    self.showError(message: NSLocalizedString("CHECK_LOG_ERROR", comment: ""))
                }
            }
            else {
                self.performSegue(withIdentifier: "showSendMail", sender: nil)
            }
        }
    }
  }

  ```

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="1d63d-162">Отправка электронного сообщения с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1d63d-162">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="1d63d-163">После настройки проекта для проверки подлинности необходимо получить электронный адрес, отображаемое имя и аватар пользователя, прошедшего проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="1d63d-163">After configuring the project to be able to authenticate, the next tasks are getting the authenticated user's email address, display name, and profile photo.</span></span> <span data-ttu-id="1d63d-164">Получив эти значения, метод отправляет аватар в OneDrive и получает URL-адрес совместного доступа для изображения.</span><span class="sxs-lookup"><span data-stu-id="1d63d-164">After the sample gets these values it uploads the profile picture to OneDrive and gets the sharing Url of the picture.</span></span> <span data-ttu-id="1d63d-165">Напоследок он отправляет сообщение пользователю с помощью API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d63d-165">Finally, it sends a mail to a user using the Microsoft Graph API.</span></span> 

<span data-ttu-id="1d63d-166">По умолчанию получателем будет вошедший пользователь, но вы можете указать любой адрес.</span><span class="sxs-lookup"><span data-stu-id="1d63d-166">By default the logged in user will be the recipient, but you have the ability to change it to any other recipient.</span></span> <span data-ttu-id="1d63d-167">Код, с которым мы будем работать, находится в классе **SendMailViewController.swift.**</span><span class="sxs-lookup"><span data-stu-id="1d63d-167">The code we'll work with here is in the class **SendMailViewController.swift.**</span></span> <span data-ttu-id="1d63d-168">Вы заметите, что там есть и другой код для пользовательского интерфейса, а также вспомогательный метод для получения данных профиля пользователя из службы Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d63d-168">You'll see that there is other code represented here for the UI, and a helper method to retrieve user profile information from the Microsoft Graph service.</span></span> <span data-ttu-id="1d63d-169">Мы сосредоточимся на методах для создания и отправки электронного сообщения.</span><span class="sxs-lookup"><span data-stu-id="1d63d-169">We'll concentrate on the methods for creating a mail message and sending that message.</span></span>

1. <span data-ttu-id="1d63d-170">Откройте класс **SendMailViewController.swift.**</span><span class="sxs-lookup"><span data-stu-id="1d63d-170">Open **SendMailViewController.swift.**</span></span>  <span data-ttu-id="1d63d-171">и найдите в нем вспомогательный метод, создающий текст сообщения:</span><span class="sxs-lookup"><span data-stu-id="1d63d-171">and find the mail body creating helper method in the class:</span></span>

  ```swift
    /**
     Creates sample email message
     
     - parameter emailAddress: recipient email address
     
     - returns: MSGraphMessage object with given recipient. The body is created from EmailBody.html
     */
    func createSampleMessage(to emailAddress: String, picLink pictureUrl: String) -> MSGraphMessage? {
        let message = MSGraphMessage()
        
        // set recipients
        
        let _ = self.userPicture
        let toRecipient = MSGraphRecipient()
        let msEmailAddress = MSGraphEmailAddress()
        msEmailAddress.address = emailAddress
        toRecipient.emailAddress = msEmailAddress
        let toRecipientList = [toRecipient]
        message.toRecipients = toRecipientList
        message.subject = NSLocalizedString("MAIL_SUBJECT", comment: "")
        let messageBody = MSGraphItemBody()
        messageBody.contentType = MSGraphBodyType.html()
        guard let emailBodyFilePath = Bundle.main.path(forResource: "EmailBody", ofType: "html") else {return nil}
        messageBody.content = try! String(contentsOfFile: emailBodyFilePath, encoding: String.Encoding.utf8)
        messageBody.content = messageBody.content.replacingOccurrences(of: "a href=%s", with: ("a href=" + pictureUrl))
        message.body = messageBody

        if let unwrappedImage = self.userPicture {
            let fileAttachment = MSGraphFileAttachment()
            let data = UIImageJPEGRepresentation(unwrappedImage, 1.0)
            fileAttachment.contentType = "image/png"
            fileAttachment.oDataType = "#microsoft.graph.fileAttachment"
            fileAttachment.contentBytes = data?.base64EncodedString()
            fileAttachment.name = "me.png"
            message.attachments.append(fileAttachment)
        }
        return message
    }

  ```
2. <span data-ttu-id="1d63d-172">Найдите приведенные ниже вспомогательные методы для получения данных пользователя и аватара, а также для отправки фотографии в OneDrive:</span><span class="sxs-lookup"><span data-stu-id="1d63d-172">find the following helper methods for getting user information, getting a profile photograph, and uploading the photograph to OneDrive:</span></span>

  ```swift
      /**
     Fetches user information such as mail and display name
     */
    func getUserInfo() {
        self.sendButton.isEnabled = false
        self.statusTextView.text = NSLocalizedString("LOADING_USER_INFO", comment: "")
        
        self.graphClient.me().request().getWithCompletion {
            (user: MSGraphUser?, error: Error?) in
            if let graphError = error {
                print(NSLocalizedString("ERROR", comment: ""), graphError)
                DispatchQueue.main.async(execute: {
                    self.statusTextView.text = NSLocalizedString("GRAPH_ERROR", comment: "")
                })
            }
            else {
                guard let userInfo = user else {
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("USER_INFO_LOAD_FAILURE", comment: "")
                    })
                    return
                }
                DispatchQueue.main.async(execute: {
                    self.emailTextField.text = userInfo.mail
                    
                    if let displayName = userInfo.displayName {
                        self.headerLabel.text = "Hi " + displayName
                    }
                    else {
                        self.headerLabel.text = NSString(format: NSLocalizedString("HI_USER", comment: "") as NSString, "") as String
                    }
                    
                    self.statusTextView.text = NSLocalizedString("USER_INFO_LOAD_SUCCESS", comment: "")
                    self.sendButton.isEnabled = true
                })
            }
        }
    }
    
    /**
     Uploads the user's profile picture (obtained via the Graph API) to the user's OneDrive drive. The OneDrive sharing url is
     returned in the completion handler.
    */
    func uploadPictureToOneDrive(uploadFile image: UIImage?, with completion: @escaping (_ result: GraphResult<String, NSError>) ->Void) {
        
        var webUrl: String = ""
        guard let unwrappedImage = image else {
            return
        }
        let data = UIImageJPEGRepresentation(unwrappedImage, 1.0)
        self.graphClient
            .me()
            .drive()
            .root()
            .children()
            .driveItem("me.png")
            .contentRequest()
            .upload(from: data, completion: {
                (driveItem: MSGraphDriveItem?, error: Error?) in
                if let nsError = error {
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("UPLOAD_PICTURE_FAILURE", comment: nsError.localizedDescription)
                    })
                    return

                } else {
                    webUrl = (driveItem?.webUrl)!
                    completion(.success(webUrl))
                }
            })
    }


    /**
     Gets the user's profile picture. Returns the picture as a UIImage via completion handler
    */
    func getUserPicture(forUser upn: String, with completion: @escaping (_ result: GraphResult<UIImage, NSError>) -> Void) {
        
        //Asynchronous Graph call. Closure is invoked after getUserPicture completes. Requires @escaping attribute
        self.graphClient.me().photoValue().download {
            (url: URL?, response: URLResponse?, error: Error?) in
            
                if let nsError = error {
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("GET_PICTURE_FAILURE", comment: nsError.localizedDescription)
                    })
                    return
                }
                guard let picUrl = url else {
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("GET_PICTURE_FAILURE", comment: "User profile picture is nil")
                    })
                    return
                }
                print(picUrl)
            
                let picData = NSData(contentsOf: picUrl)
                let picImage = UIImage(data: picData! as Data)
            
                if let validPic = picImage {
                    completion(.success(validPic))
                }
                else {
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("GET_PICTURE_FAILURE", comment: "Picture data is invalid")
                    })
                }
            }
    }

  ```

3. <span data-ttu-id="1d63d-173">Найдите в классе приведенный ниже метод отправки почты.</span><span class="sxs-lookup"><span data-stu-id="1d63d-173">Find the following send mail method in the class.</span></span>  

  ```swift
    @IBAction func sendMail(_ sender: AnyObject) {
        guard let toEmail = self.emailTextField.text else {return}
        guard let picUrl = self.userPictureUrl else {return}
        if let message = self.createSampleMessage(to: toEmail, picLink: picUrl) {
            
            let requestBuilder = graphClient.me().sendMail(with: message, saveToSentItems: false)
            let mailRequest = requestBuilder?.request()
            
            _ = mailRequest?.execute(completion: {
                (response: [AnyHashable: Any]?, error: Error?) in
                if let nsError = error {
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("SEND_FAILURE", comment: "")
                    })
                }
                else {
                    DispatchQueue.main.async(execute: {
                        self.descriptionLabel.text = "Check your inbox. You have a new message :)"
                        self.statusTextView.text = NSLocalizedString("SEND_SUCCESS", comment: "")
                    })
                }
            })
        }
    }

  ```


## <a name="run-the-app"></a><span data-ttu-id="1d63d-174">Запуск приложения</span><span class="sxs-lookup"><span data-stu-id="1d63d-174">Run the app</span></span>
1. <span data-ttu-id="1d63d-175">Прежде чем запускать пример, необходимо указать идентификатор клиента, полученный во время регистрации (раздел **Регистрация приложения**).</span><span class="sxs-lookup"><span data-stu-id="1d63d-175">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.**</span></span> <span data-ttu-id="1d63d-176">Откройте файл **ApplicationConstants.swift**.</span><span class="sxs-lookup"><span data-stu-id="1d63d-176">Open **ApplicationConstants.swift** .</span></span> <span data-ttu-id="1d63d-177">Вы увидите, что в начале файла можно добавить идентификатор клиента, скопированный в ходе регистрации.</span><span class="sxs-lookup"><span data-stu-id="1d63d-177">You'll see that the ClientID from the registration process can be added to the top of the file.:</span></span>  

  ```swift
struct ApplicationConstants {
    static let clientId = "Enter_Client_Id_Here"
    static let scopes   = ["openid", "profile", "Mail.ReadWrite","mail.send","Files.ReadWrite","User.ReadBasic.All"]
}


  ```

> <span data-ttu-id="1d63d-p117">Примечание. Вы заметите, что для этого проекта настроены следующие разрешения: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. Эти разрешения необходимы для правильной работы приложения, в частности отправки сообщения в учетную запись почты и получения данных профиля (отображаемое имя, адрес электронной почты).</span><span class="sxs-lookup"><span data-stu-id="1d63d-p117">Note: You'll notice that the following permission scopes have been configured for this project: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address) require these permissions for the app to run properly.</span></span>

2. <span data-ttu-id="1d63d-180">Запустите приложение, нажмите кнопку **Connect** (Подключиться), войдите с помощью рабочей или учебной учетной записи и предоставьте запрашиваемые разрешения.</span><span class="sxs-lookup"><span data-stu-id="1d63d-180">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="1d63d-p118">Нажмите кнопку **Отправить сообщение**. Под кнопкой появится сообщение, что отправка выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="1d63d-p118">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1d63d-183">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1d63d-183">Next steps</span></span>
- <span data-ttu-id="1d63d-184">Попробуйте REST API, используя [песочницу Graph](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="1d63d-184">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="1d63d-185">Примеры распространенных операций REST и SDK вы найдете во [фрагментах кода на языке Objective C с использованием Microsoft Graph для iOS](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span><span class="sxs-lookup"><span data-stu-id="1d63d-185">Find examples of common operations for both REST and SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="1d63d-186">См. также</span><span class="sxs-lookup"><span data-stu-id="1d63d-186">See also</span></span>
- [<span data-ttu-id="1d63d-187">Протоколы Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="1d63d-187">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="1d63d-188">Маркеры Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="1d63d-188">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
