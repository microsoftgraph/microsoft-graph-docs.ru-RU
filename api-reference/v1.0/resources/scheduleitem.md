---
title: Тип ресурса Счедулеитем
description: Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию. Этот элемент также применяется к ресурсу (комнате или оборудованию).
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fb544041948d5e46c1ae8c3f6f887f595ddb82e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034636"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="cef32-104">Тип ресурса Счедулеитем</span><span class="sxs-lookup"><span data-stu-id="cef32-104">scheduleItem resource type</span></span>

<span data-ttu-id="cef32-105">Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cef32-105">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="cef32-106">Этот элемент также применяется к ресурсу (комнате или оборудованию).</span><span class="sxs-lookup"><span data-stu-id="cef32-106">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="cef32-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cef32-107">Properties</span></span>
| <span data-ttu-id="cef32-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cef32-108">Property</span></span>     | <span data-ttu-id="cef32-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cef32-109">Type</span></span>   |<span data-ttu-id="cef32-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cef32-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cef32-111">end</span><span class="sxs-lookup"><span data-stu-id="cef32-111">end</span></span> |[<span data-ttu-id="cef32-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="cef32-112">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="cef32-113">Дата, время и часовой пояс, в течение которого заканчивается соответствующее событие.</span><span class="sxs-lookup"><span data-stu-id="cef32-113">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="cef32-114">Частный</span><span class="sxs-lookup"><span data-stu-id="cef32-114">isPrivate</span></span> |<span data-ttu-id="cef32-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="cef32-115">Boolean</span></span> |<span data-ttu-id="cef32-116">Чувствительность соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="cef32-116">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="cef32-117">Значение true, если событие помечено `private`, в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="cef32-117">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="cef32-118">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="cef32-118">Optional.</span></span>|
|<span data-ttu-id="cef32-119">location</span><span class="sxs-lookup"><span data-stu-id="cef32-119">location</span></span> |<span data-ttu-id="cef32-120">String</span><span class="sxs-lookup"><span data-stu-id="cef32-120">String</span></span> | <span data-ttu-id="cef32-121">Расположение, в котором находится соответствующее событие.</span><span class="sxs-lookup"><span data-stu-id="cef32-121">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="cef32-122">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="cef32-122">Optional.</span></span>|
|<span data-ttu-id="cef32-123">начать</span><span class="sxs-lookup"><span data-stu-id="cef32-123">start</span></span> |[<span data-ttu-id="cef32-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="cef32-124">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="cef32-125">Дата, время и часовой пояс, в котором начинается соответствующее событие.</span><span class="sxs-lookup"><span data-stu-id="cef32-125">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="cef32-126">status</span><span class="sxs-lookup"><span data-stu-id="cef32-126">status</span></span> |<span data-ttu-id="cef32-127">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="cef32-127">freeBusyStatus</span></span> | <span data-ttu-id="cef32-128">Состояние доступности пользователя или ресурса во время соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="cef32-128">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="cef32-129">Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="cef32-129">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="cef32-130">subject</span><span class="sxs-lookup"><span data-stu-id="cef32-130">subject</span></span> |<span data-ttu-id="cef32-131">String</span><span class="sxs-lookup"><span data-stu-id="cef32-131">String</span></span> | <span data-ttu-id="cef32-132">Строка темы соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="cef32-132">The corresponding event's subject line.</span></span> <span data-ttu-id="cef32-133">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="cef32-133">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="cef32-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cef32-134">JSON representation</span></span>

<span data-ttu-id="cef32-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cef32-135">The following is a JSON representation of the resource.</span></span>

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
  "tocPath": ""
}
-->
