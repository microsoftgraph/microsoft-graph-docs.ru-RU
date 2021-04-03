---
title: тип ресурса chatMessagePolicyViolationPolicyTip
description: Представляет свойства подсказки политики на объекте chatMessagePolicyViolation. Советы по политике предоставляют отправительу сведения о нарушении политики.
author: RamjotSingh
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c315dbcb37b11e7ed5771544f511c5cf07cc89a8
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582251"
---
# <a name="chatmessagepolicytip-resource-type"></a><span data-ttu-id="e4a7d-104">тип ресурса chatMessagePolicyTip</span><span class="sxs-lookup"><span data-stu-id="e4a7d-104">chatMessagePolicyTip resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4a7d-105">Представляет свойства подсказки политики на [объекте chatMessagePolicyViolation.](chatmessagepolicyviolation.md)</span><span class="sxs-lookup"><span data-stu-id="e4a7d-105">Represents the properties of a policy tip on a [chatMessagePolicyViolation](chatmessagepolicyviolation.md) object.</span></span> <span data-ttu-id="e4a7d-106">Советы по политике предоставляют отправительу сведения о нарушении политики.</span><span class="sxs-lookup"><span data-stu-id="e4a7d-106">Policy tips provide the sender with information about the policy violation.</span></span>
<span data-ttu-id="e4a7d-107">Советы по политике обычно устанавливаются приложением по предотвращению потери данных (DLP), которое следит за сообщениями, которые содержат данные, которые не должны отправлять пользователи.</span><span class="sxs-lookup"><span data-stu-id="e4a7d-107">Policy tips are typically set by a data loss prevention (DLP) app which watches for messages that contain data that users aren't supposed to send.</span></span>

## <a name="properties"></a><span data-ttu-id="e4a7d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4a7d-108">Properties</span></span>

| <span data-ttu-id="e4a7d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4a7d-109">Property</span></span>   | <span data-ttu-id="e4a7d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e4a7d-110">Type</span></span> |<span data-ttu-id="e4a7d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e4a7d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4a7d-112">complianceUrl</span><span class="sxs-lookup"><span data-stu-id="e4a7d-112">complianceUrl</span></span>|<span data-ttu-id="e4a7d-113">string</span><span class="sxs-lookup"><span data-stu-id="e4a7d-113">string</span></span>|<span data-ttu-id="e4a7d-114">URL-адрес, который пользователь может посетить, чтобы прочитать о политиках предотвращения потери данных для организации.</span><span class="sxs-lookup"><span data-stu-id="e4a7d-114">The URL a user can visit to read about the data loss prevention policies for the organization.</span></span> <span data-ttu-id="e4a7d-115">(т. е. политики о том, что пользователи не должны говорить в чатах)</span><span class="sxs-lookup"><span data-stu-id="e4a7d-115">(ie, policies about what users shouldn't say in chats)</span></span>|
|<span data-ttu-id="e4a7d-116">generalText</span><span class="sxs-lookup"><span data-stu-id="e4a7d-116">generalText</span></span>|<span data-ttu-id="e4a7d-117">string</span><span class="sxs-lookup"><span data-stu-id="e4a7d-117">string</span></span>|<span data-ttu-id="e4a7d-118">Пояснительный текст, показанный отправителю сообщения.</span><span class="sxs-lookup"><span data-stu-id="e4a7d-118">Explanatory text shown to the sender of the message.</span></span>|
|<span data-ttu-id="e4a7d-119">matchedConditionDescriptions</span><span class="sxs-lookup"><span data-stu-id="e4a7d-119">matchedConditionDescriptions</span></span>|<span data-ttu-id="e4a7d-120">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e4a7d-120">string collection</span></span>|<span data-ttu-id="e4a7d-121">Список неправильных данных в сообщении, обнаруженном приложением для предотвращения потери данных.</span><span class="sxs-lookup"><span data-stu-id="e4a7d-121">The list of improper data in the message that was detected by the data loss prevention app.</span></span> <span data-ttu-id="e4a7d-122">Каждое приложение DLP определяет свои условия, примеры включают "Номер кредитной карты" и "Номер социального обеспечения".</span><span class="sxs-lookup"><span data-stu-id="e4a7d-122">Each DLP app defines its own conditions, examples include "Credit Card Number" and "Social Security Number".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4a7d-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4a7d-123">JSON representation</span></span>

<span data-ttu-id="e4a7d-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4a7d-124">The following is a JSON representation of the resource.</span></span>

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
