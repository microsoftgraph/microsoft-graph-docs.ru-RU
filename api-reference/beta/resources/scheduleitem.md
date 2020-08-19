---
title: Тип ресурса Счедулеитем
description: Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию. Этот элемент также применяется к ресурсу.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: harini84
ms.openlocfilehash: b4bbf2586543b4f731c136eaffbc955741191db6
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812799"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="5d87f-104">Тип ресурса Счедулеитем</span><span class="sxs-lookup"><span data-stu-id="5d87f-104">scheduleItem resource type</span></span>

<span data-ttu-id="5d87f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d87f-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d87f-106">Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5d87f-106">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="5d87f-107">Этот элемент также применяется к ресурсу (комнате или оборудованию).</span><span class="sxs-lookup"><span data-stu-id="5d87f-107">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="5d87f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d87f-108">Properties</span></span>
| <span data-ttu-id="5d87f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d87f-109">Property</span></span>     | <span data-ttu-id="5d87f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5d87f-110">Type</span></span>   |<span data-ttu-id="5d87f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5d87f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d87f-112">end</span><span class="sxs-lookup"><span data-stu-id="5d87f-112">end</span></span> |[<span data-ttu-id="5d87f-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5d87f-113">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="5d87f-114">Дата, время и часовой пояс, в течение которого заканчивается соответствующее событие.</span><span class="sxs-lookup"><span data-stu-id="5d87f-114">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="5d87f-115">Частный</span><span class="sxs-lookup"><span data-stu-id="5d87f-115">isPrivate</span></span> |<span data-ttu-id="5d87f-116">Логический</span><span class="sxs-lookup"><span data-stu-id="5d87f-116">Boolean</span></span> |<span data-ttu-id="5d87f-117">Чувствительность соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="5d87f-117">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="5d87f-118">Значение true, если событие помечено `private` , в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="5d87f-118">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="5d87f-119">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="5d87f-119">Optional.</span></span> |
|<span data-ttu-id="5d87f-120">location</span><span class="sxs-lookup"><span data-stu-id="5d87f-120">location</span></span> |<span data-ttu-id="5d87f-121">String</span><span class="sxs-lookup"><span data-stu-id="5d87f-121">String</span></span> | <span data-ttu-id="5d87f-122">Расположение, в котором находится соответствующее событие.</span><span class="sxs-lookup"><span data-stu-id="5d87f-122">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="5d87f-123">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="5d87f-123">Optional.</span></span>|
|<span data-ttu-id="5d87f-124">начать</span><span class="sxs-lookup"><span data-stu-id="5d87f-124">start</span></span> |[<span data-ttu-id="5d87f-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5d87f-125">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="5d87f-126">Дата, время и часовой пояс, в котором начинается соответствующее событие.</span><span class="sxs-lookup"><span data-stu-id="5d87f-126">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="5d87f-127">status</span><span class="sxs-lookup"><span data-stu-id="5d87f-127">status</span></span> |<span data-ttu-id="5d87f-128">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="5d87f-128">freeBusyStatus</span></span> | <span data-ttu-id="5d87f-129">Состояние доступности пользователя или ресурса во время соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="5d87f-129">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="5d87f-130">Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="5d87f-130">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="5d87f-131">subject</span><span class="sxs-lookup"><span data-stu-id="5d87f-131">subject</span></span> |<span data-ttu-id="5d87f-132">String</span><span class="sxs-lookup"><span data-stu-id="5d87f-132">String</span></span> | <span data-ttu-id="5d87f-133">Строка темы соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="5d87f-133">The corresponding event's subject line.</span></span> <span data-ttu-id="5d87f-134">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="5d87f-134">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5d87f-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5d87f-135">JSON representation</span></span>

<span data-ttu-id="5d87f-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d87f-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isPrivate",
    "location",
    "subject"
  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
