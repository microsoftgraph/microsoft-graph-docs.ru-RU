# <a name="get-started-with-microsoft-graph-in-an-android-app"></a><span data-ttu-id="df142-101">Начало работы с Microsoft Graph в приложении для Android</span><span class="sxs-lookup"><span data-stu-id="df142-101">Get started with Microsoft Graph in an Android app</span></span>

> <span data-ttu-id="df142-p101">**Создаете приложения для корпоративных клиентов?** Ваше приложение может не работать, если корпоративный клиент включит функции корпоративной безопасности для мобильных устройств, например <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">условный доступ с устройств</a>. В этом случае у пользователей могут возникать ошибки, а вы не будете об этом знать.</span><span class="sxs-lookup"><span data-stu-id="df142-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="df142-p102">Для поддержки **всех корпоративных клиентов** в **любых корпоративных сценариях** необходимо использовать конечную точку Azure AD и управлять приложениями с помощью [портала управления Azure](https://aka.ms/aadapplist). Дополнительные сведения см. в разделе [Выбор между конечными точками Azure AD и Azure AD версии 2.0](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span><span class="sxs-lookup"><span data-stu-id="df142-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure Management Portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="df142-p103">В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из конечной точки Azure AD версии 2.0 и вызвать Microsoft Graph. В ней рассматривается создание [примера приложения Connect для Android](https://github.com/microsoftgraph/android-java-connect-sample) и объясняются основные понятия, которые необходимо реализовать для использования Microsoft Graph в приложении для Android. В этой статье также описывается, как получить доступ к Microsoft Graph с помощью [пакета SDK Microsoft Graph для Android](https://github.com/microsoftgraph/msgraph-sdk-android) или необработанных вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="df142-p103">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) and explains the main concepts that you implement to use Microsoft Graph in your app for Android. The article also describes how to access Microsoft Graph by using either the [Microsoft Graph SDK for Android](https://github.com/microsoftgraph/msgraph-sdk-android) or raw REST calls.</span></span>

<span data-ttu-id="df142-110">Чтобы использовать Microsoft Graph в приложении для Android, необходимо предоставить пользователям страницу входа в учетную запись Майкрософт, как показано на приведенном ниже снимке экрана.</span><span class="sxs-lookup"><span data-stu-id="df142-110">To use Microsoft Graph in your app for Android, you need to show the Microsoft sign in page to your users, as shown in the following screenshot.</span></span>

![Страница входа в учетную запись Майкрософт на Android](images/AndroidConnect.png)

<span data-ttu-id="df142-p104">**Не хотите создавать приложение?** Скачайте пример [приложения Connect для Android](https://github.com/microsoftgraph/android-java-connect-sample), на котором основана эта статья, и вы будете готовы к работе.</span><span class="sxs-lookup"><span data-stu-id="df142-p104">**Don't feel like building an app?** Get up and running fast by downloading the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) that this article is based on.</span></span>


## <a name="prerequisites"></a><span data-ttu-id="df142-114">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="df142-114">Prerequisites</span></span>

<span data-ttu-id="df142-115">Чтобы приступить к работе, вам понадобится следующее:</span><span class="sxs-lookup"><span data-stu-id="df142-115">To get started, you'll need:</span></span> 

- <span data-ttu-id="df142-116">[Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](http://dev.office.com/devprogram).</span><span class="sxs-lookup"><span data-stu-id="df142-116">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
- <span data-ttu-id="df142-117">Android Studio 2.0 или более новой версии</span><span class="sxs-lookup"><span data-stu-id="df142-117">Android Studio 2.0 or newer version</span></span>


## <a name="configure-a-new-project"></a><span data-ttu-id="df142-118">Настройка нового проекта</span><span class="sxs-lookup"><span data-stu-id="df142-118">Configure a new project</span></span>

<span data-ttu-id="df142-119">Если вы скачали [приложение Connect для Android](https://github.com/microsoftgraph/android-java-connect-sample), пропустите этот шаг.</span><span class="sxs-lookup"><span data-stu-id="df142-119">If you have downloaded the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample), skip this step.</span></span> 

<span data-ttu-id="df142-p105">Создайте новый проект в Android Studio. Большинство параметров в мастере можно оставить без изменений, но обязательно выберите следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="df142-p105">Start a new project in Android Studio. You can leave the default values for most of the wizard, just make sure to choose the following options:</span></span>

* <span data-ttu-id="df142-122">На странице Target Android Devices (Целевые устройства Android) установите флажок **Phone and Tablet (Телефон и планшет)**</span><span class="sxs-lookup"><span data-stu-id="df142-122">Target Android Devices - **Phone and Tablet**</span></span>
    * <span data-ttu-id="df142-123">В поле Minimum SDK (Минимальная версия пакета SDK) выберите значение **API 16: Android 4.1 (Jelly Bean)**</span><span class="sxs-lookup"><span data-stu-id="df142-123">Minimum SDK - **API 16: Android 4.1 (Jelly Bean)**</span></span>
* <span data-ttu-id="df142-124">На странице Add an Activity to Mobile (Добавить действие к мобильному устройству) выберите **Basic Activity (Основное действие)**</span><span class="sxs-lookup"><span data-stu-id="df142-124">Add an Activity to Mobile - **Basic Activity**</span></span>
 
<span data-ttu-id="df142-125">В результате получится проект Android с действием и кнопкой для аутентификации пользователя.</span><span class="sxs-lookup"><span data-stu-id="df142-125">This provides you with an Android project with an activity and a button that you can use to authenticate the user.</span></span>


## <a name="register-the-application"></a><span data-ttu-id="df142-126">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="df142-126">Register the application</span></span>

<span data-ttu-id="df142-127">Вам нужно зарегистрировать приложение на [портале Майкрософт](https://apps.dev.microsoft.com/) независимо от того, скачали ли вы приложение Connect или создали новый проект.</span><span class="sxs-lookup"><span data-stu-id="df142-127">You need to register your app on the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) whether you've downloaded the connect sample or created a new project.</span></span>

<span data-ttu-id="df142-p106">Зарегистрируйте приложение на портале Майкрософт. При этом будет создан идентификатор приложения, который понадобится при его настройке.</span><span class="sxs-lookup"><span data-stu-id="df142-p106">Register an app on the Microsoft App Registration Portal. This generates the app ID that you'll use to configure the app.</span></span>

1. <span data-ttu-id="df142-130">Войдите на [портал регистрации приложений Майкрософт](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="df142-130">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="df142-131">Нажмите кнопку **Добавить приложение**.</span><span class="sxs-lookup"><span data-stu-id="df142-131">Choose **Add an app**.</span></span>

><span data-ttu-id="df142-132">Совет. Если вы скачали [приложение Connect для Android](https://github.com/microsoftgraph/android-java-connect-sample) и просто регистрируете его, снимите флажок **Инструкции по настройке** перед нажатием кнопки **Создать**.</span><span class="sxs-lookup"><span data-stu-id="df142-132">Tip: If you have downloaded the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) and are just creating a registration for it, uncheck **Guided Setup** before chosing the **Create** button.</span></span>

3. <span data-ttu-id="df142-133">Введите имя приложения и нажмите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="df142-133">Enter a name for the app, and choose **Create**.</span></span> 
    
    <span data-ttu-id="df142-134">С **инструкциями по настройке**:</span><span class="sxs-lookup"><span data-stu-id="df142-134">For the  **Guided Setup** flow:</span></span>
 
    <span data-ttu-id="df142-p107">a. Выберите **Мобильные и классические приложения**, чтобы определить тип создаваемого приложения.</span><span class="sxs-lookup"><span data-stu-id="df142-p107">a. Choose **Mobile and Desktop App** to define the kind of app you are creating.</span></span>

    <span data-ttu-id="df142-p108">b. Выберите **Android**, чтобы определить используемую мобильную технологию.</span><span class="sxs-lookup"><span data-stu-id="df142-p108">b. Choose **Android** to define the mobile technology you are using.</span></span>

    <span data-ttu-id="df142-p109">c. Просмотрите общие сведения и, когда закончите, нажмите кнопку **Установка** в нижней части страницы.</span><span class="sxs-lookup"><span data-stu-id="df142-p109">c. Review the introductory topic and when finished, click the **Setup** button at the end of the page.</span></span>

    <span data-ttu-id="df142-p110">d. Следуйте инструкциям на странице **Установка**, чтобы добавить библиотеку MSAL в build.gradle вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="df142-p110">d. Follow the instructions on the **Setup** step to add the MSAL library to your app build.gradle.</span></span>

    <span data-ttu-id="df142-p111">e. Следуйте инструкциям на странице **Использование**, чтобы добавить логику MSAL в новый проект.</span><span class="sxs-lookup"><span data-stu-id="df142-p111">e. Follow the directions on the **Use** step to add MSAL logic to your new project</span></span>

    <span data-ttu-id="df142-p112">f. На странице **Настройка** портал создаст для вас уникальный идентификатор приложения. Используйте его для настройки приложения.</span><span class="sxs-lookup"><span data-stu-id="df142-p112">f. On the **Configure** page, the portal has created a unique application ID for you. Use it to configure your app.</span></span>

    <span data-ttu-id="df142-148">Без инструкций по настройке:</span><span class="sxs-lookup"><span data-stu-id="df142-148">For the unguided flow:</span></span>

    <span data-ttu-id="df142-149">Откроется страница регистрации со свойствами приложения.</span><span class="sxs-lookup"><span data-stu-id="df142-149">The registration page displays, listing the properties of your app.</span></span>

    <span data-ttu-id="df142-p113">a. Скопируйте идентификатор приложения. Это уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="df142-p113">a. Copy the application ID. This is the unique identifier for your app.</span></span> 

    <span data-ttu-id="df142-p114">b. Нажмите **Добавление платформы** и выберите **Собственное приложение**.</span><span class="sxs-lookup"><span data-stu-id="df142-p114">b. Choose **Add Platform** and **Native Application**.</span></span>

    > <span data-ttu-id="df142-p115">**Примечание.** Портал регистрации приложений предоставляет URI перенаправления, который выглядит следующим образом: *msalНОВЫЙ ИДЕНТИФИКАТОР ПРИЛОЖЕНИЯ://auth*. Не используйте встроенные URI перенаправления. [Приложение Connect для Android](https://github.com/microsoftgraph/android-java-connect-sample) использует библиотеку аутентификации MSAL, которой нужен этот URI перенаправления. При использовании [поддерживаемой сторонней библиотеки](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-libraries#compatible-client-libraries) или библиотеки **ADAL** необходимо использовать встроенные URI перенаправления.</span><span class="sxs-lookup"><span data-stu-id="df142-p115">**Note:** The Application Registration Portal provides a Redirect URI with a value of *msalYOUR NEW APP ID://auth*. Do not use the built-in redirect URIs. The [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) implements the MSAL authentication library which requires this redirect URI. If using a [supported third party library](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-libraries#compatible-client-libraries) or the **ADAL** library then you must use the built-in redirect URIs.</span></span>

    <span data-ttu-id="df142-158">С инструкциями по настройке и без них</span><span class="sxs-lookup"><span data-stu-id="df142-158">For Guided Setup flow and unguided flow</span></span>

    <span data-ttu-id="df142-p116">a. Добавьте делегированные разрешения. Вам потребуются разрешения **profile**, **Mail.ReadWrite**, **Mail.Send**, **Files.ReadWrite** и **User.ReadBasic.All**.</span><span class="sxs-lookup"><span data-stu-id="df142-p116">a. Add delegated permissions. You'll need **profile**, **Mail.ReadWrite**, **Mail.Send**, **Files.ReadWrite**, and **User.ReadBasic.All**.</span></span> 
   
    <span data-ttu-id="df142-p117">b. Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="df142-p117">b. Choose **Save**.</span></span>


## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="df142-164">Проверка подлинности пользователя и получение маркера доступа</span><span class="sxs-lookup"><span data-stu-id="df142-164">Authenticate the user and get an access token</span></span>

> <span data-ttu-id="df142-p118">**Примечание.** Если для создания нового приложения вы следовали **инструкциям по настройке** от портала регистрации приложения, эти действия можно пропустить. Дополнительные сведения о Graph API см. в разделе [Вызов Microsoft Graph с помощью пакета SDK Microsoft Graph](#call-microsoft-graph-using-the-microsoft-graph-sdk).</span><span class="sxs-lookup"><span data-stu-id="df142-p118">**Note:** If you followed the instructions in the **Guided Setup** flow from the application registration portal to create a new application, you can skip these steps. Go to [Call Microsoft Graph using the Microsoft Graph SDK](#call-microsoft-graph-using-the-microsoft-graph-sdk) to learn more about the Graph API.</span></span>

<span data-ttu-id="df142-167">Рассмотрим [приложение Connect для Android](https://github.com/microsoftgraph/android-java-connect-sample), чтобы узнать о добавленном коде MSAL и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="df142-167">Let's walk through the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) to learn about the MSAL and Microsoft Graph code we've added.</span></span>

### <a name="add-the-dependency-to-appbuildgradle"></a><span data-ttu-id="df142-168">Добавление зависимости в файл app/build.gradle</span><span class="sxs-lookup"><span data-stu-id="df142-168">Add the dependency to app/build.gradle</span></span>

<span data-ttu-id="df142-169">Откройте файл `build.gradle` в модуле приложения и найдите следующую зависимость:</span><span class="sxs-lookup"><span data-stu-id="df142-169">Open the `build.gradle` file in the app module and find the following dependency:</span></span>

```gradle
    compile ('com.microsoft.identity.client:msal:0.1.+') {
        exclude group: 'com.android.support', module: 'appcompat-v7'
    }
    compile 'com.android.volley:volley:1.0.0'

```

### <a name="start-the-authentication-flow"></a><span data-ttu-id="df142-170">Запуск потока аутентификации</span><span class="sxs-lookup"><span data-stu-id="df142-170">Start the authentication flow</span></span>

1. <span data-ttu-id="df142-171">Откройте файл **AuthenticationManager** и найдите объявление объекта **PublicClientApplication**, а затем значение instation в методе **getInstance**.</span><span class="sxs-lookup"><span data-stu-id="df142-171">Open the **AuthenticationManager** file and find the **PublicClientApplication** object declaration and then the instation in the **getInstance** method.</span></span>

   ```java
    private static PublicClientApplication mPublicClientApplication;
    ....

    public static synchronized AuthenticationManager getInstance() {
        if (INSTANCE == null) {
            INSTANCE = new AuthenticationManager();
            if (mPublicClientApplication == null) {
                mPublicClientApplication = new PublicClientApplication(Connect.getInstance());
            }
        }
        return INSTANCE;
    }

   ```


2. <span data-ttu-id="df142-p119">В классе **ConnectActivity** найдите обработчик событий для события нажатия кнопки **mConnectButton**. Найдите метод **onClick** и просмотрите соответствующий код.</span><span class="sxs-lookup"><span data-stu-id="df142-p119">In the **ConnectActivity** class, locate the event handler for the click event of the **mConnectButton**. Find the **onClick** method and review relevant code.</span></span>
  
    <span data-ttu-id="df142-p120">Метод **connect** позволяет вести журнал личных сведений, а также получает экземпляр вспомогательного класса **AuthenticationManager** и коллекцию пользователей объекта платформы MSAL. Если пользователей нет, запускается поток аутентификации и авторизации Azure AD для нового пользователя. В противном случае токен аутентификации будет получен автоматически.</span><span class="sxs-lookup"><span data-stu-id="df142-p120">The **connect** method enables personally identifyable information (PII) logging, gets an instance of the sample helper class **AuthenticationManager**, and gets the MSAL platform object users collection. If there are no users, the new user is taken to the Azure AD authentication and authorization flow. Otherwise, an authentication token is obtained silently.</span></span>

   ```java
    @Override
    public void onClick(View view) {
        ....
        connect();
    }

        private void connect() {

        if (mEnablePiiLogging) {
            Logger.getInstance().setEnablePII(true);
        } else {
            Logger.getInstance().setEnablePII(false);
        }

        AuthenticationManager mgr = AuthenticationManager.getInstance();

        List<User> users = null;

        try {
            users = mgr.getPublicClient().getUsers();

            if (users != null && users.size() == 1) {
                mUser = users.get(0);
                mgr.callAcquireTokenSilent(mUser, true, this);
            } else {
                mgr.callAcquireToken(
                        this,
                        this);
            }
        } catch (MsalClientException e) {
            Log.d(TAG, "MSAL Exception Generated while getting users: " + e.toString());

        } catch (IndexOutOfBoundsException e) {
            Log.d(TAG, "User at this position does not exist: " + e.toString());
        }
    }

   ```
3. <span data-ttu-id="df142-p121">Найдите обработчик событий, который обрабатывает ответ перенаправления Azure AD, созданный при закрытии пользователем диалогового окна аутентификации. Этот обработчик находится в классе **ConnectActivity**.</span><span class="sxs-lookup"><span data-stu-id="df142-p121">Find the event handler that processes the Azure AD redirect response generated by Azure AD when the user closes the authintication dialog. This handler is in the **ConnectActivity** class.</span></span>

   ```java
       /**
     * Handles redirect response from https://login.microsoftonline.com/common and
     * notifies the MSAL library that the user has completed the authentication
     * dialog
     * @param requestCode
     * @param resultCode
     * @param data
     */
    @Override
    protected void onActivityResult(int requestCode, int resultCode, Intent data) {
        super.onActivityResult(requestCode, resultCode, data);
        if (AuthenticationManager
                .getInstance()
                .getPublicClient() != null) {
            AuthenticationManager
                    .getInstance()
                    .getPublicClient()
                    .handleInteractiveRequestRedirect(requestCode, resultCode, data);
        }
    }

   ```    
3. <span data-ttu-id="df142-179">Найдите метод обратного вызова аутентификации, который кэширует токен аутентификации, используемый в вызовах Graph API.</span><span class="sxs-lookup"><span data-stu-id="df142-179">Find the authentication callback method that caches the authentication token that is used in Graph API calls.</span></span>

 

```java
    /* Callback used for interactive request.  If succeeds we use the access
         * token to call the Microsoft Graph. Does not check cache
         */
    private AuthenticationCallback getAuthInteractiveCallback() {
        return new AuthenticationCallback() {
            @Override
            public void onSuccess(AuthenticationResult authenticationResult) {
            /* Successfully got a token, call graph now */
                Log.d(TAG, "Successfully authenticated");
                Log.d(TAG, "ID Token: " + authenticationResult.getIdToken());

            /* Store the auth result */
                mAuthResult = authenticationResult;
                if (mActivityCallback != null)
                    mActivityCallback.onSuccess(mAuthResult);
            }

            @Override
            public void onError(MsalException exception) {
            /* Failed to acquireToken */
                Log.d(TAG, "Authentication failed: " + exception.toString());
                if (mActivityCallback != null)
                    mActivityCallback.onError(exception);
            }

            @Override
            public void onCancel() {
            /* User canceled the authentication */
                Log.d(TAG, "User cancelled login.");
            }
        };
    }

```
    
<span data-ttu-id="df142-p122">Приложение Connect имеет кнопку **Подключиться** в основном действии. При ее нажатии в первый раз приложение открывает страницу проверки подлинности в браузере устройства. Теперь необходимо обработать код, отправляемый сервером авторизации на URI перенаправления, и обменять его на токен доступа.</span><span class="sxs-lookup"><span data-stu-id="df142-p122">The connect sample app has a **Connect** button on the main activity. If you press the button, on first use, the app presents an authentication page using the device's browser. The next step is to handle the code that the authorization server sends to the redirect URI and exchange it for an access token.</span></span>

### <a name="exchange-the-authorization-code-for-an-access-token"></a><span data-ttu-id="df142-183">Обмен кода авторизации на маркер доступа</span><span class="sxs-lookup"><span data-stu-id="df142-183">Exchange the authorization code for an access token</span></span>

<span data-ttu-id="df142-184">Приложение необходимо подготовить к обработке ответа от сервера авторизации, содержащего код, который можно обменять на маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="df142-184">You need to make your app ready to handle the authorization server response, which contains a code that you can exchange for an access token.</span></span>

1. <span data-ttu-id="df142-p123">Необходимо сообщить системе Android, что приложение Connect может обрабатывать запросы, поступающие на URL-адрес перенаправления, настроенный при регистрации приложения. Для этого откройте файл **AndroidManifest** и добавьте представленные ниже дочерние элементы в элемент проекта **\<application/\>**.</span><span class="sxs-lookup"><span data-stu-id="df142-p123">We need to tell the Android system that Connect app can handle requests to the redirect URL configured in the application registration. To do this open the **AndroidManifest** file and add the following children to the projects  **\<application/\>** element.</span></span>
    ```xml
        <uses-sdk tools:overrideLibrary="com.microsoft.identity.msal" />
        <application ...>
            ...
            <activity
                android:name="com.microsoft.identity.client.BrowserTabActivity">
                <intent-filter>
                    <action android:name="android.intent.action.VIEW" />
                    <category android:name="android.intent.category.DEFAULT" />
                    <category android:name="android.intent.category.BROWSABLE" />
                    <data android:scheme="msalENTER_YOUR_CLIENT_ID"
                        android:host="auth" />
                </intent-filter>
            </activity>
            <meta-data
                android:name="https://login.microsoftonline.com/common"
                android:value="authority string"/>
            <meta-data
                android:name="com.microsoft.identity.client.ClientId"
                android:value="ENTER_YOUR_CLIENT_ID"/>
        </application>
    ```
2. <span data-ttu-id="df142-p124">Библиотеке **MSAL** нужен доступ к идентификатору приложения, назначенному порталом регистрации. **В библиотеке MSAL идентификатор приложения обозначается как "Идентификатор клиента"**. Библиотека получает идентификатор приложения (идентификатор клиента) из контекста приложения, передаваемого в конструктор библиотеки.</span><span class="sxs-lookup"><span data-stu-id="df142-p124">The **MSAL** library needs access to the application Id assigned by the registration portal. **The MSAL library refers to the application Id as the "Client Id"**. It gets the application Id (Client Id) from the application context that you pass in the library constructor.</span></span> 

   ><span data-ttu-id="df142-190">Примечание. Вы также можете указать идентификатор клиента во время выполнения, передав строковый параметр в конструктор.</span><span class="sxs-lookup"><span data-stu-id="df142-190">Note: You can also provide the client Id at run-time by passing a string parameter to the constructor.</span></span> 

3. <span data-ttu-id="df142-p125">Это действие вызывается, когда сервер авторизации отправляет ответ. Запросите токен доступа с ответом от сервера авторизации. Перейдите в класс **AuthenticationManager** и найдите следующий код.</span><span class="sxs-lookup"><span data-stu-id="df142-p125">The activity is invoked when the authorization server sends a response. Request an access token with the response from the authorization server. Go to your **AuthenticationManager** and find the following code in the class.</span></span>

   ```java
    /**
     * Authenticates the user and lets the user authorize the app for the requested permissions.
     * An authentication token is returned via the getAuthInteractiveCalback method
     * @param activity
     * @param authenticationCallback
     */
    public void connect(Activity activity, final MSALAuthenticationCallback authenticationCallback){
        mActivityCallback = authenticationCallback;
        mPublicClientApplication.acquireToken(
                activity, Constants.SCOPES, getAuthInteractiveCallback());
    }


     /* Callback used for interactive request.  If succeeds we use the access
         * token to call the Microsoft Graph. Does not check cache
         */
    private AuthenticationCallback getAuthInteractiveCallback() {
        return new AuthenticationCallback() {
            @Override
            public void onSuccess(AuthenticationResult authenticationResult) {
            /* Successfully got a token, call graph now */
                Log.d(TAG, "Successfully authenticated");
                Log.d(TAG, "ID Token: " + authenticationResult.getIdToken());

            /* Store the auth result */
                mAuthResult = authenticationResult;
                if (mActivityCallback != null)
                    mActivityCallback.onSuccess(mAuthResult);
            }

            @Override
            public void onError(MsalException exception) {
            /* Failed to acquireToken */
                Log.d(TAG, "Authentication failed: " + exception.toString());
                if (mActivityCallback != null)
                    mActivityCallback.onError(exception);
            }

            @Override
            public void onCancel() {
            /* User canceled the authentication */
                Log.d(TAG, "User cancelled login.");
            }
        };
    }

     /**
     * Returns the access token obtained in authentication
     *
     * @return mAccessToken
     */
    public String getAccessToken() throws AuthenticatorException, IOException, OperationCanceledException {
        return  mAuthResult.getAccessToken();
    }

   ```


## <a name="call-microsoft-graph"></a><span data-ttu-id="df142-194">Вызов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="df142-194">Call Microsoft Graph</span></span>
<span data-ttu-id="df142-195">Для вызова Microsoft Graph можно [использовать пакет SDK Microsoft Graph](#call-microsoft-graph-using-the-microsoft-graph-sdk) или [Microsoft Graph REST API](#call-microsoft-graph-using-the-microsoft-graph-rest-api).</span><span class="sxs-lookup"><span data-stu-id="df142-195">You can [use the Microsoft Graph SDK](#call-microsoft-graph-using-the-microsoft-graph-sdk) or the [Microsoft Graph REST API](#call-microsoft-graph-using-the-microsoft-graph-rest-api) to call Microsoft Graph.</span></span>

### <a name="call-microsoft-graph-using-the-microsoft-graph-sdk"></a><span data-ttu-id="df142-196">Вызов Microsoft Graph с помощью пакета SDK Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="df142-196">Call Microsoft Graph using the Microsoft Graph SDK</span></span>
<span data-ttu-id="df142-p126">[Пакет SDK Microsoft Graph для Android](https://github.com/microsoftgraph/msgraph-sdk-android) содержит классы, которые создают запросы и обрабатывают результаты из Microsoft Graph. Чтобы использовать пакет SDK Microsoft Graph, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="df142-p126">The [Microsoft Graph SDK for Android](https://github.com/microsoftgraph/msgraph-sdk-android) provides classes that build requests and process results from Microsoft Graph. Follow these steps to use the Microsoft Graph SDK.</span></span>

1. <span data-ttu-id="df142-p127">Предоставьте приложению разрешения на доступ к Интернету. Откройте файл **AndroidManifest** и добавьте к элементу манифеста представленный ниже дочерний элемент.</span><span class="sxs-lookup"><span data-stu-id="df142-p127">Add Internet permissions to your app. Open the **AndroidManifest** file and add the following child to the manifest element.</span></span>
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
    <uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />

    ```

2. <span data-ttu-id="df142-201">Добавьте зависимости в пакет SDK Microsoft Graph и GSON.</span><span class="sxs-lookup"><span data-stu-id="df142-201">Add dependencies to the Microsoft Graph SDK and GSON.</span></span>
   ```gradle
    compile 'com.microsoft.graph:msgraph-sdk-android:1.3.2'
    compile 'com.google.code.gson:gson:2.7'
   ```


3. <span data-ttu-id="df142-p128">Добавьте токен аутентификации в новые запросы, используя вспомогательный метод **uthenticateRequest**. Этот метод реализует тот же метод, что и интерфейс аутентификации Microsoft Graph **IAuthenticationProvider**.</span><span class="sxs-lookup"><span data-stu-id="df142-p128">Add authentication token to new requests using the **uthenticateRequest** helper method. This method implements the same method from the Microsoft Graph Authentication **IAuthenticationProvider** interface</span></span>
    
   ```java
    /**
     * Appends an access token obtained from the {@link AuthenticationManager} class to the
     * Authorization header of the request.
     * @param request
     */
    @Override
    public void authenticateRequest(IHttpRequest request)  {
        try {
            request.addHeader("Authorization", "Bearer "
                    + AuthenticationManager.getInstance()
                    .getAccessToken());
            // This header has been added to identify this sample in the Microsoft Graph service.
            // If you're using this code for your project please remove the following line.
            request.addHeader("SampleID", "android-java-connect-sample");
        } catch (AuthenticatorException e) {
            e.printStackTrace();
        } catch (IOException e) {
            e.printStackTrace();
        }  catch (OperationCanceledException e) {
            e.printStackTrace();
        } catch (NullPointerException e) {
            e.printStackTrace();
        }
    }
   ```

4. <span data-ttu-id="df142-204">Создайте черновик сообщения электронной почты и отправьте его, используя следующие вспомогательные методы из класса **GraphServiceController**.</span><span class="sxs-lookup"><span data-stu-id="df142-204">Create a draft email and send it using the following helper methods from the **GraphServiceController** helper class.</span></span>

   ```java
    /**
     * Creates a draft email message using the Microsoft Graph API on Office 365. The mail is sent
     * from the address of the signed in user.
     *
     * @param senderPreferredName The mail senders principal user name (email addr)
     * @param emailAddress        The recipient email address.
     * @param subject             The subject to use in the mail message.
     * @param body                The body of the message.
     * @param callback            The callback method to invoke on completion of the POST request
     */
    public void createDraftMail(
            final String senderPreferredName,
            final String emailAddress,
            final String subject,
            final String body,
            ICallback<Message> callback
    ) {
        try {
            // create the email message
            Message message = createMessage(subject, body, emailAddress);
            mGraphServiceClient
                    .getMe()
                    .getMessages()
                    .buildRequest()
                    .post(message, callback);

        } catch (Exception ex) {
            showException(ex, "exception on send mail","Send mail failed", "The send mail method failed");
        }
    }

        /**
     * Creates a new Message object 
     */
    Message createMessage(
            String subject,
            String body,
            String address) {

        if (address == null || address.isEmpty()) {
            throw new IllegalArgumentException("The address parameter can't be null or empty.");
        } else {
            // perform a simple validation of the email address
            String addressParts[] = address.split("@");
            if (addressParts.length != 2 || addressParts[0].length() == 0 || addressParts[1].indexOf('.') == -1) {
                throw new IllegalArgumentException(
                        String.format("The address parameter must be a valid email address {0}", address)
                );
            }
        }
        Message message = new Message();
        EmailAddress emailAddress = new EmailAddress();
        emailAddress.address = address;
        Recipient recipient = new Recipient();
        recipient.emailAddress = emailAddress;
        message.toRecipients = Collections.singletonList(recipient);
        ItemBody itemBody = new ItemBody();
        itemBody.content = body;
        itemBody.contentType = BodyType.html;
        message.body = itemBody;
        message.subject = subject;
        return message;
    }
    /**
     * Sends a draft message to the specified recipients
     *
     * @param messageId String. The id of the message to send
     * @param callback
     */
    public void sendDraftMessage(String messageId,
                                 ICallback<Void> callback) {
        try {

            mGraphServiceClient
                    .getMe()
                    .getMessages(messageId)
                    .getSend()
                    .buildRequest()
                    .post(callback);

        } catch (Exception ex) {
            showException(ex, "exception on send draft message ","Send draft mail failed", "The send draft mail method failed");
        }
    }

   ```
### <a name="call-microsoft-graph-using-the-microsoft-graph-rest-api"></a><span data-ttu-id="df142-205">Вызов Microsoft Graph с помощью REST API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="df142-205">Call Microsoft Graph using the Microsoft Graph REST API</span></span>
<span data-ttu-id="df142-p129">[Microsoft Graph REST API](http://developer.microsoft.com/en-us/graph/docs) предоставляет несколько API-интерфейсов из облачных служб Майкрософт через одну конечную точку REST API. Чтобы использовать REST API, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="df142-p129">The [Microsoft Graph REST API](http://developer.microsoft.com/en-us/graph/docs) exposes multiple APIs from Microsoft cloud services through a single REST API endpoint. Follow these steps to use the REST API.</span></span>

1. <span data-ttu-id="df142-p130">Предоставьте приложению разрешения на доступ к Интернету. Откройте файл **AndroidManifest** и добавьте к элементу манифеста представленный ниже дочерний элемент.</span><span class="sxs-lookup"><span data-stu-id="df142-p130">Add Internet permissions to your app. Open the **AndroidManifest** file and add the following child to the manifest element.</span></span>
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    ```

2. <span data-ttu-id="df142-210">Добавьте зависимость от библиотеки HTTP Volley.</span><span class="sxs-lookup"><span data-stu-id="df142-210">Add a dependency to the Volley HTTP library.</span></span>

    ```gradle
    compile 'com.android.volley:volley:1.0.0'
    ```
   
3. <span data-ttu-id="df142-p131">Замените строку `String accessToken = tokenResponse.accessToken;` приведенным ниже кодом. Вставьте свой адрес электронной почты вместо заполнителя **\<YOUR_EMAIL_ADDRESS\>**.</span><span class="sxs-lookup"><span data-stu-id="df142-p131">Replace the line `String accessToken = tokenResponse.accessToken;` with the following code. Insert your email address in the placeholder marked with **\<YOUR_EMAIL_ADDRESS\>**.</span></span>
   ```java
    final String accessToken = tokenResponse.accessToken;

    final RequestQueue queue = Volley.newRequestQueue(getApplicationContext());
    String url ="https://graph.microsoft.com/v1.0/me/sendMail";
    final String body = "{" +
        "  Message: {" +
        "    subject: 'Sent using the Microsoft Graph REST API'," +
        "    body: {" +
        "      contentType: 'text'," +
        "      content: 'This is the email body'" +
        "    }," +
        "    toRecipients: [" +
        "      {" +
        "        emailAddress: {" +
        "          address: '<YOUR_EMAIL_ADDRESS>'" +
        "        }" +
        "      }" +
        "    ]}" +
        "}";

    final StringRequest stringRequest = new StringRequest(Request.Method.POST, url,
        new Response.Listener<String>() {
            @Override
            public void onResponse(String response) {
                Log.d("Response", response);
            }
        },
        new Response.ErrorListener() {
            @Override
            public void onErrorResponse(VolleyError error) {
                Log.d("ERROR","error => " + error.getMessage());
            }
        }
    ) {
        @Override
        public Map<String, String> getHeaders() throws AuthFailureError {
            Map<String,String> params = new HashMap<>();
            params.put("Authorization", "Bearer " + accessToken);
            params.put("Content-Length", String.valueOf(body.getBytes().length));
            return params;
        }
        @Override
        public String getBodyContentType() {
            return "application/json";
        }
        @Override
        public byte[] getBody() throws AuthFailureError {
            return body.getBytes();
        }
    };

    AsyncTask.execute(new Runnable() {
        @Override
        public void run() {
            queue.add(stringRequest);
        }
    });
   ```

## <a name="run-the-app"></a><span data-ttu-id="df142-213">Запуск приложения</span><span class="sxs-lookup"><span data-stu-id="df142-213">Run the app</span></span>
<span data-ttu-id="df142-214">Теперь вы можете испытать свое приложение для Android.</span><span class="sxs-lookup"><span data-stu-id="df142-214">You're ready to try your Android app.</span></span>

1. <span data-ttu-id="df142-215">Запустите эмулятор Android или подключите к компьютеру физическое устройство.</span><span class="sxs-lookup"><span data-stu-id="df142-215">Start your Android emulator or connect your physical device to your computer.</span></span>
2. <span data-ttu-id="df142-216">Нажмите в Android Studio клавиши SHIFT+F10, чтобы запустить приложение.</span><span class="sxs-lookup"><span data-stu-id="df142-216">In Android Studio, press Shift + F10 to run your app.</span></span>
3. <span data-ttu-id="df142-217">Выберите эмулятор Android или устройство в диалоговом окне развертывания.</span><span class="sxs-lookup"><span data-stu-id="df142-217">Choose your Android emulator or device from the deployment dialog box.</span></span>
4. <span data-ttu-id="df142-218">Нажмите плавающую кнопку основного действия.</span><span class="sxs-lookup"><span data-stu-id="df142-218">Tap the Floating Action Button on the main activity.</span></span>
5. <span data-ttu-id="df142-219">Войдите с помощью личной, рабочей или учебной учетной записи и предоставьте необходимые разрешения.</span><span class="sxs-lookup"><span data-stu-id="df142-219">Sign in with your personal or work or school account and grant the requested permissions.</span></span>
6. <span data-ttu-id="df142-220">Чтобы продолжить, выберите свое приложение в диалоговом окне выбора приложения.</span><span class="sxs-lookup"><span data-stu-id="df142-220">In the app selection dialog, tap your app to continue.</span></span>

<span data-ttu-id="df142-p132">Проверьте папку "Входящие" в почтовом ящике, выбранном в разделе [Вызов Microsoft Graph](#call-microsoft-graph). Вы должны получить сообщение от учетной записи, которая использовалась для входа в приложение.</span><span class="sxs-lookup"><span data-stu-id="df142-p132">Check the inbox of the email address that you configured in [Call Microsoft Graph](#call-microsoft-graph). You should have an email from the account that you used to sign in to the app.</span></span>

## <a name="next-steps"></a><span data-ttu-id="df142-223">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="df142-223">Next steps</span></span>
- <span data-ttu-id="df142-224">Опробуйте [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="df142-224">Try out the [Microsoft Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="df142-225">Вы можете найти примеры распространенных операций в [примере приложения Snippets для Android](https://github.com/microsoftgraph/android-java-snippets-sample) и других [примерах для Android](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=android) на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="df142-225">Find examples of common operations in the [Snippets Sample for Android](https://github.com/microsoftgraph/android-java-snippets-sample), or explore our other [Android samples](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=android) on GitHub.</span></span>


## <a name="see-also"></a><span data-ttu-id="df142-226">См. также</span><span class="sxs-lookup"><span data-stu-id="df142-226">See also</span></span>
- [<span data-ttu-id="df142-227">Пакет SDK Microsoft Graph для Android</span><span class="sxs-lookup"><span data-stu-id="df142-227">Microsoft Graph SDK for Android</span></span>](https://github.com/microsoftgraph/msgraph-sdk-android) 
- [<span data-ttu-id="df142-228">Получение токенов доступа для вызова Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="df142-228">Get access tokens to call Microsoft Graph</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [<span data-ttu-id="df142-229">Получение доступа от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="df142-229">Get access on behalf of a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [<span data-ttu-id="df142-230">Получение доступа без пользователя</span><span class="sxs-lookup"><span data-stu-id="df142-230">Get access without a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)
