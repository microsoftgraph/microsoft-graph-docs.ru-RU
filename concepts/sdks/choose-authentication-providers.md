---
title: Выберите поставщика проверки подлинности Microsoft Graph
description: Узнайте, как выбрать поставщиков проверки подлинности по сценарию для приложения.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 726fbf1334a99ab6a854bd4627052d154187105c
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921128"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a><span data-ttu-id="b24ee-103">Выберите поставщика проверки подлинности Microsoft Graph в зависимости от сценария</span><span class="sxs-lookup"><span data-stu-id="b24ee-103">Choose a Microsoft Graph authentication provider based on scenario</span></span>

<span data-ttu-id="b24ee-104">Поставщики проверки подлинности реализуют код, необходимый для приобретения маркера с помощью Библиотеки проверки подлинности Майкрософт (MSAL); обработка ряда потенциальных ошибок для таких случаев, как постепенное согласие, просроченные пароли и условный доступ; а затем установите заглавную головку авторизации http-запроса.</span><span class="sxs-lookup"><span data-stu-id="b24ee-104">Authentication providers implement the code required to acquire a token using the Microsoft Authentication Library (MSAL); handle a number of potential errors for cases like incremental consent, expired passwords, and conditional access; and then set the HTTP request authorization header.</span></span> <span data-ttu-id="b24ee-105">В следующей таблице перечислены поставщики, которые соответствуют сценариям для различных [типов приложений.](/azure/active-directory/develop/v2-app-types)</span><span class="sxs-lookup"><span data-stu-id="b24ee-105">The following table lists the set of providers that match the scenarios for different [application types](/azure/active-directory/develop/v2-app-types).</span></span>

