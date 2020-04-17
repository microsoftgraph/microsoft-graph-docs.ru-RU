---
title: Выбор поставщика проверки подлинности Microsoft Graph
description: Сведения о том, как выбрать поставщиков проверки подлинности для конкретного сценария для вашего приложения.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 678468abae61fa0f9830c0dd1b1578d9aafa177a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868536"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a><span data-ttu-id="bbe1b-103">Выбор поставщика проверки подлинности Microsoft Graph на основе сценария</span><span class="sxs-lookup"><span data-stu-id="bbe1b-103">Choose a Microsoft Graph authentication provider based on scenario</span></span>

<span data-ttu-id="bbe1b-104">Поставщики проверки подлинности реализуют код, необходимый для получения маркера с помощью библиотеки проверки подлинности Microsoft (MSAL); обрабатывать ряд потенциальных ошибок в случае появления добавочного согласия, просроченных паролей и условного доступа; а затем задайте заголовок авторизации HTTP-запроса.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-104">Authentication providers implement the code required to acquire a token using the Microsoft Authentication Library (MSAL); handle a number of potential errors for cases like incremental consent, expired passwords, and conditional access; and then set the HTTP request authorization header.</span></span> <span data-ttu-id="bbe1b-105">В следующей таблице перечислены поставщики, которые отвечают сценариям для различных [типов приложений](/azure/active-directory/develop/v2-app-types).</span><span class="sxs-lookup"><span data-stu-id="bbe1b-105">The following table lists the set of providers that match the scenarios for different [application types](/azure/active-directory/develop/v2-app-types).</span></span>

