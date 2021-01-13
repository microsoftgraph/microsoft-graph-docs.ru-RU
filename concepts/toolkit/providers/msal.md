---
title: Поставщик MSAL
description: Поставщик MSAL использует MSAL.js для регистрации пользователей и получения маркеров для использования с Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: d3b3d82ae3c60080beaaff7f39a1324022d3ab2a
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659176"
---
# <a name="msal-provider"></a><span data-ttu-id="200e6-103">Поставщик MSAL</span><span class="sxs-lookup"><span data-stu-id="200e6-103">MSAL provider</span></span>

<span data-ttu-id="200e6-104">Поставщик MSAL использует [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) для регистрации пользователей и получения маркеров для использования с Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="200e6-104">The MSAL provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with Microsoft Graph.</span></span>

<span data-ttu-id="200e6-105">Дополнительные узнать см. [в поставщиках.](./providers.md)</span><span class="sxs-lookup"><span data-stu-id="200e6-105">To learn more, see [providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="200e6-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="200e6-106">Get started</span></span>

<span data-ttu-id="200e6-107">Вы можете инициализировать поставщика MSAL в HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="200e6-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="200e6-108">Инициализация на HTML-странице</span><span class="sxs-lookup"><span data-stu-id="200e6-108">Initialize in your HTML page</span></span>

<span data-ttu-id="200e6-109">Инициализация поставщика MSAL в HTML является простейшим способом создания нового поставщика.</span><span class="sxs-lookup"><span data-stu-id="200e6-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="200e6-110">Используйте `mgt-msal-provider` компонент, чтобы установить **ид клиента и** другие свойства.</span><span class="sxs-lookup"><span data-stu-id="200e6-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="200e6-111">При этом будет создаваться новый экземпляр, который будет использоваться для проверки подлинности `UserAgentApplication` и получения маркеров.</span><span class="sxs-lookup"><span data-stu-id="200e6-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""></mgt-msal-provider>
```

| <span data-ttu-id="200e6-112">Атрибут</span><span class="sxs-lookup"><span data-stu-id="200e6-112">Attribute</span></span>    | <span data-ttu-id="200e6-113">Описание</span><span class="sxs-lookup"><span data-stu-id="200e6-113">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="200e6-114">client-id</span><span class="sxs-lookup"><span data-stu-id="200e6-114">client-id</span></span>    | <span data-ttu-id="200e6-115">Строка ИД клиента (см. статью "Создание ИД приложения/клиента").</span><span class="sxs-lookup"><span data-stu-id="200e6-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="200e6-116">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="200e6-116">Required.</span></span>                                                                                                                                                                                                           |
| <span data-ttu-id="200e6-117">тип входа</span><span class="sxs-lookup"><span data-stu-id="200e6-117">login-type</span></span>   | <span data-ttu-id="200e6-118">Enumeration between `redirect` and - default value is `popup` `redirect` .</span><span class="sxs-lookup"><span data-stu-id="200e6-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="200e6-119">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="200e6-119">Optional.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="200e6-120">scopes</span><span class="sxs-lookup"><span data-stu-id="200e6-120">scopes</span></span>       | <span data-ttu-id="200e6-121">Разделенные запятой строки для областей, на которые пользователь должен согласиться при входе.</span><span class="sxs-lookup"><span data-stu-id="200e6-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="200e6-122">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="200e6-122">Optional.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="200e6-123">authority</span><span class="sxs-lookup"><span data-stu-id="200e6-123">authority</span></span>    | <span data-ttu-id="200e6-124">Строка "Полномочия" — по умолчанию является общим органом.</span><span class="sxs-lookup"><span data-stu-id="200e6-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="200e6-125">Для приложений с одним клиентом используйте свой ИД клиента или имя клиента.</span><span class="sxs-lookup"><span data-stu-id="200e6-125">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="200e6-126">Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]` .</span><span class="sxs-lookup"><span data-stu-id="200e6-126">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="200e6-127">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="200e6-127">Optional.</span></span> |
| <span data-ttu-id="200e6-128">redirect-uri</span><span class="sxs-lookup"><span data-stu-id="200e6-128">redirect-uri</span></span> | <span data-ttu-id="200e6-129">Строка URI перенаправления — по умолчанию используется URI текущего окна.</span><span class="sxs-lookup"><span data-stu-id="200e6-129">Redirect URI string - by default the current window URI is used.</span></span> <span data-ttu-id="200e6-130">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="200e6-130">Optional.</span></span>                                                                                                                                                                                            |
| <span data-ttu-id="200e6-131">зависит от</span><span class="sxs-lookup"><span data-stu-id="200e6-131">depends-on</span></span>   | <span data-ttu-id="200e6-132">Строка селектора элементов другого компонента поставщика с более высоким приоритетом.</span><span class="sxs-lookup"><span data-stu-id="200e6-132">Element selector string of another higher priority provider component.</span></span> <span data-ttu-id="200e6-133">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="200e6-133">Optional.</span></span>                                                                                                                                                                                      |

### <a name="initialize-in-javascript"></a><span data-ttu-id="200e6-134">Инициализация в JavaScript</span><span class="sxs-lookup"><span data-stu-id="200e6-134">Initialize in JavaScript</span></span>

<span data-ttu-id="200e6-135">Вы можете предоставить дополнительные параметры, инициализируя поставщика в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="200e6-135">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="200e6-136">Параметр конструктора можно настроить двумя способами, как описано `MsalProvider` в следующих разделах.</span><span class="sxs-lookup"><span data-stu-id="200e6-136">You can configure the `MsalProvider` constructor parameter in two ways, as described in the following sections.</span></span>

#### <a name="provide-a-clientid-to-create-a-new-useragentapplication"></a><span data-ttu-id="200e6-137">Предоставление a `clientId` для создания нового `UserAgentApplication`</span><span class="sxs-lookup"><span data-stu-id="200e6-137">Provide a `clientId` to create a new `UserAgentApplication`</span></span>

<span data-ttu-id="200e6-138">Этот вариант имеет смысл, если набор средств Graph отвечает за всю проверку подлинности в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="200e6-138">This option makes sense when Graph Toolkit is responsible for all authentication in your application.</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string
  options?: Configuration; // msal js Configuration object
}
```

#### <a name="pass-an-existing-useragentapplication-in-the-useragentapplication-property"></a><span data-ttu-id="200e6-139">Передав `UserAgentApplication` существующий объект в `userAgentApplication` свойстве.</span><span class="sxs-lookup"><span data-stu-id="200e6-139">Pass an existing `UserAgentApplication` in the `userAgentApplication` property.</span></span>

<span data-ttu-id="200e6-140">Используйте это, когда ваше приложение использует функции MSAL помимо возможностей, которые функциональность microsoft Graph набор средств `MsalProvider` функций.</span><span class="sxs-lookup"><span data-stu-id="200e6-140">Use this when your app uses MSAL functionality beyond what's exposed by the `MsalProvider` and other Microsoft Graph Toolkit features.</span></span> <span data-ttu-id="200e6-141">Это особенно целесообразно, если в структуре автоматически делается и предоставляется a для вас, например при использовании `UserAgentApplication` [msal-angular.](https://docs.microsoft.com/azure/active-directory/develop/tutorial-v2-angular)</span><span class="sxs-lookup"><span data-stu-id="200e6-141">This is particularly appropriate if a framework automatically instantiates and exposes a `UserAgentApplication` for you; for example, when using [msal-angular](https://docs.microsoft.com/azure/active-directory/develop/tutorial-v2-angular).</span></span>

<span data-ttu-id="200e6-142">При использовании этого параметра необходимо понимать возможности для столкновений.</span><span class="sxs-lookup"><span data-stu-id="200e6-142">Be sure to understand opportunities for collisions when using this option.</span></span> <span data-ttu-id="200e6-143">По своей природе существует риск того, что состояние сеанса может измениться, например, при входе пользователя или согласии на `MsalProvider` дополнительные области.</span><span class="sxs-lookup"><span data-stu-id="200e6-143">By its very nature, there is a risk that the `MsalProvider` can change the state of a session, for example by having the user sign in or consent to additional scopes.</span></span> <span data-ttu-id="200e6-144">Убедитесь, что ваше приложение и другие структуры корректно реагируют на эти изменения в состоянии, или рассмотрите возможность использования [настраиваемого поставщика.](/graph/toolkit/providers/custom)</span><span class="sxs-lookup"><span data-stu-id="200e6-144">Make sure that your app and other frameworks respond gracefully to these changes in state, or consider using a [custom provider](/graph/toolkit/providers/custom) instead.</span></span>

```ts
interface MsalConfig {
  userAgentApplication: UserAgentApplication;
  scopes?: string[];
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string;
}
```

<span data-ttu-id="200e6-145">Дополнительные MSAL.js и дополнительные параметры, которые можно использовать при инициализации библиотеки MSAL, см. в [документации MSAL.](/azure/active-directory/develop/msal-js-initializing-client-applications)</span><span class="sxs-lookup"><span data-stu-id="200e6-145">To learn more about MSAL.js and for additional options you can use when initializing the MSAL library, see the [MSAL documentation](/azure/active-directory/develop/msal-js-initializing-client-applications).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="200e6-146">Создание приложения или ИД клиента</span><span class="sxs-lookup"><span data-stu-id="200e6-146">Creating an app/client ID</span></span>

<span data-ttu-id="200e6-147">Дополнительные сведения о том, как зарегистрировать приложение и получить ИД клиента, см. в подстановке ["Создание приложения Azure Active Directory".](../get-started/add-aad-app-registration.md)</span><span class="sxs-lookup"><span data-stu-id="200e6-147">For details about how to register an app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>
