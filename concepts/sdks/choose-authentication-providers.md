---
title: Выбор поставщика проверки подлинности Microsoft Graph
description: Сведения о том, как выбрать поставщиков проверки подлинности для конкретного сценария для вашего приложения.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 5061b38249f31a6eea959ecec94899337bf57326
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630197"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-oauth-flow"></a><span data-ttu-id="22ebe-103">Выбор поставщика проверки подлинности Microsoft Graph на основе процесса OAuth</span><span class="sxs-lookup"><span data-stu-id="22ebe-103">Choose a Microsoft Graph authentication provider based on OAuth flow</span></span>

<span data-ttu-id="22ebe-104">Поставщики проверки подлинности упрощают извлечение маркера доступа путем абстракции параметров, необходимых для клиентских библиотек проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="22ebe-104">Authentication providers simplify getting an access token by abstracting the parameters required by the authentication client libraries.</span></span> <span data-ttu-id="22ebe-105">Поставщики проверки подлинности Microsoft Graph упрощают использование библиотеки проверки подлинности Microsoft (MSAL), предоставляя адаптеры для каждой платформы.</span><span class="sxs-lookup"><span data-stu-id="22ebe-105">The Microsoft Graph authentication providers simplify the use of the Microsoft Authentication Library (MSAL) by providing adapters for each platform.</span></span> <span data-ttu-id="22ebe-106">Эти адаптеры обрабатывают получение маркера для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="22ebe-106">These adapters handle token acquisition for your application.</span></span> <span data-ttu-id="22ebe-107">Поставщики проверки подлинности Microsoft Graph сопоставляются с процессом предоставления OAuth.</span><span class="sxs-lookup"><span data-stu-id="22ebe-107">The Microsoft Graph authentication providers map to an OAuth grant flow.</span></span> <span data-ttu-id="22ebe-108">Необходимо знать, какой способ предоставления OAuth используется для вашего приложения, чтобы выбрать соответствующий поставщик проверки подлинности для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="22ebe-108">You'll need to know which OAuth grant flow to use for your application in order to select the appropriate authentication provider for your application.</span></span>

## <a name="authorization-code-oauth-flow"></a><span data-ttu-id="22ebe-109">Потоки кода авторизации OAuth</span><span class="sxs-lookup"><span data-stu-id="22ebe-109">Authorization code OAuth flow</span></span>

