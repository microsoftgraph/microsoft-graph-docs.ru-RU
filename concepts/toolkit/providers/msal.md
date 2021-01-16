---
title: Поставщик MSAL
description: Поставщик MSAL использует MSAL.js для регистрации пользователей и получения маркеров для использования с Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 738e8ebcd24b3e7e528bdf0a1676dd54103ee2ea
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883027"
---
# <a name="msal-provider"></a><span data-ttu-id="c502a-103">Поставщик MSAL</span><span class="sxs-lookup"><span data-stu-id="c502a-103">MSAL provider</span></span>

<span data-ttu-id="c502a-104">Поставщик MSAL использует [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) для регистрации пользователей и получения маркеров для использования с Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c502a-104">The MSAL provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with Microsoft Graph.</span></span>

<span data-ttu-id="c502a-105">Дополнительные узнать см. [в поставщиках.](./providers.md)</span><span class="sxs-lookup"><span data-stu-id="c502a-105">To learn more, see [providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="c502a-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="c502a-106">Get started</span></span>

<span data-ttu-id="c502a-107">Вы можете инициализировать поставщика MSAL в HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="c502a-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="c502a-108">Инициализация на HTML-странице</span><span class="sxs-lookup"><span data-stu-id="c502a-108">Initialize in your HTML page</span></span>

<span data-ttu-id="c502a-109">Инициализация поставщика MSAL в HTML является простейшим способом создания нового поставщика.</span><span class="sxs-lookup"><span data-stu-id="c502a-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="c502a-110">Используйте `mgt-msal-provider` компонент, чтобы установить **ид клиента** и другие свойства.</span><span class="sxs-lookup"><span data-stu-id="c502a-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="c502a-111">При этом будет создаваться новый экземпляр, который будет использоваться для проверки подлинности `UserAgentApplication` и получения маркеров.</span><span class="sxs-lookup"><span data-stu-id="c502a-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""></mgt-msal-provider>
```

| <span data-ttu-id="c502a-112">Атрибут</span><span class="sxs-lookup"><span data-stu-id="c502a-112">Attribute</span></span>    | <span data-ttu-id="c502a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="c502a-113">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c502a-114">client-id</span><span class="sxs-lookup"><span data-stu-id="c502a-114">client-id</span></span>    | <span data-ttu-id="c502a-115">Строка ИД клиента (см. статью "Создание приложения или клиента").</span><span class="sxs-lookup"><span data-stu-id="c502a-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="c502a-116">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c502a-116">Required.</span></span>                                                                                                                                                                                                           |
| <span data-ttu-id="c502a-117">тип входа</span><span class="sxs-lookup"><span data-stu-id="c502a-117">login-type</span></span>   | <span data-ttu-id="c502a-118">Enumeration between `redirect` and - default value is `popup` `redirect` .</span><span class="sxs-lookup"><span data-stu-id="c502a-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="c502a-119">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c502a-119">Optional.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="c502a-120">scopes</span><span class="sxs-lookup"><span data-stu-id="c502a-120">scopes</span></span>       | <span data-ttu-id="c502a-121">Строки с разделителями-запятыми для областей, которым пользователь должен предоставить согласие при входе.</span><span class="sxs-lookup"><span data-stu-id="c502a-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="c502a-122">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="c502a-122">Optional.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="c502a-123">authority</span><span class="sxs-lookup"><span data-stu-id="c502a-123">authority</span></span>    | <span data-ttu-id="c502a-124">Строка "Полномочия" — по умолчанию является общим органом.</span><span class="sxs-lookup"><span data-stu-id="c502a-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="c502a-125">Для однотенантного приложения используйте идентификатор клиента или имя клиента.</span><span class="sxs-lookup"><span data-stu-id="c502a-125">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="c502a-126">Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]`.</span><span class="sxs-lookup"><span data-stu-id="c502a-126">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="c502a-127">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="c502a-127">Optional.</span></span> |
| <span data-ttu-id="c502a-128">redirect-uri</span><span class="sxs-lookup"><span data-stu-id="c502a-128">redirect-uri</span></span> | <span data-ttu-id="c502a-129">Строка URI перенаправления — по умолчанию используется URI текущего окна.</span><span class="sxs-lookup"><span data-stu-id="c502a-129">Redirect URI string - by default the current window URI is used.</span></span> <span data-ttu-id="c502a-130">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="c502a-130">Optional.</span></span>                                                                                                                                                                                            |
| <span data-ttu-id="c502a-131">depends-on</span><span class="sxs-lookup"><span data-stu-id="c502a-131">depends-on</span></span>   | <span data-ttu-id="c502a-132">Строка селектора элементов другого компонента поставщика с более высоким приоритетом.</span><span class="sxs-lookup"><span data-stu-id="c502a-132">Element selector string of another higher priority provider component.</span></span> <span data-ttu-id="c502a-133">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c502a-133">Optional.</span></span>                                                                                                                                                                                      |

### <a name="initialize-in-javascript"></a><span data-ttu-id="c502a-134">Инициализация в JavaScript</span><span class="sxs-lookup"><span data-stu-id="c502a-134">Initialize in JavaScript</span></span>

<span data-ttu-id="c502a-135">Вы можете предоставить дополнительные параметры, инициализируя поставщика в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="c502a-135">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="c502a-136">Параметр конструктора можно настроить двумя способами, как описано `MsalProvider` в следующих разделах.</span><span class="sxs-lookup"><span data-stu-id="c502a-136">You can configure the `MsalProvider` constructor parameter in two ways, as described in the following sections.</span></span>

#### <a name="provide-a-clientid-to-create-a-new-useragentapplication"></a><span data-ttu-id="c502a-137">Предоставление a `clientId` для создания нового `UserAgentApplication`</span><span class="sxs-lookup"><span data-stu-id="c502a-137">Provide a `clientId` to create a new `UserAgentApplication`</span></span>

<span data-ttu-id="c502a-138">Этот вариант имеет смысл, если набор средств Graph отвечает за всю проверку подлинности в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="c502a-138">This option makes sense when Graph Toolkit is responsible for all authentication in your application.</span></span>

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

#### <a name="pass-an-existing-useragentapplication-in-the-useragentapplication-property"></a><span data-ttu-id="c502a-139">Передав `UserAgentApplication` существующий объект в `userAgentApplication` свойстве.</span><span class="sxs-lookup"><span data-stu-id="c502a-139">Pass an existing `UserAgentApplication` in the `userAgentApplication` property.</span></span>

<span data-ttu-id="c502a-140">Используйте это, когда ваше приложение использует функции MSAL помимо возможностей, которые пользуется другими функциями `MsalProvider` Microsoft Graph набор средств.</span><span class="sxs-lookup"><span data-stu-id="c502a-140">Use this when your app uses MSAL functionality beyond what's exposed by the `MsalProvider` and other Microsoft Graph Toolkit features.</span></span> <span data-ttu-id="c502a-141">Это особенно целесообразно, если в структуре автоматически делается и предоставляется a для вас, например при использовании `UserAgentApplication` [msal-angular.](/azure/active-directory/develop/tutorial-v2-angular)</span><span class="sxs-lookup"><span data-stu-id="c502a-141">This is particularly appropriate if a framework automatically instantiates and exposes a `UserAgentApplication` for you; for example, when using [msal-angular](/azure/active-directory/develop/tutorial-v2-angular).</span></span>

<span data-ttu-id="c502a-142">При использовании этого параметра необходимо понимать возможности для столкновений.</span><span class="sxs-lookup"><span data-stu-id="c502a-142">Be sure to understand opportunities for collisions when using this option.</span></span> <span data-ttu-id="c502a-143">По своей природе существует риск того, что состояние сеанса может измениться, например, с помощью входов или согласия пользователя на `MsalProvider` дополнительные области.</span><span class="sxs-lookup"><span data-stu-id="c502a-143">By its very nature, there is a risk that the `MsalProvider` can change the state of a session, for example by having the user sign in or consent to additional scopes.</span></span> <span data-ttu-id="c502a-144">Убедитесь, что ваше приложение и другие структуры корректно реагируют на эти изменения в состоянии, или рассмотрите возможность использования [настраиваемого поставщика.](./custom.md)</span><span class="sxs-lookup"><span data-stu-id="c502a-144">Make sure that your app and other frameworks respond gracefully to these changes in state, or consider using a [custom provider](./custom.md) instead.</span></span>

```ts
interface MsalConfig {
  userAgentApplication: UserAgentApplication;
  scopes?: string[];
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string;
}
```

<span data-ttu-id="c502a-145">Дополнительные MSAL.js и дополнительные параметры, которые можно использовать при инициализации библиотеки MSAL, см. в [документации MSAL.](/azure/active-directory/develop/msal-js-initializing-client-applications)</span><span class="sxs-lookup"><span data-stu-id="c502a-145">To learn more about MSAL.js and for additional options you can use when initializing the MSAL library, see the [MSAL documentation](/azure/active-directory/develop/msal-js-initializing-client-applications).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="c502a-146">Создание идентификатора клиента/приложения</span><span class="sxs-lookup"><span data-stu-id="c502a-146">Creating an app/client ID</span></span>

<span data-ttu-id="c502a-147">Дополнительные сведения о том, как зарегистрировать приложение и получить ИД клиента, см. в подстановке ["Создание приложения Azure Active Directory".](../get-started/add-aad-app-registration.md)</span><span class="sxs-lookup"><span data-stu-id="c502a-147">For details about how to register an app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>