|<span data-ttu-id="b24ee-106">Сценарий</span><span class="sxs-lookup"><span data-stu-id="b24ee-106">Scenario</span></span> | <span data-ttu-id="b24ee-107">Flow/Grant</span><span class="sxs-lookup"><span data-stu-id="b24ee-107">Flow/Grant</span></span> | <span data-ttu-id="b24ee-108">Аудитория</span><span class="sxs-lookup"><span data-stu-id="b24ee-108">Audience</span></span> | <span data-ttu-id="b24ee-109">Поставщик</span><span class="sxs-lookup"><span data-stu-id="b24ee-109">Provider</span></span>|
|--|--|--|--|
| [<span data-ttu-id="b24ee-110">Приложение для одной страницы</span><span class="sxs-lookup"><span data-stu-id="b24ee-110">Single Page App</span></span>](/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | <span data-ttu-id="b24ee-111">Неявный поток</span><span class="sxs-lookup"><span data-stu-id="b24ee-111">Implicit</span></span> | <span data-ttu-id="b24ee-112">Делегированная потребительская/org</span><span class="sxs-lookup"><span data-stu-id="b24ee-112">Delegated Consumer/Org</span></span> |[<span data-ttu-id="b24ee-113">Неявный поставщик</span><span class="sxs-lookup"><span data-stu-id="b24ee-113">Implicit Provider</span></span>](#ImplicitProvider) |
| [<span data-ttu-id="b24ee-114">Веб-приложение, которое вызывает веб-API</span><span class="sxs-lookup"><span data-stu-id="b24ee-114">Web App that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | <span data-ttu-id="b24ee-115">Authorization Code</span><span class="sxs-lookup"><span data-stu-id="b24ee-115">Authorization Code</span></span> | <span data-ttu-id="b24ee-116">Делегированная потребительская/org</span><span class="sxs-lookup"><span data-stu-id="b24ee-116">Delegated Consumer/Org</span></span> | [<span data-ttu-id="b24ee-117">Поставщик кода авторизации</span><span class="sxs-lookup"><span data-stu-id="b24ee-117">Authorization Code Provider</span></span>](#AuthCodeProvider) |
| | <span data-ttu-id="b24ee-118">Учетные данные клиента</span><span class="sxs-lookup"><span data-stu-id="b24ee-118">Client Credentials</span></span>  | <span data-ttu-id="b24ee-119">Только приложение</span><span class="sxs-lookup"><span data-stu-id="b24ee-119">App Only</span></span> | [<span data-ttu-id="b24ee-120">Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="b24ee-120">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="b24ee-121">Веб-API, который вызывает веб-API</span><span class="sxs-lookup"><span data-stu-id="b24ee-121">Web API that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | <span data-ttu-id="b24ee-122">От имени</span><span class="sxs-lookup"><span data-stu-id="b24ee-122">On Behalf Of</span></span> | <span data-ttu-id="b24ee-123">Делегированная потребительская/org</span><span class="sxs-lookup"><span data-stu-id="b24ee-123">Delegated Consumer/Org</span></span> | [<span data-ttu-id="b24ee-124">От имени поставщика</span><span class="sxs-lookup"><span data-stu-id="b24ee-124">On Behalf Of Provider</span></span>](#OnBehalfOfProvider) |
| | <span data-ttu-id="b24ee-125">Учетные данные клиента</span><span class="sxs-lookup"><span data-stu-id="b24ee-125">Client Credentials</span></span>  | <span data-ttu-id="b24ee-126">Только приложение</span><span class="sxs-lookup"><span data-stu-id="b24ee-126">App Only</span></span> | [<span data-ttu-id="b24ee-127">Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="b24ee-127">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="b24ee-128">Настольное приложение, которое вызывает веб-API</span><span class="sxs-lookup"><span data-stu-id="b24ee-128">Desktop app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | <span data-ttu-id="b24ee-129">Интерактивны</span><span class="sxs-lookup"><span data-stu-id="b24ee-129">Interactive</span></span> | <span data-ttu-id="b24ee-130">Делегированная потребительская/org</span><span class="sxs-lookup"><span data-stu-id="b24ee-130">Delegated Consumer/Org</span></span> | [<span data-ttu-id="b24ee-131">Интерактивный поставщик</span><span class="sxs-lookup"><span data-stu-id="b24ee-131">Interactive Provider</span></span>](#InteractiveProvider) |
| | <span data-ttu-id="b24ee-132">Интегрированная Windows</span><span class="sxs-lookup"><span data-stu-id="b24ee-132">Integrated Windows</span></span> | <span data-ttu-id="b24ee-133">Делегированная org</span><span class="sxs-lookup"><span data-stu-id="b24ee-133">Delegated Org</span></span> | [<span data-ttu-id="b24ee-134">Интегрированный поставщик Windows</span><span class="sxs-lookup"><span data-stu-id="b24ee-134">Integrated Windows Provider</span></span>](#IntegratedWindowsProvider) |
| | <span data-ttu-id="b24ee-135">Владелец ресурса</span><span class="sxs-lookup"><span data-stu-id="b24ee-135">Resource Owner</span></span>  | <span data-ttu-id="b24ee-136">Делегированная org</span><span class="sxs-lookup"><span data-stu-id="b24ee-136">Delegated Org</span></span> | [<span data-ttu-id="b24ee-137">Имя пользователя / Поставщик паролей</span><span class="sxs-lookup"><span data-stu-id="b24ee-137">Username / Password Provider</span></span>](#UsernamePasswordProvider) |
| | <span data-ttu-id="b24ee-138">Код устройства</span><span class="sxs-lookup"><span data-stu-id="b24ee-138">Device Code</span></span>  | <span data-ttu-id="b24ee-139">Делегированная org</span><span class="sxs-lookup"><span data-stu-id="b24ee-139">Delegated Org</span></span> | [<span data-ttu-id="b24ee-140">Поставщик кода устройства</span><span class="sxs-lookup"><span data-stu-id="b24ee-140">Device Code Provider</span></span>](#DeviceCodeProvider) |
| [<span data-ttu-id="b24ee-141">Приложение Daemon</span><span class="sxs-lookup"><span data-stu-id="b24ee-141">Daemon app</span></span>](/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | <span data-ttu-id="b24ee-142">Учетные данные клиента</span><span class="sxs-lookup"><span data-stu-id="b24ee-142">Client Credentials</span></span>  | <span data-ttu-id="b24ee-143">Только приложение</span><span class="sxs-lookup"><span data-stu-id="b24ee-143">App Only</span></span> | [<span data-ttu-id="b24ee-144">Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="b24ee-144">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="b24ee-145">Мобильное приложение, которое вызывает веб-API</span><span class="sxs-lookup"><span data-stu-id="b24ee-145">Mobile app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | <span data-ttu-id="b24ee-146">Интерактивны</span><span class="sxs-lookup"><span data-stu-id="b24ee-146">Interactive</span></span> | <span data-ttu-id="b24ee-147">Делегированная потребительская/org</span><span class="sxs-lookup"><span data-stu-id="b24ee-147">Delegated Consumer/Org</span></span> | [<span data-ttu-id="b24ee-148">Интерактивный поставщик</span><span class="sxs-lookup"><span data-stu-id="b24ee-148">Interactive Provider</span></span>](#InteractiveProvider) |

> <span data-ttu-id="b24ee-149">Примечание. Разработчикам Java и Android необходимо добавить библиотеку [azure-identity,](/java/api/overview/azure/identity-readme?view=azure-java-stable) чтобы получить доступ к различным типам учетных данных.</span><span class="sxs-lookup"><span data-stu-id="b24ee-149">Note: Java and android developers need to add the [azure-identity](/java/api/overview/azure/identity-readme?view=azure-java-stable) library in order to get access to the different credentials types.</span></span>

## <a name="authorization-code-provider"></a><a name="AuthCodeProvider" ></a><span data-ttu-id="b24ee-150">Поставщик кода авторизации</span><span class="sxs-lookup"><span data-stu-id="b24ee-150">Authorization code provider</span></span>

<span data-ttu-id="b24ee-151">Поток кода авторизации позволяет родным и веб-приложениям безопасно получать маркеры от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="b24ee-151">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="b24ee-152">Дополнительные данные см. в записи платформы удостоверений Майкрософт и потока кода авторизации [OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-auth-code-flow)</span><span class="sxs-lookup"><span data-stu-id="b24ee-152">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="b24ee-153">C#</span><span class="sxs-lookup"><span data-stu-id="b24ee-153">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="b24ee-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="b24ee-154">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="b24ee-155">Код авторизации, учетные данные клиентов и потоки OAuth от имени требуют, чтобы вы реализовали настраиваемого поставщика проверки подлинности в это время.</span><span class="sxs-lookup"><span data-stu-id="b24ee-155">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="b24ee-156">Дополнительные сведения см. в [специальном поставщике проверки подлинности.](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)</span><span class="sxs-lookup"><span data-stu-id="b24ee-156">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="b24ee-157">Java</span><span class="sxs-lookup"><span data-stu-id="b24ee-157">Java</span></span>](#tab/Java)

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

# <a name="android"></a>[<span data-ttu-id="b24ee-158">Android</span><span class="sxs-lookup"><span data-stu-id="b24ee-158">Android</span></span>](#tab/Android)

<span data-ttu-id="b24ee-159">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-159">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="b24ee-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b24ee-160">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="b24ee-161">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-161">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="b24ee-162">PHP</span><span class="sxs-lookup"><span data-stu-id="b24ee-162">PHP</span></span>](#tab/PHP)

<span data-ttu-id="b24ee-163">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="b24ee-163">Not yet available.</span></span> <span data-ttu-id="b24ee-164">Пожалуйста, поддержите или откройте [запрос на функцию Microsoft Graph,](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) если это важно для вас.</span><span class="sxs-lookup"><span data-stu-id="b24ee-164">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="b24ee-165">Ruby</span><span class="sxs-lookup"><span data-stu-id="b24ee-165">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="b24ee-166">Пока недоступна.</span><span class="sxs-lookup"><span data-stu-id="b24ee-166">Not available, yet.</span></span> <span data-ttu-id="b24ee-167">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="b24ee-167">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="client-credentials-provider"></a><a name="ClientCredentialsProvider"></a><span data-ttu-id="b24ee-168">Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="b24ee-168">Client credentials provider</span></span>

<span data-ttu-id="b24ee-169">Поток клиентских учетных данных позволяет приложениям-службам работать без взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="b24ee-169">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="b24ee-170">Доступ основан на удостоверении приложения.</span><span class="sxs-lookup"><span data-stu-id="b24ee-170">Access is based on the identity of the application.</span></span> <span data-ttu-id="b24ee-171">Дополнительные сведения см. в веб-сайте Платформы удостоверений Майкрософт и потока учетных данных клиента [OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)</span><span class="sxs-lookup"><span data-stu-id="b24ee-171">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="b24ee-172">C#</span><span class="sxs-lookup"><span data-stu-id="b24ee-172">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascript"></a>[<span data-ttu-id="b24ee-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="b24ee-173">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="b24ee-174">Код авторизации, учетные данные клиентов и потоки OAuth от имени требуют, чтобы вы реализовали настраиваемого поставщика проверки подлинности в это время.</span><span class="sxs-lookup"><span data-stu-id="b24ee-174">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="b24ee-175">Дополнительные сведения см. в [специальном поставщике проверки подлинности.](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)</span><span class="sxs-lookup"><span data-stu-id="b24ee-175">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="b24ee-176">Java</span><span class="sxs-lookup"><span data-stu-id="b24ee-176">Java</span></span>](#tab/Java)

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

# <a name="android"></a>[<span data-ttu-id="b24ee-177">Android</span><span class="sxs-lookup"><span data-stu-id="b24ee-177">Android</span></span>](#tab/Android)

<span data-ttu-id="b24ee-178">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-178">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="b24ee-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b24ee-179">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="b24ee-180">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-180">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="b24ee-181">PHP</span><span class="sxs-lookup"><span data-stu-id="b24ee-181">PHP</span></span>](#tab/PHP)

<span data-ttu-id="b24ee-182">Пока недоступна.</span><span class="sxs-lookup"><span data-stu-id="b24ee-182">Not available, yet.</span></span> <span data-ttu-id="b24ee-183">Пожалуйста, поддержите или откройте [запрос на функцию Microsoft Graph,](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) если это важно для вас.</span><span class="sxs-lookup"><span data-stu-id="b24ee-183">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="b24ee-184">Ruby</span><span class="sxs-lookup"><span data-stu-id="b24ee-184">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="b24ee-185">Пока недоступна.</span><span class="sxs-lookup"><span data-stu-id="b24ee-185">Not available, yet.</span></span> <span data-ttu-id="b24ee-186">Пожалуйста, поддержите или откройте [запрос на функцию Microsoft Graph,](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) если это важно для вас.</span><span class="sxs-lookup"><span data-stu-id="b24ee-186">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="on-behalf-of-provider"></a><a name="OnBehalfOfProvider"></a><span data-ttu-id="b24ee-187">От имени поставщика</span><span class="sxs-lookup"><span data-stu-id="b24ee-187">On-behalf-of provider</span></span>

<span data-ttu-id="b24ee-188">Поток от имени применим, когда приложение вызывает API службы/веб-службы, который по очереди вызывает API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b24ee-188">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="b24ee-189">Узнайте больше, прочитав платформу удостоверений Майкрософт и [поток OAuth 2.0 On-Behalf-Of](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="b24ee-189">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="c"></a>[<span data-ttu-id="b24ee-190">C#</span><span class="sxs-lookup"><span data-stu-id="b24ee-190">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="b24ee-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="b24ee-191">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="b24ee-192">Код авторизации, учетные данные клиентов и потоки OAuth от имени требуют, чтобы вы реализовали настраиваемого поставщика проверки подлинности в это время.</span><span class="sxs-lookup"><span data-stu-id="b24ee-192">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="b24ee-193">Дополнительные сведения читайте в [публикации "Использование](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) поставщика настраиваемой проверки подлинности".</span><span class="sxs-lookup"><span data-stu-id="b24ee-193">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="java"></a>[<span data-ttu-id="b24ee-194">Java</span><span class="sxs-lookup"><span data-stu-id="b24ee-194">Java</span></span>](#tab/Java)

<span data-ttu-id="b24ee-195">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="b24ee-195">Not yet available.</span></span> <span data-ttu-id="b24ee-196">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="b24ee-196">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="b24ee-197">Android</span><span class="sxs-lookup"><span data-stu-id="b24ee-197">Android</span></span>](#tab/Android)

<span data-ttu-id="b24ee-198">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-198">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="b24ee-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b24ee-199">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="b24ee-200">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-200">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="b24ee-201">PHP</span><span class="sxs-lookup"><span data-stu-id="b24ee-201">PHP</span></span>](#tab/PHP)

<span data-ttu-id="b24ee-202">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="b24ee-202">Not yet available.</span></span> <span data-ttu-id="b24ee-203">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="b24ee-203">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="b24ee-204">Ruby</span><span class="sxs-lookup"><span data-stu-id="b24ee-204">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="b24ee-205">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="b24ee-205">Not yet available.</span></span> <span data-ttu-id="b24ee-206">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="b24ee-206">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="implicit-provider"></a><a name="ImplicitProvider"></a><span data-ttu-id="b24ee-207">Неявный поставщик</span><span class="sxs-lookup"><span data-stu-id="b24ee-207">Implicit provider</span></span>

<span data-ttu-id="b24ee-208">Неявный поток грантов используется в браузерных приложениях.</span><span class="sxs-lookup"><span data-stu-id="b24ee-208">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="b24ee-209">Дополнительные сведения см. в [записи платформы удостоверений Майкрософт и потока неявных грантов.](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)</span><span class="sxs-lookup"><span data-stu-id="b24ee-209">For more information, see [Microsoft identity platform and Implicit grant flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="b24ee-210">C#</span><span class="sxs-lookup"><span data-stu-id="b24ee-210">C#</span></span>](#tab/CS)

<span data-ttu-id="b24ee-211">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-211">Not applicable.</span></span>

# <a name="javascript"></a>[<span data-ttu-id="b24ee-212">Javascript</span><span class="sxs-lookup"><span data-stu-id="b24ee-212">Javascript</span></span>](#tab/Javascript)

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

# <a name="java"></a>[<span data-ttu-id="b24ee-213">Java</span><span class="sxs-lookup"><span data-stu-id="b24ee-213">Java</span></span>](#tab/Java)

<span data-ttu-id="b24ee-214">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-214">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="b24ee-215">Android</span><span class="sxs-lookup"><span data-stu-id="b24ee-215">Android</span></span>](#tab/Android)

<span data-ttu-id="b24ee-216">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-216">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="b24ee-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b24ee-217">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="b24ee-218">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-218">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="b24ee-219">PHP</span><span class="sxs-lookup"><span data-stu-id="b24ee-219">PHP</span></span>](#tab/PHP)

<span data-ttu-id="b24ee-220">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-220">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="b24ee-221">Ruby</span><span class="sxs-lookup"><span data-stu-id="b24ee-221">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="b24ee-222">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-222">Not applicable.</span></span>

---

##  <a name="device-code-provider"></a><a name="DeviceCodeProvider"></a><span data-ttu-id="b24ee-223">Поставщик кода устройств</span><span class="sxs-lookup"><span data-stu-id="b24ee-223">Device code provider</span></span>

<span data-ttu-id="b24ee-224">Поток кода устройства позволяет войти на устройства с помощью другого устройства.</span><span class="sxs-lookup"><span data-stu-id="b24ee-224">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="b24ee-225">Подробные сведения см. в материале Платформа удостоверений Майкрософт и поток кода [кода устройств OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-device-code)</span><span class="sxs-lookup"><span data-stu-id="b24ee-225">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="c"></a>[<span data-ttu-id="b24ee-226">C#</span><span class="sxs-lookup"><span data-stu-id="b24ee-226">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascript"></a>[<span data-ttu-id="b24ee-227">Javascript</span><span class="sxs-lookup"><span data-stu-id="b24ee-227">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="b24ee-228">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="b24ee-228">Not yet available.</span></span> <span data-ttu-id="b24ee-229">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="b24ee-229">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="b24ee-230">Java</span><span class="sxs-lookup"><span data-stu-id="b24ee-230">Java</span></span>](#tab/Java)

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

# <a name="android"></a>[<span data-ttu-id="b24ee-231">Android</span><span class="sxs-lookup"><span data-stu-id="b24ee-231">Android</span></span>](#tab/Android)

<span data-ttu-id="b24ee-232">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-232">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="b24ee-233">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b24ee-233">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="b24ee-234">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-234">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="b24ee-235">PHP</span><span class="sxs-lookup"><span data-stu-id="b24ee-235">PHP</span></span>](#tab/PHP)

<span data-ttu-id="b24ee-236">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="b24ee-236">Not yet available.</span></span> <span data-ttu-id="b24ee-237">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="b24ee-237">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="b24ee-238">Ruby</span><span class="sxs-lookup"><span data-stu-id="b24ee-238">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="b24ee-239">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="b24ee-239">Not yet available.</span></span> <span data-ttu-id="b24ee-240">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="b24ee-240">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="integrated-windows-provider"></a><a name="IntegratedWindowsProvider"></a><span data-ttu-id="b24ee-241">Интегрированный поставщик Windows</span><span class="sxs-lookup"><span data-stu-id="b24ee-241">Integrated Windows provider</span></span>

<span data-ttu-id="b24ee-242">Интегрированный поток Windows позволяет компьютерам Windows безмолвно приобретать маркер доступа при присоединении к домену.</span><span class="sxs-lookup"><span data-stu-id="b24ee-242">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="b24ee-243">Подробные сведения см. [в материале Интегрированная проверка подлинности Windows.](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)</span><span class="sxs-lookup"><span data-stu-id="b24ee-243">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="c"></a>[<span data-ttu-id="b24ee-244">C#</span><span class="sxs-lookup"><span data-stu-id="b24ee-244">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="b24ee-245">Javascript</span><span class="sxs-lookup"><span data-stu-id="b24ee-245">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="b24ee-246">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-246">Not applicable.</span></span>

# <a name="java"></a>[<span data-ttu-id="b24ee-247">Java</span><span class="sxs-lookup"><span data-stu-id="b24ee-247">Java</span></span>](#tab/Java)

<span data-ttu-id="b24ee-248">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-248">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="b24ee-249">Android</span><span class="sxs-lookup"><span data-stu-id="b24ee-249">Android</span></span>](#tab/Android)

<span data-ttu-id="b24ee-250">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-250">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="b24ee-251">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b24ee-251">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="b24ee-252">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-252">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="b24ee-253">PHP</span><span class="sxs-lookup"><span data-stu-id="b24ee-253">PHP</span></span>](#tab/PHP)

<span data-ttu-id="b24ee-254">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-254">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="b24ee-255">Ruby</span><span class="sxs-lookup"><span data-stu-id="b24ee-255">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="b24ee-256">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-256">Not applicable.</span></span>

---

##  <a name="interactive-provider"></a><a name="InteractiveProvider"></a><span data-ttu-id="b24ee-257">Интерактивный поставщик</span><span class="sxs-lookup"><span data-stu-id="b24ee-257">Interactive provider</span></span>

<span data-ttu-id="b24ee-258">Интерактивный поток используется мобильными приложениями (Xamarin и UWP) и настольными приложениями для вызова Microsoft Graph от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="b24ee-258">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="b24ee-259">Подробные сведения см. [в материале Эквайринг маркеров в интерактивном режиме.](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)</span><span class="sxs-lookup"><span data-stu-id="b24ee-259">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="c"></a>[<span data-ttu-id="b24ee-260">C#</span><span class="sxs-lookup"><span data-stu-id="b24ee-260">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="b24ee-261">Javascript</span><span class="sxs-lookup"><span data-stu-id="b24ee-261">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="b24ee-262">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="b24ee-262">Not yet available.</span></span> <span data-ttu-id="b24ee-263">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="b24ee-263">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="b24ee-264">Java</span><span class="sxs-lookup"><span data-stu-id="b24ee-264">Java</span></span>](#tab/Java)

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

# <a name="android"></a>[<span data-ttu-id="b24ee-265">Android</span><span class="sxs-lookup"><span data-stu-id="b24ee-265">Android</span></span>](#tab/Android)

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

# <a name="objective-c"></a>[<span data-ttu-id="b24ee-266">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b24ee-266">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID"
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication
 andOptions:authProviderOptions];
```

# <a name="php"></a>[<span data-ttu-id="b24ee-267">PHP</span><span class="sxs-lookup"><span data-stu-id="b24ee-267">PHP</span></span>](#tab/PHP)

<span data-ttu-id="b24ee-268">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-268">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="b24ee-269">Ruby</span><span class="sxs-lookup"><span data-stu-id="b24ee-269">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="b24ee-270">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-270">Not applicable.</span></span>

---

##  <a name="usernamepassword-provider"></a><a name="UsernamePasswordProvider"></a><span data-ttu-id="b24ee-271">Поставщик имен пользователей и паролей</span><span class="sxs-lookup"><span data-stu-id="b24ee-271">Username/password provider</span></span>

<span data-ttu-id="b24ee-272">Поставщик имен пользователей и паролей позволяет приложению войти в пользователя с помощью имени пользователя и пароля.</span><span class="sxs-lookup"><span data-stu-id="b24ee-272">The username/password provider allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="b24ee-273">Используйте этот поток только в том случае, если вы не можете использовать другие потоки OAuth.</span><span class="sxs-lookup"><span data-stu-id="b24ee-273">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="b24ee-274">Дополнительные сведения см. в веб-сайте Платформы удостоверений Майкрософт и учетных данных владельца паролей владельца ресурсов [OAuth 2.0.](/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="b24ee-274">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="c"></a>[<span data-ttu-id="b24ee-275">C#</span><span class="sxs-lookup"><span data-stu-id="b24ee-275">C#</span></span>](#tab/CS)

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

# <a name="javascript"></a>[<span data-ttu-id="b24ee-276">Javascript</span><span class="sxs-lookup"><span data-stu-id="b24ee-276">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="b24ee-277">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="b24ee-277">Not yet available.</span></span> <span data-ttu-id="b24ee-278">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="b24ee-278">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="b24ee-279">Java</span><span class="sxs-lookup"><span data-stu-id="b24ee-279">Java</span></span>](#tab/Java)

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

# <a name="android"></a>[<span data-ttu-id="b24ee-280">Android</span><span class="sxs-lookup"><span data-stu-id="b24ee-280">Android</span></span>](#tab/Android)

<span data-ttu-id="b24ee-281">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-281">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="b24ee-282">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b24ee-282">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="b24ee-283">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b24ee-283">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="b24ee-284">PHP</span><span class="sxs-lookup"><span data-stu-id="b24ee-284">PHP</span></span>](#tab/PHP)

<span data-ttu-id="b24ee-285">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="b24ee-285">Not yet available.</span></span> <span data-ttu-id="b24ee-286">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="b24ee-286">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="b24ee-287">Ruby</span><span class="sxs-lookup"><span data-stu-id="b24ee-287">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="b24ee-288">Еще не доступно.</span><span class="sxs-lookup"><span data-stu-id="b24ee-288">Not yet available.</span></span> <span data-ttu-id="b24ee-289">Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="b24ee-289">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="b24ee-290">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b24ee-290">Next steps</span></span>

* <span data-ttu-id="b24ee-291">Поставщикам проверки подлинности требуется идентификация клиента.</span><span class="sxs-lookup"><span data-stu-id="b24ee-291">Authentication providers require an client ID.</span></span> <span data-ttu-id="b24ee-292">Вы захотите [зарегистрировать свое приложение после](https://portal.azure.com/) того, как настроите поставщика проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b24ee-292">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="b24ee-293">Дайте нам знать, если необходимый поток OAuth в настоящее время не поддерживается путем голосования или открытия запроса [функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span><span class="sxs-lookup"><span data-stu-id="b24ee-293">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>