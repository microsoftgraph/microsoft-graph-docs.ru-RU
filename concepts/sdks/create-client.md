---
title: Создание клиента Microsoft Graph
description: Описывается создание клиента, который будет использоваться для звонков в Microsoft Graph. Включает как настроить проверку подлинности и выбрать облако публичном.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 3d120f626f3623545366a105aaf9c072c8501e1b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630190"
---
# <a name="create-a-microsoft-graph-client"></a><span data-ttu-id="c799f-104">Создание клиента Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c799f-104">Create a Microsoft Graph client</span></span>

<span data-ttu-id="c799f-105">Клиент Microsoft Graph предназначен для упрощения вызовов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c799f-105">The Microsoft Graph client is designed to make it simple to make calls to Microsoft Graph.</span></span> <span data-ttu-id="c799f-106">Вы можете использовать один экземпляр клиента в течение всего времени существования приложения.</span><span class="sxs-lookup"><span data-stu-id="c799f-106">You can use a single client instance for the lifetime of the application.</span></span> <span data-ttu-id="c799f-107">Сведения о том, как добавить и установить клиентский пакет Microsoft Graph в свой проект, можно найти в [статье Установка пакета SDK](sdk-installation.md).</span><span class="sxs-lookup"><span data-stu-id="c799f-107">For information about how to add and install the Microsoft Graph client package into your project, see  [Install the SDK](sdk-installation.md).</span></span>

<span data-ttu-id="c799f-108">В приведенных ниже примерах кода показано, как создать экземпляр клиента Microsoft Graph с поставщиком проверки подлинности на поддерживаемых языках.</span><span class="sxs-lookup"><span data-stu-id="c799f-108">The following code examples show how to create an instance of a Microsoft Graph client with an authentication provider in the supported languages.</span></span> <span data-ttu-id="c799f-109">Поставщик проверки подлинности будет обрабатывать получение маркеров доступа для приложения.</span><span class="sxs-lookup"><span data-stu-id="c799f-109">The authentication provider will handle acquiring access tokens for the application.</span></span> <span data-ttu-id="c799f-110">Для каждого языка и платформы доступно множество различных поставщиков проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c799f-110">Many different authentication providers are available for each language and platform.</span></span> <span data-ttu-id="c799f-111">Различные поставщики приложений поддерживают различные сценарии клиентов.</span><span class="sxs-lookup"><span data-stu-id="c799f-111">The different application providers support different client scenarios.</span></span> <span data-ttu-id="c799f-112">Для получения дополнительных сведений о поставщиках и параметрах, которые подходят для вашего сценария, ознакомьтесь со статьей [Выбор поставщика проверки](choose-authentication-providers.md)подлинности.</span><span class="sxs-lookup"><span data-stu-id="c799f-112">For details about which provider and options are appropriate for your scenario, see [Choose an Authentication Provider](choose-authentication-providers.md).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="c799f-113">Языках</span><span class="sxs-lookup"><span data-stu-id="c799f-113">C#</span></span>](#tab/CS)

```csharp
var app = DeviceCodeProvider.CreateClientApplication("INSERT-CLIENT-APP-ID");
var authProvider = new DeviceCodeProvider(app);
var client = new GraphServiceClient(authProvider);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c799f-114">Язык</span><span class="sxs-lookup"><span data-stu-id="c799f-114">Javascript</span></span>](#tab/Javascript)

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
const authProvider = new MSALAuthenticationProvider(userAgentApplication, scopes);
```

# <a name="javatabjava"></a>[<span data-ttu-id="c799f-115">Java</span><span class="sxs-lookup"><span data-stu-id="c799f-115">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(CLIENT_ID, SCOPES, CLIENT_SECRET, TENANT_GUID, NATIONAL_CLOUD);

IGraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(authProvider)
                .buildClient();
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="c799f-116">Android</span><span class="sxs-lookup"><span data-stu-id="c799f-116">Android</span></span>](#tab/Android)

```java
PublicClientApplication publicClientApplication = new PublicClientApplication(getApplicationContext(), "INSERT-CLIENT-APP-ID");

MSALAuthenticationProvider msalAuthenticationProvider = new MSALAuthenticationProvider(
    getActivity(),
    getApplication(),
    publicClientApplication,
    scopes);

IGraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(authProvider)
                .buildClient();
```

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c799f-117">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c799f-117">Objective-C</span></span>](#tab/Objective-C)

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

# <a name="phptabphp"></a>[<span data-ttu-id="c799f-118">PHP</span><span class="sxs-lookup"><span data-stu-id="c799f-118">PHP</span></span>](#tab/PHP)

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
