---
title: Поставщик MSAL
description: Поставщик MSAL использует MSAL.js для регистрации пользователей и приобретения маркеров для использования в Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e612e11e7b1a26765175ba10097c8e54317e9e1d
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579762"
---
# <a name="msal-provider"></a><span data-ttu-id="ee24b-103">Поставщик MSAL</span><span class="sxs-lookup"><span data-stu-id="ee24b-103">MSAL provider</span></span>

<span data-ttu-id="ee24b-104">Поставщик MSAL [использует](https://github.com/AzureAD/microsoft-authentication-library-for-js)MSAL.jsдля регистрации пользователей и приобретения маркеров для использования в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ee24b-104">The MSAL provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with Microsoft Graph.</span></span>

<span data-ttu-id="ee24b-105">Дополнительные дополнительные новости см. [в см. в руберсе "Поставщики услуг".](./providers.md)</span><span class="sxs-lookup"><span data-stu-id="ee24b-105">To learn more, see [providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="ee24b-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="ee24b-106">Get started</span></span>

<span data-ttu-id="ee24b-107">Вы можете инициализировать поставщика MSAL в HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="ee24b-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="ee24b-108">Инициализация на странице HTML</span><span class="sxs-lookup"><span data-stu-id="ee24b-108">Initialize in your HTML page</span></span>

<span data-ttu-id="ee24b-109">Инициализация поставщика MSAL в HTML является простейшим способом создания нового поставщика.</span><span class="sxs-lookup"><span data-stu-id="ee24b-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="ee24b-110">Используйте компонент `mgt-msal-provider` для набора **клиентских и** других свойств.</span><span class="sxs-lookup"><span data-stu-id="ee24b-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="ee24b-111">Это создаст новый экземпляр, который будет использоваться для всех маркеров проверки подлинности и `UserAgentApplication` приобретения.</span><span class="sxs-lookup"><span data-stu-id="ee24b-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""
                   domainHint="mydomain.com"
                   prompt="consent"></mgt-msal-provider>
```

| <span data-ttu-id="ee24b-112">Атрибут</span><span class="sxs-lookup"><span data-stu-id="ee24b-112">Attribute</span></span>    | <span data-ttu-id="ee24b-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ee24b-113">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ee24b-114">client-id</span><span class="sxs-lookup"><span data-stu-id="ee24b-114">client-id</span></span>    | <span data-ttu-id="ee24b-115">Строковая ID клиента (см. статью Создание ID приложения/клиента).</span><span class="sxs-lookup"><span data-stu-id="ee24b-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="ee24b-116">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="ee24b-116">Required.</span></span>                                                                                                                                                                                                           |
| <span data-ttu-id="ee24b-117">тип входа</span><span class="sxs-lookup"><span data-stu-id="ee24b-117">login-type</span></span>   | <span data-ttu-id="ee24b-118">Переумеление между `redirect` и по умолчанию является `popup` `redirect` значением .</span><span class="sxs-lookup"><span data-stu-id="ee24b-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="ee24b-119">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ee24b-119">Optional.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="ee24b-120">scopes</span><span class="sxs-lookup"><span data-stu-id="ee24b-120">scopes</span></span>       | <span data-ttu-id="ee24b-121">Строки с разделителями-запятыми для областей, которым пользователь должен предоставить согласие при входе.</span><span class="sxs-lookup"><span data-stu-id="ee24b-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="ee24b-122">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="ee24b-122">Optional.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="ee24b-123">authority</span><span class="sxs-lookup"><span data-stu-id="ee24b-123">authority</span></span>    | <span data-ttu-id="ee24b-124">Строка Authority — по умолчанию является общим органом.</span><span class="sxs-lookup"><span data-stu-id="ee24b-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="ee24b-125">Для однотенантного приложения используйте идентификатор клиента или имя клиента.</span><span class="sxs-lookup"><span data-stu-id="ee24b-125">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="ee24b-126">Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]`.</span><span class="sxs-lookup"><span data-stu-id="ee24b-126">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="ee24b-127">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="ee24b-127">Optional.</span></span> |
| <span data-ttu-id="ee24b-128">redirect-uri</span><span class="sxs-lookup"><span data-stu-id="ee24b-128">redirect-uri</span></span> | <span data-ttu-id="ee24b-129">Строка URI перенаправления — по умолчанию используется текущее окно URI.</span><span class="sxs-lookup"><span data-stu-id="ee24b-129">Redirect URI string - by default the current window URI is used.</span></span> <span data-ttu-id="ee24b-130">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="ee24b-130">Optional.</span></span>                                                                                                                                                                                            |
| <span data-ttu-id="ee24b-131">depends-on</span><span class="sxs-lookup"><span data-stu-id="ee24b-131">depends-on</span></span>   | <span data-ttu-id="ee24b-132">Строка селектора элементов другого компонента поставщика с более высоким приоритетом.</span><span class="sxs-lookup"><span data-stu-id="ee24b-132">Element selector string of another higher priority provider component.</span></span> <span data-ttu-id="ee24b-133">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ee24b-133">Optional.</span></span> 
| <span data-ttu-id="ee24b-134">подсказка домена</span><span class="sxs-lookup"><span data-stu-id="ee24b-134">domain-hint</span></span>  | <span data-ttu-id="ee24b-135">Строка запроса расположения домена для переададации в опытом.</span><span class="sxs-lookup"><span data-stu-id="ee24b-135">Query string of domain location for forwarding sign in experience.</span></span> <span data-ttu-id="ee24b-136">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ee24b-136">Optional.</span></span>              
| <span data-ttu-id="ee24b-137">Подсказка</span><span class="sxs-lookup"><span data-stu-id="ee24b-137">prompt</span></span> | <span data-ttu-id="ee24b-138">Выбор типа взаимодействия с пользователем, необходимого для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="ee24b-138">Selection for type of user interaction required to login.</span></span> <span data-ttu-id="ee24b-139">Допустимые параметры:</span><span class="sxs-lookup"><span data-stu-id="ee24b-139">Valid options include:</span></span> <ul><li><span data-ttu-id="ee24b-140">`login` заставляет пользователя вводить учетные данные по запросу</span><span class="sxs-lookup"><span data-stu-id="ee24b-140">`login` forces the user to enter credentials on request</span></span> </li><li><span data-ttu-id="ee24b-141">`none` без интерактивной подсказки</span><span class="sxs-lookup"><span data-stu-id="ee24b-141">`none` for no interactive prompt</span></span></li> <li><span data-ttu-id="ee24b-142">`select_account` отправка пользователя в выборщик учетной записи</span><span class="sxs-lookup"><span data-stu-id="ee24b-142">`select_account` to send the user to an account picker</span></span></li><li><span data-ttu-id="ee24b-143">`consent` отправка пользователя в диалоговое окно согласия OAuth</span><span class="sxs-lookup"><span data-stu-id="ee24b-143">`consent` to send the user to a OAuth consent dialog</span></span></li></ul> <span data-ttu-id="ee24b-144">Дополнительные сведения см. в статье [оперативное ](/azure/active-directory/develop/msal-js-prompt-behavior) поведение MSAL.jsстатье.</span><span class="sxs-lookup"><span data-stu-id="ee24b-144">For more prompt information, see the [prompt behavior in MSAL.js](/azure/active-directory/develop/msal-js-prompt-behavior) article.</span></span> <span data-ttu-id="ee24b-145">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ee24b-145">Optional.</span></span>                                                                                                                                                                            |


### <a name="initialize-in-javascript"></a><span data-ttu-id="ee24b-146">Инициализация в JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee24b-146">Initialize in JavaScript</span></span>

<span data-ttu-id="ee24b-147">Вы можете предоставить больше вариантов, инициализируя поставщика в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="ee24b-147">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="ee24b-148">Параметр конструктора можно настроить двумя способами, как описано `MsalProvider` в следующих разделах.</span><span class="sxs-lookup"><span data-stu-id="ee24b-148">You can configure the `MsalProvider` constructor parameter in two ways, as described in the following sections.</span></span>

#### <a name="provide-a-clientid-to-create-a-new-useragentapplication"></a><span data-ttu-id="ee24b-149">Предоставление для `clientId` создания нового `UserAgentApplication`</span><span class="sxs-lookup"><span data-stu-id="ee24b-149">Provide a `clientId` to create a new `UserAgentApplication`</span></span>

<span data-ttu-id="ee24b-150">Этот параметр имеет смысл, Graph набор средств несет ответственность за всю проверку подлинности в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="ee24b-150">This option makes sense when Graph Toolkit is responsible for all authentication in your application.</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string
  options?: Configuration; // msal js Configuration object
  domainHint?: string;
  prompt?: string; // "login", "none", "select_account", "consent"
}
```

#### <a name="pass-an-existing-useragentapplication-in-the-useragentapplication-property"></a><span data-ttu-id="ee24b-151">Передай `UserAgentApplication` существующее `userAgentApplication` в свойстве.</span><span class="sxs-lookup"><span data-stu-id="ee24b-151">Pass an existing `UserAgentApplication` in the `userAgentApplication` property.</span></span>

<span data-ttu-id="ee24b-152">Используйте это, когда ваше приложение использует функции MSAL за пределами возможностей, открытых другими функциями `MsalProvider` Microsoft Graph набор средств.</span><span class="sxs-lookup"><span data-stu-id="ee24b-152">Use this when your app uses MSAL functionality beyond what's exposed by the `MsalProvider` and other Microsoft Graph Toolkit features.</span></span> <span data-ttu-id="ee24b-153">Это особенно уместно, если фреймворк автоматически мгновенно и предоставляет для вас значение a; например, при использовании `UserAgentApplication` [msal-angular](/azure/active-directory/develop/tutorial-v2-angular).</span><span class="sxs-lookup"><span data-stu-id="ee24b-153">This is particularly appropriate if a framework automatically instantiates and exposes a `UserAgentApplication` for you; for example, when using [msal-angular](/azure/active-directory/develop/tutorial-v2-angular).</span></span>

<span data-ttu-id="ee24b-154">При использовании этого параметра необходимо понимать возможности для столкновений.</span><span class="sxs-lookup"><span data-stu-id="ee24b-154">Be sure to understand opportunities for collisions when using this option.</span></span> <span data-ttu-id="ee24b-155">По своей природе существует риск того, что состояние сеанса может измениться, например, путем входов пользователя или согласия на `MsalProvider` дополнительные области.</span><span class="sxs-lookup"><span data-stu-id="ee24b-155">By its very nature, there is a risk that the `MsalProvider` can change the state of a session, for example by having the user sign in or consent to additional scopes.</span></span> <span data-ttu-id="ee24b-156">Убедитесь, что ваше приложение и другие фреймворки реагируют на эти изменения в состоянии, или рассмотрите возможность использования [пользовательского поставщика.](./custom.md)</span><span class="sxs-lookup"><span data-stu-id="ee24b-156">Make sure that your app and other frameworks respond gracefully to these changes in state, or consider using a [custom provider](./custom.md) instead.</span></span>

```ts
interface MsalConfig {
  userAgentApplication: UserAgentApplication;
  scopes?: string[];
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string;
}
```

<span data-ttu-id="ee24b-157">Дополнительные дополнительные MSAL.js и дополнительные возможности, которые можно использовать при инициализации библиотеки MSAL, см. в [документации MSAL.](/azure/active-directory/develop/msal-js-initializing-client-applications)</span><span class="sxs-lookup"><span data-stu-id="ee24b-157">To learn more about MSAL.js and for additional options you can use when initializing the MSAL library, see the [MSAL documentation](/azure/active-directory/develop/msal-js-initializing-client-applications).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="ee24b-158">Создание идентификатора клиента/приложения</span><span class="sxs-lookup"><span data-stu-id="ee24b-158">Creating an app/client ID</span></span>

<span data-ttu-id="ee24b-159">Дополнительные сведения о том, как зарегистрировать приложение и получить клиентский ID, см. в Azure Active Directory [app.](../get-started/add-aad-app-registration.md)</span><span class="sxs-lookup"><span data-stu-id="ee24b-159">For details about how to register an app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>
