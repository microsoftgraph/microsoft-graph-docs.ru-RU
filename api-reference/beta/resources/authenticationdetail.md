---
title: Тип ресурса Аусентикатиондетаил
description: Предоставляет сведения о проверке подлинности для входа пользователя, например сведения о многофакторной проверке подлинности (MFA) и сведения о ПТА/ФС.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 14f2121aabaae591187d3033903e569b482b8727
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521245"
---
# <a name="authenticationdetail-resource-type"></a><span data-ttu-id="cda86-103">Тип ресурса Аусентикатиондетаил</span><span class="sxs-lookup"><span data-stu-id="cda86-103">authenticationDetail resource type</span></span>

<span data-ttu-id="cda86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cda86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cda86-105">Предоставляет сведения о проверке подлинности для входа пользователя, например сведения о многофакторной проверке подлинности (MFA) и сведения о ПТА/ФС.</span><span class="sxs-lookup"><span data-stu-id="cda86-105">Provides the authentication details for a user sign-in, such as multi-factor authentication (MFA) information and PTA/PHS details.</span></span>

## <a name="properties"></a><span data-ttu-id="cda86-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cda86-106">Properties</span></span>

| <span data-ttu-id="cda86-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cda86-107">Property</span></span>                       | <span data-ttu-id="cda86-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cda86-108">Type</span></span>           | <span data-ttu-id="cda86-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cda86-109">Description</span></span>                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cda86-110">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="cda86-110">authenticationMethod</span></span>           | <span data-ttu-id="cda86-111">String</span><span class="sxs-lookup"><span data-stu-id="cda86-111">String</span></span>         | <span data-ttu-id="cda86-112">Тип метода проверки подлинности, используемый для выполнения этого этапа проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="cda86-112">The type of authentication method used to perform this step of authentication.</span></span> <span data-ttu-id="cda86-113">Возможные значения: `Password` , `SMS` , `Voice` , `Authenticator App` , `Software OATH token` , `Satisfied by token` .</span><span class="sxs-lookup"><span data-stu-id="cda86-113">Possible values: `Password`, `SMS`, `Voice`, `Authenticator App`, `Software OATH token`, `Satisfied by token`.</span></span>                            |
| <span data-ttu-id="cda86-114">аусентикатионмесоддетаил</span><span class="sxs-lookup"><span data-stu-id="cda86-114">authenticationMethodDetail</span></span>     | <span data-ttu-id="cda86-115">String</span><span class="sxs-lookup"><span data-stu-id="cda86-115">String</span></span>         | <span data-ttu-id="cda86-116">Сведения о методе проверки подлинности, используемом для выполнения этой процедуры проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="cda86-116">Details about the authentication method used to perform this authentication step.</span></span> <span data-ttu-id="cda86-117">Например, номер телефона (для SMS и голосовой связи), имя устройства (для приложения проверки подлинности) и источник пароля (Cloud, AD FS, ПТА, ФС).</span><span class="sxs-lookup"><span data-stu-id="cda86-117">For example, phone number (for SMS and voice), device name (for Authenticator app), and password source (e.g. cloud, AD FS, PTA, PHS).</span></span> |
| <span data-ttu-id="cda86-118">аусентикатионстепдатетиме</span><span class="sxs-lookup"><span data-stu-id="cda86-118">authenticationStepDateTime</span></span>     | <span data-ttu-id="cda86-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cda86-119">DateTimeOffset</span></span> | <span data-ttu-id="cda86-120">Представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="cda86-120">Represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cda86-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cda86-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>                                           |
| <span data-ttu-id="cda86-122">аусентикатионстепрекуиремент</span><span class="sxs-lookup"><span data-stu-id="cda86-122">authenticationStepRequirement</span></span>  | <span data-ttu-id="cda86-123">String</span><span class="sxs-lookup"><span data-stu-id="cda86-123">String</span></span>         | <span data-ttu-id="cda86-124">Шаг проверки подлинности, который удовлетворен.</span><span class="sxs-lookup"><span data-stu-id="cda86-124">The step of authentication that this satisfied.</span></span> <span data-ttu-id="cda86-125">Например, Первичная проверка подлинности или многофакторная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="cda86-125">For example, primary authentication, or multi-factor authentication.</span></span>                                                                                                     |
| <span data-ttu-id="cda86-126">аусентикатионстепресултдетаил</span><span class="sxs-lookup"><span data-stu-id="cda86-126">authenticationStepResultDetail</span></span> | <span data-ttu-id="cda86-127">String</span><span class="sxs-lookup"><span data-stu-id="cda86-127">String</span></span>         | <span data-ttu-id="cda86-128">Сведения о причине успешного или неудачного завершения этапа.</span><span class="sxs-lookup"><span data-stu-id="cda86-128">Details about why the step succeeded or failed.</span></span> <span data-ttu-id="cda86-129">Например, пользователь блокируется, заменяется мошеннический код, не используется ввод с истекшим сроком ожидания, Телефон недоступен или утвержден в маркере.</span><span class="sxs-lookup"><span data-stu-id="cda86-129">For examples, user is blocked, fraud code entered, no phone input - timed out, phone unreachable, or claim in token.</span></span>                                                     |
| <span data-ttu-id="cda86-130">закончил</span><span class="sxs-lookup"><span data-stu-id="cda86-130">succeeded</span></span>                      | <span data-ttu-id="cda86-131">Логический</span><span class="sxs-lookup"><span data-stu-id="cda86-131">Boolean</span></span>        | <span data-ttu-id="cda86-132">Указывает состояние этапа проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="cda86-132">Indicates the status of the authentication step.</span></span> <span data-ttu-id="cda86-133">Возможные значения: `succeeded` , `failed` .</span><span class="sxs-lookup"><span data-stu-id="cda86-133">Possible values: `succeeded`, `failed`.</span></span>                                                                                                                                 |

## <a name="json-representation"></a><span data-ttu-id="cda86-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cda86-134">JSON representation</span></span>

<span data-ttu-id="cda86-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cda86-135">The following is a JSON representation of the resource.</span></span>

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

