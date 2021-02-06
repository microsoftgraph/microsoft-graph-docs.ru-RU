---
title: Тип ресурса authenticationDetail
description: Предоставляет сведения о проверке подлинности для пользователя, такие как сведения о многофакторной проверке подлинности (MFA) и PTA/PHS.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: b888ec232a95c821ab00f6baa16e787cfbc7dd7f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136628"
---
# <a name="authenticationdetail-resource-type"></a><span data-ttu-id="6583f-103">Тип ресурса authenticationDetail</span><span class="sxs-lookup"><span data-stu-id="6583f-103">authenticationDetail resource type</span></span>

<span data-ttu-id="6583f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6583f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6583f-105">Предоставляет сведения о проверке подлинности для пользователя, такие как сведения о многофакторной проверке подлинности (MFA) и PTA/PHS.</span><span class="sxs-lookup"><span data-stu-id="6583f-105">Provides the authentication details for a user sign-in, such as multi-factor authentication (MFA) information and PTA/PHS details.</span></span>

## <a name="properties"></a><span data-ttu-id="6583f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6583f-106">Properties</span></span>

| <span data-ttu-id="6583f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6583f-107">Property</span></span>                       | <span data-ttu-id="6583f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6583f-108">Type</span></span>           | <span data-ttu-id="6583f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6583f-109">Description</span></span>                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6583f-110">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6583f-110">authenticationMethod</span></span>           | <span data-ttu-id="6583f-111">Строка</span><span class="sxs-lookup"><span data-stu-id="6583f-111">String</span></span>         | <span data-ttu-id="6583f-112">Тип метода проверки подлинности, используемого для выполнения этого шага проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6583f-112">The type of authentication method used to perform this step of authentication.</span></span> <span data-ttu-id="6583f-113">Возможные значения: `Password` , , , , `SMS` `Voice` `Authenticator App` `Software OATH token` `Satisfied by token` .</span><span class="sxs-lookup"><span data-stu-id="6583f-113">Possible values: `Password`, `SMS`, `Voice`, `Authenticator App`, `Software OATH token`, `Satisfied by token`.</span></span>                            |
| <span data-ttu-id="6583f-114">authenticationMethodDetail</span><span class="sxs-lookup"><span data-stu-id="6583f-114">authenticationMethodDetail</span></span>     | <span data-ttu-id="6583f-115">Строка</span><span class="sxs-lookup"><span data-stu-id="6583f-115">String</span></span>         | <span data-ttu-id="6583f-116">Сведения о методе проверки подлинности, используемом для выполнения этого шага проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6583f-116">Details about the authentication method used to perform this authentication step.</span></span> <span data-ttu-id="6583f-117">Например, номер телефона (для SMS и голосовой связи), имя устройства (для приложения Authenticator) и источник пароля (например, облако, AD FS, PTA, PHS).</span><span class="sxs-lookup"><span data-stu-id="6583f-117">For example, phone number (for SMS and voice), device name (for Authenticator app), and password source (e.g. cloud, AD FS, PTA, PHS).</span></span> |
| <span data-ttu-id="6583f-118">authenticationStepDateTime</span><span class="sxs-lookup"><span data-stu-id="6583f-118">authenticationStepDateTime</span></span>     | <span data-ttu-id="6583f-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6583f-119">DateTimeOffset</span></span> | <span data-ttu-id="6583f-120">Представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6583f-120">Represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6583f-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6583f-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>                                           |
| <span data-ttu-id="6583f-122">authenticationStepRequirement</span><span class="sxs-lookup"><span data-stu-id="6583f-122">authenticationStepRequirement</span></span>  | <span data-ttu-id="6583f-123">Строка</span><span class="sxs-lookup"><span data-stu-id="6583f-123">String</span></span>         | <span data-ttu-id="6583f-124">Шаг проверки подлинности, который это удовлетворит.</span><span class="sxs-lookup"><span data-stu-id="6583f-124">The step of authentication that this satisfied.</span></span> <span data-ttu-id="6583f-125">Например, основная или многофакторная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="6583f-125">For example, primary authentication, or multi-factor authentication.</span></span>                                                                                                     |
| <span data-ttu-id="6583f-126">authenticationStepResultDetail</span><span class="sxs-lookup"><span data-stu-id="6583f-126">authenticationStepResultDetail</span></span> | <span data-ttu-id="6583f-127">Строка</span><span class="sxs-lookup"><span data-stu-id="6583f-127">String</span></span>         | <span data-ttu-id="6583f-128">Сведения о том, почему шаг был успешным или неудачным.</span><span class="sxs-lookup"><span data-stu-id="6583f-128">Details about why the step succeeded or failed.</span></span> <span data-ttu-id="6583f-129">Например, пользователь заблокирован, введен код мошенничества, не ввод данных с телефона : время и время действия, недостижимый телефон или утверждение в маркере.</span><span class="sxs-lookup"><span data-stu-id="6583f-129">For examples, user is blocked, fraud code entered, no phone input - timed out, phone unreachable, or claim in token.</span></span>                                                     |
| <span data-ttu-id="6583f-130">succeeded</span><span class="sxs-lookup"><span data-stu-id="6583f-130">succeeded</span></span>                      | <span data-ttu-id="6583f-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="6583f-131">Boolean</span></span>        | <span data-ttu-id="6583f-132">Указывает состояние шага проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6583f-132">Indicates the status of the authentication step.</span></span> <span data-ttu-id="6583f-133">Возможные значения: `succeeded` , `failed` .</span><span class="sxs-lookup"><span data-stu-id="6583f-133">Possible values: `succeeded`, `failed`.</span></span>                                                                                                                                 |

## <a name="json-representation"></a><span data-ttu-id="6583f-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6583f-134">JSON representation</span></span>

<span data-ttu-id="6583f-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6583f-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationDetail",
  "baseType": null
}-->

```json
{
  "authenticationMethod": "String",
  "authenticationMethodDetail": "String",
  "authenticationStepDateTime": "String (timestamp)",
  "authenticationStepRequirement": "String",
  "authenticationStepResultDetail": "String",
  "succeeded": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

