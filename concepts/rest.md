# <a name="get-started-with-microsoft-graph-and-rest"></a><span data-ttu-id="e2dd4-101">Начало работы с Microsoft Graph и REST</span><span class="sxs-lookup"><span data-stu-id="e2dd4-101">Get started with Microsoft Graph and REST</span></span>

<span data-ttu-id="e2dd4-p101">В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из конечной точки Azure AD версии 2.0 и вызвать Microsoft Graph с помощью вызовов REST. В ней описывается последовательность запросов и ответов, которую приложение использует для проверки подлинности и получения электронных сообщений.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph using REST calls. It describes the sequence of requests and responses that an app uses to authenticate and retrieve email messages.</span></span>

<span data-ttu-id="e2dd4-104">Для начала необходимо зарегистрировать приложение в службе Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="e2dd4-104">First, you need register your app with Azure Active Directory (Azure AD).</span></span> 

## <a name="register-the-application"></a><span data-ttu-id="e2dd4-105">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="e2dd4-105">Register the application</span></span>

<span data-ttu-id="e2dd4-106">В настоящее время существует два способа регистрации приложения в Azure AD:</span><span class="sxs-lookup"><span data-stu-id="e2dd4-106">There are currently two options to register your app with Azure AD.</span></span>

  - <span data-ttu-id="e2dd4-107">Регистрация приложения для использования конечной точки Azure AD версии 2.0, которая подходит как для личных удостоверений (учетных записей Майкрософт), так и для рабочих и учебных учетных записей (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="e2dd4-107">Register an app to use the Azure AD v2.0 endpoint that works for both personal (Microsoft) identities and work and school (Azure AD) accounts.</span></span>
  - <span data-ttu-id="e2dd4-108">Регистрация приложения для использования конечной точки Azure AD, которая поддерживает только рабочие и учебные учетные записи.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-108">Register an app to use the Azure AD endpoint that supports work and school accounts only.</span></span>

<span data-ttu-id="e2dd4-p102">В этой статье рассматривается регистрация с помощью конечной точки версии 2.0, поэтому мы будем использовать [портал регистрации приложений](https://apps.dev.microsoft.com/). Чтобы зарегистрировать приложение, выполните действия, указанные в статье [Регистрация приложения Microsoft Graph с помощью конечной точки Azure AD версии 2.0](../concepts/auth_register_app_v2.md). Сведения об использовании конечной точки Azure AD см. в статье [Проверка подлинности с помощью Azure AD](../concepts/auth_v2_user.md).</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p102">This article assumes a v2.0 registration, so you'll register your app on the [Application Registration Portal](https://apps.dev.microsoft.com/). Follow the instructions in [Register your Microsoft Graph application with the Azure AD v2.0 endpoint](../concepts/auth_register_app_v2.md) to register your app. For information about using the Azure AD endpoint, see [Authenticate using Azure AD](../concepts/auth_v2_user.md).</span></span>

> <span data-ttu-id="e2dd4-p103">При использовании конечной точки версии 2.0 действуют некоторые ограничения. Сведения о том, как выбрать подходящий способ, см. в статье [Следует ли мне использовать конечную точку версии 2.0?](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/)</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p103">Some limitations apply when using the v2.0 endpoint. To decide if it's right for you, see [Should I use the v2.0 endpoint?](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/)</span></span>

## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="e2dd4-114">Проверка подлинности пользователя и получение маркера доступа</span><span class="sxs-lookup"><span data-stu-id="e2dd4-114">Authenticate the user and get an access token</span></span>

<span data-ttu-id="e2dd4-p104">В описанном здесь приложении реализован [поток предоставления кода авторизации](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-code/) для получения маркеров доступа из конечной точки Azure AD версии 2.0 в соответствии со стандартными [протоколами OAuth 2.0](http://tools.ietf.org/html/rfc6749). Полное руководство по потокам, поддерживаемым в конечной точке Azure AD версии 2.0, см. в статье [Типы конечной точки версии 2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-flows/).</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p104">The app described in this article implements the [Authorization Code Grant flow](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-code/) to get access tokens from the Azure AD v2.0 endpoint, following standard [OAuth 2.0 protocols](http://tools.ietf.org/html/rfc6749). For a complete guide to the flows supported in the Azure AD v2.0 endpoint see [Types of the v2.0 endpoint](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-flows/).</span></span>

<span data-ttu-id="e2dd4-117">В потоке предоставления кода авторизации вы сначала получаете код авторизации, а затем обмениваете его на маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-117">With the Authorization Code Grant flow, first you get an authorization code and then you exchange the code for an access token.</span></span>

### <a name="getting-an-authorization-code"></a><span data-ttu-id="e2dd4-118">Получение кода авторизации</span><span class="sxs-lookup"><span data-stu-id="e2dd4-118">Getting an authorization code</span></span>

<span data-ttu-id="e2dd4-p105">Чтобы использовать поток предоставления кода авторизации, сначала необходимо получить код. Приложение получает код от сервера авторизации, когда пользователь выполняет вход и предоставляет приложению запрашиваемые разрешения.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p105">The first step in the Authorization Code Grant flow is to get an authorization code. The code is returned to the app by the authorization server when the user signs in and consents to the permissions requested by the app.</span></span>

<span data-ttu-id="e2dd4-p106">Чтобы запросить код авторизации, необходимо отправить запрос GET конечной точке Azure AD версии 2.0. Этот URL-адрес нужно открыть в браузере, чтобы пользователь мог выполнить вход и предоставить требуемые разрешения.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p106">You request an authorization code by sending a GET request to the Azure AD v2.0 endpoint. This URL must be opened in a browser so that the user can sign in and provide consent.</span></span>

#### <a name="construct-the-request"></a><span data-ttu-id="e2dd4-123">Создание запроса</span><span class="sxs-lookup"><span data-stu-id="e2dd4-123">Construct the request</span></span>

<span data-ttu-id="e2dd4-124">1. Начните с базового URL-адреса:</span><span class="sxs-lookup"><span data-stu-id="e2dd4-124">1- Start with the base URL:</span></span>

```
https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
```

<span data-ttu-id="e2dd4-p107">сегмент *tenant* в пути указывает, кто может входить в приложение. Допустимые значения: *common*, *organizations*, *consumers* и идентификаторы клиентов. Дополнительные сведения см. в разделе [Endpoints](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/#endpoints).</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p107">The *tenant* segment in the path controls who can sign into the application. Allowed values are *common*, *organizations*, *consumers*, and tenant identifiers. For more information, see [Protocol endpoints](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/#endpoints).</span></span>

<span data-ttu-id="e2dd4-p108">2. Добавьте параметры запроса к базовому URL-адресу. Они используются для идентификации приложения, запрашиваемых разрешений и других данных запроса на проверку подлинности. В приведенной ниже таблице описываются некоторые распространенные параметры.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p108">2- Append query parameters to the base URL. These are used to identify the app, the requested permissions, and other auth request information. The following table describes some common parameters.</span></span>

| <span data-ttu-id="e2dd4-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="e2dd4-131">Parameter</span></span> | <span data-ttu-id="e2dd4-132">Описания</span><span class="sxs-lookup"><span data-stu-id="e2dd4-132">Descriptions</span></span> |
|:------|:------|
| <span data-ttu-id="e2dd4-133">client_id</span><span class="sxs-lookup"><span data-stu-id="e2dd4-133">client_id</span></span> | <span data-ttu-id="e2dd4-p109">Идентификатор приложения, создаваемый при его регистрации. С его помощью Azure AD определяет приложения, которые запрашивают вход.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p109">The app ID generated by registering the app. This lets Azure AD know which app is requesting the logon.</span></span> |
| <span data-ttu-id="e2dd4-136">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="e2dd4-136">redirect_uri</span></span> | <span data-ttu-id="e2dd4-p110">Адрес, на который Azure перенаправит пользователя после того, как он разрешит приложению доступ. Это значение должно соответствовать значению **URI перенаправления**, которое использовалось при регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p110">The location that Azure will redirect to after the user has granted consent to the app. This value must correspond to the value of **Redirect URI** used when registering the app.</span></span> |
| <span data-ttu-id="e2dd4-139">response_type</span><span class="sxs-lookup"><span data-stu-id="e2dd4-139">response_type</span></span> | <span data-ttu-id="e2dd4-p111">Тип ответа, который ожидается приложением. Для потока предоставления кода авторизации используется значение `code`.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p111">The type of response the app is expecting. This value is `code` for the Authorization Code Grant flow.</span></span> |
| <span data-ttu-id="e2dd4-142">Область</span><span class="sxs-lookup"><span data-stu-id="e2dd4-142">scope</span></span> | <span data-ttu-id="e2dd4-p112">Разделенный пробелами список [разрешений Microsoft Graph](./permissions_reference.md), запрашиваемых приложением. Вы также можете указать [области OpenId Connect](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#openid-connect-scopes) для [единого входа](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oidc/).</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p112">A space-separated list of [Microsoft Graph permission scopes](./permissions_reference.md) that the app is requesting. You can also specify [OpenId Connect scopes](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#openid-connect-scopes) for [single sign-on](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oidc/).</span></span>  |
| <span data-ttu-id="e2dd4-145">state</span><span class="sxs-lookup"><span data-stu-id="e2dd4-145">state</span></span> | <span data-ttu-id="e2dd4-146">Включенное в запрос значение, которое также возвращается в ответе с маркером и используется для проверки.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-146">A value included in the request that will also be returned in the token response, used for validation.</span></span> |

<span data-ttu-id="e2dd4-147">Например, URL-адрес запроса для приложения, которому требуется доступ на чтение почты, может выглядеть так:</span><span class="sxs-lookup"><span data-stu-id="e2dd4-147">For example, the request URL for an application that requires read access to mail might look like the following.</span></span>

```
GET https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=<app ID>&redirect_uri=http%3A%2F%2Flocalhost/myapp%2F&response_type=code&state=1234&scope=mail.read
```

<span data-ttu-id="e2dd4-p113">3. Перенаправьте пользователя на страницу URL-адреса для входа. Отображается экран входа с названием приложения. После входа отображается список необходимых приложению разрешений, и пользователь может разрешить или запретить доступ. Если пользователь разрешил доступ, в браузере открывается URI перенаправления с кодом и состоянием авторизации в строке запроса, как показано в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p113">3- Redirect the user to the logon URL. The user is presented with a sign in screen that displays the name of the app. After signing in, the user is presented with the list of the permissions the app requires and prompted to allow or deny. If the user consents, the browser redirects to the redirect URI with the authorization code and state in the query string, as shown in the following example.</span></span>

```
http://localhost/myapp/?code=AwABAAAA...cZZ6IgAA&state=1234
```

<span data-ttu-id="e2dd4-152">Далее необходимо заменить возвращенный код авторизации на маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-152">The next step is to exchange the authorization code returned for an access token.</span></span>

### <a name="getting-an-access-token"></a><span data-ttu-id="e2dd4-153">Получение маркера доступа</span><span class="sxs-lookup"><span data-stu-id="e2dd4-153">Getting an access token</span></span>

<span data-ttu-id="e2dd4-154">Чтобы получить маркер доступа, приложение помещает параметры, закодированные с использованием формы, в URL-адрес запроса маркера (например, `https://login.microsoftonline.com/common/oauth2/v2.0/token`). При этом применяются указанные ниже параметры.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-154">To get an access token, the app posts form-encoded parameters to the token request URL (for example, `https://login.microsoftonline.com/common/oauth2/v2.0/token`) with the following parameters.</span></span>

| <span data-ttu-id="e2dd4-155">Параметр</span><span class="sxs-lookup"><span data-stu-id="e2dd4-155">Parameter</span></span> | <span data-ttu-id="e2dd4-156">Описания</span><span class="sxs-lookup"><span data-stu-id="e2dd4-156">Descriptions</span></span> |
|:------|:------|
| <span data-ttu-id="e2dd4-157">client_id</span><span class="sxs-lookup"><span data-stu-id="e2dd4-157">client_id</span></span> | <span data-ttu-id="e2dd4-158">Идентификатор приложения, создаваемый при его регистрации.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-158">The app ID generated by registering the app.</span></span> |
| <span data-ttu-id="e2dd4-159">client_secret</span><span class="sxs-lookup"><span data-stu-id="e2dd4-159">client_secret</span></span> | <span data-ttu-id="e2dd4-160">Секрет приложения, создаваемый при его регистрации.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-160">The app secret generated when registering the app.</span></span> |
| <span data-ttu-id="e2dd4-161">code</span><span class="sxs-lookup"><span data-stu-id="e2dd4-161">code</span></span> | <span data-ttu-id="e2dd4-162">Код авторизации, полученный на предыдущем этапе.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-162">The authorization code obtained in the prior step.</span></span> |
| <span data-ttu-id="e2dd4-163">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="e2dd4-163">redirect_uri</span></span> | <span data-ttu-id="e2dd4-164">Это значение должно совпадать со значением, используемым в запросе кода авторизации.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-164">This value must be the same as the value used in the authorization code request.</span></span> |
| <span data-ttu-id="e2dd4-165">grant_type</span><span class="sxs-lookup"><span data-stu-id="e2dd4-165">grant_type</span></span> | <span data-ttu-id="e2dd4-p114">Тип предоставления, используемый приложением. Для потока предоставления кода авторизации используется значение `code`.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p114">The type of grant the app is using. This value is `code` for the Authorization Code Grant flow.</span></span> |
| <span data-ttu-id="e2dd4-168">Область</span><span class="sxs-lookup"><span data-stu-id="e2dd4-168">scope</span></span> | <span data-ttu-id="e2dd4-169">Разделенный пробелами список [разрешений Microsoft Graph](./permissions_reference.md), запрашиваемых приложением.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-169">A space-separated list of [Microsoft Graph permission scopes](./permissions_reference.md) that the app is requesting.</span></span> |

<span data-ttu-id="e2dd4-170">URL-адрес запроса для нашего приложения с кодом, полученным на предыдущем этапе, выглядит так:</span><span class="sxs-lookup"><span data-stu-id="e2dd4-170">The request URL for our application, using the code from the previous step, looks like the following.</span></span>

```
POST https://login.microsoftonline.com/common/oauth2/v2.0/token
Content-Type: application/x-www-form-urlencoded

{
  grant_type=authorization_code
  &code=AwABAAAA...cZZ6IgAA
  &redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
  &resource=https%3A%2F%2Fgraph.microsoft.com%2F
  &scope=mail.read
  &client\_id=<app ID>
  &client\_secret=<app SECRET>
}
```

<span data-ttu-id="e2dd4-171">Ответ сервера содержит полезные данные JSON, которые включают маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-171">The server responds with a JSON payload which includes the access token.</span></span>

```
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8

{
  "token_type":"Bearer",
  "expires_in":"3600",
  "access_token":"eyJ0eXAi...b66LoPVA",
  "scope":"https://graph.microsoft.com/mail.read",
  ...
}
```

<span data-ttu-id="e2dd4-p115">Токен доступа находится в поле `access_token` полезных данных JSON. С помощью этого значения приложение задает заголовок Authorization, когда выполняет вызовы REST к API.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p115">The access token is found in the `access_token` field of the JSON payload. The app uses this value to set the Authorization header when making REST calls to the API.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="e2dd4-174">Вызов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e2dd4-174">Call Microsoft Graph</span></span>

<span data-ttu-id="e2dd4-p116">После получения маркера доступа приложение готово к вызову Microsoft Graph. Так как этот пример приложения получает сообщения, он будет использовать HTTP-запрос GET к конечной точке `https://graph.microsoft.com/v1.0/me/messages`.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p116">After the app has an access token, it's ready to call Microsoft Graph. Because this sample app is retrieving messages, it will use an HTTP GET request to the `https://graph.microsoft.com/v1.0/me/messages` endpoint.</span></span>

### <a name="refine-the-request"></a><span data-ttu-id="e2dd4-177">Уточнение запроса</span><span class="sxs-lookup"><span data-stu-id="e2dd4-177">Refine the request</span></span>

<span data-ttu-id="e2dd4-p117">Вы можете управлять запросами GET в приложении с помощью параметров запроса OData. Рекомендуем использовать эти параметры для ограничения числа возвращаемых результатов, а также полей, возвращаемых для каждого элемента.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p117">Apps can control the behavior of GET requests by using OData query parameters. We recommend that apps use these parameters to limit the number of results that are returned and to limit the fields that are returned for each item.</span></span> 

<span data-ttu-id="e2dd4-p118">В этом приложении сообщения отображаются в таблице, где указаны тема, отправитель, дата и время получения сообщения. Таблица содержит не более 25 строк: сообщения сортируются по дате получения от новых к старым. Для получения таких результатов приложение использует следующие параметры запроса:</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p118">This sample app will display messages in a table that shows the subject, sender, and the date and time the message was received. The table displays a maximum of 25 rows and is sorted so that the most recently received message is at the top. The app uses the following query parameters to get these results.</span></span>

- <span data-ttu-id="e2dd4-183">`$select`: задает только поля `subject`, `sender` и `dateTimeReceived`.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-183">`$select` - Specifies only the `subject`, `sender`, and `dateTimeReceived` fields.</span></span>
- <span data-ttu-id="e2dd4-184">`$top`: задает до 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-184">`$top` - Specifies a maximum of 25 items.</span></span>
- <span data-ttu-id="e2dd4-185">`$orderby`: сортирует результаты по полю `dateTimeReceived`.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-185">`$orderby` - Sorts the results by the `dateTimeReceived` field.</span></span>

<span data-ttu-id="e2dd4-186">В результате мы получаем следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="e2dd4-186">This results in the following request.</span></span>

```
GET https://graph.microsoft.com/v1.0/me/messages?$select=subject,from,receivedDateTime&$top=25&$orderby=receivedDateTime%20DESC
Accept: application/json
Authorization: Bearer eyJ0eXAi...b66LoPVA
```

<span data-ttu-id="e2dd4-p119">Теперь вы знаете, как вызывать Microsoft Graph, и можете создавать другие вызовы, необходимые для вашего приложения, используя справочник по API. Обратите внимание, что необходимые для вызовов разрешения настраиваются во время регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="e2dd4-p119">Now that you've seen how to make calls to Microsoft Graph, you can use the API reference to construct any other kinds of calls your app needs to make. However, bear in mind that your app needs to have the appropriate permissions configured on the app registration for the calls it makes.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e2dd4-189">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="e2dd4-189">Next steps</span></span>
- <span data-ttu-id="e2dd4-190">Попробуйте другие возможности REST API, используя [песочницу Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="e2dd4-190">Try out more of the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

## <a name="see-also"></a><span data-ttu-id="e2dd4-191">См. также</span><span class="sxs-lookup"><span data-stu-id="e2dd4-191">See also</span></span>
- [<span data-ttu-id="e2dd4-192">Протоколы Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="e2dd4-192">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="e2dd4-193">Маркеры Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="e2dd4-193">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
