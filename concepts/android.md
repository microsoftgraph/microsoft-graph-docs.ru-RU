# <a name="get-started-with-microsoft-graph-in-an-android-app"></a>Начало работы с Microsoft Graph в приложении для Android

> **Создаете приложения для корпоративных клиентов?** Ваше приложение может не работать, если корпоративный клиент включит функции корпоративной безопасности для мобильных устройств, например <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">условный доступ с устройств</a>. В этом случае у пользователей могут возникать ошибки, а вы не будете об этом знать. 

> Для поддержки **всех корпоративных клиентов** в **любых корпоративных сценариях** необходимо использовать конечную точку Azure AD и управлять приложениями с помощью [портала управления Azure](https://aka.ms/aadapplist). Дополнительные сведения см. в разделе [Выбор между конечными точками Azure AD и Azure AD версии 2.0](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).

В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из конечной точки Azure AD версии 2.0 и вызвать Microsoft Graph. В ней рассматривается создание [примера приложения Connect для Android](https://github.com/microsoftgraph/android-java-connect-sample) и объясняются основные понятия, которые необходимо реализовать для использования Microsoft Graph в приложении для Android. В этой статье также описывается, как получить доступ к Microsoft Graph с помощью [пакета SDK Microsoft Graph для Android](https://github.com/microsoftgraph/msgraph-sdk-android) или необработанных вызовов REST.

Чтобы использовать Microsoft Graph в приложении для Android, необходимо предоставить пользователям страницу входа в учетную запись Майкрософт, как показано на приведенном ниже снимке экрана.

![Страница входа в учетную запись Майкрософт на Android](images/AndroidConnect.png)

**Не хотите создавать приложение?** Скачайте пример [приложения Connect для Android](https://github.com/microsoftgraph/android-java-connect-sample), на котором основана эта статья, и вы будете готовы к работе.


## <a name="prerequisites"></a>Необходимые условия

Чтобы приступить к работе, вам понадобится следующее: 

- [Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](http://dev.office.com/devprogram).
- Android Studio 2.0 или более новой версии


## <a name="configure-a-new-project"></a>Настройка нового проекта

Если вы скачали [приложение Connect для Android](https://github.com/microsoftgraph/android-java-connect-sample), пропустите этот шаг. 

Создайте новый проект в Android Studio. Большинство параметров в мастере можно оставить без изменений, но обязательно выберите следующие параметры:

* На странице Target Android Devices (Целевые устройства Android) установите флажок **Phone and Tablet (Телефон и планшет)**
    * В поле Minimum SDK (Минимальная версия пакета SDK) выберите значение **API 16: Android 4.1 (Jelly Bean)**
* На странице Add an Activity to Mobile (Добавить действие к мобильному устройству) выберите **Basic Activity (Основное действие)**
 
В результате получится проект Android с действием и кнопкой для аутентификации пользователя.


## <a name="register-the-application"></a>Регистрация приложения

Вам нужно зарегистрировать приложение на [портале Майкрософт](https://apps.dev.microsoft.com/) независимо от того, скачали ли вы приложение Connect или создали новый проект.

Зарегистрируйте приложение на портале Майкрософт. При этом будет создан идентификатор приложения, который понадобится при его настройке.

1. Войдите на [портал регистрации приложений Майкрософт](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.

2. Нажмите кнопку **Добавить приложение**.

>Совет. Если вы скачали [приложение Connect для Android](https://github.com/microsoftgraph/android-java-connect-sample) и просто регистрируете его, снимите флажок **Инструкции по настройке** перед нажатием кнопки **Создать**.

3. Введите имя приложения и нажмите **Создать**. 
    
    С **инструкциями по настройке**:
 
    a. Выберите **Мобильные и классические приложения**, чтобы определить тип создаваемого приложения.

    b. Выберите **Android**, чтобы определить используемую мобильную технологию.

    c. Просмотрите общие сведения и, когда закончите, нажмите кнопку **Установка** в нижней части страницы.

    d. Следуйте инструкциям на странице **Установка**, чтобы добавить библиотеку MSAL в build.gradle вашего приложения.

    e. Следуйте инструкциям на странице **Использование**, чтобы добавить логику MSAL в новый проект.

    f. На странице **Настройка** портал создаст для вас уникальный идентификатор приложения. Используйте его для настройки приложения.

    Без инструкций по настройке:

    Откроется страница регистрации со свойствами приложения.

    a. Скопируйте идентификатор приложения. Это уникальный идентификатор приложения. 

    b. Нажмите **Добавление платформы** и выберите **Собственное приложение**.

    > **Примечание.** Портал регистрации приложений предоставляет URI перенаправления, который выглядит следующим образом: *msalНОВЫЙ ИДЕНТИФИКАТОР ПРИЛОЖЕНИЯ://auth*. Не используйте встроенные URI перенаправления. [Приложение Connect для Android](https://github.com/microsoftgraph/android-java-connect-sample) использует библиотеку аутентификации MSAL, которой нужен этот URI перенаправления. При использовании [поддерживаемой сторонней библиотеки](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-libraries#compatible-client-libraries) или библиотеки **ADAL** необходимо использовать встроенные URI перенаправления.

    С инструкциями по настройке и без них

    a. Добавьте делегированные разрешения. Вам потребуются разрешения **profile**, **Mail.ReadWrite**, **Mail.Send**, **Files.ReadWrite** и **User.ReadBasic.All**. 
   
    b. Нажмите кнопку **Сохранить**.


## <a name="authenticate-the-user-and-get-an-access-token"></a>Проверка подлинности пользователя и получение маркера доступа

> **Примечание.** Если для создания нового приложения вы следовали **инструкциям по настройке** от портала регистрации приложения, эти действия можно пропустить. Дополнительные сведения о Graph API см. в разделе [Вызов Microsoft Graph с помощью пакета SDK Microsoft Graph](#call-microsoft-graph-using-the-microsoft-graph-sdk).

Рассмотрим [приложение Connect для Android](https://github.com/microsoftgraph/android-java-connect-sample), чтобы узнать о добавленном коде MSAL и Microsoft Graph.

### <a name="add-the-dependency-to-appbuildgradle"></a>Добавление зависимости в файл app/build.gradle

Откройте файл `build.gradle` в модуле приложения и найдите следующую зависимость:

```gradle
    compile ('com.microsoft.identity.client:msal:0.1.+') {
        exclude group: 'com.android.support', module: 'appcompat-v7'
    }
    compile 'com.android.volley:volley:1.0.0'

```

### <a name="start-the-authentication-flow"></a>Запуск потока аутентификации

1. Откройте файл **AuthenticationManager** и найдите объявление объекта **PublicClientApplication**, а затем значение instation в методе **getInstance**.

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


2. В классе **ConnectActivity** найдите обработчик событий для события нажатия кнопки **mConnectButton**. Найдите метод **onClick** и просмотрите соответствующий код.
  
    Метод **connect** позволяет вести журнал личных сведений, а также получает экземпляр вспомогательного класса **AuthenticationManager** и коллекцию пользователей объекта платформы MSAL. Если пользователей нет, запускается поток аутентификации и авторизации Azure AD для нового пользователя. В противном случае токен аутентификации будет получен автоматически.

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
3. Найдите обработчик событий, который обрабатывает ответ перенаправления Azure AD, созданный при закрытии пользователем диалогового окна аутентификации. Этот обработчик находится в классе **ConnectActivity**.

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
3. Найдите метод обратного вызова аутентификации, который кэширует токен аутентификации, используемый в вызовах Graph API.

 

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
    
Приложение Connect имеет кнопку **Подключиться** в основном действии. При ее нажатии в первый раз приложение открывает страницу проверки подлинности в браузере устройства. Теперь необходимо обработать код, отправляемый сервером авторизации на URI перенаправления, и обменять его на токен доступа.

### <a name="exchange-the-authorization-code-for-an-access-token"></a>Обмен кода авторизации на маркер доступа

Приложение необходимо подготовить к обработке ответа от сервера авторизации, содержащего код, который можно обменять на маркер доступа.

1. Необходимо сообщить системе Android, что приложение Connect может обрабатывать запросы, поступающие на URL-адрес перенаправления, настроенный при регистрации приложения. Для этого откройте файл **AndroidManifest** и добавьте представленные ниже дочерние элементы в элемент проекта **\<application/\>**.
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
2. Библиотеке **MSAL** нужен доступ к идентификатору приложения, назначенному порталом регистрации. **В библиотеке MSAL идентификатор приложения обозначается как "Идентификатор клиента"**. Библиотека получает идентификатор приложения (идентификатор клиента) из контекста приложения, передаваемого в конструктор библиотеки. 

   >Примечание. Вы также можете указать идентификатор клиента во время выполнения, передав строковый параметр в конструктор. 

3. Это действие вызывается, когда сервер авторизации отправляет ответ. Запросите токен доступа с ответом от сервера авторизации. Перейдите в класс **AuthenticationManager** и найдите следующий код.

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


## <a name="call-microsoft-graph"></a>Вызов Microsoft Graph
Для вызова Microsoft Graph можно [использовать пакет SDK Microsoft Graph](#call-microsoft-graph-using-the-microsoft-graph-sdk) или [Microsoft Graph REST API](#call-microsoft-graph-using-the-microsoft-graph-rest-api).

### <a name="call-microsoft-graph-using-the-microsoft-graph-sdk"></a>Вызов Microsoft Graph с помощью пакета SDK Microsoft Graph
[Пакет SDK Microsoft Graph для Android](https://github.com/microsoftgraph/msgraph-sdk-android) содержит классы, которые создают запросы и обрабатывают результаты из Microsoft Graph. Чтобы использовать пакет SDK Microsoft Graph, выполните указанные ниже действия.

1. Предоставьте приложению разрешения на доступ к Интернету. Откройте файл **AndroidManifest** и добавьте к элементу манифеста представленный ниже дочерний элемент.
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
    <uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />

    ```

2. Добавьте зависимости в пакет SDK Microsoft Graph и GSON.
   ```gradle
    compile 'com.microsoft.graph:msgraph-sdk-android:1.3.2'
    compile 'com.google.code.gson:gson:2.7'
   ```


3. Добавьте токен аутентификации в новые запросы, используя вспомогательный метод **uthenticateRequest**. Этот метод реализует тот же метод, что и интерфейс аутентификации Microsoft Graph **IAuthenticationProvider**.
    
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

4. Создайте черновик сообщения электронной почты и отправьте его, используя следующие вспомогательные методы из класса **GraphServiceController**.

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
### <a name="call-microsoft-graph-using-the-microsoft-graph-rest-api"></a>Вызов Microsoft Graph с помощью REST API Microsoft Graph
[Microsoft Graph REST API](http://developer.microsoft.com/en-us/graph/docs) предоставляет несколько API-интерфейсов из облачных служб Майкрософт через одну конечную точку REST API. Чтобы использовать REST API, выполните указанные ниже действия.

1. Предоставьте приложению разрешения на доступ к Интернету. Откройте файл **AndroidManifest** и добавьте к элементу манифеста представленный ниже дочерний элемент.
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    ```

2. Добавьте зависимость от библиотеки HTTP Volley.

    ```gradle
    compile 'com.android.volley:volley:1.0.0'
    ```
   
3. Замените строку `String accessToken = tokenResponse.accessToken;` приведенным ниже кодом. Вставьте свой адрес электронной почты вместо заполнителя **\<YOUR_EMAIL_ADDRESS\>**.
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

## <a name="run-the-app"></a>Запуск приложения
Теперь вы можете испытать свое приложение для Android.

1. Запустите эмулятор Android или подключите к компьютеру физическое устройство.
2. Нажмите в Android Studio клавиши SHIFT+F10, чтобы запустить приложение.
3. Выберите эмулятор Android или устройство в диалоговом окне развертывания.
4. Нажмите плавающую кнопку основного действия.
5. Войдите с помощью личной, рабочей или учебной учетной записи и предоставьте необходимые разрешения.
6. Чтобы продолжить, выберите свое приложение в диалоговом окне выбора приложения.

Проверьте папку "Входящие" в почтовом ящике, выбранном в разделе [Вызов Microsoft Graph](#call-microsoft-graph). Вы должны получить сообщение от учетной записи, которая использовалась для входа в приложение.

## <a name="next-steps"></a>Дальнейшие действия
- Опробуйте [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).
- Вы можете найти примеры распространенных операций в [примере приложения Snippets для Android](https://github.com/microsoftgraph/android-java-snippets-sample) и других [примерах для Android](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=android) на сайте GitHub.


## <a name="see-also"></a>См. также
- [Пакет SDK Microsoft Graph для Android](https://github.com/microsoftgraph/msgraph-sdk-android) 
- [Получение токенов доступа для вызова Microsoft Graph](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [Получение доступа от имени пользователя](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [Получение доступа без пользователя](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)
