# <a name="get-started-with-microsoft-graph-in-a-swift-ios-app"></a>Начало работы с Microsoft Graph в приложении Swift для iOS

> **Создаете приложения для корпоративных клиентов?** Ваше приложение может не работать, если корпоративный клиент включит функции корпоративной безопасности для мобильных устройств, например <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">условный доступ с устройств</a>. В этом случае у пользователей могут возникать ошибки, а вы не будете об этом знать. 

> Для поддержки **всех корпоративных клиентов** в **любых корпоративных сценариях** необходимо использовать конечную точку Azure AD и управлять приложениями с помощью [портала управления Azure](https://aka.ms/aadapplist). Дополнительные сведения см. в разделе [Выбор между конечными точками Azure AD и Azure AD версии 2.0](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).

В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из [конечной точки Azure AD версии 2.0](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) и вызвать Microsoft Graph. В ней представлен разбор кода [приложения Office 365 Connect для iOS (пакет SDK)](https://github.com/microsoftgraph/ios-swift-connect-sample) и рассматриваются основные понятия, которые необходимо реализовать в приложении, использующем Microsoft Graph. Кроме того, в ней описывается доступ к Microsoft Graph с помощью [пакета SDK Microsoft Graph для iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).

Вы можете скачать подходящую вам версию приложения из следующего репозитория GitHub:

* [Приложение Office 365 Connect для iOS, использующее пакет SDK Microsoft Graph](https://github.com/microsoftgraph/ios-objectivec-connect-sample)

На приведенном ниже рисунке показано создаваемое приложение.

![В пошаговом руководстве по этому примеру показаны подключение и отправка электронного сообщения в приложении](./images/iOSConnectWalkthrough.png)


Рабочий процесс состоит из подключения к Microsoft Graph, проверки подлинности, входа с помощью рабочей или личной учетной записи и отправки сообщения получателю.

**Не хотите создавать приложение?** С помощью [краткого руководства по Microsoft Graph](https://graph.microsoft.io/en-us/getting-started) вы сможете быстро приступить к работе.

## <a name="prerequisites"></a>Необходимые компоненты

Чтобы приступить к работе, вам понадобится следующее: 

* [Xcode](https://developer.apple.com/xcode/downloads/) от Apple.
* Установка [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) в качестве диспетчера зависимостей.
* [Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](http://dev.office.com/devprogram).
* [Начальный проект Microsoft Graph для iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample). Этот шаблон содержит классы, в которые вы можете добавлять код. Чтобы получить этот проект, клонируйте или скачайте пример проекта из этого расположения и используйте рабочую область в папке **starter-project** (**ios-objectivec-connect-sample.xcworkspace**).

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

1. Клонируйте этот репозиторий, [Приложение Office 365 Connect для iOS, использующее пакет SDK Microsoft Graph](https://github.com/microsoftgraph/ios-objectivec-connect-sample). 
>ВАЖНО! Используйте пример из папки starter-project, а не из корневого каталога проекта.

2. Импортируйте зависимости пакета SDK Microsoft Graph и проверки подлинности с помощью CocoaPods. Этот пример приложения уже содержит файл, который добавит компоненты pod в проект. Перейдите к папке **starter-project** в приложении **Терминал**, а затем из приложения **Терминал** выполните следующую команду:

        pod install

   Вы получите подтверждение импорта компонентов pod в проект. Дополнительные сведения см. в статье [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html).


## <a name="enable-keychain-sharing"></a>Включение общего доступа к цепочке ключей
 
Для Xcode 8 необходимо добавить группу цепочки ключей. В противном случае приложению не удастся получить доступ к цепочке ключей. Чтобы добавить группу цепочки ключей:
 
1. На панели управления проектом в Xcode выберите нужный проект (клавиши ⌘+1).
 
2. Выберите **iOS-ObjectiveC-Connect-Sample**.
 
3. На вкладке "Возможности" включите **общий доступ к цепочке ключей**.
 
4. Добавьте **com.microsoft.ios-objectivec-connect-sample** в группы цепочек ключей.

## <a name="authenticating-with-microsoft-graph"></a>Проверка подлинности с помощью Microsoft Graph

Чтобы вернуться к рабочему процессу пользовательского интерфейса, приложение должно выполнить проверку подлинности пользователя, после чего оно сможет отправить сообщение указанному пользователю. Чтобы отправлять запросы службе Microsoft Graph, необходимо указать поставщика проверки подлинности, который способен выполнять аутентификацию HTTPS-запросов с помощью соответствующего токена носителя OAuth 2.0. Пример проекта содержит готовую структуру проверки подлинности с именем **Authentication.swift.** Мы добавим функцию, которая запрашивает (и получает) маркер доступа для вызова API Microsoft Graph. 

1. Откройте рабочую область проекта Xcode (**Graph-iOS-Swift-Connect.xcworkspace**) и откройте файл расширения структуры **Authentication.swift**. Найдите в этом расширении приведенный ниже код.


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


2. Мы вызовем этот метод из файла **ConnectViewController.swift**. Этот контроллер является представлением по умолчанию для приложения и содержит одну кнопку с надписью **Connect** (Подключиться), при нажатии который запускается проверка подлинности. Этот метод принимает один параметр, **scopes**. Мы подробнее рассмотрим области далее в этой статье. Добавьте приведенное ниже действие в файл **ConnectViewController.swift**.

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

## <a name="send-an-email-with-microsoft-graph"></a>Отправка электронного сообщения с помощью Microsoft Graph

После настройки проекта для проверки подлинности необходимо получить электронный адрес, отображаемое имя и аватар пользователя, прошедшего проверку подлинности. Получив эти значения, метод отправляет аватар в OneDrive и получает URL-адрес совместного доступа для изображения. Напоследок он отправляет сообщение пользователю с помощью API Microsoft Graph. 

По умолчанию получателем будет вошедший пользователь, но вы можете указать любой адрес. Код, с которым мы будем работать, находится в классе **SendMailViewController.swift.** Вы заметите, что там есть и другой код для пользовательского интерфейса, а также вспомогательный метод для получения данных профиля пользователя из службы Microsoft Graph. Мы сосредоточимся на методах для создания и отправки электронного сообщения.

1. Откройте класс **SendMailViewController.swift.**  и найдите в нем вспомогательный метод, создающий текст сообщения:

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
2. Найдите приведенные ниже вспомогательные методы для получения данных пользователя и аватара, а также для отправки фотографии в OneDrive:

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

3. Найдите в классе приведенный ниже метод отправки почты.  

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


## <a name="run-the-app"></a>Запуск приложения
1. Прежде чем запускать пример, необходимо указать идентификатор клиента, полученный во время регистрации (раздел **Регистрация приложения**). Откройте файл **ApplicationConstants.swift**. Вы увидите, что в начале файла можно добавить идентификатор клиента, скопированный в ходе регистрации.  

  ```swift
struct ApplicationConstants {
    static let clientId = "Enter_Client_Id_Here"
    static let scopes   = ["openid", "profile", "Mail.ReadWrite","mail.send","Files.ReadWrite","User.ReadBasic.All"]
}


  ```

> Примечание. Вы заметите, что для этого проекта настроены следующие разрешения: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. Эти разрешения необходимы для правильной работы приложения, в частности отправки сообщения в учетную запись почты и получения данных профиля (отображаемое имя, адрес электронной почты).

2. Запустите приложение, нажмите кнопку **Connect** (Подключиться), войдите с помощью рабочей или учебной учетной записи и предоставьте запрашиваемые разрешения.

3. Нажмите кнопку **Отправить сообщение**. Под кнопкой появится сообщение, что отправка выполнена успешно.

## <a name="next-steps"></a>Дальнейшие действия
- Попробуйте REST API, используя [песочницу Graph](https://graph.microsoft.io/graph-explorer).
- Примеры распространенных операций REST и SDK вы найдете во [фрагментах кода на языке Objective C с использованием Microsoft Graph для iOS](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).

## <a name="see-also"></a>См. также
- [Протоколы Azure AD версии 2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Маркеры Azure AD версии 2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
