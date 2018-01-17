# <a name="get-started-with-microsoft-graph-in-a-nodejs-app"></a><span data-ttu-id="e7719-101">Начало работы с Microsoft Graph в приложении Node.js</span><span class="sxs-lookup"><span data-stu-id="e7719-101">Get started with Microsoft Graph in a Node.js app</span></span>

<span data-ttu-id="e7719-102">В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из конечной точки Azure AD версии 2.0 и вызвать Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e7719-102">This article describes the tasks required to get an access token from the v2.0 authentication endpoint and call  Microsoft Graph.</span></span> <span data-ttu-id="e7719-103">В ней рассмотрен [пример кода для подключения приложения Node.js от корпорации Майкрософт](https://github.com/microsoftgraph/nodejs-connect-rest-sample) и объясняются основные понятия, которые необходимо реализовать для использования Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e7719-103">It walks you through building the [Connect Sample for PHP](https://github.com/microsoftgraph/nodejs-connect-rest-sample) and explains the main concepts that you implement to use Microsoft Graph.</span></span> <span data-ttu-id="e7719-104">В этой статье рассказывается, как получить доступ к API Microsoft Graph с помощью необработанных вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="e7719-104">The article describes how to access Microsoft Graph by using direct REST calls.</span></span> <span data-ttu-id="e7719-105">Если вы хотите создать приложение Node.js, которое подключается к Microsoft Graph с помощью пакета SDK для JavaScript, ознакомьтесь с [примером кода подключения на базе пакета SDK Microsoft Graph для Node.js](https://github.com/microsoftgraph/nodejs-connect-sample).</span><span class="sxs-lookup"><span data-stu-id="e7719-105">If you're interested in building a Node.js app that connects to Microsoft Graph with the JavaScript SDK, see our [Microsoft Graph SDK-based Node.js Connect sample](https://github.com/microsoftgraph/nodejs-connect-sample).</span></span>

<span data-ttu-id="e7719-106">На приведенном ниже изображении показано создаваемое приложение.</span><span class="sxs-lookup"><span data-stu-id="e7719-106">The following image shows is the app you'll create.</span></span> 

![Веб-приложение после входа с кнопкой "Отправить сообщение"](./images/web-screenshot.png)


<span data-ttu-id="e7719-p102">**Не хотите создавать приложение?** С помощью [краткого руководства по Microsoft Graph](https://graph.microsoft.io/ru-RU/getting-started) вы сможете быстро приступить к работе.</span><span class="sxs-lookup"><span data-stu-id="e7719-p102">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/ru-RU/getting-started) to get up and running fast.</span></span>

<span data-ttu-id="e7719-110">Скачать вариант этого примера, использующий конечную точку Azure AD, можно на странице [приложения Microsoft Graph Connect для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample/releases/tag/last_v1_auth).</span><span class="sxs-lookup"><span data-stu-id="e7719-110">To download a version of the Connect sample that uses the Azure AD endpoint, see [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample/releases/tag/last_v1_auth).</span></span>


## <a name="prerequisites"></a><span data-ttu-id="e7719-111">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="e7719-111">Prerequisites</span></span>

<span data-ttu-id="e7719-112">Чтобы приступить к работе, вам понадобится следующее:</span><span class="sxs-lookup"><span data-stu-id="e7719-112">To get started, you'll need:</span></span> 

- <span data-ttu-id="e7719-113">[Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](http://dev.office.com/devprogram).</span><span class="sxs-lookup"><span data-stu-id="e7719-113">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
- [<span data-ttu-id="e7719-114">Node.js с npm</span><span class="sxs-lookup"><span data-stu-id="e7719-114">Node.js with npm</span></span>](https://nodejs.org/en/download/) 
- <span data-ttu-id="e7719-115">[Пример подключения для Node.js от корпорации Майкрософт](https://github.com/microsoftgraph/nodejs-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="e7719-115">The [Microsoft Connect sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).</span></span> <span data-ttu-id="e7719-116">Вы будете использовать папку **starter-project** в примерах файлов для этого пошагового руководства.</span><span class="sxs-lookup"><span data-stu-id="e7719-116">The Microsoft Connect Sample for AngularJS. You'll use the **starter-project** folder in the sample files for this walkthrough.</span></span>

## <a name="register-the-application"></a><span data-ttu-id="e7719-117">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="e7719-117">Register the application</span></span>
<span data-ttu-id="e7719-p104">Зарегистрируйте приложение на портале регистрации приложений (Майкрософт). При этом будут созданы идентификатор и пароль приложения, которые понадобятся при его настройке в Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="e7719-p104">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app in Visual Studio.</span></span>

1. <span data-ttu-id="e7719-120">Войдите на [портал регистрации приложений Майкрософт](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="e7719-120">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="e7719-121">Нажмите кнопку **Добавить приложение**.</span><span class="sxs-lookup"><span data-stu-id="e7719-121">Choose **Add an app**.</span></span>

3. <span data-ttu-id="e7719-122">Введите имя приложения и нажмите кнопку **Создать приложение**.</span><span class="sxs-lookup"><span data-stu-id="e7719-122">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="e7719-123">Откроется страница регистрации со свойствами приложения.</span><span class="sxs-lookup"><span data-stu-id="e7719-123">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="e7719-p105">Скопируйте идентификатор приложения. Это уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="e7719-p105">Copy the application ID. This is the unique identifier for your app.</span></span> 

5. <span data-ttu-id="e7719-p106">В разделе **Секреты приложения** нажмите кнопку **Создать новый пароль**. Скопируйте пароль из диалогового окна **Новый пароль создан**.</span><span class="sxs-lookup"><span data-stu-id="e7719-p106">Under **Application Secrets**, choose **Generate New Password**. Copy the password from the **New password generated** dialog.</span></span>

    <span data-ttu-id="e7719-128">Идентификатор и пароль (секрет) приложения используются для его настройки.</span><span class="sxs-lookup"><span data-stu-id="e7719-128">You'll use the application ID and application password (secret) to configure the app.</span></span> 

6. <span data-ttu-id="e7719-129">В разделе **Платформы** выберите **Добавление платформы** > **Веб**.</span><span class="sxs-lookup"><span data-stu-id="e7719-129">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="e7719-130">Введите URI перенаправления *http://localhost:3000/token*.</span><span class="sxs-lookup"><span data-stu-id="e7719-130">Enter *http://localhost:3000/token* as the Redirect URI.</span></span> 

8. <span data-ttu-id="e7719-131">Нажмите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="e7719-131">Choose **Save**.</span></span>


## <a name="configure-the-project"></a><span data-ttu-id="e7719-132">Настройка проекта</span><span class="sxs-lookup"><span data-stu-id="e7719-132">Configure the project</span></span>
1. <span data-ttu-id="e7719-133">Откройте папку **starter-project** с файлами примера.</span><span class="sxs-lookup"><span data-stu-id="e7719-133">Open the **starter-project** folder in the sample files.</span></span>

1. <span data-ttu-id="e7719-p107">Откройте командную строку и выполните приведенную ниже команду в корневом каталоге начального проекта. При этом устанавливаются зависимости проекта.</span><span class="sxs-lookup"><span data-stu-id="e7719-p107">In a command prompt, run the following command in the root directory of the starter project. This installs the project dependencies.</span></span>

        npm install

1. <span data-ttu-id="e7719-136">В файлах начального проекта откройте utils\config.js.</span><span class="sxs-lookup"><span data-stu-id="e7719-136">In the starter project files, open utils\config.js.</span></span>


1. <span data-ttu-id="e7719-137">В поле **credentials** замените строки **ENTER\_YOUR\_CLIENT\_ID** и **ENTER\_YOUR\_SECRET** скопированными только что значениями.</span><span class="sxs-lookup"><span data-stu-id="e7719-137">In the **credentials** field, replace the **ENTER\_YOUR\_CLIENT\_ID** and **ENTER\_YOUR\_SECRET** placeholder values with the values you just copied.</span></span>

  
## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="e7719-138">Проверка подлинности пользователя и получение маркера доступа</span><span class="sxs-lookup"><span data-stu-id="e7719-138">Authenticate the user and get an access token</span></span>
<span data-ttu-id="e7719-p108">На этом этапе вы добавите код для входа и управления маркером. Но для начала подробнее рассмотрим поток проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e7719-p108">In this step, you'll add sign-in and token management code. But first, let's take a closer look at the auth flow.</span></span>

<span data-ttu-id="e7719-p109">В этом приложении используется поток предоставления кода авторизации с делегированным удостоверением пользователя. В веб-приложении для этого потока требуются идентификатор, секрет и URI перенаправления зарегистрированного приложения.</span><span class="sxs-lookup"><span data-stu-id="e7719-p109">This app uses the authorization code grant flow with a delegated user identity. For a web application, the flow requires the application ID, secret, and redirect URI from the registered app.</span></span> 

<span data-ttu-id="e7719-143">Поток проверки подлинности можно разделить на следующие основные этапы:</span><span class="sxs-lookup"><span data-stu-id="e7719-143">The auth flow can be broken down into these basic steps:</span></span>

1. <span data-ttu-id="e7719-144">Перенаправление пользователя для проверки подлинности и согласия</span><span class="sxs-lookup"><span data-stu-id="e7719-144">Redirect the user for authentication and consent</span></span>
2. <span data-ttu-id="e7719-145">Получение кода авторизации</span><span class="sxs-lookup"><span data-stu-id="e7719-145">Get an authorization code</span></span>
3. <span data-ttu-id="e7719-146">Обмен кода авторизации на маркер доступа</span><span class="sxs-lookup"><span data-stu-id="e7719-146">Redeem the authorization code for an access token</span></span>
4. <span data-ttu-id="e7719-147">Использование маркера обновления для получения нового маркера доступа по истечении срока действия текущего</span><span class="sxs-lookup"><span data-stu-id="e7719-147">Use the refresh token to get a new access token when the access token expires</span></span>

<span data-ttu-id="e7719-p110">В приложении используется ПО промежуточного слоя [oauth](https://www.npmjs.com/package/oauth) для проверки подлинности и получения маркеров. С помощью ПО промежуточного слоя [cookie-parser](https://www.npmjs.com/package/cookie-parser) приложение кэширует сведения о маркере в файлах cookie. Код, используемый для хранения сведений о маркере и доступа к ним, находится в контроллере index.js.</span><span class="sxs-lookup"><span data-stu-id="e7719-p110">The app uses the [oauth](https://www.npmjs.com/package/oauth) middleware to authenticate and obtain tokens. It uses the [cookie-parser](https://www.npmjs.com/package/cookie-parser) middleware to cache token information in cookies. The code used to store and access token information is found in the index.js controller.</span></span>
    
   ><span data-ttu-id="e7719-p111">**Важно!** Простые процедуры проверки подлинности и обработки маркеров в этом проекте представлены исключительно в качестве примера. В рабочем приложении следует реализовать более надежную процедуру проверки подлинности, включающую утверждение и безопасную обработку маркеров.</span><span class="sxs-lookup"><span data-stu-id="e7719-p111">**Important** The simple authentication and token handling in this project is for sample purposes only. In a production app, you should construct a more robust way of handling authentication, including validation and secure token handling.</span></span>

<span data-ttu-id="e7719-153">Теперь вы готовы добавить код для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e7719-153">Now you're ready to add code to call Microsoft Graph.</span></span> 

## <a name="call-microsoft-graph"></a><span data-ttu-id="e7719-154">Вызов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e7719-154">Call Microsoft Graph</span></span>
<span data-ttu-id="e7719-p112">Приложение вызывает Microsoft Graph, чтобы получить данные пользователя и отправить электронное сообщение от его имени. Такие вызовы отправляются из контроллера index.js в ответ на события пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="e7719-p112">The app calls Microsoft Graph to get user information and to send an email on the user's behalf. These calls are initiated from the index.js controller in response to UI events.</span></span>

1. <span data-ttu-id="e7719-157">Откройте utils\graphHelper.js.</span><span class="sxs-lookup"><span data-stu-id="e7719-157">Open utils\graphHelper.js.</span></span>

1. <span data-ttu-id="e7719-p113">Замените функцию **getUserData** приведенным ниже кодом. Этот код настраивает и отправляет запрос GET конечной точке */me*, а затем обрабатывает ответ.</span><span class="sxs-lookup"><span data-stu-id="e7719-p113">Replace the **getUserData** function with the following code. This configures and sends the GET request to the */me* endpoint and processes the response.</span></span>

        function getUserData(accessToken, callback) {
          request
           .get('https://graph.microsoft.com/v1.0/me')
           .set('Authorization', 'Bearer ' + accessToken)
           .end((err, res) => {
             callback(err, res);
           });
        }

1. <span data-ttu-id="e7719-p114">Замените функцию **getProfilePhoto** приведенным ниже кодом. Этот код настраивает и отправляет запрос GET конечной точке */me/photo/$value*, а затем обрабатывает ответ. Обратите внимание, что фотографии профиля в настоящее время недоступны для учетных записей MSA.</span><span class="sxs-lookup"><span data-stu-id="e7719-p114">Replace the **getProfilePhoto** function with the following code. This configures and sends the GET request to the */me/photo/$value* endpoint and processes the response. Note that profile photos aren't currently available for MSA accounts.</span></span>
    
        function getProfilePhoto(accessToken, callback) {
          // Get the profile photo of the current user (from the user's mailbox on Exchange Online).
          // This operation in version 1.0 supports only work or school mailboxes, not personal mailboxes.
          request
           .get('https://graph.microsoft.com/v1.0/me/photo/$value')
           .set('Authorization', 'Bearer ' + accessToken)
           .end((err, res) => {
             // Returns 200 OK and the photo in the body. If no photo exists, returns 404 Not Found.
             callback(err, res.body);
           });
        }

1. <span data-ttu-id="e7719-p115">Замените функцию **uploadFile** следующим кодом. Он настраивает и отправляет запрос PUT в конечную точку */me/drive/root/children/mypic.jpg/content*. Если файл существует, этот запрос обновляет содержимое. В противном случае он создает файл и добавляет фотографию профиля.</span><span class="sxs-lookup"><span data-stu-id="e7719-p115">Replace the **uploadFile** function with the following code. This configures and sends the PUT request to the */me/drive/root/children/mypic.jpg/content* endpoint. If the file exists, this requests updates the content. If it doesn't exist, it creates the file and uploads the contents of the profile photo.</span></span> 

        function uploadFile(accessToken, file, callback) {
          // This operation only supports files up to 4MB in size.
          // To upload larger files, see `https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/item_createUploadSession`.
          request
           .put('https://graph.microsoft.com/v1.0/me/drive/root/children/mypic.jpg/content')
           .send(file)
           .set('Authorization', 'Bearer ' + accessToken)
           .set('Content-Type', 'image/jpg')
           .end((err, res) => {
             // Returns 200 OK and the file metadata in the body.
             callback(err, res.body);
           });
        }

1. <span data-ttu-id="e7719-p116">Замените функцию **getSharingLink** приведенным ниже кодом. Он настраивает и отправляет запрос GET в конечную точку */me/drive/items/{идентификатор файла}/createLink* и обрабатывает результат (ссылку для общего доступа к файлу, которая будет включена в сообщение).</span><span class="sxs-lookup"><span data-stu-id="e7719-p116">Replace the **getSharingLink** function with the following code. This configures and sends the GET request to the */me/drive/items/{file id}/createLink* endpoint and processes the result. The result is a sharing link to the file that will be included in the message.</span></span>

        function getSharingLink(accessToken, id, callback) {
          request
           .post('https://graph.microsoft.com/v1.0/me/drive/items/' + id + '/createLink')
           .send({ type: 'view' })
           .set('Authorization', 'Bearer ' + accessToken)
           .set('Content-Type', 'application/json')
           .end((err, res) => {
             // Returns 200 OK and the permission with the link in the body.
             callback(err, res.body.link);
           });
        }

1. <span data-ttu-id="e7719-p117">Замените функцию **postSendMail** приведенным ниже кодом. Этот код настраивает и отправляет запрос POST конечной точке */me/sendMail*, а затем обрабатывает ответ.</span><span class="sxs-lookup"><span data-stu-id="e7719-p117">Replace the **postSendMail** function with the following code. This configures and sends the POST request to the */me/sendMail* endpoint and processes the response.</span></span>

        function postSendMail(accessToken, message, callback) {
          request
           .post('https://graph.microsoft.com/v1.0/me/sendMail')
           .send(message)
           .set('Authorization', 'Bearer ' + accessToken)
           .set('Content-Type', 'application/json')
           .set('Content-Length', message.length)
           .end((err, res) => {
             // Returns 202 if successful.
             // Note: If you receive a 500 - Internal Server Error
             // while using a Microsoft account (outlook.com, hotmail.com or live.com),
             // it's possible that your account has not been migrated to support this flow.
             // Check the inner error object for code 'ErrorInternalServerTransientError'.
             // You can try using a newly created Microsoft account or contact support.
             callback(err, res);
           });
        }

1. <span data-ttu-id="e7719-172">Откройте utils\emailer.js.</span><span class="sxs-lookup"><span data-stu-id="e7719-172">Open utils\emailer.js.</span></span>

1. <span data-ttu-id="e7719-p118">Замените функцию **wrapEmail** приведенным ниже кодом. Этот код создает полезные данные, представляющие отправляемое сообщение.</span><span class="sxs-lookup"><span data-stu-id="e7719-p118">Replace the **wrapEmail** function with the following code. This builds the payload that represents the email message to send.</span></span>

        function wrapEmail(content, recipient, file) {
          const attachments = [{
            '@odata.type': '#microsoft.graph.fileAttachment',
            ContentBytes: file,
            Name: 'mypic.jpg'
          }];
          const emailAsPayload = {
            Message: {
              Subject: 'Welcome to Microsoft Graph development with Node.js and the Microsoft Graph Connect sample',
              Body: {
                ContentType: 'HTML',
                Content: content
              },
              ToRecipients: [
                {
                  EmailAddress: {
                    Address: recipient
                  }
                }
              ]
            },
            SaveToSentItems: true,
            Attachments: attachments
          };
          return emailAsPayload;
        }

## <a name="run-the-app"></a><span data-ttu-id="e7719-175">Запуск приложения</span><span class="sxs-lookup"><span data-stu-id="e7719-175">Run the app</span></span>

1. <span data-ttu-id="e7719-176">Откройте командную строку и выполните приведенную ниже команду в корневом каталоге начального проекта.</span><span class="sxs-lookup"><span data-stu-id="e7719-176">In a command prompt, run the following command in the root directory of the starter project.</span></span>


        npm start

1. <span data-ttu-id="e7719-177">Введите в браузере адрес *http://localhost:3000* и нажмите кнопку **Подключиться к Office 365**.</span><span class="sxs-lookup"><span data-stu-id="e7719-177">In a browser, navigate to *http://localhost:3000* and choose the **Connect to Office 365** button.</span></span>

1. <span data-ttu-id="e7719-178">Выполните вход и предоставьте запрашиваемые разрешения.</span><span class="sxs-lookup"><span data-stu-id="e7719-178">Sign in and grant the requested permissions.</span></span> 

1. <span data-ttu-id="e7719-p119">При необходимости измените электронный адрес получателя и нажмите кнопку **Отправить сообщение**. Под кнопкой появится сообщение, что отправка выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="e7719-p119">Optionally edit the recipient's email address, and then choose the **Send mail** button. When the mail is sent, a Success message is displayed below the button.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="e7719-181">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="e7719-181">Next steps</span></span>
- <span data-ttu-id="e7719-182">Попробуйте REST API, используя [песочницу Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="e7719-182">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="e7719-183">Просмотрите другие [примеры для Node.js](https://github.com/search?utf8=%E2%9C%93&q=node+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="e7719-183">Explore our other [Node.js samples](https://github.com/search?utf8=%E2%9C%93&q=node+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) on GitHub.</span></span>
- <span data-ttu-id="e7719-184">Использование [типов TypeScript для Microsoft Graph](https://github.com/microsoftgraph/msgraph-typescript-typings)</span><span class="sxs-lookup"><span data-stu-id="e7719-184">Use the [Microsoft Graph TypeScript types](https://github.com/microsoftgraph/msgraph-typescript-typings)</span></span>
- <span data-ttu-id="e7719-185">Использование [пакета SDK JavaScript для Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript)</span><span class="sxs-lookup"><span data-stu-id="e7719-185">Try the [Microsoft Graph JavaScript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript)</span></span>

## <a name="see-also"></a><span data-ttu-id="e7719-186">См. также</span><span class="sxs-lookup"><span data-stu-id="e7719-186">See also</span></span>
- [<span data-ttu-id="e7719-187">Протоколы Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="e7719-187">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/ru-RU/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="e7719-188">Маркеры Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="e7719-188">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/ru-RU/documentation/articles/active-directory-v2-tokens/)
- [<span data-ttu-id="e7719-189">Пример подключения для Node.js с использованием SDK JavaScript для Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e7719-189">Microsoft Graph JavaScript SDK Node.js Connect sample</span></span>](https://github.com/microsoftgraph/nodejs-connect-sample)
