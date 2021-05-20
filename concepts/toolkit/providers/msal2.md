---
title: Поставщик MSAL 2
description: Поставщик MSAL 2 использует msal-browser для регистрации пользователей и приобретения маркеров для использования в Microsoft Graph
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: f583845f5c1929669242323501d08fa4a861197e
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579847"
---
# <a name="msal-2--provider"></a><span data-ttu-id="e0e7b-103">Поставщик MSAL 2</span><span class="sxs-lookup"><span data-stu-id="e0e7b-103">MSAL 2  provider</span></span>

<span data-ttu-id="e0e7b-104">Поставщик MSAL 2 использует [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) для регистрации пользователей и приобретения маркеров для использования в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-104">The MSAL 2 provider uses [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) to sign in users and acquire tokens to use with Microsoft Graph.</span></span>
<span data-ttu-id="e0e7b-105">Дополнительные дополнительные новости см. [в см. в руберсе "Поставщики услуг".](./providers.md)</span><span class="sxs-lookup"><span data-stu-id="e0e7b-105">To learn more, see [providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="e0e7b-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="e0e7b-106">Get started</span></span>

<span data-ttu-id="e0e7b-107">Вы можете инициализировать поставщика MSAL 2.0 в HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-107">You can initialize the MSAL 2.0 provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="e0e7b-108">Инициализация на странице HTML</span><span class="sxs-lookup"><span data-stu-id="e0e7b-108">Initialize in your HTML page</span></span>

<span data-ttu-id="e0e7b-109">Инициализация поставщика MSAL 2 в HTML — самый простой способ создания нового поставщика.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-109">Initializing the MSAL 2 provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="e0e7b-110">Используйте компонент `mgt-msal2-provider` для набора **клиентских и** других свойств.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-110">Use the `mgt-msal2-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="e0e7b-111">Это создаст новый экземпляр, который будет использоваться для всех маркеров проверки подлинности и `PublicClientApplication` приобретения.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-111">This will create a new `PublicClientApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
    <mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"
                        login-type="redirect/popup" 
                        scopes="user.read,people.read" 
                        redirect-uri="https://my.redirect/uri" 
                        authority=""> 
    </mgt-msal2-provider> 
```

| <span data-ttu-id="e0e7b-112">Атрибут</span><span class="sxs-lookup"><span data-stu-id="e0e7b-112">Attribute</span></span>    | <span data-ttu-id="e0e7b-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e0e7b-113">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e0e7b-114">client-id</span><span class="sxs-lookup"><span data-stu-id="e0e7b-114">client-id</span></span>    | <span data-ttu-id="e0e7b-115">Строковая ID клиента (см. статью Создание ID приложения/клиента).</span><span class="sxs-lookup"><span data-stu-id="e0e7b-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="e0e7b-116">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-116">Required.</span></span>                                                                                                                                                                                                           |
| <span data-ttu-id="e0e7b-117">тип входа</span><span class="sxs-lookup"><span data-stu-id="e0e7b-117">login-type</span></span>   | <span data-ttu-id="e0e7b-118">Переумеление между `redirect` и по умолчанию является `popup` `redirect` значением .</span><span class="sxs-lookup"><span data-stu-id="e0e7b-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="e0e7b-119">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-119">Optional.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="e0e7b-120">scopes</span><span class="sxs-lookup"><span data-stu-id="e0e7b-120">scopes</span></span>       | <span data-ttu-id="e0e7b-121">Строки с разделителями-запятыми для областей, которым пользователь должен предоставить согласие при входе.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="e0e7b-122">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-122">Optional.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="e0e7b-123">authority</span><span class="sxs-lookup"><span data-stu-id="e0e7b-123">authority</span></span>    | <span data-ttu-id="e0e7b-124">Строка Authority — по умолчанию является общим органом.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="e0e7b-125">Для однотенантного приложения используйте идентификатор клиента или имя клиента.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-125">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="e0e7b-126">Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]`.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-126">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="e0e7b-127">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-127">Optional.</span></span> |
| <span data-ttu-id="e0e7b-128">redirect-uri</span><span class="sxs-lookup"><span data-stu-id="e0e7b-128">redirect-uri</span></span> | <span data-ttu-id="e0e7b-129">Строка URI перенаправления — по умолчанию используется текущее окно URI.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-129">Redirect URI string - by default the current window URI is used.</span></span> <span data-ttu-id="e0e7b-130">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-130">Optional.</span></span>                                                                                                                                                                                            |
| <span data-ttu-id="e0e7b-131">Подсказка</span><span class="sxs-lookup"><span data-stu-id="e0e7b-131">prompt</span></span>       | <span data-ttu-id="e0e7b-132">Тип запроса для входа, между ```SELECT_ACCOUNT``` и ```CONSENT``` ```LOGIN``` .</span><span class="sxs-lookup"><span data-stu-id="e0e7b-132">Type of prompt to use for login, between ```SELECT_ACCOUNT```, ```CONSENT``` and ```LOGIN```.</span></span> <span data-ttu-id="e0e7b-133">Значение по умолчанию: ```SELECT_ACCOUNT```.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-133">Default is ```SELECT_ACCOUNT```.</span></span> <span data-ttu-id="e0e7b-134">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-134">Optional.</span></span>

### <a name="initialize-in-javascript"></a><span data-ttu-id="e0e7b-135">Инициализация в JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0e7b-135">Initialize in JavaScript</span></span>

<span data-ttu-id="e0e7b-136">Вы можете предоставить больше вариантов, инициализируя поставщика в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-136">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
    import {Providers, LoginType} from '@microsoft/mgt-element';
    import {Msal2Provider, PromptType} from '@microsoft/mgt-msal2-provider';

    // initialize the auth provider globally
    Providers.globalProvider = new Msal2Provider({
      clientId: 'REPLACE_WITH_CLIENTID',
      scopes?: string[],
      authority?: string,
      redirectUri?: string,
      loginType?: LoginType, // LoginType.Popup or LoginType.Redirect (redirect is default)
      prompt?: PromptType, // PromptType.CONSENT, PromptType.LOGIN or PromptType.SELECT_ACCOUNT
      sid?: string, // Session ID
      loginHint?: string,
      domainHint?: string,
      options?: Configuration // msal js Configuration object
    });
```

## <a name="creating-an-appclient-id"></a><span data-ttu-id="e0e7b-137">Создание идентификатора клиента/приложения</span><span class="sxs-lookup"><span data-stu-id="e0e7b-137">Creating an app/client ID</span></span>

<span data-ttu-id="e0e7b-138">Дополнительные сведения о том, как зарегистрировать приложение и получить клиентский ID, см. в Azure Active Directory [app.](../get-started/add-aad-app-registration.md)</span><span class="sxs-lookup"><span data-stu-id="e0e7b-138">For details about how to register an app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>

## <a name="difference-between-msal2provider-and-msalprovider"></a><span data-ttu-id="e0e7b-139">Разница между Msal2Provider и MsalProvider</span><span class="sxs-lookup"><span data-stu-id="e0e7b-139">Difference between Msal2Provider and MsalProvider</span></span>
<span data-ttu-id="e0e7b-140">Несмотря на то, что использование очень похоже, MsalProvider и Msal2Provider построены на основе различных потоков OAuth.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-140">Although the usage is very similar, MsalProvider and Msal2Provider are built on top of different OAuth flows.</span></span> <span data-ttu-id="e0e7b-141">MsalProvider построен на вершине MSAL.js, которая реализует неявный грант OAuth2.0 [Flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="e0e7b-141">MsalProvider is built on top of MSAL.js, which implements the OAuth2.0 [Implicit Grant Flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span> <span data-ttu-id="e0e7b-142">Msal2Provider построен на основе [msal-browser,](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser)который реализует код авторизации OAuth 2.0 [Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow) с PKCE.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-142">Msal2Provider is built on top of [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser), which implements the OAuth 2.0 [Authorization Code Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow) with PKCE.</span></span>
<span data-ttu-id="e0e7b-143">Код авторизации Flow более безопасный, чем неявный грант Flow для веб-приложений, поэтому рекомендуется использовать MSAL2Provider над MSALProvider.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-143">Authorization Code Flow is deemed more secure than Implicit Grant Flow for web applications, so we recommend usage of MSAL2Provider over MSALProvider.</span></span> <span data-ttu-id="e0e7b-144">Сведения о проблемах безопасности, связанных с неявным потоком грантов, см. в материале [Недостатки неявного потока.](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6)</span><span class="sxs-lookup"><span data-stu-id="e0e7b-144">For details about security issues related to implicit grant flow, see [Disadvantages of the implicit flow](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6).</span></span>

## <a name="migrating-from-msal-provider-to-msal-2-provider"></a><span data-ttu-id="e0e7b-145">Переход от поставщика MSAL к поставщику MSAL 2</span><span class="sxs-lookup"><span data-stu-id="e0e7b-145">Migrating from MSAL Provider to MSAL 2 Provider</span></span>
<span data-ttu-id="e0e7b-146">Чтобы перенести приложение, использующее поставщика MSAL, к поставщику MSAL 2:</span><span class="sxs-lookup"><span data-stu-id="e0e7b-146">To migrate an application that's using MSAL provider to the MSAL 2 Provider:</span></span>
1. <span data-ttu-id="e0e7b-147">Перейдите на портал Azure по адресу https://portal.azure.com.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-147">Go to the Azure portal at https://portal.azure.com.</span></span>
1. <span data-ttu-id="e0e7b-148">В меню выберите **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-148">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="e0e7b-149">В меню Azure Active Directory выберите **Регистрация приложений**.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-149">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="e0e7b-150">Выберите регистрацию приложения, используемого в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-150">Select the app registration of the app that you're currently using.</span></span> 
1. <span data-ttu-id="e0e7b-151">Перейдите **к проверке подлинности** в левом меню.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-151">Go to **Authentication** on the left menu.</span></span>
1. <span data-ttu-id="e0e7b-152">В **настройках платформы** нажмите кнопку **Добавить платформу** и выберите **одно-страницное приложение.**</span><span class="sxs-lookup"><span data-stu-id="e0e7b-152">Under **Platform configurations**, click on **Add a platform** and select **Single-page Application**.</span></span>
1. <span data-ttu-id="e0e7b-153">Удалите все URL-адреса перенаправления, зарегистрированные в **интернете,** и добавьте их в **одностражном приложении.**</span><span class="sxs-lookup"><span data-stu-id="e0e7b-153">Remove all the redirect URIs that you have currently registered under **Web**, and instead add them under **Single-page application**.</span></span>
1. <span data-ttu-id="e0e7b-154">В коде замените MSALProvider на MSAL2Provider.</span><span class="sxs-lookup"><span data-stu-id="e0e7b-154">In your code, replace MSALProvider with MSAL2Provider.</span></span>

    <span data-ttu-id="e0e7b-155">Если вы инициализируете поставщика в коде JS/TS, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="e0e7b-155">If you are initializing your provider in the JS/TS code, follow these steps:</span></span>
    
    <span data-ttu-id="e0e7b-156">Замените заявление на ```mgt-msal-provider``` импорт</span><span class="sxs-lookup"><span data-stu-id="e0e7b-156">Replace the import statement for ```mgt-msal-provider``` with</span></span> 
    ```ts 
    import {Msal2Provider, PromptType} from '@microsoft/mgt-msal2-provider';
    ```

    <span data-ttu-id="e0e7b-157">Замените инициализацию MsalProvider</span><span class="sxs-lookup"><span data-stu-id="e0e7b-157">Replace the initialization of MsalProvider with</span></span>
    ```ts
    Providers.globalProvider = new Msal2Provider({ 
      clientId: 'REPLACE_WITH_CLIENTID'
      ...
    })
    ```
    <span data-ttu-id="e0e7b-158">Если вы инициализируете поставщика в HTML, замените</span><span class="sxs-lookup"><span data-stu-id="e0e7b-158">If you are initializing the provider in HTML, replace</span></span> 
    ```html
    <mgt-msal-provider client-id="" ... ></mgt-msal-provider>
    ``` 
    <span data-ttu-id="e0e7b-159">с</span><span class="sxs-lookup"><span data-stu-id="e0e7b-159">with</span></span> 
    ```html
    <mgt-msal2-provider  client-id="" ... ></mgt-msal2-provider>
     ```
    <span data-ttu-id="e0e7b-160">Подробные сведения см. [в материале Initialize на странице HTML.](#initialize-in-your-html-page)</span><span class="sxs-lookup"><span data-stu-id="e0e7b-160">For details, see [Initialize in your HTML page](#initialize-in-your-html-page).</span></span>
