---
title: Поставщик MSAL
description: Поставщик MSAL использует MSAL. js для входа пользователей и получения маркеров для использования с Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b66fd9a640c6baa84767e1ab08821b80384a5464
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243077"
---
# <a name="msal-provider"></a><span data-ttu-id="b9069-103">Поставщик MSAL</span><span class="sxs-lookup"><span data-stu-id="b9069-103">MSAL provider</span></span>

<span data-ttu-id="b9069-104">Поставщик MSAL использует [MSAL. js](https://github.com/AzureAD/microsoft-authentication-library-for-js) для входа пользователей и получения маркеров для использования с Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b9069-104">The MSAL Provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with the Microsoft Graph.</span></span>

<span data-ttu-id="b9069-105">Чтобы узнать больше, ознакомьтесь со статьей [поставщики](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="b9069-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="b9069-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="b9069-106">Get started</span></span>

<span data-ttu-id="b9069-107">Вы можете инициализировать поставщик MSAL в HTML или JavaScript.</span><span class="sxs-lookup"><span data-stu-id="b9069-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="b9069-108">Инициализация на HTML-странице</span><span class="sxs-lookup"><span data-stu-id="b9069-108">Initialize in your HTML page</span></span>

<span data-ttu-id="b9069-109">Инициализация поставщика MSAL в HTML является самым простым способом создания нового поставщика.</span><span class="sxs-lookup"><span data-stu-id="b9069-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="b9069-110">Используйте `mgt-msal-provider` компонент, чтобы задать **идентификатор клиента** и другие свойства.</span><span class="sxs-lookup"><span data-stu-id="b9069-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="b9069-111">При этом будет создан новый `UserAgentApplication` экземпляр, который будет использоваться для всех проверок подлинности и получения маркеров.</span><span class="sxs-lookup"><span data-stu-id="b9069-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   authority=""></mgt-msal-provider>
```

><span data-ttu-id="b9069-112">**Примечание:** `login-type` и `authority` являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="b9069-112">**Note:** `login-type` and `authority` are optional.</span></span>

### <a name="initialize-in-javascript"></a><span data-ttu-id="b9069-113">Инициализация в JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9069-113">Initialize in JavaScript</span></span>

<span data-ttu-id="b9069-114">Вы можете предоставить дополнительные параметры, инициализируя поставщик в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="b9069-114">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="b9069-115">где Мсалконфиг:</span><span class="sxs-lookup"><span data-stu-id="b9069-115">where MsalConfig is:</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  loginType?: LoginType;
  options?: Configuration; // msal js Configuration object
}
```

<span data-ttu-id="b9069-116">Необходимо указать `clientId` (чтобы создать новый `UserAgentApplication`).</span><span class="sxs-lookup"><span data-stu-id="b9069-116">You must provide a `clientId` (to create a new `UserAgentApplication`).</span></span>

<span data-ttu-id="b9069-117">Дополнительные сведения см. в [документации по MSAL](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics).</span><span class="sxs-lookup"><span data-stu-id="b9069-117">To learn more, see the [MSAL documentation](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="b9069-118">Создание идентификатора приложения или клиента</span><span class="sxs-lookup"><span data-stu-id="b9069-118">Creating an app/client ID</span></span>

<span data-ttu-id="b9069-119">Сведения о том, как зарегистрировать приложение и получить идентификатор клиента, можно найти в разделе [Регистрация краткого руководства по работе с приложением](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app).</span><span class="sxs-lookup"><span data-stu-id="b9069-119">For details about how to register an app and get a client ID, see the [Register an app quick start](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app).</span></span>

><span data-ttu-id="b9069-120">**Примечание:** MSAL поддерживает только неявный поток для OAuth.</span><span class="sxs-lookup"><span data-stu-id="b9069-120">**Note:** MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="b9069-121">Не забудьте включить неявный поток в приложении на портале Azure (по умолчанию он не включен).</span><span class="sxs-lookup"><span data-stu-id="b9069-121">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="b9069-122">В **разделе Проверка**подлинности найдите раздел неявный **предоставление** и установите флажки для **маркеров доступа** и **маркеров ID**.</span><span class="sxs-lookup"><span data-stu-id="b9069-122">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span>
