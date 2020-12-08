---
title: Выбор поставщика проверки подлинности Microsoft Graph
description: Сведения о том, как выбрать поставщиков проверки подлинности для конкретного сценария для вашего приложения.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 29f7ea60080ed1f1a2ed6ea02256e03f5b91e6cd
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49580972"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a><span data-ttu-id="ce6b3-103">Выбор поставщика проверки подлинности Microsoft Graph на основе сценария</span><span class="sxs-lookup"><span data-stu-id="ce6b3-103">Choose a Microsoft Graph authentication provider based on scenario</span></span>

<span data-ttu-id="ce6b3-104">Поставщики проверки подлинности реализуют код, необходимый для получения маркера с помощью библиотеки проверки подлинности Microsoft (MSAL); обрабатывать ряд потенциальных ошибок в случае появления добавочного согласия, просроченных паролей и условного доступа; а затем задайте заголовок авторизации HTTP-запроса.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-104">Authentication providers implement the code required to acquire a token using the Microsoft Authentication Library (MSAL); handle a number of potential errors for cases like incremental consent, expired passwords, and conditional access; and then set the HTTP request authorization header.</span></span> <span data-ttu-id="ce6b3-105">В следующей таблице перечислены поставщики, которые отвечают сценариям для различных [типов приложений](/azure/active-directory/develop/v2-app-types).</span><span class="sxs-lookup"><span data-stu-id="ce6b3-105">The following table lists the set of providers that match the scenarios for different [application types](/azure/active-directory/develop/v2-app-types).</span></span>

