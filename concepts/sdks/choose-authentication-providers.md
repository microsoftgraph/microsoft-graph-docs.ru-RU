---
title: Выберите поставщика проверки подлинности Microsoft Graph
description: Узнайте, как выбрать поставщиков проверки подлинности по сценарию для приложения.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: f174ae516ca6bde01456349a7a0ed7742b8b0ba1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953371"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a><span data-ttu-id="c0249-103">Выберите поставщика проверки подлинности Microsoft Graph в зависимости от сценария</span><span class="sxs-lookup"><span data-stu-id="c0249-103">Choose a Microsoft Graph authentication provider based on scenario</span></span>

<span data-ttu-id="c0249-104">Поставщики проверки подлинности реализуют код, необходимый для приобретения маркера с помощью Библиотеки проверки подлинности Майкрософт (MSAL); обработка ряда потенциальных ошибок для таких случаев, как постепенное согласие, просроченные пароли и условный доступ; а затем установите заглавную головку авторизации http-запроса.</span><span class="sxs-lookup"><span data-stu-id="c0249-104">Authentication providers implement the code required to acquire a token using the Microsoft Authentication Library (MSAL); handle a number of potential errors for cases like incremental consent, expired passwords, and conditional access; and then set the HTTP request authorization header.</span></span> <span data-ttu-id="c0249-105">В следующей таблице перечислены поставщики, которые соответствуют сценариям для различных [типов приложений.](/azure/active-directory/develop/v2-app-types)</span><span class="sxs-lookup"><span data-stu-id="c0249-105">The following table lists the set of providers that match the scenarios for different [application types](/azure/active-directory/develop/v2-app-types).</span></span>

