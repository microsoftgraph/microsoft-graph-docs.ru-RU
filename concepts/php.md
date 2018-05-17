# <a name="get-started-with-microsoft-graph-in-a-php-app"></a><span data-ttu-id="e8f9e-101">Начало работы с Microsoft Graph в приложении PHP</span><span class="sxs-lookup"><span data-stu-id="e8f9e-101">Get started with Microsoft Graph in a PHP app</span></span>

<span data-ttu-id="e8f9e-p101">В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из конечной точки Azure AD версии 2.0 и вызвать Microsoft Graph. В ней рассматривается создание [приложения Connect для PHP (REST)](https://github.com/microsoftgraph/php-connect-rest-sample) и объясняются основные понятия, которые необходимо реализовать для использования Microsoft Graph. Кроме того, в этой статье рассказывается, как получить доступ к Microsoft Graph с помощью вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call  Microsoft Graph. It walks you through building the [Connect Sample for PHP (REST)](https://github.com/microsoftgraph/php-connect-rest-sample) and explains the main concepts that you implement to use Microsoft Graph. The article also describes how to access Microsoft Graph by using REST calls.</span></span>

<span data-ttu-id="e8f9e-p102">Чтобы использовать Microsoft Graph в приложении PHP, необходимо предоставить пользователям страницу входа в учетную запись Майкрософт. На приведенном ниже снимке экрана показана страница входа в учетную запись Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-p102">To use Microsoft Graph in your PHP app, you need to show the Microsoft sign in page to your users. The following screenshot shows a sign in page for Microsoft accounts.</span></span>

![Страница входа в учетную запись Майкрософт](images/MicrosoftSignIn.png)

<span data-ttu-id="e8f9e-108">**Не хотите создавать приложение?**</span><span class="sxs-lookup"><span data-stu-id="e8f9e-108">**Don't feel like building an app?**</span></span> <span data-ttu-id="e8f9e-109">Скачайте [пример кода подключения для PHP (REST)](https://github.com/microsoftgraph/php-connect-rest-sample), который упоминается в этой статье, и вы будете готовы к работе.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-109">Get up and running fast by downloading the [Connect Sample for PHP (REST)](https://github.com/microsoftgraph/php-connect-rest-sample) that this article is based on.</span></span> <span data-ttu-id="e8f9e-110">Или попробуйте [пример кода подключения для PHP (SDK)](https://github.com/microsoftgraph/php-connect-sample), использующий [библиотеку Microsoft Graph для PHP](https://github.com/microsoftgraph/msgraph-sdk-php).</span><span class="sxs-lookup"><span data-stu-id="e8f9e-110">Or try out the [Connect Sample for PHP (SDK)](https://github.com/microsoftgraph/php-connect-sample) version that uses the [Microsoft Graph Library for PHP](https://github.com/microsoftgraph/msgraph-sdk-php).</span></span>


## <a name="prerequisites"></a><span data-ttu-id="e8f9e-111">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e8f9e-111">Prerequisites</span></span>

<span data-ttu-id="e8f9e-112">Чтобы приступить к работе, вам понадобится следующее:</span><span class="sxs-lookup"><span data-stu-id="e8f9e-112">To get started, you'll need:</span></span> 

- <span data-ttu-id="e8f9e-113">[Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types).</span><span class="sxs-lookup"><span data-stu-id="e8f9e-113">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types)</span></span>
- <span data-ttu-id="e8f9e-114">PHP версии 5.5.9 или выше.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-114">PHP version 5.5.9 or greater</span></span>
- <span data-ttu-id="e8f9e-115">[Композитор](https://getcomposer.org/).</span><span class="sxs-lookup"><span data-stu-id="e8f9e-115">[Composer](https://getcomposer.org/)</span></span>


## <a name="register-the-application"></a><span data-ttu-id="e8f9e-116">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="e8f9e-116">Register the application</span></span>
<span data-ttu-id="e8f9e-p104">Зарегистрируйте приложение на портале регистрации приложений Майкрософт. При этом будут созданы идентификатор и пароль приложения, которые понадобятся при его настройке.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-p104">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app.</span></span>

1. <span data-ttu-id="e8f9e-119">Войдите на [портал регистрации приложений Майкрософт](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-119">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="e8f9e-120">Нажмите кнопку **Добавить приложение**.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-120">Choose **Add an app**.</span></span>

3. <span data-ttu-id="e8f9e-121">Введите имя приложения и нажмите кнопку **Создать приложение**.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-121">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="e8f9e-122">Откроется страница регистрации со свойствами приложения.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-122">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="e8f9e-123">Нажмите **Создать новый пароль**.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-123">Choose **Generate New Password**.</span></span>

5. <span data-ttu-id="e8f9e-124">Скопируйте идентификатор и пароль приложения.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-124">Copy the application ID and password.</span></span>

6. <span data-ttu-id="e8f9e-125">Нажмите кнопку **Добавление платформы** и выберите **Веб**.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-125">Choose **Add Platform** and **Web**.</span></span>

7. <span data-ttu-id="e8f9e-126">В поле **URI перенаправления** введите `http://localhost:8000/oauth`.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-126">In the **Redirect URI** field, type `http://localhost:8000/oauth`.</span></span>

8. <span data-ttu-id="e8f9e-127">Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-127">Choose **Save**.</span></span>


## <a name="configure-the-project"></a><span data-ttu-id="e8f9e-128">Настройка проекта</span><span class="sxs-lookup"><span data-stu-id="e8f9e-128">Configure the project</span></span>

<span data-ttu-id="e8f9e-p105">Создайте проект с помощью композитора. Чтобы создать проект PHP с помощью платформы Laravel, используйте следующую команду:</span><span class="sxs-lookup"><span data-stu-id="e8f9e-p105">Start a new project using composer. To create a new PHP project using the Laravel framework, use the following command:</span></span>

```bash
composer create-project --prefer-dist laravel/laravel getstarted
```
 
<span data-ttu-id="e8f9e-131">Будет создана папка **getstarted**, которую можно использовать для этого проекта.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-131">This creates a **getstarted** folder that you can use for this project.</span></span>

> <span data-ttu-id="e8f9e-132">Примечание. Вы также можете использовать [начальный проект](https://github.com/microsoftgraph/php-connect-rest-sample/tree/master/starter-project) с готовой конфигурацией, чтобы сосредоточиться на программировании.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-132">Note: You can also use the [Starter project](https://github.com/microsoftgraph/php-connect-rest-sample/tree/master/starter-project) that takes care of the project configuration so you can focus on the coding sections of this walkthrough.</span></span>

## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="e8f9e-133">Проверка подлинности пользователя и получение маркера доступа</span><span class="sxs-lookup"><span data-stu-id="e8f9e-133">Authenticate the user and get an access token</span></span>
<span data-ttu-id="e8f9e-p106">Для упрощения проверки подлинности мы будем использовать библиотеку OAuth. [PHP League](http://thephpleague.com/) предоставляет [клиентскую библиотеку OAuth](https://github.com/thephpleague/oauth2-client), которую можно использовать в этом проекте.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-p106">Use an OAuth library to simplify the authentication process. [The PHP League](http://thephpleague.com/) provides an [OAuth client library](https://github.com/thephpleague/oauth2-client) that you can use in this project.</span></span>

### <a name="add-the-dependency-to-composer"></a><span data-ttu-id="e8f9e-136">Добавление зависимости в композитор</span><span class="sxs-lookup"><span data-stu-id="e8f9e-136">Add the dependency to composer</span></span>

<span data-ttu-id="e8f9e-137">Откройте файл `composer.json` и добавьте следующую зависимость в разделе **require**:</span><span class="sxs-lookup"><span data-stu-id="e8f9e-137">Open the `composer.json` file and include the following dependency in the **require** section:</span></span>

```json
"league/oauth2-client": "^1.4"
```

<span data-ttu-id="e8f9e-138">Обновите зависимости, выполнив следующую команду:</span><span class="sxs-lookup"><span data-stu-id="e8f9e-138">Update the dependencies by running the following command:</span></span>

```bash
composer update
```

### <a name="start-the-authentication-flow"></a><span data-ttu-id="e8f9e-139">Запуск потока проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="e8f9e-139">Start the authentication flow</span></span>

1. <span data-ttu-id="e8f9e-p107">Откройте файл **resources** > **views** > **welcome.blade.php**. Замените элемент div **title** приведенным ниже кодом.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-p107">Open the **resources** > **views** > **welcome.blade.php** file. Replace the **title** div element with the following code.</span></span>
    ```html
    <div class="title" onClick="window.location='/oauth'">Sign in to Microsoft</div>
    ```
    
2. <span data-ttu-id="e8f9e-p108">Добавьте подсказку типа для класса `Illuminate\Http\Request` в файле **app** > **Http** > **routes.php**. Добавляйте приведенную ниже строку перед каждым объявлением маршрута.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-p108">Type-hint the `Illuminate\Http\Request` class on the **app** > **Http** > **routes.php** file. Add the following line before any route declaration.</span></span>
    ```php
    use Illuminate\Http\Request;
    ```
    
3. <span data-ttu-id="e8f9e-p109">Добавьте маршрут */oauth* в файл **app** > **Http** > **routes.php**. Чтобы добавить маршрут, вставьте приведенный ниже код после объявления маршрута по умолчанию. Вставьте **идентификатор приложения** и **пароль** вместо заполнителей **\<YOUR_APPLICATION_ID\>** и **\<YOUR_PASSWORD\>** соответственно.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-p109">Add an */oauth* route to the **app** > **Http** > **routes.php** file. To add the route, copy the following code after the default route declaration. Insert the **application ID** and **password** of your app in the placeholder marked with **\<YOUR_APPLICATION_ID\>** and **\<YOUR_PASSWORD\>** respectively.</span></span>
    ```php
    Route::get('/oauth', function () {
        $provider = new \League\OAuth2\Client\Provider\GenericProvider([
            'clientId'                => '<YOUR_APPLICATION_ID>',
            'clientSecret'            => '<YOUR_PASSWORD>',
            'redirectUri'             => 'http://localhost:8000/oauth',
            'urlAuthorize'            => 'https://login.microsoftonline.com/common/oauth2/v2.0/authorize',
            'urlAccessToken'          => 'https://login.microsoftonline.com/common/oauth2/v2.0/token',
            'urlResourceOwnerDetails' => '',
            'scopes'                  => 'openid mail.send'
        ]);

        if (!$request->has('code')) {
            return redirect($provider->getAuthorizationUrl());
        }
    });
    ```
    
<span data-ttu-id="e8f9e-p110">На этом этапе у вас должно получиться приложение PHP, отображающее страницу *входа в учетную запись Майкрософт*. Если нажать текст, приложение откроет страницу входа в учетную запись Майкрософт. Теперь необходимо обработать код, отправляемый сервером авторизации на URI перенаправления, и обменять его на маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-p110">At this point, you should have a PHP app that displays *Sign in to Microsoft*. If you click the text, the app presents the Microsoft sign-in page. The next step is to handle the code that the authorization server sends to the redirect URI and exchange it for an access token.</span></span>

### <a name="exchange-the-authorization-code-for-an-access-token"></a><span data-ttu-id="e8f9e-150">Обмен кода авторизации на маркер доступа</span><span class="sxs-lookup"><span data-stu-id="e8f9e-150">Exchange the authorization code for an access token</span></span>

<span data-ttu-id="e8f9e-151">Необходимо обработать ответ сервера авторизации, содержащий код, который можно обменять на маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-151">You need to handle the authorization server response, which contains a code that you can exchange for an access token.</span></span>

<span data-ttu-id="e8f9e-p111">Измените маршрут */oauth* так, чтобы приложение могло получать маркер доступа с помощью кода авторизации. Для этого откройте файл **app** > **Http** > **routes.php** и добавьте условное предложение *else* к оператору *if*.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-p111">Update the */oauth* route so it can get an access token with the authorization code. To do this, open the **app** > **Http** > **routes.php** file and add the following *else* conditional clause to the existing *if* statement.</span></span>

```php
if (!$request->has('code')) {
    ...
    // add the following lines
} else {
    $accessToken = $provider->getAccessToken('authorization_code', [
        'code'     => $request->input('code')
    ]);
    exit($accessToken->getToken());
}
```
    
<span data-ttu-id="e8f9e-p112">Обратите внимание, что маркер доступа содержится в строке `exit($accessToken->getToken());`. Теперь вы готовы добавить код для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-p112">Note that you have an access token in this line: `exit($accessToken->getToken());`. Now you're ready to add code to call Microsoft Graph.</span></span> 

## <a name="call-microsoft-graph-using-rest"></a><span data-ttu-id="e8f9e-156">Вызов Microsoft Graph с помощью REST</span><span class="sxs-lookup"><span data-stu-id="e8f9e-156">Call Microsoft Graph using REST</span></span>
<span data-ttu-id="e8f9e-p113">Microsoft Graph можно вызвать с помощью REST. Замените строку `exit($accessToken->getToken());` приведенным ниже кодом. Вставьте свой адрес электронной почты вместо заполнителя **\<YOUR_EMAIL_ADDRESS\>**.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-p113">You can call Microsoft Graph using REST. Replace the line `exit($accessToken->getToken());` with the following code. Insert your email address in the placeholder marked with **\<YOUR_EMAIL_ADDRESS\>**.</span></span>

```php
$client = new \GuzzleHttp\Client();

$email = "{
    Message: {
    Subject: 'Sent using the Microsoft Graph REST API',
    Body: {
        ContentType: 'text',
        Content: 'This is the email body'
    },
    ToRecipients: [
        {
            EmailAddress: {
            Address: '<YOUR_EMAIL_ADDRESS>'
            }
        }
    ]
    }}";

$response = $client->request('POST', 'https://graph.microsoft.com/v1.0/me/sendmail', [
    'headers' => [
        'Authorization' => 'Bearer ' . $accessToken->getToken(),
        'Content-Type' => 'application/json;odata.metadata=minimal;odata.streaming=true'
    ],
    'body' => $email
]);
if($response.getStatusCode() === 201) {
    exit('Email sent, check your inbox');
} else {
    exit('There was an error sending the email. Status code: ' . $response.getStatusCode());
}
```

## <a name="run-the-app"></a><span data-ttu-id="e8f9e-160">Запуск приложения</span><span class="sxs-lookup"><span data-stu-id="e8f9e-160">Run the app</span></span>
<span data-ttu-id="e8f9e-161">Теперь вы можете испытать свое приложение PHP.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-161">You're ready to try your PHP app.</span></span>

1. <span data-ttu-id="e8f9e-162">В командной консоли введите следующую команду:</span><span class="sxs-lookup"><span data-stu-id="e8f9e-162">In your shell, type the following command:</span></span>
    ```bash
    php artisan serve
    ```
    
2. <span data-ttu-id="e8f9e-163">Введите адрес `http://localhost:8000` в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-163">Go to `http://localhost:8000` in your web browser.</span></span>
3. <span data-ttu-id="e8f9e-164">Нажмите **Войти в учетную запись Майкрософт**.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-164">Choose **Sign in to Microsoft**.</span></span>
4. <span data-ttu-id="e8f9e-165">Войдите с помощью личной, рабочей или учебной учетной записи и предоставьте необходимые разрешения.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-165">Sign in with your personal or work or school account and grant the requested permissions.</span></span>

<span data-ttu-id="e8f9e-p114">Проверьте папку "Входящие" в почтовом ящике, выбранном в разделе [Вызов Microsoft Graph с помощью REST](#call-microsoft-graph-using-rest). Вы должны получить сообщение от учетной записи, которая использовалась для входа в приложение.</span><span class="sxs-lookup"><span data-stu-id="e8f9e-p114">Check the inbox of the email address that you configured in [Call the Microsoft Graph using REST](#call-microsoft-graph-using-rest) section. You should have an email from the account that you used to sign in to the app.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e8f9e-168">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="e8f9e-168">Next steps</span></span>
- <span data-ttu-id="e8f9e-169">Опробуйте [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="e8f9e-169">Try out the [Microsoft Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>


## <a name="see-also"></a><span data-ttu-id="e8f9e-170">См. также</span><span class="sxs-lookup"><span data-stu-id="e8f9e-170">See also</span></span>
* [<span data-ttu-id="e8f9e-171">Протоколы Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="e8f9e-171">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
* [<span data-ttu-id="e8f9e-172">Маркеры Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="e8f9e-172">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
