---
title: Поставщик MSAL
description: Поставщик MSAL использует MSAL. js для входа пользователей и получения маркеров для использования с Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: aa3eecb6bd9f2adae7ff689f30ab69539e1d27f1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955780"
---
# <a name="msal-provider"></a><span data-ttu-id="4a474-103">Поставщик MSAL</span><span class="sxs-lookup"><span data-stu-id="4a474-103">MSAL provider</span></span>

<span data-ttu-id="4a474-104">Поставщик MSAL использует [MSAL. js](https://github.com/AzureAD/microsoft-authentication-library-for-js) для входа пользователей и получения маркеров для использования с Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4a474-104">The MSAL Provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with the Microsoft Graph.</span></span>

<span data-ttu-id="4a474-105">Чтобы узнать больше, ознакомьтесь со статьей [поставщики](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="4a474-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="4a474-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="4a474-106">Get started</span></span>

<span data-ttu-id="4a474-107">Вы можете инициализировать поставщик MSAL в HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="4a474-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="4a474-108">Инициализация на HTML-странице</span><span class="sxs-lookup"><span data-stu-id="4a474-108">Initialize in your HTML page</span></span>

<span data-ttu-id="4a474-109">Инициализация поставщика MSAL в HTML является самым простым способом создания нового поставщика.</span><span class="sxs-lookup"><span data-stu-id="4a474-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="4a474-110">Используйте `mgt-msal-provider` компонент, чтобы задать **идентификатор клиента** и другие свойства.</span><span class="sxs-lookup"><span data-stu-id="4a474-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="4a474-111">При этом будет создан новый `UserAgentApplication` экземпляр, который будет использоваться для всех проверок подлинности и получения маркеров.</span><span class="sxs-lookup"><span data-stu-id="4a474-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   authority=""></mgt-msal-provider>
```

| <span data-ttu-id="4a474-112">Атрибут</span><span class="sxs-lookup"><span data-stu-id="4a474-112">Attribute</span></span> | <span data-ttu-id="4a474-113">Описание</span><span class="sxs-lookup"><span data-stu-id="4a474-113">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="4a474-114">Client — ID</span><span class="sxs-lookup"><span data-stu-id="4a474-114">client-id</span></span>   | <span data-ttu-id="4a474-115">Идентификатор строкового клиента (см. Создание идентификатора приложения или клиента).</span><span class="sxs-lookup"><span data-stu-id="4a474-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="4a474-116">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="4a474-116">Required.</span></span>|
| <span data-ttu-id="4a474-117">Тип входа</span><span class="sxs-lookup"><span data-stu-id="4a474-117">login-type</span></span>  | <span data-ttu-id="4a474-118">`redirect` Перечисление `popup` между значением и значением `redirect`по умолчанию —.</span><span class="sxs-lookup"><span data-stu-id="4a474-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="4a474-119">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="4a474-119">Optional.</span></span> |
| <span data-ttu-id="4a474-120">scopes</span><span class="sxs-lookup"><span data-stu-id="4a474-120">scopes</span></span>  | <span data-ttu-id="4a474-121">Строки, разделенные запятыми, для областей, которые пользователь должен согласиться на вход в систему.</span><span class="sxs-lookup"><span data-stu-id="4a474-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="4a474-122">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="4a474-122">Optional.</span></span>|
| <span data-ttu-id="4a474-123">авторитет</span><span class="sxs-lookup"><span data-stu-id="4a474-123">authority</span></span>  | <span data-ttu-id="4a474-124">Строка Authority — значение по умолчанию — общий центр.</span><span class="sxs-lookup"><span data-stu-id="4a474-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="4a474-125">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="4a474-125">Optional.</span></span>|
| <span data-ttu-id="4a474-126">зависит от</span><span class="sxs-lookup"><span data-stu-id="4a474-126">depends-on</span></span> | <span data-ttu-id="4a474-127">Строка выбора элемента с другим компонентом поставщика более высокого приоритета.</span><span class="sxs-lookup"><span data-stu-id="4a474-127">Element selector string of another higher priority provider component.</span></span> <span data-ttu-id="4a474-128">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="4a474-128">Optional.</span></span> |

### <a name="initialize-in-javascript"></a><span data-ttu-id="4a474-129">Инициализация в JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a474-129">Initialize in JavaScript</span></span>

<span data-ttu-id="4a474-130">Вы можете предоставить дополнительные параметры, инициализируя поставщик в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="4a474-130">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="4a474-131">где Мсалконфиг:</span><span class="sxs-lookup"><span data-stu-id="4a474-131">where MsalConfig is:</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  loginType?: LoginType;
  options?: Configuration; // msal js Configuration object
}
```

<span data-ttu-id="4a474-132">Необходимо указать `clientId` (чтобы создать новый `UserAgentApplication`).</span><span class="sxs-lookup"><span data-stu-id="4a474-132">You must provide a `clientId` (to create a new `UserAgentApplication`).</span></span>

<span data-ttu-id="4a474-133">Дополнительные сведения см. в [документации по MSAL](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics).</span><span class="sxs-lookup"><span data-stu-id="4a474-133">To learn more, see the [MSAL documentation](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="4a474-134">Создание идентификатора приложения или клиента</span><span class="sxs-lookup"><span data-stu-id="4a474-134">Creating an app/client ID</span></span>

<span data-ttu-id="4a474-135">Сведения о том, как зарегистрировать приложение и получить идентификатор клиента, можно найти в статье [Регистрация краткого руководства](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app)по использованию приложения.</span><span class="sxs-lookup"><span data-stu-id="4a474-135">For details about how to register an app and get a client ID, see [Register an app quick start](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app).</span></span>

><span data-ttu-id="4a474-136">**Примечание:** MSAL поддерживает только неявный поток для OAuth.</span><span class="sxs-lookup"><span data-stu-id="4a474-136">**Note:** MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="4a474-137">Не забудьте включить неявный поток в приложении на портале Azure (по умолчанию он не включен).</span><span class="sxs-lookup"><span data-stu-id="4a474-137">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="4a474-138">В разделе **Проверка подлинности**найдите раздел **неявный предоставление** и установите флажки для **маркеров доступа** и **маркеров ID**.</span><span class="sxs-lookup"><span data-stu-id="4a474-138">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span>
