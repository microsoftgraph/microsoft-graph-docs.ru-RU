# <a name="get-started-with-microsoft-graph-in-a-swift-ios-app"></a><span data-ttu-id="6628a-101">Начало работы с Microsoft Graph в приложении Swift для iOS</span><span class="sxs-lookup"><span data-stu-id="6628a-101">Get started with Microsoft Graph in a Swift iOS App</span></span>

> <span data-ttu-id="6628a-p101">**Создаете приложения для корпоративных клиентов?** Ваше приложение может не работать, если корпоративный клиент включит функции корпоративной безопасности для мобильных устройств, например <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">условный доступ с устройств</a>. В этом случае у пользователей могут возникать ошибки, а вы не будете об этом знать.</span><span class="sxs-lookup"><span data-stu-id="6628a-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="6628a-p102">Для поддержки **всех корпоративных клиентов** в **любых корпоративных сценариях** необходимо использовать конечную точку Azure AD и управлять приложениями с помощью [портала Azure](https://aka.ms/aadapplist). Дополнительные сведения см. в разделе [Выбор между конечными точками Azure AD и Azure AD версии 2.0](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span><span class="sxs-lookup"><span data-stu-id="6628a-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="6628a-p103">В этой статье описывается, как получить маркер доступа из [конечной точки Azure AD версии 2.0](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) и вызвать Microsoft Graph. В ней на примере кода [Office 365 Connect Sample for iOS (REST)](https://github.com/microsoftgraph/ios-swift-connect-rest-sample) рассматриваются основные понятия, которые необходимо реализовать в приложении, использующем Microsoft Graph. Кроме того, в ней описывается, как получить доступ к Microsoft Graph, используя операции REST в асинхронном шаблоне **Цепочка обещаний**. Обещания в примере внедряются с помощью CocoaPod [mxcl/PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/README.md).</span><span class="sxs-lookup"><span data-stu-id="6628a-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (REST)](https://github.com/microsoftgraph/ios-swift-connect-rest-sample) to explain the main concepts that you implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using REST operations in an asynchronous **Promise chain** pattern.  Promises in the sample are implemented by using the [mxcl/PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/README.md) CocoaPod.</span></span> 

<span data-ttu-id="6628a-111">Пример был создан с помощью **XCode 9.2** и **Swift 3.2**.</span><span class="sxs-lookup"><span data-stu-id="6628a-111">The sample was created using **XCode 9.2** and **Swift 3.2**.</span></span>

<span data-ttu-id="6628a-112">Вы можете скачать подходящую вам версию приложения из следующего репозитория GitHub:</span><span class="sxs-lookup"><span data-stu-id="6628a-112">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="6628a-113">Приложение Office 365 Connect для iOS, использующее пакет SDK Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6628a-113">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-swift-connect-rest-sample)

<span data-ttu-id="6628a-114">Ниже показано приложение, которое вы создадите.</span><span class="sxs-lookup"><span data-stu-id="6628a-114">The following image shows the app you'll create.</span></span>

![Разбор примера Connect, показаны подключение и отправка сообщения в приложении](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="6628a-116">Рабочий процесс выполняет аутентификацию и авторизацию для доступа к ресурсам Microsoft Graph, входит, используя рабочую или личную учетную запись, и отправляет почту получателю.</span><span class="sxs-lookup"><span data-stu-id="6628a-116">The workflow authenticates and authorizes the sample to access  Microsoft Graph resources, signs in with your work or personal account, and finally sends a mail to a recipient.</span></span>

<span data-ttu-id="6628a-p104">**Не хотите создавать приложение?** С помощью [краткого руководства по Microsoft Graph](https://developer.microsoft.com/en-us/graph/quick-start) вы сможете быстро приступить к работе.</span><span class="sxs-lookup"><span data-stu-id="6628a-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://developer.microsoft.com/en-us/graph/quick-start) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6628a-119">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="6628a-119">Prerequisites</span></span>

<span data-ttu-id="6628a-120">Чтобы приступить к работе, вам понадобится следующее:</span><span class="sxs-lookup"><span data-stu-id="6628a-120">To get started, you'll need:</span></span> 

* <span data-ttu-id="6628a-121">[Xcode](https://developer.apple.com/xcode/downloads/) от Apple;</span><span class="sxs-lookup"><span data-stu-id="6628a-121">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="6628a-122">установить [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) в качестве диспетчера зависимостей;</span><span class="sxs-lookup"><span data-stu-id="6628a-122">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="6628a-123">установить [Carthage](https://github.com/Carthage/Carthage) для импорта и создания библиотеки **MSAL**;</span><span class="sxs-lookup"><span data-stu-id="6628a-123">Installation of [Carthage](https://github.com/Carthage/Carthage) to import and build the **MSAL** library.</span></span>
* <span data-ttu-id="6628a-124">установить Cocoapod [PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/Documentation/Installation.md);</span><span class="sxs-lookup"><span data-stu-id="6628a-124">Installation of the [PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/Documentation/Installation.md) Cocoapod.</span></span> 
* <span data-ttu-id="6628a-125">[учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types).</span><span class="sxs-lookup"><span data-stu-id="6628a-125">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types)</span></span>

## <a name="register-the-app"></a><span data-ttu-id="6628a-126">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="6628a-126">Register the app</span></span>
 
1. <span data-ttu-id="6628a-127">Войдите на [портал регистрации приложений](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="6628a-127">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="6628a-128">Выберите пункт **Добавить приложение**.</span><span class="sxs-lookup"><span data-stu-id="6628a-128">Select **Add an app**.</span></span>
3. <span data-ttu-id="6628a-129">Введите имя приложения и выберите пункт **Создать приложение**.</span><span class="sxs-lookup"><span data-stu-id="6628a-129">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="6628a-130">Откроется страница регистрации со свойствами приложения.</span><span class="sxs-lookup"><span data-stu-id="6628a-130">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="6628a-131">В разделе **Платформы** нажмите **Добавление платформы**.</span><span class="sxs-lookup"><span data-stu-id="6628a-131">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="6628a-132">Выберите пункт **Собственная платформа**.</span><span class="sxs-lookup"><span data-stu-id="6628a-132">Select **Native platform**.</span></span>
6. <span data-ttu-id="6628a-p105">Скопируйте идентификатор клиента в буфер обмена. Это значение потребуется ввести в примере приложения.</span><span class="sxs-lookup"><span data-stu-id="6628a-p105">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="6628a-135">Идентификатор приложения является уникальным.</span><span class="sxs-lookup"><span data-stu-id="6628a-135">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="6628a-136">Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="6628a-136">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="6628a-137">Импорт зависимостей проекта</span><span class="sxs-lookup"><span data-stu-id="6628a-137">Importing the project dependencies</span></span>

1. <span data-ttu-id="6628a-138">Клонируйте [этот репозиторий](https://github.com/microsoftgraph/ios-swift-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="6628a-138">Clone this repository, [Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-swift-connect-rest-sample).</span></span> 


2. <span data-ttu-id="6628a-139">Используйте CocoaPods для импорта зависимостей PromiseKit.</span><span class="sxs-lookup"><span data-stu-id="6628a-139">Use CocoaPods to import the PromiseKit dependencies.</span></span> <span data-ttu-id="6628a-140">Этот пример приложения уже содержит podfile, который добавит компоненты pod в проект.</span><span class="sxs-lookup"><span data-stu-id="6628a-140">This sample app already contains a podfile that will get the pods into the project.</span></span> <span data-ttu-id="6628a-141">Перейдите в корневую папку проекта в приложении **Терминал** и выполните следующую команду:****</span><span class="sxs-lookup"><span data-stu-id="6628a-141">Navigate to the root folder of the project in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="6628a-p107">Вы получите подтверждение импорта компонентов pod в проект. Дополнительные сведения см. в статье [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html).</span><span class="sxs-lookup"><span data-stu-id="6628a-p107">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>

## <a name="install-the-msal-authentication-framework"></a><span data-ttu-id="6628a-144">Установка платформы аутентификации MSAL</span><span class="sxs-lookup"><span data-stu-id="6628a-144">Install the MSAL authentication framework</span></span>

<span data-ttu-id="6628a-145">Ознакомительная версия MSAL распространяется в виде файлов заголовков и символов с помощью Carthage.</span><span class="sxs-lookup"><span data-stu-id="6628a-145">The preview version of MSAL is distributed as header and symbol files using Carthage.</span></span> <span data-ttu-id="6628a-146">Для установки MSAL в проекте выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="6628a-146">To install MSAL in the project, do these steps:</span></span>

1. <span data-ttu-id="6628a-147">Откройте терминал Bash и перейдите к корневой папке приложения.</span><span class="sxs-lookup"><span data-stu-id="6628a-147">Open the Bash terminal and go to the app root folder.</span></span>
2. <span data-ttu-id="6628a-148">Создайте **cartfile**: скопируйте `echo "github \"AzureAD/microsoft-authentication-library-for-objc\" \"master\"" > Cartfile` в терминал и выполните команду.</span><span class="sxs-lookup"><span data-stu-id="6628a-148">Create a **cartfile**: Copy `echo "github \"AzureAD/microsoft-authentication-library-for-objc\" \"master\"" > Cartfile`  into the terminal and run the command.</span></span>
3. <span data-ttu-id="6628a-149">Создайте библиотеку MSAL: скопируйте `carthage update` в терминал и выполните команду.</span><span class="sxs-lookup"><span data-stu-id="6628a-149">Build the MSAL library: Copy `carthage update` into the terminal and run the command.</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="6628a-150">Включение общего доступа к цепочке ключей</span><span class="sxs-lookup"><span data-stu-id="6628a-150">Enable keychain sharing</span></span>
 
<span data-ttu-id="6628a-p109">Для Xcode 8 необходимо добавить группу цепочки ключей. В противном случае приложению не удастся получить доступ к цепочке ключей. Чтобы добавить группу цепочки ключей:</span><span class="sxs-lookup"><span data-stu-id="6628a-p109">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="6628a-153">На панели управления проектом в XCode выберите нужный проект</span><span class="sxs-lookup"><span data-stu-id="6628a-153">Select the project on the project manager panel in XCode.</span></span> <span data-ttu-id="6628a-154">(⌘ + 1).</span><span class="sxs-lookup"><span data-stu-id="6628a-154">(⌘ + 1).</span></span>
 
2. <span data-ttu-id="6628a-155">Выберите цель **O365-iOS-Microsoft-Graph-Connect-swift**.</span><span class="sxs-lookup"><span data-stu-id="6628a-155">Select the **O365-iOS-Microsoft-Graph-Connect-swift** target.</span></span>

3. <span data-ttu-id="6628a-156">Убедитесь, что на вкладке **Общие**, в разделе **Подпись**, установлен флажок **Automatically manage signing** (Автоматически управлять подписями), а у вас есть действительный сертификат для подписи.</span><span class="sxs-lookup"><span data-stu-id="6628a-156">On the **General** tab and **Signing** section, verify that **Automatically manage signing** is checked and you have a valid signing certificate.</span></span>
 
3. <span data-ttu-id="6628a-157">На вкладке **Capabilities** (Возможности) включите **Keychain Sharing** (Общий доступ к цепочке ключей).</span><span class="sxs-lookup"><span data-stu-id="6628a-157">On the **Capabilities** tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="6628a-158">Если **com.microsoft.O365-iOS-Microsoft-Graph-Connect-Swift-REST** нет в списке групп цепочек ключей, добавьте.</span><span class="sxs-lookup"><span data-stu-id="6628a-158">If **com.microsoft.O365-iOS-Microsoft-Graph-Connect-Swift-REST** is not in the list of Keychain Groups, add it.</span></span>

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="6628a-159">Аутентификация с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6628a-159">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="6628a-160">Далее описана последовательность действий в пользовательском интерфейсе. Приложение предлагает пользователю пройти аутентификацию.</span><span class="sxs-lookup"><span data-stu-id="6628a-160">The UI workflow is as follows: The app asks the user to authenticate.</span></span> <span data-ttu-id="6628a-161">После аутентификации пользователь может отправлять почту другому пользователю.</span><span class="sxs-lookup"><span data-stu-id="6628a-161">After authentication, the user can send a mail to another user.</span></span> <span data-ttu-id="6628a-162">Пример использует библиотеку аутентификации **MSAL** для аутентификации HTTPS-запросов с помощью соответствующего токена OAuth 2.0 Bearer.</span><span class="sxs-lookup"><span data-stu-id="6628a-162">To make requests against Microsoft Graph, the sample uses the **MSAL** authentication library to authenticate HTTPS requests with an appropriate OAuth 2.0 bearer token.</span></span> <span data-ttu-id="6628a-163">В примере проекта класс **AuthenticationClass.swift.**</span><span class="sxs-lookup"><span data-stu-id="6628a-163">In the sample project the **AuthenticationClass.swift.**</span></span> <span data-ttu-id="6628a-164">импортирует библиотеку **MSAL** и получает токен доступа, необходимый для операций Microsoft Graph REST.</span><span class="sxs-lookup"><span data-stu-id="6628a-164">class imports the **MSAL** library and acquires the access token needed for Microsoft Graph REST operations.</span></span>

1. <span data-ttu-id="6628a-165">Откройте рабочую область проекта **XCode** (**Graph-iOS-Swift-Connect.xcworkspace**) и откройте файл класса **AuthenticationClass.swift**. Найдите в этом классе указанный ниже код.</span><span class="sxs-lookup"><span data-stu-id="6628a-165">Open the **XCode** project workspace (**Graph-iOS-Swift-Connect.xcworkspace**), and open the class file **AuthenticationClass.swift** Find the following code in that class.</span></span>


  ```swift
     /**
     Authenticates to Microsoft Graph.
     If a user has previously signed in before and not disconnected, silent log in
     will take place.
     If not, authentication will ask for credentials
     */
    func connectToGraph(scopes: [String],
                        completion:@escaping (_ error: ApplicationConstants.MSGraphError?, _ accessToken: String) -> Bool)  {
        do {
            if let initError = self.lastInitError {
                if initError.lengthOfBytes(using: String.Encoding.ascii) > 1 {
                    throw NSError.init(domain: initError, code: 0, userInfo: nil)
                }
            }
            // We check to see if we have a current logged in user. If we don't, then we need to sign someone in.
            // We throw an interactionRequired so that we trigger the interactive signin.
            if  try authenticationProvider.users().isEmpty {
                throw NSError.init(domain: "MSALErrorDomain", code: MSALErrorCode.interactionRequired.rawValue, userInfo: nil)
            } else {
                // Acquire a token for an existing user silently
                try authenticationProvider.acquireTokenSilent(forScopes: scopes, user: authenticationProvider.users().first) { (result, error) in
                    if error == nil {
                        self.accessToken = (result?.accessToken)!
                        _ = completion(nil, self.accessToken);
                    } else {
                        //"Could not acquire token silently: \(error ?? "No error information" as! Error )"
                       var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error! as NSError), "");
                    }
                }
            }
        }  catch let error as NSError {
            // interactionRequired means we need to ask the user to sign-in. This usually happens
            // when the user's Refresh Token is expired or if the user has changed their password
            // among other possible reasons.
            if error.code == MSALErrorCode.interactionRequired.rawValue {
                authenticationProvider.acquireToken(forScopes: scopes) { (result, error) in
                    if error == nil {
                        self.accessToken = (result?.accessToken)!
                        var _ = completion(nil, self.accessToken);
                    } else  {
                        var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error! as NSError), "");
                    }
                }
            } else {
                var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error as NSError), error.localizedDescription);

            }
        } catch {
            // This is the catch all error.
            var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error as NSError), error.localizedDescription);
        }
    }

  ```


2. <span data-ttu-id="6628a-166">Мы вызовем функцию **connectToGraph** из **ConnectViewController.swift**.</span><span class="sxs-lookup"><span data-stu-id="6628a-166">We'll call the **connectToGraph** function from **ConnectViewController.swift**.</span></span> <span data-ttu-id="6628a-167">Этот контроллер — загружаемое приложением представление с одной кнопкой **Connect** (Подключиться), при нажатии на которую начинается аутентификация.</span><span class="sxs-lookup"><span data-stu-id="6628a-167">This controller is the default view that the app loads with a single button named **Connect** that the user taps to start authenticating.</span></span> 

  ```swift
// MARK: Authentication
private extension ConnectViewController {
    func authenticate() {
        loadingUI(show: true)
        let scopes = ApplicationConstants.kScopes
        AuthenticationClass.sharedInstance?.connectToGraph( scopes: scopes) {
            (result: ApplicationConstants.MSGraphError?, accessToken: String) -> Bool  in
            defer {self.loadingUI(show: false)}
            if let graphError = result {
                switch graphError {
                case .nsErrorType(let nsError):
                    print(NSLocalizedString("ERROR", comment: ""), nsError.userInfo)
                    self.showError(message: NSLocalizedString("CHECK_LOG_ERROR", comment: ""))
                }
                return false
            }
            else {
                // run on main thread!!
                DispatchQueue.main.async {
                    self.performSegue(withIdentifier: "sendMail", sender: nil)
                }
                return true
            }
        }
    }
}

  ```

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="6628a-168">Отправка электронного сообщения с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6628a-168">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="6628a-169">После подключения пользователя к Microsoft Graph пример получает адрес электронной почты, отображаемое имя и фотографию профиля прошедшего аутентификацию пользователя.</span><span class="sxs-lookup"><span data-stu-id="6628a-169">After connecting the user to Microsoft Graph, the sample gets the authenticated user's email address, display name, and profile photo.</span></span> <span data-ttu-id="6628a-170">Пример передает фотографию профиля в корневую папку OneDrive пользователя и запрашивает в OneDrive ссылку для общего доступа к фото.</span><span class="sxs-lookup"><span data-stu-id="6628a-170">The sample uploads the profile photo to the user's OneDrive root folder and asks OneDrive for the sharing Url of the picture.</span></span> <span data-ttu-id="6628a-171">Наконец, пример публикует запрос REST в Microsoft Graph, чтобы отправить почтовое сообщение на указанный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6628a-171">Finally, the sample posts a REST request to Microsoft Graph to send a mail message to the provided email address.</span></span> 

<span data-ttu-id="6628a-172">Текст сообщения содержит ссылку для общего доступа к фото и само фото в виде вложенного файла изображения.</span><span class="sxs-lookup"><span data-stu-id="6628a-172">The message body contains the picture sharing link and the picture itself as an attached image file.</span></span> <span data-ttu-id="6628a-173">Получателем по умолчанию является прошедший аутентификацию пользователь, но пример позволяет пользователю указать адрес электронной почты другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="6628a-173">The default recipient is the authenticated user, but the sample allows the user to provide the email address of any other user.</span></span> 

<span data-ttu-id="6628a-174">Код, с которым мы будем работать, находится в классе **SendMailViewController_WithPromise.swift.**</span><span class="sxs-lookup"><span data-stu-id="6628a-174">The code we'll work with here is in the class **SendMailViewController_WithPromise.swift.**</span></span> <span data-ttu-id="6628a-175">Функция `viewDidLoad()` считывает значение `self.emailTextField.text`, чтобы получить адрес электронной почты получателя, а затем запускает **цепочку обещаний**, чтобы получить фото профиля прошедшего аутентификацию пользователя.</span><span class="sxs-lookup"><span data-stu-id="6628a-175">The `viewDidLoad()` function reads the `self.emailTextField.text` value to get the mail recipient's email address and then starts a **promise chain** to get the authenticated user's profile picture.</span></span> <span data-ttu-id="6628a-176">В случае отклонения обещания `sendMailButton` не включается.</span><span class="sxs-lookup"><span data-stu-id="6628a-176">If the promise is rejected, the `sendMailButton` is not enabled.</span></span>

1. <span data-ttu-id="6628a-177">Откройте **SendMailViewController_WithPromise.swift.**</span><span class="sxs-lookup"><span data-stu-id="6628a-177">Open **SendMailViewController_WithPromise.swift.**</span></span> <span data-ttu-id="6628a-178">и найдите функцию `viewDidLoad`.</span><span class="sxs-lookup"><span data-stu-id="6628a-178">and find the `viewDidLoad` function.</span></span> <span data-ttu-id="6628a-179">Функция `self.userPictureWork` вызывается для запуска цепочки обещаний.</span><span class="sxs-lookup"><span data-stu-id="6628a-179">The `self.userPictureWork` function is called to start the promise chain.</span></span>

   ```swift
    override func viewDidLoad() {
        super.viewDidLoad()
        //Get user state values before creating mail message to be sent
        do
        {
            try self.userName = AuthenticationClass.sharedInstance?.authenticationProvider.users()[0].name!
            try self.emailTextField.text = AuthenticationClass.sharedInstance?.authenticationProvider.users()[0].displayableId
            self.userEmailAddress = self.emailTextField.text
            self.headerLabel.text = "Hi, \(self.userName! )"
            
            updateUI(showActivityIndicator: true, statusText: "Getting picture", sendMail: true)

            //Important: Break out of async promise chain by declaring result returns Void
            _ = self.userPictureWork().then{
                result -> Void in
                    self.userPictureUrl = (result[1] as! String)
                    self.userProfilePicture = (result[0] as! UIImage)
                    self.updateUI(showActivityIndicator: false, statusText: "", sendMail: true)

            }.catch{err -> Void  in
                self.updateUI(showActivityIndicator: false, statusText: "", sendMail: false)

            }
        } catch _ as NSError{
            self.updateUI(showActivityIndicator: false,
                          statusText: "Error getting user profile picture.", sendMail: false)
        }
    }
  
   ```

   

1. <span data-ttu-id="6628a-180">Найдите в классе вспомогательную функцию для создания почтового запроса:</span><span class="sxs-lookup"><span data-stu-id="6628a-180">Find the mail request creation helper function in the class:</span></span>

   ```swift
    /**
     Prepare mail content by loading the JSON request payload template and HTML message body template from resources and replacing placeholders in the templates with appropriate values.
     */
    func mailContent() -> Data? {
        if let emailFilePath = Bundle.main.path(forResource: "EmailPostContent", ofType: "json"),
            let emailBodyFilePath = Bundle.main.path(forResource: "EmailBody", ofType: "html")
        {
            do {
                // Prepare upload content
                let emailContent = try String(contentsOfFile: emailFilePath, encoding: String.Encoding.utf8)
                let emailBodyRaw = try String(contentsOfFile: emailBodyFilePath, encoding: String.Encoding.utf8)
                // Request doesn't accept a single quotation mark("), so change it to the acceptable form (\")
                var emailValidBody: String;
                emailValidBody = emailBodyRaw.replacingOccurrences(of: "\"", with: "\\\"")
                emailValidBody = emailValidBody.replacingOccurrences(of: "a href=%s", with: ("a href=" + self.userPictureUrl!))
                let imageData: NSData = UIImagePNGRepresentation(self.userProfilePicture!)! as NSData;
                let emailPostContent = emailContent.replacingOccurrences(of: "<EMAIL>", with: self.emailTextField.text!)
                    .replacingOccurrences(of: "<CONTENTTYPE>", with: "HTML")
                    .replacingOccurrences(of: "<CONTENT>", with: emailValidBody)
                    .replacingOccurrences(of: "<ODATA.TYPE>", with: "#microsoft.graph.fileAttachment")
                    .replacingOccurrences(of: "<IMAGE.TYPE>", with: "image\\/png")
                    .replacingOccurrences(of: "<CONTENTBYTES>", with: imageData.base64EncodedString())
                    .replacingOccurrences(of: "<NAME>", with: "me.png")
                // Return JSON payload with mail body as HTML string and attached picture as a file attachment of type NSData
                return emailPostContent.data(using: String.Encoding.utf8)
            }
            catch {
                // Error handling in case file loading fails.
                return nil
            }
        }
        // Error handling in case files aren't present.
        return nil
    }

   ```
2. <span data-ttu-id="6628a-181">Найдите следующие вспомогательные функции для получения фото профиля пользователя, загрузки фотографии в OneDrive и запроса ссылки для общего доступа к фото:</span><span class="sxs-lookup"><span data-stu-id="6628a-181">Find the following helper functions for getting the user's profile picture,  uploading the photograph to OneDrive, and requesting a sharing link for the picture:</span></span>

   ```swift
    /**
      Async func. Get user's profile photo, upload photo to OneDrive, and get sharing link
     - returns:
        Promise<UIImage>. The user's profile picture
     */
    func getUserPicture()->Promise<UIImage?>{
        return Promise{ fulfill, reject in
            let urlRequest = self.buildRequest(operation: "GET", resource: "photo/$value") as URLRequest
            let task = URLSession.shared.dataTask(with:urlRequest){ data , res , err in
                if let err:Error = err {
                    print(err.localizedDescription)
                    return reject(err)
                }
                if ((self.checkResult(result: res!)) != HTTPError.NoError) {
                    return fulfill(self.getDefaultPicture())
                }
                if let data = data {
                    if let userImage: UIImage = UIImage(data:data) {
                        self.userProfilePicture = userImage
                        return fulfill(userImage)
                    } else {
                        return reject("no image" as! Error)
                    }
                } else {
                    return fulfill(self.getDefaultPicture())
                }
            }
            task.resume()
        }
    }
    
    /**
     Async func. Uploads a UIImage object to the signed in user's OneDrive root folder
     - Returns:
        A Promise encapsulating an array of AnyObject. Element 0 contains the user profile photo obtained in the previous chained async call
        Element 1 contains the web sharing URL of the photo in OneDrive as a String
     - Parameters:
     - UIImage: The image to upload to OneDrive
     */
    func uploadPicture(photo: UIImage) -> Promise<[AnyObject]> {
        return Promise<[AnyObject]>{ fulfill, reject in
            let uploadRequestUrl = self.buildRequest(operation: "PUT", resource: "drive/root:/me.jpg:/content", content: UIImageJPEGRepresentation(photo, 1.0)!) as URLRequest
            let task = URLSession.shared.dataTask(with:uploadRequestUrl){ data, res, err in
                if let err = err{
                    return reject(err)
                }
                if ((self.checkResult(result: res!)) != HTTPError.NoError) {
                    return reject(HTTPError.InvalidRequest)
                }
                //data can be serialized to a DriveItem object
                //https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/driveitem
                var itemId: String = "";
                if let responseContent = data {
                    itemId = self.getValueFromResponse(json: responseContent, key: "id" )
                    var returnValues = [AnyObject]();
                    returnValues.append(photo as AnyObject)
                    returnValues.append(itemId as AnyObject)
                    return fulfill(returnValues)
                }
            }
            task.resume()
        }
    }

    /**
     Async func. Requests a new sharing link for the OneDrive item specified by the item id.
     - returns:
     - Promise<String: AnyObject>. The new sharing link and the image wrapped in a Promise
     */
    func createSharingLink(itemId: String, image: UIImage) ->Promise<[AnyObject]>{
        return Promise<[AnyObject]>{ fulfill, reject in
            //Create Data object for the JSON payload
            if let sharingLinkFilePath = Bundle.main.path(forResource: "CreateSharingLink", ofType: "json")
            {
                do {
                    let sharingLinkcontent = try String(contentsOfFile: sharingLinkFilePath, encoding: String.Encoding.utf8)
                    let jsonPayload: Data = sharingLinkcontent.data(using: String.Encoding.utf8)!
                    let uploadRequestUrl = self.buildRequest(
                        operation: "POST", resource: "drive/items/"+itemId+"/createLink", content: jsonPayload) as URLRequest
                    let task = URLSession.shared.dataTask(with:uploadRequestUrl){ data, res, err in
                        if let err = err{
                            return reject(err)
                        }
                        if ((self.checkResult(result: res!)) != HTTPError.NoError) {
                            return reject(HTTPError.InvalidRequest)
                        }
                        //data can be serialized to a DriveItem object
                        //https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/driveitem
                        var sharingLink: String = "";
                        if let responseContent = data {
                            do {
                                let resultJson = try JSONSerialization.jsonObject(
                                    with: responseContent, options: []) as? [String:AnyObject]
                                sharingLink = (OneDriveFileLink.init(json:resultJson!)?.webUrl)!

                            } catch let error as NSError {
                                print(error)
                            }
                            var returnValues = [AnyObject]();
                            returnValues.append(image as AnyObject)
                            returnValues.append(sharingLink as AnyObject)
                            return fulfill(returnValues)
                        }
                    }
                    task.resume()

                }
            }
        }
   ```

3. <span data-ttu-id="6628a-182">Найдите в классе приведенную ниже функцию отправки почты.</span><span class="sxs-lookup"><span data-stu-id="6628a-182">Find the following send mail function in the class.</span></span>  
 
   ```swift
    /**
     POSTS a new message to the sendmail resource
     - parameters:
        - Data: The body of the message
     */
    func sendMailRESTWithContent(_ content: Data) {
        let _ = self.sendCRUDMessage(resource: "microsoft.graph.sendmail",
                                     operation: "POST",
                                     content: content)
    }
    
    /**
     Send a create, read, update, delete (CRUD) message.
     Create= POST, Update= PUT, Delete= DELETE.
     Read= GET. Use sendGETMessage(resource: String) to read Graph contents
     - returns:
     JSON response as Data
     - parameters:
        - String: The REST resource receiving the CRUD request
        - String: the REST operation requested
        - Data: The json (as Data) representing the values to update
     */
    func sendCRUDMessage(resource: String, operation:String, content: Data)->Data  {
        var returnData: Data;
        returnData = Data.init();
        if  (self.connectToGraph()){
            if (operation == "GET") {
                return self.sendGETMessage(resource: resource)
            }
            let request = self.buildRequest(operation: operation, resource: resource, content:content);
            let task = URLSession.shared.dataTask(with:request as URLRequest, completionHandler:{ data, res, err in
                if let err = err{
                    self.updateUI(showActivityIndicator: false,
                             statusText: "Error assembling the mail content." + err.localizedDescription, sendMail: false)
                }
                let nttpError = self.checkResult(result: res!)
                if (nttpError != HTTPError.NoError) {
                    self.updateUI(showActivityIndicator: false,
                                  statusText: "Error sending the mail.", sendMail: false)
                }
                else {
                    self.updateUI(showActivityIndicator: false, statusText: "", sendMail: true)
                }
            }) // let task
             task.resume()
        }
        return returnData;
    }

   ```


## <a name="run-the-app"></a><span data-ttu-id="6628a-183">Запуск приложения</span><span class="sxs-lookup"><span data-stu-id="6628a-183">Run the app</span></span>
1. <span data-ttu-id="6628a-184">Прежде чем запускать пример, необходимо указать идентификатор клиента, полученный во время регистрации (раздел **Регистрация приложения**).</span><span class="sxs-lookup"><span data-stu-id="6628a-184">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.**</span></span> <span data-ttu-id="6628a-185">Откройте **Info.plist** в виде исходного кода.</span><span class="sxs-lookup"><span data-stu-id="6628a-185">Open **Info.plist** as source code.</span></span> 

   - <span data-ttu-id="6628a-186">Замените `ENTER_CLIENT_ID_HERE` **идентификатором клиента**, полученным в процессе регистрации.</span><span class="sxs-lookup"><span data-stu-id="6628a-186">Replace  `ENTER_CLIENT_ID_HERE` with the **ClientID** from the registration process.</span></span> <span data-ttu-id="6628a-187">Убедитесь, что значение `msal` не заменено.</span><span class="sxs-lookup"><span data-stu-id="6628a-187">Be sure that `msal` is not replaced.</span></span> <span data-ttu-id="6628a-188">После замены строки значение строки массива будет выглядеть примерно так: `msal48d31887-5fad-4d73-a9f5-3c356e68a038`, где часть GUID — **ваш** идентификатор клиента:</span><span class="sxs-lookup"><span data-stu-id="6628a-188">After you replace the string, the array string value looks like `msal48d31887-5fad-4d73-a9f5-3c356e68a038` where the GUID portion is **your** client Id:</span></span>  

   <span data-ttu-id="6628a-189">Например:</span><span class="sxs-lookup"><span data-stu-id="6628a-189">For example,</span></span> 

  ```xml
    <key>CFBundleURLTypes</key>
    <array>
        <dict>
            <key>CFBundleTypeRole</key>
            <string>Editor</string>
            <key>CFBundleURLName</key>
            <string>$(PRODUCT_BUNDLE_IDENTIFIER)</string>
            <key>CFBundleURLSchemes</key>
            <array>
                <string>msalENTER_CLIENT_ID_HERE</string>
                <string>auth</string>
            </array>
        </dict>
    </array>
  ```

     <span data-ttu-id="6628a-190">превращается в...</span><span class="sxs-lookup"><span data-stu-id="6628a-190">becomes...</span></span> 

  ```xml
    <key>CFBundleURLTypes</key>
    <array>
        <dict>
            <key>CFBundleTypeRole</key>
            <string>Editor</string>
            <key>CFBundleURLName</key>
            <string>$(PRODUCT_BUNDLE_IDENTIFIER)</string>
            <key>CFBundleURLSchemes</key>
            <array>
                <string>msal48d31887-5fad-4d73-a9f5-3c356e68a038</string>
                <string>auth</string>
            </array>
        </dict>
    </array>
  ```

> <span data-ttu-id="6628a-191">**Примечание.** Вы заметите, что для этого проекта настроены следующие разрешения: `["https://graph.microsoft.com/Mail.ReadWrite","https://graph.microsoft.com/Mail.Send","https://graph.microsoft.com/Files.ReadWrite","https://graph.microsoft.com/User.ReadBasic.All"]` .</span><span class="sxs-lookup"><span data-stu-id="6628a-191">**Note:** You'll notice that the following permission scopes have been configured for this project: `["https://graph.microsoft.com/Mail.ReadWrite","https://graph.microsoft.com/Mail.Send","https://graph.microsoft.com/Files.ReadWrite","https://graph.microsoft.com/User.ReadBasic.All"]` .</span></span> <span data-ttu-id="6628a-192">Эти разрешения необходимы для вызова служб, используемых в этом проекте отправки почты в вашу учетную запись и получения информации профиля (отображаемого имени, адреса электронной почты), а также записи данных в корневой каталог OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="6628a-192">The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address), and writing to the user's OneDrive root require these permissions for the app to run without a permissions error.</span></span>

2. <span data-ttu-id="6628a-193">Запустите приложение, нажмите кнопку **Connect** (Подключиться), войдите с помощью рабочей или учебной учетной записи и предоставьте запрашиваемые разрешения.</span><span class="sxs-lookup"><span data-stu-id="6628a-193">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="6628a-p120">Нажмите кнопку **Отправить сообщение**. Под кнопкой появится сообщение, что отправка выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="6628a-p120">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6628a-196">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="6628a-196">Next steps</span></span>
- <span data-ttu-id="6628a-197">Опробуйте REST API, используя [песочницу Graph](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="6628a-197">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="6628a-198">Примеры распространенных операций SDK вы найдете во [фрагментах кода на языке Objective C с использованием Microsoft Graph для iOS](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span><span class="sxs-lookup"><span data-stu-id="6628a-198">Find examples of common operations for SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="6628a-199">См. также</span><span class="sxs-lookup"><span data-stu-id="6628a-199">See also</span></span>
- [<span data-ttu-id="6628a-200">Протоколы Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="6628a-200">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="6628a-201">Маркеры Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="6628a-201">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
