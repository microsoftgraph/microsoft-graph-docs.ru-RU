---
title: Поставщик MSAL
description: Поставщик MSAL использует MSAL.js для входа пользователей и получения маркеров для использования с Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c3c921cfa473e2001d2a150096741d2bddf39f10
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288163"
---
# <a name="msal-provider"></a><span data-ttu-id="25bd1-103">Поставщик MSAL</span><span class="sxs-lookup"><span data-stu-id="25bd1-103">MSAL provider</span></span>

<span data-ttu-id="25bd1-104">Поставщик MSAL использует [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) для входа пользователей и получения маркеров для использования с Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="25bd1-104">The MSAL provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with Microsoft Graph.</span></span>

<span data-ttu-id="25bd1-105">Чтобы узнать больше, ознакомьтесь со статьей [поставщики](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="25bd1-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="25bd1-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="25bd1-106">Get started</span></span>

<span data-ttu-id="25bd1-107">Вы можете инициализировать поставщик MSAL в HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="25bd1-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="25bd1-108">Инициализация на HTML-странице</span><span class="sxs-lookup"><span data-stu-id="25bd1-108">Initialize in your HTML page</span></span>

<span data-ttu-id="25bd1-109">Инициализация поставщика MSAL в HTML является самым простым способом создания нового поставщика.</span><span class="sxs-lookup"><span data-stu-id="25bd1-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="25bd1-110">Используйте `mgt-msal-provider` компонент, чтобы задать **идентификатор клиента** и другие свойства.</span><span class="sxs-lookup"><span data-stu-id="25bd1-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="25bd1-111">При этом будет создан новый `UserAgentApplication` экземпляр, который будет использоваться для всех проверок подлинности и получения маркеров.</span><span class="sxs-lookup"><span data-stu-id="25bd1-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""></mgt-msal-provider>
```

| <span data-ttu-id="25bd1-112">Атрибут</span><span class="sxs-lookup"><span data-stu-id="25bd1-112">Attribute</span></span>    | <span data-ttu-id="25bd1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="25bd1-113">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="25bd1-114">Client — ID</span><span class="sxs-lookup"><span data-stu-id="25bd1-114">client-id</span></span>    | <span data-ttu-id="25bd1-115">Идентификатор строкового клиента (см. Создание идентификатора приложения или клиента).</span><span class="sxs-lookup"><span data-stu-id="25bd1-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="25bd1-116">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="25bd1-116">Required.</span></span>                                                                                                                                                                                                           |
| <span data-ttu-id="25bd1-117">Тип входа</span><span class="sxs-lookup"><span data-stu-id="25bd1-117">login-type</span></span>   | <span data-ttu-id="25bd1-118">Перечисление между `redirect` `popup` значением и значением по умолчанию — `redirect` .</span><span class="sxs-lookup"><span data-stu-id="25bd1-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="25bd1-119">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="25bd1-119">Optional.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="25bd1-120">scopes</span><span class="sxs-lookup"><span data-stu-id="25bd1-120">scopes</span></span>       | <span data-ttu-id="25bd1-121">Строки, разделенные запятыми, для областей, которые пользователь должен согласиться на вход в систему.</span><span class="sxs-lookup"><span data-stu-id="25bd1-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="25bd1-122">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="25bd1-122">Optional.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="25bd1-123">авторитет</span><span class="sxs-lookup"><span data-stu-id="25bd1-123">authority</span></span>    | <span data-ttu-id="25bd1-124">Строка Authority — значение по умолчанию — общий центр.</span><span class="sxs-lookup"><span data-stu-id="25bd1-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="25bd1-125">Для приложений с одним клиентом используйте идентификатор клиента или имя клиента.</span><span class="sxs-lookup"><span data-stu-id="25bd1-125">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="25bd1-126">Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]` .</span><span class="sxs-lookup"><span data-stu-id="25bd1-126">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="25bd1-127">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="25bd1-127">Optional.</span></span> |
| <span data-ttu-id="25bd1-128">Redirect — URI</span><span class="sxs-lookup"><span data-stu-id="25bd1-128">redirect-uri</span></span> | <span data-ttu-id="25bd1-129">Строка URI перенаправления — по умолчанию используется текущий URI окна.</span><span class="sxs-lookup"><span data-stu-id="25bd1-129">Redirect URI string - by default the current window URI is used.</span></span> <span data-ttu-id="25bd1-130">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="25bd1-130">Optional.</span></span>                                                                                                                                                                                            |
| <span data-ttu-id="25bd1-131">зависит от</span><span class="sxs-lookup"><span data-stu-id="25bd1-131">depends-on</span></span>   | <span data-ttu-id="25bd1-132">Строка выбора элемента с другим компонентом поставщика более высокого приоритета.</span><span class="sxs-lookup"><span data-stu-id="25bd1-132">Element selector string of another higher priority provider component.</span></span> <span data-ttu-id="25bd1-133">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="25bd1-133">Optional.</span></span>                                                                                                                                                                                      |

### <a name="initialize-in-javascript"></a><span data-ttu-id="25bd1-134">Инициализация в JavaScript</span><span class="sxs-lookup"><span data-stu-id="25bd1-134">Initialize in JavaScript</span></span>

<span data-ttu-id="25bd1-135">Вы можете предоставить дополнительные параметры, инициализируя поставщик в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="25bd1-135">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="25bd1-136">где Мсалконфиг:</span><span class="sxs-lookup"><span data-stu-id="25bd1-136">where MsalConfig is:</span></span>

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

<span data-ttu-id="25bd1-137">Необходимо указать `clientId` (чтобы создать новый `UserAgentApplication` ).</span><span class="sxs-lookup"><span data-stu-id="25bd1-137">You must provide a `clientId` (to create a new `UserAgentApplication`).</span></span>

<span data-ttu-id="25bd1-138">Дополнительные сведения о MSAL.js и дополнительных параметрах, которые можно использовать при инициализации библиотеки MSAL, приведены в [документации по MSAL](/azure/active-directory/develop/msal-js-initializing-client-applications).</span><span class="sxs-lookup"><span data-stu-id="25bd1-138">To learn more about MSAL.js and for additional options you can use when initializing the MSAL library, see the [MSAL documentation](/azure/active-directory/develop/msal-js-initializing-client-applications).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="25bd1-139">Создание идентификатора приложения или клиента</span><span class="sxs-lookup"><span data-stu-id="25bd1-139">Creating an app/client ID</span></span>

<span data-ttu-id="25bd1-140">Сведения о том, как зарегистрировать приложение и получить идентификатор клиента, можно найти в разделе [Регистрация краткого руководства по работе с приложением](/azure/active-directory/develop/quickstart-register-app).</span><span class="sxs-lookup"><span data-stu-id="25bd1-140">For details about how to register an app and get a client ID, see the [Register an app quick start](/azure/active-directory/develop/quickstart-register-app).</span></span>

><span data-ttu-id="25bd1-141">**Примечание:** MSAL поддерживает только неявный поток для OAuth.</span><span class="sxs-lookup"><span data-stu-id="25bd1-141">**Note:** MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="25bd1-142">Не забудьте включить неявный поток в приложении на портале Azure (по умолчанию он не включен).</span><span class="sxs-lookup"><span data-stu-id="25bd1-142">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="25bd1-143">В разделе **Проверка подлинности**найдите раздел **неявный предоставление** и установите флажки для **маркеров доступа** и **маркеров ID**.</span><span class="sxs-lookup"><span data-stu-id="25bd1-143">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> <span data-ttu-id="25bd1-144">Чтобы использовать общий орган, задайте **учетную запись в любом организационном каталоге**.</span><span class="sxs-lookup"><span data-stu-id="25bd1-144">To use the common authority, set **Account in any organizational directory**.</span></span> <span data-ttu-id="25bd1-145">Чтобы использовать определенный клиент, задайте `authority` во время инициализации.</span><span class="sxs-lookup"><span data-stu-id="25bd1-145">To use a specific tenant, set the `authority` during initialization.</span></span>