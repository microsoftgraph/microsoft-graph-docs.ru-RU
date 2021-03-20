---
title: Создание клиента Microsoft Graph
description: Описывает, как создать клиента для звонков в Microsoft Graph. Включает в себя настройка проверки подлинности и выбор суверенного облака.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: f32a779ac57d88da1ea66820a2b5a0bb30cbb89e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953357"
---
# <a name="create-a-microsoft-graph-client"></a><span data-ttu-id="ef17a-104">Создание клиента Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ef17a-104">Create a Microsoft Graph client</span></span>

<span data-ttu-id="ef17a-105">Клиент Microsoft Graph разработан таким образом, чтобы сделать вызовы в Microsoft Graph простыми.</span><span class="sxs-lookup"><span data-stu-id="ef17a-105">The Microsoft Graph client is designed to make it simple to make calls to Microsoft Graph.</span></span> <span data-ttu-id="ef17a-106">Можно использовать один экземпляр клиента в течение всего срока службы приложения.</span><span class="sxs-lookup"><span data-stu-id="ef17a-106">You can use a single client instance for the lifetime of the application.</span></span> <span data-ttu-id="ef17a-107">Сведения о том, как добавить и установить клиентский пакет Microsoft Graph в проект, см. в [сайте Install the SDK.](sdk-installation.md)</span><span class="sxs-lookup"><span data-stu-id="ef17a-107">For information about how to add and install the Microsoft Graph client package into your project, see  [Install the SDK](sdk-installation.md).</span></span>

<span data-ttu-id="ef17a-108">В следующих примерах кода покажите, как создать экземпляр клиента Microsoft Graph с поставщиком проверки подлинности на поддерживаемых языках.</span><span class="sxs-lookup"><span data-stu-id="ef17a-108">The following code examples show how to create an instance of a Microsoft Graph client with an authentication provider in the supported languages.</span></span> <span data-ttu-id="ef17a-109">Поставщик проверки подлинности будет обрабатывать получение маркеров доступа для приложения.</span><span class="sxs-lookup"><span data-stu-id="ef17a-109">The authentication provider will handle acquiring access tokens for the application.</span></span> <span data-ttu-id="ef17a-110">Для каждого языка и платформы доступно множество различных поставщиков проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ef17a-110">Many different authentication providers are available for each language and platform.</span></span> <span data-ttu-id="ef17a-111">Различные поставщики приложений поддерживают различные клиентские сценарии.</span><span class="sxs-lookup"><span data-stu-id="ef17a-111">The different application providers support different client scenarios.</span></span> <span data-ttu-id="ef17a-112">Дополнительные сведения о том, какой поставщик и какие параметры подходят для вашего сценария, см. в материале [Выберите поставщика проверки подлинности.](choose-authentication-providers.md)</span><span class="sxs-lookup"><span data-stu-id="ef17a-112">For details about which provider and options are appropriate for your scenario, see [Choose an Authentication Provider](choose-authentication-providers.md).</span></span>

# <a name="c"></a>[<span data-ttu-id="ef17a-113">C#</span><span class="sxs-lookup"><span data-stu-id="ef17a-113">C#</span></span>](#tab/CS)

```csharp
// Build a client application.
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create("INSERT-CLIENT-APP-ID")
            .Build();
// Create an authentication provider by passing in a client application and graph scopes.
DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, graphScopes);
// Create a new instance of GraphServiceClient with the authentication provider.
GraphServiceClient graphClient = new GraphServiceClient(authProvider);
```

# <a name="javascript"></a>[<span data-ttu-id="ef17a-114">Javascript</span><span class="sxs-lookup"><span data-stu-id="ef17a-114">Javascript</span></span>](#tab/Javascript)

```javascript
const clientId = "INSERT-CLIENT-APP-ID"; // Client Id of the registered application
const callback = (errorDesc, token, error, tokenType) => {};
// An Optional options for initializing the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#configuration-options
const options = {
    redirectUri: "Your redirect URI",
};
const graphScopes = ["user.read", "mail.send"]; // An array of graph scopes

// Initialize the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#initialization-of-msal
const userAgentApplication = new UserAgentApplication(clientId, undefined, callback, options);
const authProvider = new MSALAuthenticationProvider(userAgentApplication, graphScopes );
```

# <a name="java"></a>[<span data-ttu-id="ef17a-115">Java</span><span class="sxs-lookup"><span data-stu-id="ef17a-115">Java</span></span>](#tab/Java)

```java
final ClientSecretCredential clientSecretCredential = new ClientSecretCredentialBuilder()
        .clientId(CLIENT_ID)
        .clientSecret(CLIENT_SECRET)
        .tenantId(TENANT_GUID)
        .build();

final TokenCredentialAuthProvider tokenCredAuthProvider = new TokenCredentialAuthProvider(SCOPES, clientSecretCredential);

final GraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(tokenCredAuthProvider)
                .buildClient();
```

# <a name="android"></a>[<span data-ttu-id="ef17a-116">Android</span><span class="sxs-lookup"><span data-stu-id="ef17a-116">Android</span></span>](#tab/Android)

```java
final InteractiveBrowserCredential interactiveBrowserCredential = new InteractiveBrowserCredentialBuilder()
                .clientId(CLIENT_ID)
                .redirectUrl("http://localhost:8765")
                .build();

final TokenCredentialAuthProvider tokenCredAuthProvider = new TokenCredentialAuthProvider(SCOPES, interactiveBrowserCredential);

GraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(tokenCredAuthProvider)
                .buildClient();
```

# <a name="objective-c"></a>[<span data-ttu-id="ef17a-117">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef17a-117">Objective-C</span></span>](#tab/Objective-C)

```objc
// Create the authenticationProvider.
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];
MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];
 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];

// Create the client with the authenticationProvider and create a request to the /me resource.
MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me"]]];

// Create the task to send the request and handle the response.
MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest
    completionHandler:^(NSData *data, NSURLResponse *response, NSError *error) {

    //Do something

    }];

[meDataTask execute];
```

# <a name="php"></a>[<span data-ttu-id="ef17a-118">PHP</span><span class="sxs-lookup"><span data-stu-id="ef17a-118">PHP</span></span>](#tab/PHP)

```php
// PHP client currently doesn't have an authentication provider. You will need to handle
// getting an access token. The following example demonstrates the client credential
// OAuth flow and assumes that an administrator has consented to the application.
$guzzle = new \GuzzleHttp\Client();
$url = 'https://login.microsoftonline.com/' . $tenantId . '/oauth2/token?api-version=1.0';
$token = json_decode($guzzle->post($url, [
    'form_params' => [
        'client_id' => $clientId,
        'client_secret' => $clientSecret,
        'resource' => 'https://graph.microsoft.com/',
        'grant_type' => 'client_credentials',
    ],
])->getBody()->getContents());
$accessToken = $token->access_token;

// Create a new Graph client.
$graph = new Graph();
$graph->setAccessToken($accessToken);

// Make a call to /me Graph resource.
$user = $graph->createRequest("GET", "/me")
                ->setReturnType(Model\User::class)
                ->execute();
```
---