<span data-ttu-id="22ebe-110">Потоки кода авторизации позволяют встроенным и веб-приложениям безопасно получать маркеры в имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="22ebe-110">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="22ebe-111">Для получения дополнительных сведений см [код кода авторизации платформы Microsoft Identity и OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span><span class="sxs-lookup"><span data-stu-id="22ebe-111">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="22ebe-112">Языках</span><span class="sxs-lookup"><span data-stu-id="22ebe-112">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = AuthorizationCodeProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22ebe-113">Язык</span><span class="sxs-lookup"><span data-stu-id="22ebe-113">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="22ebe-114">В настоящее время код авторизации, учетные данные клиента и потоки OAuth "от имени" требуют реализации настраиваемого поставщика проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="22ebe-114">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="22ebe-115">Дополнительные сведения см. в разделе [Использование настраиваемого поставщика проверки](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)подлинности.</span><span class="sxs-lookup"><span data-stu-id="22ebe-115">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="22ebe-116">Java</span><span class="sxs-lookup"><span data-stu-id="22ebe-116">Java</span></span>](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="22ebe-117">Android</span><span class="sxs-lookup"><span data-stu-id="22ebe-117">Android</span></span>](#tab/Android)

<span data-ttu-id="22ebe-118">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-118">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="22ebe-119">Цель — C</span><span class="sxs-lookup"><span data-stu-id="22ebe-119">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="22ebe-120">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-120">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="22ebe-121">PHP</span><span class="sxs-lookup"><span data-stu-id="22ebe-121">PHP</span></span>](#tab/PHP)

<span data-ttu-id="22ebe-122">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-122">Not yet available.</span></span> <span data-ttu-id="22ebe-123">Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-123">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="22ebe-124">Ruby</span><span class="sxs-lookup"><span data-stu-id="22ebe-124">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="22ebe-125">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-125">Not available, yet.</span></span> <span data-ttu-id="22ebe-126">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="22ebe-126">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="client-credential-oauth-flow"></a><span data-ttu-id="22ebe-127">Потоки учетных данных клиента OAuth</span><span class="sxs-lookup"><span data-stu-id="22ebe-127">Client credential OAuth flow</span></span>

<span data-ttu-id="22ebe-128">Поток учетных данных клиента позволяет приложениям службы работать без взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="22ebe-128">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="22ebe-129">Доступ зависит от удостоверения приложения.</span><span class="sxs-lookup"><span data-stu-id="22ebe-129">Access is based on the identity of the application.</span></span> <span data-ttu-id="22ebe-130">Дополнительные сведения см. [в статье платформа идентификации Майкрософт и процесс учетных данных клиента OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="22ebe-130">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="22ebe-131">Языках</span><span class="sxs-lookup"><span data-stu-id="22ebe-131">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = ClientCredentialProvider.CreateClientApplication(clientId, clientCredential);
ClientCredentialProvider authProvider = new ClientCredentialProvider(clientApplication);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22ebe-132">Язык</span><span class="sxs-lookup"><span data-stu-id="22ebe-132">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="22ebe-133">В настоящее время код авторизации, учетные данные клиента и потоки OAuth "от имени" требуют реализации настраиваемого поставщика проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="22ebe-133">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="22ebe-134">Дополнительные сведения см. в разделе [Использование настраиваемого поставщика проверки](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)подлинности.</span><span class="sxs-lookup"><span data-stu-id="22ebe-134">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="22ebe-135">Java</span><span class="sxs-lookup"><span data-stu-id="22ebe-135">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="22ebe-136">Android</span><span class="sxs-lookup"><span data-stu-id="22ebe-136">Android</span></span>](#tab/Android)

<span data-ttu-id="22ebe-137">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-137">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="22ebe-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="22ebe-138">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="22ebe-139">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-139">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="22ebe-140">PHP</span><span class="sxs-lookup"><span data-stu-id="22ebe-140">PHP</span></span>](#tab/PHP)

<span data-ttu-id="22ebe-141">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-141">Not available, yet.</span></span> <span data-ttu-id="22ebe-142">Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-142">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="22ebe-143">Ruby</span><span class="sxs-lookup"><span data-stu-id="22ebe-143">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="22ebe-144">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-144">Not available, yet.</span></span> <span data-ttu-id="22ebe-145">Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-145">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="on-behalf-of-oauth-flow"></a><span data-ttu-id="22ebe-146">Последовательность OAuth "от имени"</span><span class="sxs-lookup"><span data-stu-id="22ebe-146">On-behalf-of OAuth flow</span></span>

<span data-ttu-id="22ebe-147">Потоки "от имени" применяются, когда приложение вызывает службу или веб-API, которые в своюмся вызывает API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="22ebe-147">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="22ebe-148">Узнайте больше, прочитав [платформу Microsoft Identity и OAuth 2,0 от имени по поручению](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="22ebe-148">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="22ebe-149">Языках</span><span class="sxs-lookup"><span data-stu-id="22ebe-149">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = OnBehalfOfProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
OnBehalfOfProvider authProvider = new OnBehalfOfProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22ebe-150">Язык</span><span class="sxs-lookup"><span data-stu-id="22ebe-150">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="22ebe-151">В настоящее время код авторизации, учетные данные клиента и потоки OAuth "от имени" требуют реализации настраиваемого поставщика проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="22ebe-151">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="22ebe-152">Для получения дополнительных сведений ознакомьтесь [с использованием настраиваемого поставщика проверки](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) подлинности.</span><span class="sxs-lookup"><span data-stu-id="22ebe-152">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="22ebe-153">Java</span><span class="sxs-lookup"><span data-stu-id="22ebe-153">Java</span></span>](#tab/Java)

<span data-ttu-id="22ebe-154">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-154">Not yet available.</span></span> <span data-ttu-id="22ebe-155">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="22ebe-155">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="22ebe-156">Android</span><span class="sxs-lookup"><span data-stu-id="22ebe-156">Android</span></span>](#tab/Android)

<span data-ttu-id="22ebe-157">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-157">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="22ebe-158">Цель — C</span><span class="sxs-lookup"><span data-stu-id="22ebe-158">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="22ebe-159">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-159">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="22ebe-160">PHP</span><span class="sxs-lookup"><span data-stu-id="22ebe-160">PHP</span></span>](#tab/PHP)

<span data-ttu-id="22ebe-161">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-161">Not yet available.</span></span> <span data-ttu-id="22ebe-162">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="22ebe-162">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="22ebe-163">Ruby</span><span class="sxs-lookup"><span data-stu-id="22ebe-163">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="22ebe-164">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-164">Not yet available.</span></span> <span data-ttu-id="22ebe-165">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="22ebe-165">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="implicit-grant-oauth-flow"></a><span data-ttu-id="22ebe-166">Неявный поток предоставления OAuth</span><span class="sxs-lookup"><span data-stu-id="22ebe-166">Implicit grant OAuth flow</span></span>

<span data-ttu-id="22ebe-167">Неявный поток предоставления используется в приложениях, основанных на браузерах.</span><span class="sxs-lookup"><span data-stu-id="22ebe-167">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="22ebe-168">Для получения дополнительных сведений см [Microsoft Identity Platform и неявный поток предоставления разрешений](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="22ebe-168">For more information, see [Microsoft identity platform and Implicit grant flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="22ebe-169">Языках</span><span class="sxs-lookup"><span data-stu-id="22ebe-169">C#</span></span>](#tab/CS)

<span data-ttu-id="22ebe-170">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-170">Not applicable.</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22ebe-171">Язык</span><span class="sxs-lookup"><span data-stu-id="22ebe-171">Javascript</span></span>](#tab/Javascript)

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
const authProvider = new MicrosoftGraph.MSALAuthenticationProvider(userAgentApplication, graphScopes);

const options = {
    authProvider, // An instance created from previous step
};
const Client = MicrosoftGraph.Client;
const client = Client.initWithMiddleware(options);
```

# <a name="javatabjava"></a>[<span data-ttu-id="22ebe-172">Java</span><span class="sxs-lookup"><span data-stu-id="22ebe-172">Java</span></span>](#tab/Java)

<span data-ttu-id="22ebe-173">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-173">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="22ebe-174">Android</span><span class="sxs-lookup"><span data-stu-id="22ebe-174">Android</span></span>](#tab/Android)

<span data-ttu-id="22ebe-175">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-175">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="22ebe-176">Цель — C</span><span class="sxs-lookup"><span data-stu-id="22ebe-176">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="22ebe-177">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-177">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="22ebe-178">PHP</span><span class="sxs-lookup"><span data-stu-id="22ebe-178">PHP</span></span>](#tab/PHP)

<span data-ttu-id="22ebe-179">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-179">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="22ebe-180">Ruby</span><span class="sxs-lookup"><span data-stu-id="22ebe-180">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="22ebe-181">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-181">Not applicable.</span></span>

---

## <a name="device-code-oauth-flow"></a><span data-ttu-id="22ebe-182">Процесс обработки OAuth кода устройства</span><span class="sxs-lookup"><span data-stu-id="22ebe-182">Device code OAuth flow</span></span>

<span data-ttu-id="22ebe-183">Потоки кода устройства позволяют выполнять вход на устройства с помощью другого устройства.</span><span class="sxs-lookup"><span data-stu-id="22ebe-183">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="22ebe-184">Дополнительные сведения см. [в статье платформа идентификации Майкрософт и код устройства OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).</span><span class="sxs-lookup"><span data-stu-id="22ebe-184">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="22ebe-185">Языках</span><span class="sxs-lookup"><span data-stu-id="22ebe-185">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = DeviceCodeProvider.CreateClientApplication(clientId);
DeviceCodeProvider authProvider = new DeviceCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22ebe-186">Язык</span><span class="sxs-lookup"><span data-stu-id="22ebe-186">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="22ebe-187">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-187">Not yet available.</span></span> <span data-ttu-id="22ebe-188">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="22ebe-188">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="22ebe-189">Java</span><span class="sxs-lookup"><span data-stu-id="22ebe-189">Java</span></span>](#tab/Java)

<span data-ttu-id="22ebe-190">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-190">Not available, yet.</span></span> <span data-ttu-id="22ebe-191">Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-191">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="22ebe-192">Android</span><span class="sxs-lookup"><span data-stu-id="22ebe-192">Android</span></span>](#tab/Android)

<span data-ttu-id="22ebe-193">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-193">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="22ebe-194">Цель — C</span><span class="sxs-lookup"><span data-stu-id="22ebe-194">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="22ebe-195">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-195">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="22ebe-196">PHP</span><span class="sxs-lookup"><span data-stu-id="22ebe-196">PHP</span></span>](#tab/PHP)

<span data-ttu-id="22ebe-197">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-197">Not yet available.</span></span> <span data-ttu-id="22ebe-198">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="22ebe-198">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="22ebe-199">Ruby</span><span class="sxs-lookup"><span data-stu-id="22ebe-199">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="22ebe-200">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-200">Not yet available.</span></span> <span data-ttu-id="22ebe-201">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="22ebe-201">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="integrated-windows-flow"></a><span data-ttu-id="22ebe-202">Встроенный Windows Flow</span><span class="sxs-lookup"><span data-stu-id="22ebe-202">Integrated Windows flow</span></span>

<span data-ttu-id="22ebe-203">Интегрированный поток Windows предоставляет компьютеру Windows способ получить маркер доступа без уведомления при присоединении к домену.</span><span class="sxs-lookup"><span data-stu-id="22ebe-203">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="22ebe-204">Подробнее: встроенная [Проверка подлинности Windows](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span><span class="sxs-lookup"><span data-stu-id="22ebe-204">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="22ebe-205">Языках</span><span class="sxs-lookup"><span data-stu-id="22ebe-205">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = IntegratedWindowsAuthenticationProvider.CreateClientApplication(clientId);
IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22ebe-206">Язык</span><span class="sxs-lookup"><span data-stu-id="22ebe-206">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="22ebe-207">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-207">Not applicable.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="22ebe-208">Java</span><span class="sxs-lookup"><span data-stu-id="22ebe-208">Java</span></span>](#tab/Java)

<span data-ttu-id="22ebe-209">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-209">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="22ebe-210">Android</span><span class="sxs-lookup"><span data-stu-id="22ebe-210">Android</span></span>](#tab/Android)

<span data-ttu-id="22ebe-211">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-211">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="22ebe-212">Цель — C</span><span class="sxs-lookup"><span data-stu-id="22ebe-212">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="22ebe-213">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-213">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="22ebe-214">PHP</span><span class="sxs-lookup"><span data-stu-id="22ebe-214">PHP</span></span>](#tab/PHP)

<span data-ttu-id="22ebe-215">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-215">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="22ebe-216">Ruby</span><span class="sxs-lookup"><span data-stu-id="22ebe-216">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="22ebe-217">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-217">Not applicable.</span></span>

---

## <a name="interactive-flow"></a><span data-ttu-id="22ebe-218">Интерактивный процесс</span><span class="sxs-lookup"><span data-stu-id="22ebe-218">Interactive flow</span></span>

<span data-ttu-id="22ebe-219">Интерактивный обмен используется приложениями для мобильных устройств (Xamarin и UWP) и приложениями для настольных ПК, чтобы вызывать Microsoft Graph в имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="22ebe-219">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="22ebe-220">Дополнительные сведения см в разделе [получение маркеров в интерактивном режиме](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span><span class="sxs-lookup"><span data-stu-id="22ebe-220">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="22ebe-221">Языках</span><span class="sxs-lookup"><span data-stu-id="22ebe-221">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = InteractiveAuthenticationProvider.CreateClientApplication(clientId);
InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22ebe-222">Язык</span><span class="sxs-lookup"><span data-stu-id="22ebe-222">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="22ebe-223">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-223">Not yet available.</span></span> <span data-ttu-id="22ebe-224">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="22ebe-224">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="22ebe-225">Java</span><span class="sxs-lookup"><span data-stu-id="22ebe-225">Java</span></span>](#tab/Java)

<span data-ttu-id="22ebe-226">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-226">Not yet available.</span></span> <span data-ttu-id="22ebe-227">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="22ebe-227">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="22ebe-228">Android</span><span class="sxs-lookup"><span data-stu-id="22ebe-228">Android</span></span>](#tab/Android)

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

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="22ebe-229">Цель — C</span><span class="sxs-lookup"><span data-stu-id="22ebe-229">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];
```

# <a name="phptabphp"></a>[<span data-ttu-id="22ebe-230">PHP</span><span class="sxs-lookup"><span data-stu-id="22ebe-230">PHP</span></span>](#tab/PHP)

<span data-ttu-id="22ebe-231">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-231">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="22ebe-232">Ruby</span><span class="sxs-lookup"><span data-stu-id="22ebe-232">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="22ebe-233">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-233">Not applicable.</span></span>

---

## <a name="resource-owner-password-credential-grant-oauth-flow"></a><span data-ttu-id="22ebe-234">Пароль владельца ресурса. предоставление учетных данных для передачи OAuth</span><span class="sxs-lookup"><span data-stu-id="22ebe-234">Resource owner password credential grant OAuth flow</span></span>

<span data-ttu-id="22ebe-235">Потоки учетных данных для пароля владельца ресурса позволяют приложению выполнить вход в систему, используя имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="22ebe-235">The resource owner password credential flow allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="22ebe-236">Используйте этот поток, только если вы не можете использовать другие потоки OAuth.</span><span class="sxs-lookup"><span data-stu-id="22ebe-236">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="22ebe-237">Для получения дополнительных сведений см [платформа идентификации Майкрософт и учетные данные пароля владельца ресурса OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="22ebe-237">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="ctabcs"></a>[<span data-ttu-id="22ebe-238">Языках</span><span class="sxs-lookup"><span data-stu-id="22ebe-238">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = UsernamePasswordProvider.CreateClientApplication(clientId);
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22ebe-239">Язык</span><span class="sxs-lookup"><span data-stu-id="22ebe-239">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="22ebe-240">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-240">Not yet available.</span></span> <span data-ttu-id="22ebe-241">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="22ebe-241">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="22ebe-242">Java</span><span class="sxs-lookup"><span data-stu-id="22ebe-242">Java</span></span>](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="22ebe-243">Android</span><span class="sxs-lookup"><span data-stu-id="22ebe-243">Android</span></span>](#tab/Android)

<span data-ttu-id="22ebe-244">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-244">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="22ebe-245">Цель — C</span><span class="sxs-lookup"><span data-stu-id="22ebe-245">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="22ebe-246">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="22ebe-246">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="22ebe-247">PHP</span><span class="sxs-lookup"><span data-stu-id="22ebe-247">PHP</span></span>](#tab/PHP)

<span data-ttu-id="22ebe-248">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-248">Not yet available.</span></span> <span data-ttu-id="22ebe-249">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="22ebe-249">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="22ebe-250">Ruby</span><span class="sxs-lookup"><span data-stu-id="22ebe-250">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="22ebe-251">Пока недоступно.</span><span class="sxs-lookup"><span data-stu-id="22ebe-251">Not yet available.</span></span> <span data-ttu-id="22ebe-252">Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .</span><span class="sxs-lookup"><span data-stu-id="22ebe-252">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="22ebe-253">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="22ebe-253">Next steps</span></span>

* <span data-ttu-id="22ebe-254">Для поставщиков проверки подлинности требуется идентификатор клиента.</span><span class="sxs-lookup"><span data-stu-id="22ebe-254">Authentication providers require an client ID.</span></span> <span data-ttu-id="22ebe-255">Вы захотите [зарегистрировать приложение](https://portal.azure.com/) после настройки поставщика проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="22ebe-255">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="22ebe-256">Сообщите нам, если требуемый потоки OAuth в настоящее время не поддерживается голосованием или открытием [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span><span class="sxs-lookup"><span data-stu-id="22ebe-256">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>