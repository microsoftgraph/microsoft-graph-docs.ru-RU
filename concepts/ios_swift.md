# <a name="get-started-with-microsoft-graph-in-a-swift-ios-app"></a>Начало работы с Microsoft Graph в приложении Swift для iOS

> **Создаете приложения для корпоративных клиентов?** Ваше приложение может не работать, если корпоративный клиент включит функции корпоративной безопасности для мобильных устройств, например <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">условный доступ с устройств</a>. В этом случае у пользователей могут возникать ошибки, а вы не будете об этом знать. 

> Для поддержки **всех корпоративных клиентов** в **любых корпоративных сценариях** необходимо использовать конечную точку Azure AD и управлять приложениями с помощью [портала Azure](https://aka.ms/aadapplist). Дополнительные сведения см. в разделе [Выбор между конечными точками Azure AD и Azure AD версии 2.0](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).

В этой статье описывается, как получить маркер доступа из [конечной точки Azure AD версии 2.0](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) и вызвать Microsoft Graph. В ней на примере кода [Office 365 Connect Sample for iOS (REST)](https://github.com/microsoftgraph/ios-swift-connect-rest-sample) рассматриваются основные понятия, которые необходимо реализовать в приложении, использующем Microsoft Graph. Кроме того, в ней описывается, как получить доступ к Microsoft Graph, используя операции REST в асинхронном шаблоне **Цепочка обещаний**. Обещания в примере внедряются с помощью CocoaPod [mxcl/PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/README.md). 

Пример был создан с помощью **XCode 9.2** и **Swift 3.2**.

Вы можете скачать подходящую вам версию приложения из следующего репозитория GitHub:

* [Приложение Office 365 Connect для iOS, использующее пакет SDK Microsoft Graph](https://github.com/microsoftgraph/ios-swift-connect-rest-sample)

Ниже показано приложение, которое вы создадите.

![Разбор примера Connect, показаны подключение и отправка сообщения в приложении](./images/iOSConnectWalkthrough.png)


Рабочий процесс выполняет аутентификацию и авторизацию для доступа к ресурсам Microsoft Graph, входит, используя рабочую или личную учетную запись, и отправляет почту получателю.

**Не хотите создавать приложение?** С помощью [краткого руководства по Microsoft Graph](https://developer.microsoft.com/en-us/graph/quick-start) вы сможете быстро приступить к работе.

## <a name="prerequisites"></a>Необходимые условия

Чтобы приступить к работе, вам понадобится следующее: 

* [Xcode](https://developer.apple.com/xcode/downloads/) от Apple;
* установить [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) в качестве диспетчера зависимостей;
* установить [Carthage](https://github.com/Carthage/Carthage) для импорта и создания библиотеки **MSAL**;
* установить Cocoapod [PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/Documentation/Installation.md); 
* [учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types).

## <a name="register-the-app"></a>Регистрация приложения
 
1. Войдите на [портал регистрации приложений](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.
2. Выберите пункт **Добавить приложение**.
3. Введите имя приложения и выберите пункт **Создать приложение**.
    
    Откроется страница регистрации со свойствами приложения.
 
4. В разделе **Платформы** нажмите **Добавление платформы**.
5. Выберите пункт **Собственная платформа**.
6. Скопируйте идентификатор клиента в буфер обмена. Это значение потребуется ввести в примере приложения.

    Идентификатор приложения является уникальным. 

7. Нажмите кнопку **Сохранить**.

## <a name="importing-the-project-dependencies"></a>Импорт зависимостей проекта

1. Клонируйте [этот репозиторий](https://github.com/microsoftgraph/ios-swift-connect-rest-sample). 


2. Используйте CocoaPods для импорта зависимостей PromiseKit. Этот пример приложения уже содержит podfile, который добавит компоненты pod в проект. Перейдите в корневую папку проекта в приложении **Терминал** и выполните следующую команду:****

        pod install

   Вы получите подтверждение импорта компонентов pod в проект. Дополнительные сведения см. в статье [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html).

## <a name="install-the-msal-authentication-framework"></a>Установка платформы аутентификации MSAL

Ознакомительная версия MSAL распространяется в виде файлов заголовков и символов с помощью Carthage. Для установки MSAL в проекте выполните следующие действия:

1. Откройте терминал Bash и перейдите к корневой папке приложения.
2. Создайте **cartfile**: скопируйте `echo "github \"AzureAD/microsoft-authentication-library-for-objc\" \"master\"" > Cartfile` в терминал и выполните команду.
3. Создайте библиотеку MSAL: скопируйте `carthage update` в терминал и выполните команду.


## <a name="enable-keychain-sharing"></a>Включение общего доступа к цепочке ключей
 
Для Xcode 8 необходимо добавить группу цепочки ключей. В противном случае приложению не удастся получить доступ к цепочке ключей. Чтобы добавить группу цепочки ключей:
 
1. На панели управления проектом в XCode выберите нужный проект (⌘ + 1).
 
2. Выберите цель **O365-iOS-Microsoft-Graph-Connect-swift**.

3. Убедитесь, что на вкладке **Общие**, в разделе **Подпись**, установлен флажок **Automatically manage signing** (Автоматически управлять подписями), а у вас есть действительный сертификат для подписи.
 
3. На вкладке **Capabilities** (Возможности) включите **Keychain Sharing** (Общий доступ к цепочке ключей).
 
4. Если **com.microsoft.O365-iOS-Microsoft-Graph-Connect-Swift-REST** нет в списке групп цепочек ключей, добавьте.

## <a name="authenticating-with-microsoft-graph"></a>Аутентификация с помощью Microsoft Graph

Далее описана последовательность действий в пользовательском интерфейсе. Приложение предлагает пользователю пройти аутентификацию. После аутентификации пользователь может отправлять почту другому пользователю. Пример использует библиотеку аутентификации **MSAL** для аутентификации HTTPS-запросов с помощью соответствующего токена OAuth 2.0 Bearer. В примере проекта класс **AuthenticationClass.swift.** импортирует библиотеку **MSAL** и получает токен доступа, необходимый для операций Microsoft Graph REST.

1. Откройте рабочую область проекта **XCode** (**Graph-iOS-Swift-Connect.xcworkspace**) и откройте файл класса **AuthenticationClass.swift**. Найдите в этом классе указанный ниже код.


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


2. Мы вызовем функцию **connectToGraph** из **ConnectViewController.swift**. Этот контроллер — загружаемое приложением представление с одной кнопкой **Connect** (Подключиться), при нажатии на которую начинается аутентификация. 

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

## <a name="send-an-email-with-microsoft-graph"></a>Отправка электронного сообщения с помощью Microsoft Graph

После подключения пользователя к Microsoft Graph пример получает адрес электронной почты, отображаемое имя и фотографию профиля прошедшего аутентификацию пользователя. Пример передает фотографию профиля в корневую папку OneDrive пользователя и запрашивает в OneDrive ссылку для общего доступа к фото. Наконец, пример публикует запрос REST в Microsoft Graph, чтобы отправить почтовое сообщение на указанный адрес электронной почты. 

Текст сообщения содержит ссылку для общего доступа к фото и само фото в виде вложенного файла изображения. Получателем по умолчанию является прошедший аутентификацию пользователь, но пример позволяет пользователю указать адрес электронной почты другого пользователя. 

Код, с которым мы будем работать, находится в классе **SendMailViewController_WithPromise.swift.** Функция `viewDidLoad()` считывает значение `self.emailTextField.text`, чтобы получить адрес электронной почты получателя, а затем запускает **цепочку обещаний**, чтобы получить фото профиля прошедшего аутентификацию пользователя. В случае отклонения обещания `sendMailButton` не включается.

1. Откройте **SendMailViewController_WithPromise.swift.** и найдите функцию `viewDidLoad`. Функция `self.userPictureWork` вызывается для запуска цепочки обещаний.

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

   

1. Найдите в классе вспомогательную функцию для создания почтового запроса:

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
2. Найдите следующие вспомогательные функции для получения фото профиля пользователя, загрузки фотографии в OneDrive и запроса ссылки для общего доступа к фото:

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

3. Найдите в классе приведенную ниже функцию отправки почты.  
 
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


## <a name="run-the-app"></a>Запуск приложения
1. Прежде чем запускать пример, необходимо указать идентификатор клиента, полученный во время регистрации (раздел **Регистрация приложения**). Откройте **Info.plist** в виде исходного кода. 

   - Замените `ENTER_CLIENT_ID_HERE` **идентификатором клиента**, полученным в процессе регистрации. Убедитесь, что значение `msal` не заменено. После замены строки значение строки массива будет выглядеть примерно так: `msal48d31887-5fad-4d73-a9f5-3c356e68a038`, где часть GUID — **ваш** идентификатор клиента:  

   Например: 

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

     превращается в... 

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

> **Примечание.** Вы заметите, что для этого проекта настроены следующие разрешения: `["https://graph.microsoft.com/Mail.ReadWrite","https://graph.microsoft.com/Mail.Send","https://graph.microsoft.com/Files.ReadWrite","https://graph.microsoft.com/User.ReadBasic.All"]` . Эти разрешения необходимы для вызова служб, используемых в этом проекте отправки почты в вашу учетную запись и получения информации профиля (отображаемого имени, адреса электронной почты), а также записи данных в корневой каталог OneDrive пользователя.

2. Запустите приложение, нажмите кнопку **Connect** (Подключиться), войдите с помощью рабочей или учебной учетной записи и предоставьте запрашиваемые разрешения.

3. Нажмите кнопку **Отправить сообщение**. Под кнопкой появится сообщение, что отправка выполнена успешно.

## <a name="next-steps"></a>Дальнейшие действия
- Опробуйте REST API, используя [песочницу Graph](https://graph.microsoft.io/graph-explorer).
- Примеры распространенных операций SDK вы найдете во [фрагментах кода на языке Objective C с использованием Microsoft Graph для iOS](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).

## <a name="see-also"></a>См. также
- [Протоколы Azure AD версии 2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Маркеры Azure AD версии 2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