|<span data-ttu-id="ce6b3-106">Сценарий</span><span class="sxs-lookup"><span data-stu-id="ce6b3-106">Scenario</span></span> | <span data-ttu-id="ce6b3-107">Flow/Grant</span><span class="sxs-lookup"><span data-stu-id="ce6b3-107">Flow/Grant</span></span> | <span data-ttu-id="ce6b3-108">Аудитория</span><span class="sxs-lookup"><span data-stu-id="ce6b3-108">Audience</span></span> | <span data-ttu-id="ce6b3-109">Поставщик</span><span class="sxs-lookup"><span data-stu-id="ce6b3-109">Provider</span></span>|
|--|--|--|--|
| [<span data-ttu-id="ce6b3-110">Приложение с одной страницей</span><span class="sxs-lookup"><span data-stu-id="ce6b3-110">Single Page App</span></span>](/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | <span data-ttu-id="ce6b3-111">Неявный поток</span><span class="sxs-lookup"><span data-stu-id="ce6b3-111">Implicit</span></span> | <span data-ttu-id="ce6b3-112">Делегированный потребитель/org</span><span class="sxs-lookup"><span data-stu-id="ce6b3-112">Delegated Consumer/Org</span></span> |[<span data-ttu-id="ce6b3-113">Неявный поставщик</span><span class="sxs-lookup"><span data-stu-id="ce6b3-113">Implicit Provider</span></span>](#ImplicitProvider) |
| [<span data-ttu-id="ce6b3-114">Веб-приложение, вызывающее веб-API</span><span class="sxs-lookup"><span data-stu-id="ce6b3-114">Web App that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | <span data-ttu-id="ce6b3-115">Authorization Code</span><span class="sxs-lookup"><span data-stu-id="ce6b3-115">Authorization Code</span></span> | <span data-ttu-id="ce6b3-116">Делегированный потребитель/org</span><span class="sxs-lookup"><span data-stu-id="ce6b3-116">Delegated Consumer/Org</span></span> | [<span data-ttu-id="ce6b3-117">Поставщик кода авторизации</span><span class="sxs-lookup"><span data-stu-id="ce6b3-117">Authorization Code Provider</span></span>](#AuthCodeProvider) |
| | <span data-ttu-id="ce6b3-118">Учетные данные клиента</span><span class="sxs-lookup"><span data-stu-id="ce6b3-118">Client Credentials</span></span>  | <span data-ttu-id="ce6b3-119">Только приложение</span><span class="sxs-lookup"><span data-stu-id="ce6b3-119">App Only</span></span> | [<span data-ttu-id="ce6b3-120">Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="ce6b3-120">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="ce6b3-121">Веб-API, вызывающий веб-API</span><span class="sxs-lookup"><span data-stu-id="ce6b3-121">Web API that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | <span data-ttu-id="ce6b3-122">От имени</span><span class="sxs-lookup"><span data-stu-id="ce6b3-122">On Behalf Of</span></span> | <span data-ttu-id="ce6b3-123">Делегированный потребитель/org</span><span class="sxs-lookup"><span data-stu-id="ce6b3-123">Delegated Consumer/Org</span></span> | [<span data-ttu-id="ce6b3-124">От имени поставщика</span><span class="sxs-lookup"><span data-stu-id="ce6b3-124">On Behalf Of Provider</span></span>](#OnBehalfOfProvider) |
| | <span data-ttu-id="ce6b3-125">Учетные данные клиента</span><span class="sxs-lookup"><span data-stu-id="ce6b3-125">Client Credentials</span></span>  | <span data-ttu-id="ce6b3-126">Только приложение</span><span class="sxs-lookup"><span data-stu-id="ce6b3-126">App Only</span></span> | [<span data-ttu-id="ce6b3-127">Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="ce6b3-127">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="ce6b3-128">Классическое приложение, вызывающее веб-API</span><span class="sxs-lookup"><span data-stu-id="ce6b3-128">Desktop app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | <span data-ttu-id="ce6b3-129">Интерактивны</span><span class="sxs-lookup"><span data-stu-id="ce6b3-129">Interactive</span></span> | <span data-ttu-id="ce6b3-130">Делегированный потребитель/org</span><span class="sxs-lookup"><span data-stu-id="ce6b3-130">Delegated Consumer/Org</span></span> | [<span data-ttu-id="ce6b3-131">Интерактивный поставщик</span><span class="sxs-lookup"><span data-stu-id="ce6b3-131">Interactive Provider</span></span>](#InteractiveProvider) |
| | <span data-ttu-id="ce6b3-132">Интегрированная система Windows</span><span class="sxs-lookup"><span data-stu-id="ce6b3-132">Integrated Windows</span></span> | <span data-ttu-id="ce6b3-133">Делегированная org</span><span class="sxs-lookup"><span data-stu-id="ce6b3-133">Delegated Org</span></span> | [<span data-ttu-id="ce6b3-134">Интегрированный поставщик Windows</span><span class="sxs-lookup"><span data-stu-id="ce6b3-134">Integrated Windows Provider</span></span>](#IntegratedWindowsProvider) |
| | <span data-ttu-id="ce6b3-135">Владелец ресурса</span><span class="sxs-lookup"><span data-stu-id="ce6b3-135">Resource Owner</span></span>  | <span data-ttu-id="ce6b3-136">Делегированная org</span><span class="sxs-lookup"><span data-stu-id="ce6b3-136">Delegated Org</span></span> | [<span data-ttu-id="ce6b3-137">Имя пользователя и поставщик паролей</span><span class="sxs-lookup"><span data-stu-id="ce6b3-137">Username / Password Provider</span></span>](#UsernamePasswordProvider) |
| | <span data-ttu-id="ce6b3-138">Код устройства</span><span class="sxs-lookup"><span data-stu-id="ce6b3-138">Device Code</span></span>  | <span data-ttu-id="ce6b3-139">Делегированная org</span><span class="sxs-lookup"><span data-stu-id="ce6b3-139">Delegated Org</span></span> | [<span data-ttu-id="ce6b3-140">Поставщик кода устройства</span><span class="sxs-lookup"><span data-stu-id="ce6b3-140">Device Code Provider</span></span>](#DeviceCodeProvider) |
| [<span data-ttu-id="ce6b3-141">Приложение демона</span><span class="sxs-lookup"><span data-stu-id="ce6b3-141">Daemon app</span></span>](/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | <span data-ttu-id="ce6b3-142">Учетные данные клиента</span><span class="sxs-lookup"><span data-stu-id="ce6b3-142">Client Credentials</span></span>  | <span data-ttu-id="ce6b3-143">Только приложение</span><span class="sxs-lookup"><span data-stu-id="ce6b3-143">App Only</span></span> | [<span data-ttu-id="ce6b3-144">Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="ce6b3-144">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="ce6b3-145">Мобильное приложение, вызывающее веб-API</span><span class="sxs-lookup"><span data-stu-id="ce6b3-145">Mobile app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | <span data-ttu-id="ce6b3-146">Интерактивны</span><span class="sxs-lookup"><span data-stu-id="ce6b3-146">Interactive</span></span> | <span data-ttu-id="ce6b3-147">Делегированный потребитель/org</span><span class="sxs-lookup"><span data-stu-id="ce6b3-147">Delegated Consumer/Org</span></span> | [<span data-ttu-id="ce6b3-148">Интерактивный поставщик</span><span class="sxs-lookup"><span data-stu-id="ce6b3-148">Interactive Provider</span></span>](#InteractiveProvider) |


## <a name="authorization-code-provider"></a><a name="AuthCodeProvider" ></a><span data-ttu-id="ce6b3-149">Поставщик кода авторизации</span><span class="sxs-lookup"><span data-stu-id="ce6b3-149">Authorization code provider</span></span>

<span data-ttu-id="ce6b3-150">Потоки кода авторизации позволяют встроенным и веб-приложениям безопасно получать маркеры в имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-150">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="ce6b3-151">Для получения дополнительных сведений см [код кода авторизации платформы Microsoft Identity и OAuth 2,0](/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span><span class="sxs-lookup"><span data-stu-id="ce6b3-151">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="ce6b3-152">C#</span><span class="sxs-lookup"><span data-stu-id="ce6b3-152">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="ce6b3-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce6b3-153">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="ce6b3-154">В настоящее время код авторизации, учетные данные клиента и потоки OAuth "от имени" требуют реализации настраиваемого поставщика проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-154">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="ce6b3-155">Дополнительные сведения см. в разделе [Использование настраиваемого поставщика проверки подлинности](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="ce6b3-155">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="ce6b3-156">Java</span><span class="sxs-lookup"><span data-stu-id="ce6b3-156">Java</span></span>](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="android"></a>[<span data-ttu-id="ce6b3-157">Android</span><span class="sxs-lookup"><span data-stu-id="ce6b3-157">Android</span></span>](#tab/Android)

<span data-ttu-id="ce6b3-158">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-158">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="ce6b3-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce6b3-159">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="ce6b3-160">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-160">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="ce6b3-161">PHP</span><span class="sxs-lookup"><span data-stu-id="ce6b3-161">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ce6b3-162">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-162">Not yet available.</span></span> <span data-ttu-id="ce6b3-163">Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-163">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ce6b3-164">Ruby</span><span class="sxs-lookup"><span data-stu-id="ce6b3-164">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ce6b3-165">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-165">Not available, yet.</span></span> <span data-ttu-id="ce6b3-166">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="ce6b3-166">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="client-credentials-provider"></a><a name="ClientCredentialsProvider"></a><span data-ttu-id="ce6b3-167">Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="ce6b3-167">Client credentials provider</span></span>

<span data-ttu-id="ce6b3-168">Поток учетных данных клиента позволяет приложениям службы работать без взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-168">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="ce6b3-169">Доступ зависит от удостоверения приложения.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-169">Access is based on the identity of the application.</span></span> <span data-ttu-id="ce6b3-170">Дополнительные сведения см. [в статье платформа идентификации Майкрософт и процесс учетных данных клиента OAuth 2,0](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="ce6b3-170">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="ce6b3-171">C#</span><span class="sxs-lookup"><span data-stu-id="ce6b3-171">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascript"></a>[<span data-ttu-id="ce6b3-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce6b3-172">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="ce6b3-173">В настоящее время код авторизации, учетные данные клиента и потоки OAuth "от имени" требуют реализации настраиваемого поставщика проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-173">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="ce6b3-174">Дополнительные сведения см. в разделе [Использование настраиваемого поставщика проверки подлинности](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="ce6b3-174">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="ce6b3-175">Java</span><span class="sxs-lookup"><span data-stu-id="ce6b3-175">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    NationalCloud.Global);
```

# <a name="android"></a>[<span data-ttu-id="ce6b3-176">Android</span><span class="sxs-lookup"><span data-stu-id="ce6b3-176">Android</span></span>](#tab/Android)

<span data-ttu-id="ce6b3-177">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-177">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="ce6b3-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce6b3-178">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="ce6b3-179">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-179">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="ce6b3-180">PHP</span><span class="sxs-lookup"><span data-stu-id="ce6b3-180">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ce6b3-181">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-181">Not available, yet.</span></span> <span data-ttu-id="ce6b3-182">Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-182">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ce6b3-183">Ruby</span><span class="sxs-lookup"><span data-stu-id="ce6b3-183">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ce6b3-184">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-184">Not available, yet.</span></span> <span data-ttu-id="ce6b3-185">Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-185">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="on-behalf-of-provider"></a><a name="OnBehalfOfProvider"></a><span data-ttu-id="ce6b3-186">Поставщик от имени</span><span class="sxs-lookup"><span data-stu-id="ce6b3-186">On-behalf-of provider</span></span>

<span data-ttu-id="ce6b3-187">Потоки "от имени" применяются, когда приложение вызывает службу или веб-API, которые в своюмся вызывает API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-187">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="ce6b3-188">Узнайте больше, прочитав [платформу Microsoft Identity и OAuth 2,0 от имени по поручению](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="ce6b3-188">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="c"></a>[<span data-ttu-id="ce6b3-189">C#</span><span class="sxs-lookup"><span data-stu-id="ce6b3-189">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="ce6b3-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce6b3-190">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="ce6b3-191">В настоящее время код авторизации, учетные данные клиента и потоки OAuth "от имени" требуют реализации настраиваемого поставщика проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-191">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="ce6b3-192">Для получения дополнительных сведений ознакомьтесь [с использованием настраиваемого поставщика проверки подлинности](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) .</span><span class="sxs-lookup"><span data-stu-id="ce6b3-192">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="java"></a>[<span data-ttu-id="ce6b3-193">Java</span><span class="sxs-lookup"><span data-stu-id="ce6b3-193">Java</span></span>](#tab/Java)

<span data-ttu-id="ce6b3-194">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-194">Not yet available.</span></span> <span data-ttu-id="ce6b3-195">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="ce6b3-195">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="ce6b3-196">Android</span><span class="sxs-lookup"><span data-stu-id="ce6b3-196">Android</span></span>](#tab/Android)

<span data-ttu-id="ce6b3-197">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-197">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="ce6b3-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce6b3-198">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="ce6b3-199">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-199">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="ce6b3-200">PHP</span><span class="sxs-lookup"><span data-stu-id="ce6b3-200">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ce6b3-201">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-201">Not yet available.</span></span> <span data-ttu-id="ce6b3-202">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="ce6b3-202">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ce6b3-203">Ruby</span><span class="sxs-lookup"><span data-stu-id="ce6b3-203">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ce6b3-204">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-204">Not yet available.</span></span> <span data-ttu-id="ce6b3-205">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="ce6b3-205">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="implicit-provider"></a><a name="ImplicitProvider"></a><span data-ttu-id="ce6b3-206">Неявный поставщик</span><span class="sxs-lookup"><span data-stu-id="ce6b3-206">Implicit provider</span></span>

<span data-ttu-id="ce6b3-207">Неявный поток предоставления используется в приложениях, основанных на браузерах.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-207">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="ce6b3-208">Для получения дополнительных сведений см [Microsoft Identity Platform и неявный поток предоставления разрешений](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="ce6b3-208">For more information, see [Microsoft identity platform and Implicit grant flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="ce6b3-209">C#</span><span class="sxs-lookup"><span data-stu-id="ce6b3-209">C#</span></span>](#tab/CS)

<span data-ttu-id="ce6b3-210">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-210">Not applicable.</span></span>

# <a name="javascript"></a>[<span data-ttu-id="ce6b3-211">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce6b3-211">Javascript</span></span>](#tab/Javascript)

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

# <a name="java"></a>[<span data-ttu-id="ce6b3-212">Java</span><span class="sxs-lookup"><span data-stu-id="ce6b3-212">Java</span></span>](#tab/Java)

<span data-ttu-id="ce6b3-213">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-213">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="ce6b3-214">Android</span><span class="sxs-lookup"><span data-stu-id="ce6b3-214">Android</span></span>](#tab/Android)

<span data-ttu-id="ce6b3-215">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-215">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="ce6b3-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce6b3-216">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="ce6b3-217">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-217">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="ce6b3-218">PHP</span><span class="sxs-lookup"><span data-stu-id="ce6b3-218">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ce6b3-219">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-219">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ce6b3-220">Ruby</span><span class="sxs-lookup"><span data-stu-id="ce6b3-220">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ce6b3-221">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-221">Not applicable.</span></span>

---

##  <a name="device-code-provider"></a><a name="DeviceCodeProvider"></a><span data-ttu-id="ce6b3-222">Поставщик кода устройства</span><span class="sxs-lookup"><span data-stu-id="ce6b3-222">Device code provider</span></span>

<span data-ttu-id="ce6b3-223">Потоки кода устройства позволяют выполнять вход на устройства с помощью другого устройства.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-223">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="ce6b3-224">Дополнительные сведения см. [в статье платформа идентификации Майкрософт и код устройства OAuth 2,0](/azure/active-directory/develop/v2-oauth2-device-code).</span><span class="sxs-lookup"><span data-stu-id="ce6b3-224">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="c"></a>[<span data-ttu-id="ce6b3-225">C#</span><span class="sxs-lookup"><span data-stu-id="ce6b3-225">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascript"></a>[<span data-ttu-id="ce6b3-226">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce6b3-226">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="ce6b3-227">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-227">Not yet available.</span></span> <span data-ttu-id="ce6b3-228">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="ce6b3-228">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="ce6b3-229">Java</span><span class="sxs-lookup"><span data-stu-id="ce6b3-229">Java</span></span>](#tab/Java)

<span data-ttu-id="ce6b3-230">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-230">Not available, yet.</span></span> <span data-ttu-id="ce6b3-231">Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-231">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="ce6b3-232">Android</span><span class="sxs-lookup"><span data-stu-id="ce6b3-232">Android</span></span>](#tab/Android)

<span data-ttu-id="ce6b3-233">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-233">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="ce6b3-234">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce6b3-234">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="ce6b3-235">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-235">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="ce6b3-236">PHP</span><span class="sxs-lookup"><span data-stu-id="ce6b3-236">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ce6b3-237">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-237">Not yet available.</span></span> <span data-ttu-id="ce6b3-238">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="ce6b3-238">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ce6b3-239">Ruby</span><span class="sxs-lookup"><span data-stu-id="ce6b3-239">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ce6b3-240">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-240">Not yet available.</span></span> <span data-ttu-id="ce6b3-241">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="ce6b3-241">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="integrated-windows-provider"></a><a name="IntegratedWindowsProvider"></a><span data-ttu-id="ce6b3-242">Интегрированный поставщик Windows</span><span class="sxs-lookup"><span data-stu-id="ce6b3-242">Integrated Windows provider</span></span>

<span data-ttu-id="ce6b3-243">Интегрированный поток Windows предоставляет компьютеру Windows способ получить маркер доступа без уведомления при присоединении к домену.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-243">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="ce6b3-244">Подробнее: [Встроенная проверка подлинности Windows](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span><span class="sxs-lookup"><span data-stu-id="ce6b3-244">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="c"></a>[<span data-ttu-id="ce6b3-245">C#</span><span class="sxs-lookup"><span data-stu-id="ce6b3-245">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="ce6b3-246">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce6b3-246">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="ce6b3-247">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-247">Not applicable.</span></span>

# <a name="java"></a>[<span data-ttu-id="ce6b3-248">Java</span><span class="sxs-lookup"><span data-stu-id="ce6b3-248">Java</span></span>](#tab/Java)

<span data-ttu-id="ce6b3-249">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-249">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="ce6b3-250">Android</span><span class="sxs-lookup"><span data-stu-id="ce6b3-250">Android</span></span>](#tab/Android)

<span data-ttu-id="ce6b3-251">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-251">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="ce6b3-252">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce6b3-252">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="ce6b3-253">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-253">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="ce6b3-254">PHP</span><span class="sxs-lookup"><span data-stu-id="ce6b3-254">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ce6b3-255">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-255">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ce6b3-256">Ruby</span><span class="sxs-lookup"><span data-stu-id="ce6b3-256">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ce6b3-257">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-257">Not applicable.</span></span>

---

##  <a name="interactive-provider"></a><a name="InteractiveProvider"></a><span data-ttu-id="ce6b3-258">Интерактивный поставщик</span><span class="sxs-lookup"><span data-stu-id="ce6b3-258">Interactive provider</span></span>

<span data-ttu-id="ce6b3-259">Интерактивный обмен используется приложениями для мобильных устройств (Xamarin и UWP) и приложениями для настольных ПК, чтобы вызывать Microsoft Graph в имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-259">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="ce6b3-260">Дополнительные сведения см в разделе [получение маркеров в интерактивном режиме](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span><span class="sxs-lookup"><span data-stu-id="ce6b3-260">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="c"></a>[<span data-ttu-id="ce6b3-261">C#</span><span class="sxs-lookup"><span data-stu-id="ce6b3-261">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="ce6b3-262">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce6b3-262">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="ce6b3-263">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-263">Not yet available.</span></span> <span data-ttu-id="ce6b3-264">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="ce6b3-264">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="ce6b3-265">Java</span><span class="sxs-lookup"><span data-stu-id="ce6b3-265">Java</span></span>](#tab/Java)

<span data-ttu-id="ce6b3-266">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-266">Not yet available.</span></span> <span data-ttu-id="ce6b3-267">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="ce6b3-267">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="ce6b3-268">Android</span><span class="sxs-lookup"><span data-stu-id="ce6b3-268">Android</span></span>](#tab/Android)

```java
PublicClientApplication publicClientApplication = new PublicClientApplication(getApplicationContext(), "CLIENT_ID_OF_YOUR_APPLICATION");
MSALAuthenticationProvider msalAuthenticationProvider = new MSALAuthenticationProvider(
    getActivity(),
    getApplication(),
    publicClientApplication,
    scopes);

IGraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(msalAuthenticationProvider)
    .buildClient();
```

# <a name="objective-c"></a>[<span data-ttu-id="ce6b3-269">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce6b3-269">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID"
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication
 andOptions:authProviderOptions];
```

# <a name="php"></a>[<span data-ttu-id="ce6b3-270">PHP</span><span class="sxs-lookup"><span data-stu-id="ce6b3-270">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ce6b3-271">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-271">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ce6b3-272">Ruby</span><span class="sxs-lookup"><span data-stu-id="ce6b3-272">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ce6b3-273">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-273">Not applicable.</span></span>

---

##  <a name="usernamepassword-provider"></a><a name="UsernamePasswordProvider"></a><span data-ttu-id="ce6b3-274">Имя пользователя и поставщик паролей</span><span class="sxs-lookup"><span data-stu-id="ce6b3-274">Username/password provider</span></span>

<span data-ttu-id="ce6b3-275">Поставщик имени пользователя и пароля позволяет приложению выполнять вход в систему, используя имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-275">The username/password provider allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="ce6b3-276">Используйте этот поток, только если вы не можете использовать другие потоки OAuth.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-276">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="ce6b3-277">Для получения дополнительных сведений см [платформа идентификации Майкрософт и учетные данные пароля владельца ресурса OAuth 2,0](/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="ce6b3-277">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="c"></a>[<span data-ttu-id="ce6b3-278">C#</span><span class="sxs-lookup"><span data-stu-id="ce6b3-278">C#</span></span>](#tab/CS)

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

# <a name="javascript"></a>[<span data-ttu-id="ce6b3-279">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce6b3-279">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="ce6b3-280">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-280">Not yet available.</span></span> <span data-ttu-id="ce6b3-281">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="ce6b3-281">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="ce6b3-282">Java</span><span class="sxs-lookup"><span data-stu-id="ce6b3-282">Java</span></span>](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="android"></a>[<span data-ttu-id="ce6b3-283">Android</span><span class="sxs-lookup"><span data-stu-id="ce6b3-283">Android</span></span>](#tab/Android)

<span data-ttu-id="ce6b3-284">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-284">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="ce6b3-285">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce6b3-285">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="ce6b3-286">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-286">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="ce6b3-287">PHP</span><span class="sxs-lookup"><span data-stu-id="ce6b3-287">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ce6b3-288">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-288">Not yet available.</span></span> <span data-ttu-id="ce6b3-289">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="ce6b3-289">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ce6b3-290">Ruby</span><span class="sxs-lookup"><span data-stu-id="ce6b3-290">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ce6b3-291">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-291">Not yet available.</span></span> <span data-ttu-id="ce6b3-292">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="ce6b3-292">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="ce6b3-293">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="ce6b3-293">Next steps</span></span>

* <span data-ttu-id="ce6b3-294">Для поставщиков проверки подлинности требуется идентификатор клиента.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-294">Authentication providers require an client ID.</span></span> <span data-ttu-id="ce6b3-295">Вы захотите [зарегистрировать приложение](https://portal.azure.com/) после настройки поставщика проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ce6b3-295">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="ce6b3-296">Сообщите нам, если требуемый потоки OAuth в настоящее время не поддерживается голосованием или открытием [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span><span class="sxs-lookup"><span data-stu-id="ce6b3-296">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>
