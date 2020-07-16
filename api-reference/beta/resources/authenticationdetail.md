---
title: Тип ресурса Аусентикатиондетаил
description: Предоставляет сведения о проверке подлинности для входа пользователя, например сведения о многофакторной проверке подлинности (MFA) и сведения о ПТА/ФС.
localization_priority: Normal
author: kholtz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cdfd2abff4d947f7b51a6be0fa8bb81c1413f9c1
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845297"
---
# <a name="authenticationdetail-resource-type"></a><span data-ttu-id="504bc-103">Тип ресурса Аусентикатиондетаил</span><span class="sxs-lookup"><span data-stu-id="504bc-103">authenticationDetail resource type</span></span>

<span data-ttu-id="504bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="504bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="504bc-105">Предоставляет сведения о проверке подлинности для входа пользователя, например сведения о многофакторной проверке подлинности (MFA) и сведения о ПТА/ФС.</span><span class="sxs-lookup"><span data-stu-id="504bc-105">Provides the authentication details for a user sign-in, such as multi-factor authentication (MFA) information and PTA/PHS details.</span></span>

## <a name="properties"></a><span data-ttu-id="504bc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="504bc-106">Properties</span></span>

| <span data-ttu-id="504bc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="504bc-107">Property</span></span>                       | <span data-ttu-id="504bc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="504bc-108">Type</span></span>           | <span data-ttu-id="504bc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="504bc-109">Description</span></span>                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="504bc-110">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="504bc-110">authenticationMethod</span></span>           | <span data-ttu-id="504bc-111">String</span><span class="sxs-lookup"><span data-stu-id="504bc-111">String</span></span>         | <span data-ttu-id="504bc-112">Тип метода проверки подлинности, используемый для выполнения этого этапа проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="504bc-112">The type of authentication method used to perform this step of authentication.</span></span> <span data-ttu-id="504bc-113">Возможные значения: `Password` , `SMS` , `Voice` , `Authenticator App` , `Software OATH token` , `Satisfied by token` .</span><span class="sxs-lookup"><span data-stu-id="504bc-113">Possible values: `Password`, `SMS`, `Voice`, `Authenticator App`, `Software OATH token`, `Satisfied by token`.</span></span>                            |
| <span data-ttu-id="504bc-114">аусентикатионмесоддетаил</span><span class="sxs-lookup"><span data-stu-id="504bc-114">authenticationMethodDetail</span></span>     | <span data-ttu-id="504bc-115">String</span><span class="sxs-lookup"><span data-stu-id="504bc-115">String</span></span>         | <span data-ttu-id="504bc-116">Сведения о методе проверки подлинности, используемом для выполнения этой процедуры проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="504bc-116">Details about the authentication method used to perform this authentication step.</span></span> <span data-ttu-id="504bc-117">Например, номер телефона (для SMS и голосовой связи), имя устройства (для приложения проверки подлинности) и источник пароля (Cloud, AD FS, ПТА, ФС).</span><span class="sxs-lookup"><span data-stu-id="504bc-117">For example, phone number (for SMS and voice), device name (for Authenticator app), and password source (e.g. cloud, AD FS, PTA, PHS).</span></span> |
| <span data-ttu-id="504bc-118">аусентикатионстепдатетиме</span><span class="sxs-lookup"><span data-stu-id="504bc-118">authenticationStepDateTime</span></span>     | <span data-ttu-id="504bc-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="504bc-119">DateTimeOffset</span></span> | <span data-ttu-id="504bc-120">Представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="504bc-120">Represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="504bc-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="504bc-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>                                           |
| <span data-ttu-id="504bc-122">аусентикатионстепрекуиремент</span><span class="sxs-lookup"><span data-stu-id="504bc-122">authenticationStepRequirement</span></span>  | <span data-ttu-id="504bc-123">String</span><span class="sxs-lookup"><span data-stu-id="504bc-123">String</span></span>         | <span data-ttu-id="504bc-124">Шаг проверки подлинности, который удовлетворен.</span><span class="sxs-lookup"><span data-stu-id="504bc-124">The step of authentication that this satisfied.</span></span> <span data-ttu-id="504bc-125">Например, Первичная проверка подлинности или многофакторная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="504bc-125">For example, primary authentication, or multi-factor authentication.</span></span>                                                                                                     |
| <span data-ttu-id="504bc-126">аусентикатионстепресултдетаил</span><span class="sxs-lookup"><span data-stu-id="504bc-126">authenticationStepResultDetail</span></span> | <span data-ttu-id="504bc-127">String</span><span class="sxs-lookup"><span data-stu-id="504bc-127">String</span></span>         | <span data-ttu-id="504bc-128">Сведения о причине успешного или неудачного завершения этапа.</span><span class="sxs-lookup"><span data-stu-id="504bc-128">Details about why the step succeeded or failed.</span></span> <span data-ttu-id="504bc-129">Например, пользователь блокируется, заменяется мошеннический код, не используется ввод с истекшим сроком ожидания, Телефон недоступен или утвержден в маркере.</span><span class="sxs-lookup"><span data-stu-id="504bc-129">For examples, user is blocked, fraud code entered, no phone input - timed out, phone unreachable, or claim in token.</span></span>                                                     |
| <span data-ttu-id="504bc-130">закончил</span><span class="sxs-lookup"><span data-stu-id="504bc-130">succeeded</span></span>                      | <span data-ttu-id="504bc-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="504bc-131">Boolean</span></span>        | <span data-ttu-id="504bc-132">Указывает состояние этапа проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="504bc-132">Indicates the status of the authentication step.</span></span> <span data-ttu-id="504bc-133">Возможные значения: `succeeded` , `failed` .</span><span class="sxs-lookup"><span data-stu-id="504bc-133">Possible values: `succeeded`, `failed`.</span></span>                                                                                                                                 |

## <a name="json-representation"></a><span data-ttu-id="504bc-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="504bc-134">JSON representation</span></span>

<span data-ttu-id="504bc-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="504bc-135">The following is a JSON representation of the resource.</span></span>

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