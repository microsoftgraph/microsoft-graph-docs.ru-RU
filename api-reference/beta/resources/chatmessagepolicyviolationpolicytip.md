---
title: Тип ресурса Чатмессажеполицивиолатионполицитип
description: Представляет свойства подсказки политики для объекта Чатмессажеполицивиолатион. Подсказки политики предоставляют отправителю сведения о нарушении политики.
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7a12afbd3ffb8eac75eb89b5d2bb5095fbd2ae98
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082104"
---
# <a name="chatmessagepolicytip-resource-type"></a><span data-ttu-id="33909-104">Тип ресурса Чатмессажеполицитип</span><span class="sxs-lookup"><span data-stu-id="33909-104">chatMessagePolicyTip resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33909-105">Представляет свойства подсказки политики для объекта [чатмессажеполицивиолатион](chatmessagepolicyviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="33909-105">Represents the properties of a policy tip on a [chatMessagePolicyViolation](chatmessagepolicyviolation.md) object.</span></span> <span data-ttu-id="33909-106">Подсказки политики предоставляют отправителю сведения о нарушении политики.</span><span class="sxs-lookup"><span data-stu-id="33909-106">Policy tips provide the sender with information about the policy violation.</span></span>
<span data-ttu-id="33909-107">Подсказка политики обычно задается с помощью приложения защиты от потери данных (DLP), которое отслеживает сообщения, содержащие данные, которые не предполагается отправлять пользователям.</span><span class="sxs-lookup"><span data-stu-id="33909-107">Policy tips are typically set by a data loss prevention (DLP) app which watches for messages that contain data that users aren't supposed to send.</span></span>

## <a name="properties"></a><span data-ttu-id="33909-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="33909-108">Properties</span></span>

| <span data-ttu-id="33909-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="33909-109">Property</span></span>   | <span data-ttu-id="33909-110">Тип</span><span class="sxs-lookup"><span data-stu-id="33909-110">Type</span></span> |<span data-ttu-id="33909-111">Описание</span><span class="sxs-lookup"><span data-stu-id="33909-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33909-112">комплианцеурл</span><span class="sxs-lookup"><span data-stu-id="33909-112">complianceUrl</span></span>|<span data-ttu-id="33909-113">string</span><span class="sxs-lookup"><span data-stu-id="33909-113">string</span></span>|<span data-ttu-id="33909-114">URL-адрес, который пользователь может посетить для чтения сведений о политиках защиты от потери данных в Организации.</span><span class="sxs-lookup"><span data-stu-id="33909-114">The URL a user can visit to read about the data loss prevention policies for the organization.</span></span> <span data-ttu-id="33909-115">(IE, политики о том, что пользователи не должны говорить в беседах)</span><span class="sxs-lookup"><span data-stu-id="33909-115">(ie, policies about what users shouldn't say in chats)</span></span>|
|<span data-ttu-id="33909-116">женералтекст</span><span class="sxs-lookup"><span data-stu-id="33909-116">generalText</span></span>|<span data-ttu-id="33909-117">string</span><span class="sxs-lookup"><span data-stu-id="33909-117">string</span></span>|<span data-ttu-id="33909-118">Пояснительный текст, отображаемый отправителю сообщения.</span><span class="sxs-lookup"><span data-stu-id="33909-118">Explanatory text shown to the sender of the message.</span></span>|
|<span data-ttu-id="33909-119">матчедкондитиондескриптионс</span><span class="sxs-lookup"><span data-stu-id="33909-119">matchedConditionDescriptions</span></span>|<span data-ttu-id="33909-120">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="33909-120">string collection</span></span>|<span data-ttu-id="33909-121">Список ненужных данных в сообщении, обнаруженном приложением защиты от потери данных.</span><span class="sxs-lookup"><span data-stu-id="33909-121">The list of improper data in the message that was detected by the data loss prevention app.</span></span> <span data-ttu-id="33909-122">Каждое приложение DLP определяет собственные условия, например "номер кредитной карты" и "номер социального страхования".</span><span class="sxs-lookup"><span data-stu-id="33909-122">Each DLP app defines its own conditions, examples include "Credit Card Number" and "Social Security Number".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33909-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="33909-123">JSON representation</span></span>

<span data-ttu-id="33909-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33909-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "generalText"
  ],
  "@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip"
}-->
```json
{
  "complianceUrl": "string",
  "generalText": "string",
  "matchedConditionDescriptions": ["string 1", "string 2"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "policy violation policy tip resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