|<span data-ttu-id="bbe1b-106">Сценарий</span><span class="sxs-lookup"><span data-stu-id="bbe1b-106">Scenario</span></span> | <span data-ttu-id="bbe1b-107">Flow/Grant</span><span class="sxs-lookup"><span data-stu-id="bbe1b-107">Flow/Grant</span></span> | <span data-ttu-id="bbe1b-108">Аудитория</span><span class="sxs-lookup"><span data-stu-id="bbe1b-108">Audience</span></span> | <span data-ttu-id="bbe1b-109">Поставщик</span><span class="sxs-lookup"><span data-stu-id="bbe1b-109">Provider</span></span>|
|--|--|--|--|
| [<span data-ttu-id="bbe1b-110">Приложение с одной страницей</span><span class="sxs-lookup"><span data-stu-id="bbe1b-110">Single Page App</span></span>](/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | <span data-ttu-id="bbe1b-111">Неявный поток</span><span class="sxs-lookup"><span data-stu-id="bbe1b-111">Implicit</span></span> | <span data-ttu-id="bbe1b-112">Делегированный потребитель/org</span><span class="sxs-lookup"><span data-stu-id="bbe1b-112">Delegated Consumer/Org</span></span> |[<span data-ttu-id="bbe1b-113">Неявный поставщик</span><span class="sxs-lookup"><span data-stu-id="bbe1b-113">Implicit Provider</span></span>](#ImplicitProvider) |
| [<span data-ttu-id="bbe1b-114">Веб-приложение, вызывающее веб-API</span><span class="sxs-lookup"><span data-stu-id="bbe1b-114">Web App that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | <span data-ttu-id="bbe1b-115">Authorization Code</span><span class="sxs-lookup"><span data-stu-id="bbe1b-115">Authorization Code</span></span> | <span data-ttu-id="bbe1b-116">Делегированный потребитель/org</span><span class="sxs-lookup"><span data-stu-id="bbe1b-116">Delegated Consumer/Org</span></span> | [<span data-ttu-id="bbe1b-117">Поставщик кода авторизации</span><span class="sxs-lookup"><span data-stu-id="bbe1b-117">Authorization Code Provider</span></span>](#AuthCodeProvider) |
| | <span data-ttu-id="bbe1b-118">Учетные данные клиента</span><span class="sxs-lookup"><span data-stu-id="bbe1b-118">Client Credentials</span></span>  | <span data-ttu-id="bbe1b-119">Только приложение</span><span class="sxs-lookup"><span data-stu-id="bbe1b-119">App Only</span></span> | [<span data-ttu-id="bbe1b-120">Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="bbe1b-120">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="bbe1b-121">Веб-API, вызывающий веб-API</span><span class="sxs-lookup"><span data-stu-id="bbe1b-121">Web API that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | <span data-ttu-id="bbe1b-122">От имени</span><span class="sxs-lookup"><span data-stu-id="bbe1b-122">On Behalf Of</span></span> | <span data-ttu-id="bbe1b-123">Делегированный потребитель/org</span><span class="sxs-lookup"><span data-stu-id="bbe1b-123">Delegated Consumer/Org</span></span> | [<span data-ttu-id="bbe1b-124">От имени поставщика</span><span class="sxs-lookup"><span data-stu-id="bbe1b-124">On Behalf Of Provider</span></span>](#OnBehalfOfProvider) |
| | <span data-ttu-id="bbe1b-125">Учетные данные клиента</span><span class="sxs-lookup"><span data-stu-id="bbe1b-125">Client Credentials</span></span>  | <span data-ttu-id="bbe1b-126">Только приложение</span><span class="sxs-lookup"><span data-stu-id="bbe1b-126">App Only</span></span> | [<span data-ttu-id="bbe1b-127">Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="bbe1b-127">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="bbe1b-128">Классическое приложение, вызывающее веб-API</span><span class="sxs-lookup"><span data-stu-id="bbe1b-128">Desktop app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | <span data-ttu-id="bbe1b-129">Интерактивны</span><span class="sxs-lookup"><span data-stu-id="bbe1b-129">Interactive</span></span> | <span data-ttu-id="bbe1b-130">Делегированный потребитель/org</span><span class="sxs-lookup"><span data-stu-id="bbe1b-130">Delegated Consumer/Org</span></span> | [<span data-ttu-id="bbe1b-131">Интерактивный поставщик</span><span class="sxs-lookup"><span data-stu-id="bbe1b-131">Interactive Provider</span></span>](#InteractiveProvider) |
| | <span data-ttu-id="bbe1b-132">Интегрированная система Windows</span><span class="sxs-lookup"><span data-stu-id="bbe1b-132">Integrated Windows</span></span> | <span data-ttu-id="bbe1b-133">Делегированная org</span><span class="sxs-lookup"><span data-stu-id="bbe1b-133">Delegated Org</span></span> | [<span data-ttu-id="bbe1b-134">Интегрированный поставщик Windows</span><span class="sxs-lookup"><span data-stu-id="bbe1b-134">Integrated Windows Provider</span></span>](#IntegratedWindowsProvider) |
| | <span data-ttu-id="bbe1b-135">Владелец ресурса</span><span class="sxs-lookup"><span data-stu-id="bbe1b-135">Resource Owner</span></span>  | <span data-ttu-id="bbe1b-136">Делегированная org</span><span class="sxs-lookup"><span data-stu-id="bbe1b-136">Delegated Org</span></span> | [<span data-ttu-id="bbe1b-137">Имя пользователя и поставщик паролей</span><span class="sxs-lookup"><span data-stu-id="bbe1b-137">Username / Password Provider</span></span>](#UsernamePasswordProvider) |
| | <span data-ttu-id="bbe1b-138">Код устройства</span><span class="sxs-lookup"><span data-stu-id="bbe1b-138">Device Code</span></span>  | <span data-ttu-id="bbe1b-139">Делегированная org</span><span class="sxs-lookup"><span data-stu-id="bbe1b-139">Delegated Org</span></span> | [<span data-ttu-id="bbe1b-140">Поставщик кода устройства</span><span class="sxs-lookup"><span data-stu-id="bbe1b-140">Device Code Provider</span></span>](#DeviceCodeProvider) |
| [<span data-ttu-id="bbe1b-141">Приложение демона</span><span class="sxs-lookup"><span data-stu-id="bbe1b-141">Daemon app</span></span>](/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | <span data-ttu-id="bbe1b-142">Учетные данные клиента</span><span class="sxs-lookup"><span data-stu-id="bbe1b-142">Client Credentials</span></span>  | <span data-ttu-id="bbe1b-143">Только приложение</span><span class="sxs-lookup"><span data-stu-id="bbe1b-143">App Only</span></span> | [<span data-ttu-id="bbe1b-144">Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="bbe1b-144">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="bbe1b-145">Мобильное приложение, вызывающее веб-API</span><span class="sxs-lookup"><span data-stu-id="bbe1b-145">Mobile app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | <span data-ttu-id="bbe1b-146">Интерактивны</span><span class="sxs-lookup"><span data-stu-id="bbe1b-146">Interactive</span></span> | <span data-ttu-id="bbe1b-147">Делегированный потребитель/org</span><span class="sxs-lookup"><span data-stu-id="bbe1b-147">Delegated Consumer/Org</span></span> | [<span data-ttu-id="bbe1b-148">Интерактивный поставщик</span><span class="sxs-lookup"><span data-stu-id="bbe1b-148">Interactive Provider</span></span>](#InteractiveProvider) |


## <a name="authorization-code-provider"></a><span data-ttu-id="bbe1b-149"><a name="AuthCodeProvider"/>Поставщик кода авторизации</span><span class="sxs-lookup"><span data-stu-id="bbe1b-149"><a name="AuthCodeProvider"/>Authorization code provider</span></span>

<span data-ttu-id="bbe1b-150">Потоки кода авторизации позволяют встроенным и веб-приложениям безопасно получать маркеры в имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-150">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="bbe1b-151">Для получения дополнительных сведений см [код кода авторизации платформы Microsoft Identity и OAuth 2,0](/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span><span class="sxs-lookup"><span data-stu-id="bbe1b-151">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="bbe1b-152">C#</span><span class="sxs-lookup"><span data-stu-id="bbe1b-152">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="bbe1b-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="bbe1b-153">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="bbe1b-154">В настоящее время код авторизации, учетные данные клиента и потоки OAuth "от имени" требуют реализации настраиваемого поставщика проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-154">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="bbe1b-155">Дополнительные сведения см. в разделе [Использование настраиваемого поставщика проверки подлинности](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="bbe1b-155">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="bbe1b-156">Java</span><span class="sxs-lookup"><span data-stu-id="bbe1b-156">Java</span></span>](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="android"></a>[<span data-ttu-id="bbe1b-157">Android</span><span class="sxs-lookup"><span data-stu-id="bbe1b-157">Android</span></span>](#tab/Android)

<span data-ttu-id="bbe1b-158">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-158">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="bbe1b-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbe1b-159">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="bbe1b-160">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-160">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="bbe1b-161">PHP</span><span class="sxs-lookup"><span data-stu-id="bbe1b-161">PHP</span></span>](#tab/PHP)

<span data-ttu-id="bbe1b-162">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-162">Not yet available.</span></span> <span data-ttu-id="bbe1b-163">Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-163">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="bbe1b-164">Ruby</span><span class="sxs-lookup"><span data-stu-id="bbe1b-164">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="bbe1b-165">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-165">Not available, yet.</span></span> <span data-ttu-id="bbe1b-166">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="bbe1b-166">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="client-credentials-provider"></a><span data-ttu-id="bbe1b-167"><a name="ClientCredentialsProvider"/>Поставщик учетных данных клиента</span><span class="sxs-lookup"><span data-stu-id="bbe1b-167"><a name="ClientCredentialsProvider"/>Client credentials provider</span></span>

<span data-ttu-id="bbe1b-168">Поток учетных данных клиента позволяет приложениям службы работать без взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-168">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="bbe1b-169">Доступ зависит от удостоверения приложения.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-169">Access is based on the identity of the application.</span></span> <span data-ttu-id="bbe1b-170">Дополнительные сведения см. [в статье платформа идентификации Майкрософт и процесс учетных данных клиента OAuth 2,0](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="bbe1b-170">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="bbe1b-171">C#</span><span class="sxs-lookup"><span data-stu-id="bbe1b-171">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascript"></a>[<span data-ttu-id="bbe1b-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="bbe1b-172">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="bbe1b-173">В настоящее время код авторизации, учетные данные клиента и потоки OAuth "от имени" требуют реализации настраиваемого поставщика проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-173">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="bbe1b-174">Дополнительные сведения см. в разделе [Использование настраиваемого поставщика проверки подлинности](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="bbe1b-174">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="bbe1b-175">Java</span><span class="sxs-lookup"><span data-stu-id="bbe1b-175">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="android"></a>[<span data-ttu-id="bbe1b-176">Android</span><span class="sxs-lookup"><span data-stu-id="bbe1b-176">Android</span></span>](#tab/Android)

<span data-ttu-id="bbe1b-177">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-177">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="bbe1b-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbe1b-178">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="bbe1b-179">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-179">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="bbe1b-180">PHP</span><span class="sxs-lookup"><span data-stu-id="bbe1b-180">PHP</span></span>](#tab/PHP)

<span data-ttu-id="bbe1b-181">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-181">Not available, yet.</span></span> <span data-ttu-id="bbe1b-182">Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-182">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="bbe1b-183">Ruby</span><span class="sxs-lookup"><span data-stu-id="bbe1b-183">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="bbe1b-184">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-184">Not available, yet.</span></span> <span data-ttu-id="bbe1b-185">Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-185">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="on-behalf-of-provider"></a><span data-ttu-id="bbe1b-186"><a name="OnBehalfOfProvider"/>Поставщик от имени</span><span class="sxs-lookup"><span data-stu-id="bbe1b-186"><a name="OnBehalfOfProvider"/>On-behalf-of provider</span></span>

<span data-ttu-id="bbe1b-187">Потоки "от имени" применяются, когда приложение вызывает службу или веб-API, которые в своюмся вызывает API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-187">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="bbe1b-188">Узнайте больше, прочитав [платформу Microsoft Identity и OAuth 2,0 от имени по поручению](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="bbe1b-188">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="c"></a>[<span data-ttu-id="bbe1b-189">C#</span><span class="sxs-lookup"><span data-stu-id="bbe1b-189">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="bbe1b-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="bbe1b-190">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="bbe1b-191">В настоящее время код авторизации, учетные данные клиента и потоки OAuth "от имени" требуют реализации настраиваемого поставщика проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-191">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="bbe1b-192">Для получения дополнительных сведений ознакомьтесь [с использованием настраиваемого поставщика проверки подлинности](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) .</span><span class="sxs-lookup"><span data-stu-id="bbe1b-192">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="java"></a>[<span data-ttu-id="bbe1b-193">Java</span><span class="sxs-lookup"><span data-stu-id="bbe1b-193">Java</span></span>](#tab/Java)

<span data-ttu-id="bbe1b-194">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-194">Not yet available.</span></span> <span data-ttu-id="bbe1b-195">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="bbe1b-195">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="bbe1b-196">Android</span><span class="sxs-lookup"><span data-stu-id="bbe1b-196">Android</span></span>](#tab/Android)

<span data-ttu-id="bbe1b-197">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-197">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="bbe1b-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbe1b-198">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="bbe1b-199">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-199">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="bbe1b-200">PHP</span><span class="sxs-lookup"><span data-stu-id="bbe1b-200">PHP</span></span>](#tab/PHP)

<span data-ttu-id="bbe1b-201">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-201">Not yet available.</span></span> <span data-ttu-id="bbe1b-202">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="bbe1b-202">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="bbe1b-203">Ruby</span><span class="sxs-lookup"><span data-stu-id="bbe1b-203">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="bbe1b-204">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-204">Not yet available.</span></span> <span data-ttu-id="bbe1b-205">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="bbe1b-205">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="implicit-provider"></a><span data-ttu-id="bbe1b-206"><a name="ImplicitProvider"/>Неявный поставщик</span><span class="sxs-lookup"><span data-stu-id="bbe1b-206"><a name="ImplicitProvider"/>Implicit provider</span></span>

<span data-ttu-id="bbe1b-207">Неявный поток предоставления используется в приложениях, основанных на браузерах.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-207">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="bbe1b-208">Для получения дополнительных сведений см [Microsoft Identity Platform и неявный поток предоставления разрешений](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="bbe1b-208">For more information, see [Microsoft identity platform and Implicit grant flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="bbe1b-209">C#</span><span class="sxs-lookup"><span data-stu-id="bbe1b-209">C#</span></span>](#tab/CS)

<span data-ttu-id="bbe1b-210">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-210">Not applicable.</span></span>

# <a name="javascript"></a>[<span data-ttu-id="bbe1b-211">Javascript</span><span class="sxs-lookup"><span data-stu-id="bbe1b-211">Javascript</span></span>](#tab/Javascript)

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

# <a name="java"></a>[<span data-ttu-id="bbe1b-212">Java</span><span class="sxs-lookup"><span data-stu-id="bbe1b-212">Java</span></span>](#tab/Java)

<span data-ttu-id="bbe1b-213">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-213">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="bbe1b-214">Android</span><span class="sxs-lookup"><span data-stu-id="bbe1b-214">Android</span></span>](#tab/Android)

<span data-ttu-id="bbe1b-215">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-215">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="bbe1b-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbe1b-216">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="bbe1b-217">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-217">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="bbe1b-218">PHP</span><span class="sxs-lookup"><span data-stu-id="bbe1b-218">PHP</span></span>](#tab/PHP)

<span data-ttu-id="bbe1b-219">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-219">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="bbe1b-220">Ruby</span><span class="sxs-lookup"><span data-stu-id="bbe1b-220">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="bbe1b-221">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-221">Not applicable.</span></span>

---

##  <a name="device-code-provider"></a><span data-ttu-id="bbe1b-222"><a name="DeviceCodeProvider"/>Поставщик кода устройства</span><span class="sxs-lookup"><span data-stu-id="bbe1b-222"><a name="DeviceCodeProvider"/>Device code provider</span></span>

<span data-ttu-id="bbe1b-223">Потоки кода устройства позволяют выполнять вход на устройства с помощью другого устройства.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-223">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="bbe1b-224">Дополнительные сведения см. [в статье платформа идентификации Майкрософт и код устройства OAuth 2,0](/azure/active-directory/develop/v2-oauth2-device-code).</span><span class="sxs-lookup"><span data-stu-id="bbe1b-224">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="c"></a>[<span data-ttu-id="bbe1b-225">C#</span><span class="sxs-lookup"><span data-stu-id="bbe1b-225">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascript"></a>[<span data-ttu-id="bbe1b-226">Javascript</span><span class="sxs-lookup"><span data-stu-id="bbe1b-226">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="bbe1b-227">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-227">Not yet available.</span></span> <span data-ttu-id="bbe1b-228">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="bbe1b-228">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="bbe1b-229">Java</span><span class="sxs-lookup"><span data-stu-id="bbe1b-229">Java</span></span>](#tab/Java)

<span data-ttu-id="bbe1b-230">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-230">Not available, yet.</span></span> <span data-ttu-id="bbe1b-231">Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-231">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="bbe1b-232">Android</span><span class="sxs-lookup"><span data-stu-id="bbe1b-232">Android</span></span>](#tab/Android)

<span data-ttu-id="bbe1b-233">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-233">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="bbe1b-234">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbe1b-234">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="bbe1b-235">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-235">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="bbe1b-236">PHP</span><span class="sxs-lookup"><span data-stu-id="bbe1b-236">PHP</span></span>](#tab/PHP)

<span data-ttu-id="bbe1b-237">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-237">Not yet available.</span></span> <span data-ttu-id="bbe1b-238">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="bbe1b-238">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="bbe1b-239">Ruby</span><span class="sxs-lookup"><span data-stu-id="bbe1b-239">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="bbe1b-240">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-240">Not yet available.</span></span> <span data-ttu-id="bbe1b-241">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="bbe1b-241">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="integrated-windows-provider"></a><span data-ttu-id="bbe1b-242"><a name="IntegratedWindowsProvider"/>Интегрированный поставщик Windows</span><span class="sxs-lookup"><span data-stu-id="bbe1b-242"><a name="IntegratedWindowsProvider"/>Integrated Windows provider</span></span>

<span data-ttu-id="bbe1b-243">Интегрированный поток Windows предоставляет компьютеру Windows способ получить маркер доступа без уведомления при присоединении к домену.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-243">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="bbe1b-244">Подробнее: [Встроенная проверка подлинности Windows](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span><span class="sxs-lookup"><span data-stu-id="bbe1b-244">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="c"></a>[<span data-ttu-id="bbe1b-245">C#</span><span class="sxs-lookup"><span data-stu-id="bbe1b-245">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="bbe1b-246">Javascript</span><span class="sxs-lookup"><span data-stu-id="bbe1b-246">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="bbe1b-247">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-247">Not applicable.</span></span>

# <a name="java"></a>[<span data-ttu-id="bbe1b-248">Java</span><span class="sxs-lookup"><span data-stu-id="bbe1b-248">Java</span></span>](#tab/Java)

<span data-ttu-id="bbe1b-249">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-249">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="bbe1b-250">Android</span><span class="sxs-lookup"><span data-stu-id="bbe1b-250">Android</span></span>](#tab/Android)

<span data-ttu-id="bbe1b-251">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-251">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="bbe1b-252">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbe1b-252">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="bbe1b-253">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-253">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="bbe1b-254">PHP</span><span class="sxs-lookup"><span data-stu-id="bbe1b-254">PHP</span></span>](#tab/PHP)

<span data-ttu-id="bbe1b-255">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-255">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="bbe1b-256">Ruby</span><span class="sxs-lookup"><span data-stu-id="bbe1b-256">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="bbe1b-257">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-257">Not applicable.</span></span>

---

##  <a name="interactive-provider"></a><span data-ttu-id="bbe1b-258"><a name="InteractiveProvider"/>Интерактивный поставщик</span><span class="sxs-lookup"><span data-stu-id="bbe1b-258"><a name="InteractiveProvider"/>Interactive provider</span></span>

<span data-ttu-id="bbe1b-259">Интерактивный обмен используется приложениями для мобильных устройств (Xamarin и UWP) и приложениями для настольных ПК, чтобы вызывать Microsoft Graph в имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-259">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="bbe1b-260">Дополнительные сведения см в разделе [получение маркеров в интерактивном режиме](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span><span class="sxs-lookup"><span data-stu-id="bbe1b-260">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="c"></a>[<span data-ttu-id="bbe1b-261">C#</span><span class="sxs-lookup"><span data-stu-id="bbe1b-261">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="bbe1b-262">Javascript</span><span class="sxs-lookup"><span data-stu-id="bbe1b-262">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="bbe1b-263">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-263">Not yet available.</span></span> <span data-ttu-id="bbe1b-264">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="bbe1b-264">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="bbe1b-265">Java</span><span class="sxs-lookup"><span data-stu-id="bbe1b-265">Java</span></span>](#tab/Java)

<span data-ttu-id="bbe1b-266">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-266">Not yet available.</span></span> <span data-ttu-id="bbe1b-267">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="bbe1b-267">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="bbe1b-268">Android</span><span class="sxs-lookup"><span data-stu-id="bbe1b-268">Android</span></span>](#tab/Android)

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

# <a name="objective-c"></a>[<span data-ttu-id="bbe1b-269">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbe1b-269">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID"
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication
 andOptions:authProviderOptions];
```

# <a name="php"></a>[<span data-ttu-id="bbe1b-270">PHP</span><span class="sxs-lookup"><span data-stu-id="bbe1b-270">PHP</span></span>](#tab/PHP)

<span data-ttu-id="bbe1b-271">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-271">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="bbe1b-272">Ruby</span><span class="sxs-lookup"><span data-stu-id="bbe1b-272">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="bbe1b-273">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-273">Not applicable.</span></span>

---

##  <a name="usernamepassword-provider"></a><span data-ttu-id="bbe1b-274"><a name="UsernamePasswordProvider"/>Имя пользователя и поставщик паролей</span><span class="sxs-lookup"><span data-stu-id="bbe1b-274"><a name="UsernamePasswordProvider"/>Username/password provider</span></span>

<span data-ttu-id="bbe1b-275">Поставщик имени пользователя и пароля позволяет приложению выполнять вход в систему, используя имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-275">The username/password provider allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="bbe1b-276">Используйте этот поток, только если вы не можете использовать другие потоки OAuth.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-276">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="bbe1b-277">Для получения дополнительных сведений см [платформа идентификации Майкрософт и учетные данные пароля владельца ресурса OAuth 2,0](/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="bbe1b-277">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="c"></a>[<span data-ttu-id="bbe1b-278">C#</span><span class="sxs-lookup"><span data-stu-id="bbe1b-278">C#</span></span>](#tab/CS)

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

# <a name="javascript"></a>[<span data-ttu-id="bbe1b-279">Javascript</span><span class="sxs-lookup"><span data-stu-id="bbe1b-279">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="bbe1b-280">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-280">Not yet available.</span></span> <span data-ttu-id="bbe1b-281">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="bbe1b-281">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="bbe1b-282">Java</span><span class="sxs-lookup"><span data-stu-id="bbe1b-282">Java</span></span>](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="android"></a>[<span data-ttu-id="bbe1b-283">Android</span><span class="sxs-lookup"><span data-stu-id="bbe1b-283">Android</span></span>](#tab/Android)

<span data-ttu-id="bbe1b-284">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-284">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="bbe1b-285">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbe1b-285">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="bbe1b-286">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-286">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="bbe1b-287">PHP</span><span class="sxs-lookup"><span data-stu-id="bbe1b-287">PHP</span></span>](#tab/PHP)

<span data-ttu-id="bbe1b-288">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-288">Not yet available.</span></span> <span data-ttu-id="bbe1b-289">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="bbe1b-289">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="bbe1b-290">Ruby</span><span class="sxs-lookup"><span data-stu-id="bbe1b-290">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="bbe1b-291">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-291">Not yet available.</span></span> <span data-ttu-id="bbe1b-292">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="bbe1b-292">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="bbe1b-293">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="bbe1b-293">Next steps</span></span>

* <span data-ttu-id="bbe1b-294">Для поставщиков проверки подлинности требуется идентификатор клиента.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-294">Authentication providers require an client ID.</span></span> <span data-ttu-id="bbe1b-295">Вы захотите [зарегистрировать приложение](https://portal.azure.com/) после настройки поставщика проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-295">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="bbe1b-296">Сообщите нам, если требуемый потоки OAuth в настоящее время не поддерживается голосованием или открытием [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span><span class="sxs-lookup"><span data-stu-id="bbe1b-296">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>
