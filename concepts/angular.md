# <a name="get-started-with-microsoft-graph-in-an-angularjs-app"></a><span data-ttu-id="e49c3-101">Начало работы с Microsoft Graph в приложении AngularJS</span><span class="sxs-lookup"><span data-stu-id="e49c3-101">Get started with Microsoft Graph in an AngularJS app</span></span>

<span data-ttu-id="e49c3-p101">В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из конечной точки Azure AD версии 2.0 и вызвать Microsoft Graph. В ней рассматривается создание [приложения Microsoft Connect для AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample) и объясняются основные понятия, которые необходимо реализовать для использования Microsoft Graph. В этой статье также описывается, как получить доступ к Microsoft Graph с помощью [пакета SDK Microsoft Graph для JavaScript](https://github.com/microsoftgraph/msgraph-sdk-javascript) или необработанных вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="e49c3-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Microsoft Connect Sample for AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample) and explains the main concepts that you implement to use Microsoft Graph. The article also describes how to access Microsoft Graph by using either the [Microsoft Graph JavaScript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) or raw REST calls.</span></span>

<span data-ttu-id="e49c3-105">На приведенном ниже рисунке показано создаваемое приложение.</span><span class="sxs-lookup"><span data-stu-id="e49c3-105">The following image shows the app you'll create.</span></span> 

![Веб-приложение после входа с кнопкой "Отправить сообщение"](./images/angular-connect-sample.png)


<span data-ttu-id="e49c3-p102">**Не хотите создавать приложение?** С помощью [краткого руководства по Microsoft Graph](https://graph.microsoft.io/ru-RU/getting-started) вы сможете быстро приступить к работе.</span><span class="sxs-lookup"><span data-stu-id="e49c3-p102">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/ru-RU/getting-started) to get up and running fast.</span></span>

<span data-ttu-id="e49c3-109">Скачать вариант этого примера, использующий конечную точку Azure AD, можно на странице [приложения Microsoft Graph Connect для AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample/releases/tag/last_v1_auth).</span><span class="sxs-lookup"><span data-stu-id="e49c3-109">To download a version of the Connect sample that uses the Azure AD endpoint, see [Microsoft Graph Connect Sample for AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample/releases/tag/last_v1_auth).</span></span>


## <a name="prerequisites"></a><span data-ttu-id="e49c3-110">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="e49c3-110">Prerequisites</span></span>

<span data-ttu-id="e49c3-111">Чтобы приступить к работе, вам понадобится следующее:</span><span class="sxs-lookup"><span data-stu-id="e49c3-111">To get started, you'll need:</span></span> 

- <span data-ttu-id="e49c3-112">[Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](https://docs.microsoft.com/ru-RU/office/developer-program/office-365-developer-program-faq#account-types).</span><span class="sxs-lookup"><span data-stu-id="e49c3-112">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/ru-RU/office/developer-program/office-365-developer-program-faq#account-types)</span></span>
- <span data-ttu-id="e49c3-113">[Node.js с npm](https://nodejs.org/en/download/).</span><span class="sxs-lookup"><span data-stu-id="e49c3-113">[Node.js with npm](https://nodejs.org/en/download/)</span></span>
- <span data-ttu-id="e49c3-114">[Bower](https://bower.io).</span><span class="sxs-lookup"><span data-stu-id="e49c3-114">[Bower](https://bower.io)</span></span>
- <span data-ttu-id="e49c3-p103">[Приложение Microsoft Graph Connect для AngularJS](https://github.com/microsoftgraph/angular-connect-sample). Вы будете использовать папку **starter-project** в примерах файлов для этого пошагового руководства.</span><span class="sxs-lookup"><span data-stu-id="e49c3-p103">The [Microsoft Connect Sample for AngularJS](https://github.com/microsoftgraph/angular-connect-sample). You'll use the **starter-project** folder in the sample files for this walkthrough.</span></span>

## <a name="register-the-application"></a><span data-ttu-id="e49c3-117">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="e49c3-117">Register the application</span></span>
<span data-ttu-id="e49c3-p104">Зарегистрируйте приложение на портале регистрации приложений (Майкрософт). При этом будут созданы идентификатор и пароль приложения, которые понадобятся при его настройке в Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="e49c3-p104">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app in Visual Studio.</span></span>

1. <span data-ttu-id="e49c3-120">Войдите на [портал регистрации приложений Майкрософт](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="e49c3-120">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="e49c3-121">Нажмите кнопку **Добавить приложение**.</span><span class="sxs-lookup"><span data-stu-id="e49c3-121">Choose **Add an app**.</span></span>

3. <span data-ttu-id="e49c3-122">Введите имя приложения и нажмите кнопку **Создать приложение**.</span><span class="sxs-lookup"><span data-stu-id="e49c3-122">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="e49c3-123">Откроется страница регистрации со свойствами приложения.</span><span class="sxs-lookup"><span data-stu-id="e49c3-123">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="e49c3-p105">Скопируйте идентификатор приложения. Это уникальный идентификатор приложения, который используется для его настройки.</span><span class="sxs-lookup"><span data-stu-id="e49c3-p105">Copy the application ID. This is the unique identifier for your app that you'll use to configure the app.</span></span>

5. <span data-ttu-id="e49c3-126">В разделе **Платформы** выберите **Добавление платформы** > **Веб**.</span><span class="sxs-lookup"><span data-stu-id="e49c3-126">Under **Platforms**, choose **Add Platform** > **Web**.</span></span>

6. <span data-ttu-id="e49c3-127">Убедитесь, что установлен флажок **Разрешить неявный поток**, и введите *http://localhost:8080* в качестве URI перенаправления.</span><span class="sxs-lookup"><span data-stu-id="e49c3-127">Make sure the Allow Implicit Flow check box is selected, and enter http://localhost:8080 as the Redirect URI.</span></span> 

7. <span data-ttu-id="e49c3-128">Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="e49c3-128">Choose **Save**.</span></span>


## <a name="configure-the-project"></a><span data-ttu-id="e49c3-129">Настройка проекта</span><span class="sxs-lookup"><span data-stu-id="e49c3-129">Configure the project</span></span>
1. <span data-ttu-id="e49c3-130">Откройте папку **starter-project** с файлами примера.</span><span class="sxs-lookup"><span data-stu-id="e49c3-130">Open the **starter-project** folder in the sample files.</span></span>
2. <span data-ttu-id="e49c3-p106">Откройте командную строку и выполните приведенные ниже команды в корневом каталоге начального проекта. При этом устанавливаются зависимости проекта.</span><span class="sxs-lookup"><span data-stu-id="e49c3-p106">In a command prompt, run the following commands in the root directory of the starter project. This installs the project dependencies.</span></span>

        npm install  
        bower install
    
3. <span data-ttu-id="e49c3-133">В файлах начального проекта перейдите к папке **public/scripts** и откройте файл config.js.</span><span class="sxs-lookup"><span data-stu-id="e49c3-133">In the starter project files, in the **public/scripts** folder, open config.js.</span></span>
4. <span data-ttu-id="e49c3-134">В поле **clientID** замените текст **ENTER_YOUR_CLIENT_ID** на скопированный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="e49c3-134">In the **clientID** field, replace the **ENTER_YOUR_CLIENT_ID** placeholder value with the application ID you just copied.</span></span>

## <a name="call-microsoft-graph-with-the-sdk"></a><span data-ttu-id="e49c3-135">Вызовы Microsoft Graph с помощью пакета SDK</span><span class="sxs-lookup"><span data-stu-id="e49c3-135">Call Microsoft Graph with the SDK</span></span>
<span data-ttu-id="e49c3-p107">Приложение вызывает Microsoft Graph, чтобы получить данные пользователя и отправить электронное сообщение от его имени. Такие вызовы отправляются из MainController в ответ на события пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="e49c3-p107">The app calls Microsoft Graph to get user information and to send an email on the user's behalf. These calls are initiated from the MainController in response to UI events.</span></span>

<span data-ttu-id="e49c3-p108">Откройте файл app.js и добавьте в его конец следующий код. Этот код инициализирует пакет SDK.</span><span class="sxs-lookup"><span data-stu-id="e49c3-p108">Open app.js and add the following code to the bottom of the file. This initializes the SDK.</span></span>

    var authToken;
    var graphClient = MicrosoftGraph.Client.init({
        authProvider: function(done) {
        if (typeof authToken === "undefined") {
          done({err: "No auth token"})
        } else {
          done(null, authToken); //first parameter takes an error if you can't get an access token
        }
        }
    });

### <a name="using-the-sdk"></a><span data-ttu-id="e49c3-140">Использование пакета SDK</span><span class="sxs-lookup"><span data-stu-id="e49c3-140">Using the SDK</span></span>
1. <span data-ttu-id="e49c3-p109">В файле graphHelper.js замените строку *// Get the profile of the current user* на приведенный ниже код. Этот код настраивает и отправляет запрос GET конечной точке */me*, а затем обрабатывает ответ.</span><span class="sxs-lookup"><span data-stu-id="e49c3-p109">In graphHelper.js, replace *// Get the profile of the current user* with the following code. This configures and sends the GET request to the */me* endpoint, and processes the response.</span></span>

        // Get the profile of the current user.
        me: function me() {
          return graphClient.api('/me').get();
        },
  
2. <span data-ttu-id="e49c3-p110">Замените строку *// Send an email on behalf of the current user* на приведенный ниже код. Этот код настраивает и отправляет запрос POST конечной точке */me/sendMail*, а затем обрабатывает ответ.</span><span class="sxs-lookup"><span data-stu-id="e49c3-p110">Replace *// Send an email on behalf of the current user* with the following code. This configures and sends the POST request to the */me/sendMail* endpoint, and processes the response.</span></span>

        // Send an email on behalf of the current user.
        sendMail: function sendMail(email) {
          return graphClient.api('/me/sendMail').post({ 'message' : email, 'saveToSentItems': true });
        }

3. <span data-ttu-id="e49c3-145">В папке **public/controllers** откройте файл mainController.js.</span><span class="sxs-lookup"><span data-stu-id="e49c3-145">In the **public/controllers** folder, open mainController.js.</span></span>

4. <span data-ttu-id="e49c3-p111">Замените строку *// Set the default headers and user properties* на приведенный ниже код. Этот код добавляет маркер доступа к HTTP-запросу, вызывает **GraphHelper.me**, чтобы получить профиль текущего пользователя, и обрабатывает ответ.</span><span class="sxs-lookup"><span data-stu-id="e49c3-p111">Replace *// Set the default headers and user properties* with the following code. This adds the access token to the HTTP request, calls **GraphHelper.me** to get the current user's profile, and processes the response.</span></span>

        // Set the default headers and user properties.
        function processAuth() {

        // let the authProvider access the access token
        authToken = localStorage.token;

        if (localStorage.getItem('user') === null) {

          // Get the profile of the current user.
          GraphHelper.me().then(function(user) {

            // Save the user to localStorage.
            localStorage.setItem('user', angular.toJson(user));

            vm.displayName = user.displayName;
            vm.emailAddress = user.mail || user.userPrincipalName;
          });
        } else {
          let user = angular.fromJson(localStorage.user);

          vm.displayName = user.displayName;
          vm.emailAddress = user.mail || user.userPrincipalName;
        }

        }

5. <span data-ttu-id="e49c3-p112">Замените строку *// Send an email on behalf of the current user* на приведенный ниже код. Этот код создает электронное сообщение, вызывает метод **GraphHelper.sendMail** и обрабатывает ответ.</span><span class="sxs-lookup"><span data-stu-id="e49c3-p112">Replace *// Send an email on behalf of the current user* with the following code. This builds the email message, calls **GraphHelper.sendMail**, and processes the response.</span></span>

        // Send an email on behalf of the current user.
        function sendMail() {

          authToken = localStorage.token;       

          // Build the HTTP request payload (the Message object).
          var email = {
          Subject: 'Welcome to Microsoft Graph development with Angular and the Microsoft Graph Connect sample',
          Body: {
            ContentType: 'HTML',
            Content: getEmailContent()
          },
          ToRecipients: [
            {
              EmailAddress: {
            Address: vm.emailAddress
              }
            }
          ]
          };

          // Save email address so it doesn't get lost with two way data binding.
          vm.emailAddressSent = vm.emailAddress;
          GraphHelper.sendMail(email)
        .then(function (response) {
          $log.debug('HTTP request to the Microsoft Graph API returned successfully.', response);
          vm.requestSuccess = true;
          vm.requestFinished = true;
          $scope.$apply();
        }, function (error) {
          $log.error('HTTP request to the Microsoft Graph API failed.');
          vm.requestSuccess = false;
          vm.requestFinished = true;
          $scope.$apply();
        });

        };

6. <span data-ttu-id="e49c3-150">Сохраните все изменения.</span><span class="sxs-lookup"><span data-stu-id="e49c3-150">Save all your changes.</span></span>

## <a name="run-the-app"></a><span data-ttu-id="e49c3-151">Запуск приложения</span><span class="sxs-lookup"><span data-stu-id="e49c3-151">Run the app</span></span>

1. <span data-ttu-id="e49c3-152">Откройте командную строку и выполните приведенную ниже команду в корневом каталоге начального проекта.</span><span class="sxs-lookup"><span data-stu-id="e49c3-152">In a command prompt, run the following command in the root directory of the starter project.</span></span>

        npm start

2. <span data-ttu-id="e49c3-153">Введите в браузере адрес *http://localhost:8080* и нажмите кнопку **Подключиться**.</span><span class="sxs-lookup"><span data-stu-id="e49c3-153">In a browser, navigate to http://localhost:8080 and choose the Connect button.</span></span>

3. <span data-ttu-id="e49c3-154">Выполните вход и предоставьте запрашиваемые разрешения.</span><span class="sxs-lookup"><span data-stu-id="e49c3-154">Sign in and grant the requested permissions.</span></span> 

4. <span data-ttu-id="e49c3-p113">При необходимости измените электронный адрес получателя и нажмите кнопку **Отправить сообщение**. Под кнопкой появится сообщение, что отправка выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="e49c3-p113">Optionally edit the recipient's email address, and then choose the **Send mail** button. When the mail is sent, a Success message is displayed below the button.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="e49c3-157">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="e49c3-157">Next steps</span></span>
- <span data-ttu-id="e49c3-158">Попробуйте REST API, используя [песочницу Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="e49c3-158">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="e49c3-159">Просмотрите другие [примеры AngularJS](https://github.com/search?utf8=%E2%9C%93&q=angular+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="e49c3-159">Explore our other [AngularJS samples](https://github.com/search?utf8=%E2%9C%93&q=angular+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) on GitHub.</span></span>


## <a name="see-also"></a><span data-ttu-id="e49c3-160">См. также</span><span class="sxs-lookup"><span data-stu-id="e49c3-160">See also</span></span>
- [<span data-ttu-id="e49c3-161">Протоколы Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="e49c3-161">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/ru-RU/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="e49c3-162">Маркеры Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="e49c3-162">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/ru-RU/documentation/articles/active-directory-v2-tokens/)