|<span data-ttu-id="c0249-106">Сценарий</span><span class="sxs-lookup"><span data-stu-id="c0249-106">Scenario</span></span> | <span data-ttu-id="c0249-107">Flow/Grant</span><span class="sxs-lookup"><span data-stu-id="c0249-107">Flow/Grant</span></span> | <span data-ttu-id="c0249-108">Аудитория</span><span class="sxs-lookup"><span data-stu-id="c0249-108">Audience</span></span> | <span data-ttu-id="c0249-109">Поставщик</span><span class="sxs-lookup"><span data-stu-id="c0249-109">Provider</span></span>|
|--|--|--|--|
| [<span data-ttu-id="c0249-110">Приложение для одной страницы</span><span class="sxs-lookup"><span data-stu-id="c0249-110">Single Page App</span></span>](/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | <span data-ttu-id="c0249-111">Неявный поток</span><span class="sxs-lookup"><span data-stu-id="c0249-111">Implicit</span></span> | <span data-ttu-id="c0249-112">Делегированная потребительская/org</span><span class="sxs-lookup"><span data-stu-id="c0249-112">Delegated Consumer/Org</span></span> |[<span data-ttu-id="c0249-113">Неявный поставщик</span><span class="sxs-lookup"><span data-stu-id="c0249-113">Implicit Provider</span></span>](#ImplicitProvider) |
| [<span data-ttu-id="c0249-114">Веб-приложение, которое вызывает веб-API</span><span class="sxs-lookup"><span data-stu-id="c0249-114">Web App that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | <span data-ttu-id="c0249-115">Authorization Code</span><span class="sxs-lookup"><span data-stu-id="c0249-115">Authorization Code</span></span> | <span data-ttu-id="c0249-116">Делегированная потребительская/org</span><span class="sxs-lookup"><span data-stu-id="c0249-116">Delegated Consumer/Org</span></span> | [<span data-ttu-id="c0249-117">Поставщик кода авторизации</span><span class="sxs-lookup"><span data-stu-id="c0249-117">Authorization Code Provider</span></span>](#AuthCodeProvider) |
| | <span data-ttu-id="c0249-118">Учетные данные клиента</span><span class="sxs-lookup"><span data-stu-id="c0249-118">Client Credentials</span></span>  | <span data-ttu-id="c0249-119">Только приложение</span><span class="sxs-lookup"><span data-stu-id="c0249-119">App Only</span></span> | [<span data-ttu-id="c0249-120">Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="c0249-120">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="c0249-121">Веб-API, который вызывает веб-API</span><span class="sxs-lookup"><span data-stu-id="c0249-121">Web API that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | <span data-ttu-id="c0249-122">От имени</span><span class="sxs-lookup"><span data-stu-id="c0249-122">On Behalf Of</span></span> | <span data-ttu-id="c0249-123">Делегированная потребительская/org</span><span class="sxs-lookup"><span data-stu-id="c0249-123">Delegated Consumer/Org</span></span> | [<span data-ttu-id="c0249-124">От имени поставщика</span><span class="sxs-lookup"><span data-stu-id="c0249-124">On Behalf Of Provider</span></span>](#OnBehalfOfProvider) |
| | <span data-ttu-id="c0249-125">Учетные данные клиента</span><span class="sxs-lookup"><span data-stu-id="c0249-125">Client Credentials</span></span>  | <span data-ttu-id="c0249-126">Только приложение</span><span class="sxs-lookup"><span data-stu-id="c0249-126">App Only</span></span> | [<span data-ttu-id="c0249-127">Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="c0249-127">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="c0249-128">Настольное приложение, которое вызывает веб-API</span><span class="sxs-lookup"><span data-stu-id="c0249-128">Desktop app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | <span data-ttu-id="c0249-129">Интерактивны</span><span class="sxs-lookup"><span data-stu-id="c0249-129">Interactive</span></span> | <span data-ttu-id="c0249-130">Делегированная потребительская/org</span><span class="sxs-lookup"><span data-stu-id="c0249-130">Delegated Consumer/Org</span></span> | [<span data-ttu-id="c0249-131">Интерактивный поставщик</span><span class="sxs-lookup"><span data-stu-id="c0249-131">Interactive Provider</span></span>](#InteractiveProvider) |
| | <span data-ttu-id="c0249-132">Интегрированная Windows</span><span class="sxs-lookup"><span data-stu-id="c0249-132">Integrated Windows</span></span> | <span data-ttu-id="c0249-133">Делегированная org</span><span class="sxs-lookup"><span data-stu-id="c0249-133">Delegated Org</span></span> | [<span data-ttu-id="c0249-134">Интегрированный поставщик Windows</span><span class="sxs-lookup"><span data-stu-id="c0249-134">Integrated Windows Provider</span></span>](#IntegratedWindowsProvider) |
| | <span data-ttu-id="c0249-135">Владелец ресурса</span><span class="sxs-lookup"><span data-stu-id="c0249-135">Resource Owner</span></span>  | <span data-ttu-id="c0249-136">Делегированная org</span><span class="sxs-lookup"><span data-stu-id="c0249-136">Delegated Org</span></span> | [<span data-ttu-id="c0249-137">Имя пользователя / Поставщик паролей</span><span class="sxs-lookup"><span data-stu-id="c0249-137">Username / Password Provider</span></span>](#UsernamePasswordProvider) |
| | <span data-ttu-id="c0249-138">Код устройства</span><span class="sxs-lookup"><span data-stu-id="c0249-138">Device Code</span></span>  | <span data-ttu-id="c0249-139">Делегированная org</span><span class="sxs-lookup"><span data-stu-id="c0249-139">Delegated Org</span></span> | [<span data-ttu-id="c0249-140">Поставщик кода устройства</span><span class="sxs-lookup"><span data-stu-id="c0249-140">Device Code Provider</span></span>](#DeviceCodeProvider) |
| [<span data-ttu-id="c0249-141">Приложение Daemon</span><span class="sxs-lookup"><span data-stu-id="c0249-141">Daemon app</span></span>](/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | <span data-ttu-id="c0249-142">Учетные данные клиента</span><span class="sxs-lookup"><span data-stu-id="c0249-142">Client Credentials</span></span>  | <span data-ttu-id="c0249-143">Только приложение</span><span class="sxs-lookup"><span data-stu-id="c0249-143">App Only</span></span> | [<span data-ttu-id="c0249-144">Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="c0249-144">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="c0249-145">Мобильное приложение, которое вызывает веб-API</span><span class="sxs-lookup"><span data-stu-id="c0249-145">Mobile app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | <span data-ttu-id="c0249-146">Интерактивны</span><span class="sxs-lookup"><span data-stu-id="c0249-146">Interactive</span></span> | <span data-ttu-id="c0249-147">Делегированная потребительская/org</span><span class="sxs-lookup"><span data-stu-id="c0249-147">Delegated Consumer/Org</span></span> | [<span data-ttu-id="c0249-148">Интерактивный поставщик</span><span class="sxs-lookup"><span data-stu-id="c0249-148">Interactive Provider</span></span>](#InteractiveProvider) |

> <span data-ttu-id="c0249-149">Примечание. Разработчикам Java и Android необходимо добавить библиотеку [azure-identity,](https://docs.microsoft.com/java/api/overview/azure/identity-readme?view=azure-java-stable) чтобы получить доступ к различным типам учетных данных.</span><span class="sxs-lookup"><span data-stu-id="c0249-149">Note: Java and android developers need to add the [azure-identity](https://docs.microsoft.com/java/api/overview/azure/identity-readme?view=azure-java-stable) library in order to get access to the different credentials types.</span></span>

## <a name="authorization-code-provider"></a><a name="AuthCodeProvider" ></a><span data-ttu-id="c0249-150">Поставщик кода авторизации</span><span class="sxs-lookup"><span data-stu-id="c0249-150">Authorization code provider</span></span>

<span data-ttu-id="c0249-151">Поток кода авторизации позволяет родным и веб-приложениям безопасно получать маркеры от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="c0249-151">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="c0249-152">Дополнительные данные см. в записи платформы удостоверений Майкрософт и потока кода авторизации [OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-auth-code-flow)</span><span class="sxs-lookup"><span data-stu-id="c0249-152">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="c0249-153">C#</span><span class="sxs-lookup"><span data-stu-id="c0249-153">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="c0249-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0249-154">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="c0249-155">Код авторизации, учетные данные клиентов и потоки OAuth от имени требуют, чтобы вы реализовали настраиваемого поставщика проверки подлинности в это время.</span><span class="sxs-lookup"><span data-stu-id="c0249-155">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="c0249-156">Дополнительные сведения см. в [специальном поставщике проверки подлинности.](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)</span><span class="sxs-lookup"><span data-stu-id="c0249-156">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="c0249-157">Java</span><span class="sxs-lookup"><span data-stu-id="c0249-157">Java</span></span>](#tab/Java)

```java
final AuthorizationCodeCredential authCodeCredential = new AuthorizationCodeCredentialBuilder()
        .clientId(clientId)
        .clientSecret(clientSecret) //required for web apps, do not set for native apps
        .authorizationCode(authorizationCode)
        .redirectUrl(redirectUri)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, authCodeCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[<span data-ttu-id="c0249-158">Android</span><span class="sxs-lookup"><span data-stu-id="c0249-158">Android</span></span>](#tab/Android)

<span data-ttu-id="c0249-159">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-159">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="c0249-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0249-160">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c0249-161">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-161">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="c0249-162">PHP</span><span class="sxs-lookup"><span data-stu-id="c0249-162">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c0249-163">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="c0249-163">Not yet available.</span></span> <span data-ttu-id="c0249-164">Пожалуйста, поддержите или откройте [запрос на функцию Microsoft Graph,](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) если это важно для вас.</span><span class="sxs-lookup"><span data-stu-id="c0249-164">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="c0249-165">Ruby</span><span class="sxs-lookup"><span data-stu-id="c0249-165">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c0249-166">Пока недоступна.</span><span class="sxs-lookup"><span data-stu-id="c0249-166">Not available, yet.</span></span> <span data-ttu-id="c0249-167">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="c0249-167">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="client-credentials-provider"></a><a name="ClientCredentialsProvider"></a><span data-ttu-id="c0249-168">Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="c0249-168">Client credentials provider</span></span>

<span data-ttu-id="c0249-169">Поток клиентских учетных данных позволяет приложениям-службам работать без взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="c0249-169">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="c0249-170">Доступ основан на удостоверении приложения.</span><span class="sxs-lookup"><span data-stu-id="c0249-170">Access is based on the identity of the application.</span></span> <span data-ttu-id="c0249-171">Дополнительные сведения см. в веб-сайте Платформы удостоверений Майкрософт и потока учетных данных клиента [OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)</span><span class="sxs-lookup"><span data-stu-id="c0249-171">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="c0249-172">C#</span><span class="sxs-lookup"><span data-stu-id="c0249-172">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascript"></a>[<span data-ttu-id="c0249-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0249-173">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="c0249-174">Код авторизации, учетные данные клиентов и потоки OAuth от имени требуют, чтобы вы реализовали настраиваемого поставщика проверки подлинности в это время.</span><span class="sxs-lookup"><span data-stu-id="c0249-174">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="c0249-175">Дополнительные сведения см. в [специальном поставщике проверки подлинности.](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)</span><span class="sxs-lookup"><span data-stu-id="c0249-175">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="c0249-176">Java</span><span class="sxs-lookup"><span data-stu-id="c0249-176">Java</span></span>](#tab/Java)

```java
final ClientSecretCredential clientSecretCredential = new ClientSecretCredentialBuilder()
        .clientId(clientId)
        .clientSecret(clientSecret)
        .tenantId(tenant)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, clientSecretCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[<span data-ttu-id="c0249-177">Android</span><span class="sxs-lookup"><span data-stu-id="c0249-177">Android</span></span>](#tab/Android)

<span data-ttu-id="c0249-178">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-178">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="c0249-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0249-179">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c0249-180">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-180">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="c0249-181">PHP</span><span class="sxs-lookup"><span data-stu-id="c0249-181">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c0249-182">Пока недоступна.</span><span class="sxs-lookup"><span data-stu-id="c0249-182">Not available, yet.</span></span> <span data-ttu-id="c0249-183">Пожалуйста, поддержите или откройте [запрос на функцию Microsoft Graph,](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) если это важно для вас.</span><span class="sxs-lookup"><span data-stu-id="c0249-183">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="c0249-184">Ruby</span><span class="sxs-lookup"><span data-stu-id="c0249-184">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c0249-185">Пока недоступна.</span><span class="sxs-lookup"><span data-stu-id="c0249-185">Not available, yet.</span></span> <span data-ttu-id="c0249-186">Пожалуйста, поддержите или откройте [запрос на функцию Microsoft Graph,](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) если это важно для вас.</span><span class="sxs-lookup"><span data-stu-id="c0249-186">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="on-behalf-of-provider"></a><a name="OnBehalfOfProvider"></a><span data-ttu-id="c0249-187">От имени поставщика</span><span class="sxs-lookup"><span data-stu-id="c0249-187">On-behalf-of provider</span></span>

<span data-ttu-id="c0249-188">Поток от имени применим, когда приложение вызывает API службы/веб-службы, который по очереди вызывает API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c0249-188">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="c0249-189">Узнайте больше, прочитав платформу удостоверений Майкрософт и [поток OAuth 2.0 On-Behalf-Of](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="c0249-189">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="c"></a>[<span data-ttu-id="c0249-190">C#</span><span class="sxs-lookup"><span data-stu-id="c0249-190">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="c0249-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0249-191">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="c0249-192">Код авторизации, учетные данные клиентов и потоки OAuth от имени требуют, чтобы вы реализовали настраиваемого поставщика проверки подлинности в это время.</span><span class="sxs-lookup"><span data-stu-id="c0249-192">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="c0249-193">Дополнительные сведения читайте в [публикации "Использование](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) поставщика настраиваемой проверки подлинности".</span><span class="sxs-lookup"><span data-stu-id="c0249-193">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="java"></a>[<span data-ttu-id="c0249-194">Java</span><span class="sxs-lookup"><span data-stu-id="c0249-194">Java</span></span>](#tab/Java)

<span data-ttu-id="c0249-195">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="c0249-195">Not yet available.</span></span> <span data-ttu-id="c0249-196">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="c0249-196">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="c0249-197">Android</span><span class="sxs-lookup"><span data-stu-id="c0249-197">Android</span></span>](#tab/Android)

<span data-ttu-id="c0249-198">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-198">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="c0249-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0249-199">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c0249-200">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-200">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="c0249-201">PHP</span><span class="sxs-lookup"><span data-stu-id="c0249-201">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c0249-202">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="c0249-202">Not yet available.</span></span> <span data-ttu-id="c0249-203">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="c0249-203">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="c0249-204">Ruby</span><span class="sxs-lookup"><span data-stu-id="c0249-204">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c0249-205">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="c0249-205">Not yet available.</span></span> <span data-ttu-id="c0249-206">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="c0249-206">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="implicit-provider"></a><a name="ImplicitProvider"></a><span data-ttu-id="c0249-207">Неявный поставщик</span><span class="sxs-lookup"><span data-stu-id="c0249-207">Implicit provider</span></span>

<span data-ttu-id="c0249-208">Неявный поток грантов используется в браузерных приложениях.</span><span class="sxs-lookup"><span data-stu-id="c0249-208">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="c0249-209">Дополнительные сведения см. в [записи платформы удостоверений Майкрософт и потока неявных грантов.](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)</span><span class="sxs-lookup"><span data-stu-id="c0249-209">For more information, see [Microsoft identity platform and Implicit grant flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="c0249-210">C#</span><span class="sxs-lookup"><span data-stu-id="c0249-210">C#</span></span>](#tab/CS)

<span data-ttu-id="c0249-211">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-211">Not applicable.</span></span>

# <a name="javascript"></a>[<span data-ttu-id="c0249-212">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0249-212">Javascript</span></span>](#tab/Javascript)

```javascript
const clientId = "your_client_id"; // Client Id of the registered application
const callback = (errorDesc, token, error, tokenType) => {};
// An Optional options for initializing the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#configuration-options
const options = {
    redirectUri: "Your redirect URI",
};
const graphScopes = ["user.read", "mail.send"]; // An array of graph scopes

// Initialize the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#initialization-of-msal
const userAgentApplication = new Msal.UserAgentApplication(clientId, undefined, callback, options);
const authProvider = new MicrosoftGraph.ImplicitMSALAuthenticationProvider(userAgentApplication, graphScopes);

const options = {
    authProvider, // An instance created from previous step
};
const Client = MicrosoftGraph.Client;
const client = Client.initWithMiddleware(options);
```

# <a name="java"></a>[<span data-ttu-id="c0249-213">Java</span><span class="sxs-lookup"><span data-stu-id="c0249-213">Java</span></span>](#tab/Java)

<span data-ttu-id="c0249-214">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-214">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="c0249-215">Android</span><span class="sxs-lookup"><span data-stu-id="c0249-215">Android</span></span>](#tab/Android)

<span data-ttu-id="c0249-216">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-216">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="c0249-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0249-217">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c0249-218">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-218">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="c0249-219">PHP</span><span class="sxs-lookup"><span data-stu-id="c0249-219">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c0249-220">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-220">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="c0249-221">Ruby</span><span class="sxs-lookup"><span data-stu-id="c0249-221">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c0249-222">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-222">Not applicable.</span></span>

---

##  <a name="device-code-provider"></a><a name="DeviceCodeProvider"></a><span data-ttu-id="c0249-223">Поставщик кода устройств</span><span class="sxs-lookup"><span data-stu-id="c0249-223">Device code provider</span></span>

<span data-ttu-id="c0249-224">Поток кода устройства позволяет войти на устройства с помощью другого устройства.</span><span class="sxs-lookup"><span data-stu-id="c0249-224">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="c0249-225">Подробные сведения см. в материале Платформа удостоверений Майкрософт и поток кода [кода устройств OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-device-code)</span><span class="sxs-lookup"><span data-stu-id="c0249-225">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="c"></a>[<span data-ttu-id="c0249-226">C#</span><span class="sxs-lookup"><span data-stu-id="c0249-226">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascript"></a>[<span data-ttu-id="c0249-227">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0249-227">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="c0249-228">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="c0249-228">Not yet available.</span></span> <span data-ttu-id="c0249-229">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="c0249-229">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="c0249-230">Java</span><span class="sxs-lookup"><span data-stu-id="c0249-230">Java</span></span>](#tab/Java)

```java
final DeviceCodeCredential deviceCodeCredential = new DeviceCodeCredentialBuilder()
                    .clientId(clientId)
                    .challengeConsumer(challenge -> {
                        // lets user know of the challenge
                        System.out.println(challenge.getMessage());
                    })
                    .build();
final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, deviceCodeCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[<span data-ttu-id="c0249-231">Android</span><span class="sxs-lookup"><span data-stu-id="c0249-231">Android</span></span>](#tab/Android)

<span data-ttu-id="c0249-232">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-232">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="c0249-233">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0249-233">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c0249-234">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-234">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="c0249-235">PHP</span><span class="sxs-lookup"><span data-stu-id="c0249-235">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c0249-236">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="c0249-236">Not yet available.</span></span> <span data-ttu-id="c0249-237">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="c0249-237">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="c0249-238">Ruby</span><span class="sxs-lookup"><span data-stu-id="c0249-238">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c0249-239">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="c0249-239">Not yet available.</span></span> <span data-ttu-id="c0249-240">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="c0249-240">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="integrated-windows-provider"></a><a name="IntegratedWindowsProvider"></a><span data-ttu-id="c0249-241">Интегрированный поставщик Windows</span><span class="sxs-lookup"><span data-stu-id="c0249-241">Integrated Windows provider</span></span>

<span data-ttu-id="c0249-242">Интегрированный поток Windows позволяет компьютерам Windows безмолвно приобретать маркер доступа при присоединении к домену.</span><span class="sxs-lookup"><span data-stu-id="c0249-242">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="c0249-243">Подробные сведения см. [в материале Интегрированная проверка подлинности Windows.](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)</span><span class="sxs-lookup"><span data-stu-id="c0249-243">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="c"></a>[<span data-ttu-id="c0249-244">C#</span><span class="sxs-lookup"><span data-stu-id="c0249-244">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="c0249-245">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0249-245">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="c0249-246">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-246">Not applicable.</span></span>

# <a name="java"></a>[<span data-ttu-id="c0249-247">Java</span><span class="sxs-lookup"><span data-stu-id="c0249-247">Java</span></span>](#tab/Java)

<span data-ttu-id="c0249-248">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-248">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="c0249-249">Android</span><span class="sxs-lookup"><span data-stu-id="c0249-249">Android</span></span>](#tab/Android)

<span data-ttu-id="c0249-250">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-250">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="c0249-251">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0249-251">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c0249-252">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-252">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="c0249-253">PHP</span><span class="sxs-lookup"><span data-stu-id="c0249-253">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c0249-254">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-254">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="c0249-255">Ruby</span><span class="sxs-lookup"><span data-stu-id="c0249-255">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c0249-256">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-256">Not applicable.</span></span>

---

##  <a name="interactive-provider"></a><a name="InteractiveProvider"></a><span data-ttu-id="c0249-257">Интерактивный поставщик</span><span class="sxs-lookup"><span data-stu-id="c0249-257">Interactive provider</span></span>

<span data-ttu-id="c0249-258">Интерактивный поток используется мобильными приложениями (Xamarin и UWP) и настольными приложениями для вызова Microsoft Graph от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="c0249-258">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="c0249-259">Подробные сведения см. [в материале Эквайринг маркеров в интерактивном режиме.](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)</span><span class="sxs-lookup"><span data-stu-id="c0249-259">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="c"></a>[<span data-ttu-id="c0249-260">C#</span><span class="sxs-lookup"><span data-stu-id="c0249-260">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="c0249-261">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0249-261">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="c0249-262">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="c0249-262">Not yet available.</span></span> <span data-ttu-id="c0249-263">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="c0249-263">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="c0249-264">Java</span><span class="sxs-lookup"><span data-stu-id="c0249-264">Java</span></span>](#tab/Java)

```java
final InteractiveBrowserCredential interactiveBrowserCredential = new InteractiveBrowserCredentialBuilder()
                .clientId(clientId)
                .redirectUrl("http://localhost:8765")
                .build();
final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, interactiveBrowserCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[<span data-ttu-id="c0249-265">Android</span><span class="sxs-lookup"><span data-stu-id="c0249-265">Android</span></span>](#tab/Android)

```java
final InteractiveBrowserCredential interactiveBrowserCredential = new InteractiveBrowserCredentialBuilder()
                .clientId(clientId)
                .redirectUrl("http://localhost:8765")
                .build();
final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, interactiveBrowserCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="objective-c"></a>[<span data-ttu-id="c0249-266">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0249-266">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID"
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication
 andOptions:authProviderOptions];
```

# <a name="php"></a>[<span data-ttu-id="c0249-267">PHP</span><span class="sxs-lookup"><span data-stu-id="c0249-267">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c0249-268">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-268">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="c0249-269">Ruby</span><span class="sxs-lookup"><span data-stu-id="c0249-269">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c0249-270">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-270">Not applicable.</span></span>

---

##  <a name="usernamepassword-provider"></a><a name="UsernamePasswordProvider"></a><span data-ttu-id="c0249-271">Поставщик имен пользователей и паролей</span><span class="sxs-lookup"><span data-stu-id="c0249-271">Username/password provider</span></span>

<span data-ttu-id="c0249-272">Поставщик имен пользователей и паролей позволяет приложению войти в пользователя с помощью имени пользователя и пароля.</span><span class="sxs-lookup"><span data-stu-id="c0249-272">The username/password provider allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="c0249-273">Используйте этот поток только в том случае, если вы не можете использовать другие потоки OAuth.</span><span class="sxs-lookup"><span data-stu-id="c0249-273">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="c0249-274">Дополнительные сведения см. в веб-сайте Платформы удостоверений Майкрософт и учетных данных владельца паролей владельца ресурсов [OAuth 2.0.](/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="c0249-274">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="c"></a>[<span data-ttu-id="c0249-275">C#</span><span class="sxs-lookup"><span data-stu-id="c0249-275">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

UsernamePasswordProvider authProvider = new UsernamePasswordProvider(publicClientApplication, scopes);

GraphServiceClient graphClient = new GraphServiceClient(authProvider);

User me = await graphClient.Me.Request()
                .WithUsernamePassword(email, password)
                .GetAsync();
```

# <a name="javascript"></a>[<span data-ttu-id="c0249-276">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0249-276">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="c0249-277">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="c0249-277">Not yet available.</span></span> <span data-ttu-id="c0249-278">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="c0249-278">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="c0249-279">Java</span><span class="sxs-lookup"><span data-stu-id="c0249-279">Java</span></span>](#tab/Java)

```java
final UsernamePasswordCredential usernamePasswordCredential = new UsernamePasswordCredentialBuilder()
        .clientId(clientId)
        .username(username)
        .password(password)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, usernamePasswordCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[<span data-ttu-id="c0249-280">Android</span><span class="sxs-lookup"><span data-stu-id="c0249-280">Android</span></span>](#tab/Android)

<span data-ttu-id="c0249-281">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-281">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="c0249-282">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0249-282">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c0249-283">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="c0249-283">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="c0249-284">PHP</span><span class="sxs-lookup"><span data-stu-id="c0249-284">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c0249-285">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="c0249-285">Not yet available.</span></span> <span data-ttu-id="c0249-286">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="c0249-286">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="c0249-287">Ruby</span><span class="sxs-lookup"><span data-stu-id="c0249-287">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c0249-288">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="c0249-288">Not yet available.</span></span> <span data-ttu-id="c0249-289">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="c0249-289">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="c0249-290">Следующие шаги</span><span class="sxs-lookup"><span data-stu-id="c0249-290">Next steps</span></span>

* <span data-ttu-id="c0249-291">Поставщикам проверки подлинности требуется идентификация клиента.</span><span class="sxs-lookup"><span data-stu-id="c0249-291">Authentication providers require an client ID.</span></span> <span data-ttu-id="c0249-292">Вы захотите [зарегистрировать свое приложение после](https://portal.azure.com/) того, как настроите поставщика проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c0249-292">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="c0249-293">Дайте нам знать, если необходимый поток OAuth в настоящее время не поддерживается путем голосования или открытия запроса [функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span><span class="sxs-lookup"><span data-stu-id="c0249-293">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>
