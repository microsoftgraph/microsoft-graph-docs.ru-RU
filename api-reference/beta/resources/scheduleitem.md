---
title: Тип ресурса Счедулеитем
description: Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию. Этот элемент также применяется к ресурсу.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: ''
ms.openlocfilehash: f2901412dcf1d52d8b117afa214da159b4553a8a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008644"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="8a2ec-104">Тип ресурса Счедулеитем</span><span class="sxs-lookup"><span data-stu-id="8a2ec-104">scheduleItem resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="8a2ec-105">Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8a2ec-105">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="8a2ec-106">Этот элемент также применяется к ресурсу (комнате или оборудованию).</span><span class="sxs-lookup"><span data-stu-id="8a2ec-106">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="8a2ec-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a2ec-107">Properties</span></span>
| <span data-ttu-id="8a2ec-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a2ec-108">Property</span></span>     | <span data-ttu-id="8a2ec-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8a2ec-109">Type</span></span>   |<span data-ttu-id="8a2ec-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8a2ec-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a2ec-111">end</span><span class="sxs-lookup"><span data-stu-id="8a2ec-111">end</span></span> |[<span data-ttu-id="8a2ec-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8a2ec-112">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="8a2ec-113">Дата, время и часовой пояс, в течение которого заканчивается соответствующее событие.</span><span class="sxs-lookup"><span data-stu-id="8a2ec-113">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="8a2ec-114">Частный</span><span class="sxs-lookup"><span data-stu-id="8a2ec-114">isPrivate</span></span> |<span data-ttu-id="8a2ec-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a2ec-115">Boolean</span></span> |<span data-ttu-id="8a2ec-116">Чувствительность соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="8a2ec-116">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="8a2ec-117">Значение true, если событие помечено `private`, в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="8a2ec-117">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="8a2ec-118">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8a2ec-118">Optional.</span></span> |
|<span data-ttu-id="8a2ec-119">location</span><span class="sxs-lookup"><span data-stu-id="8a2ec-119">location</span></span> |<span data-ttu-id="8a2ec-120">String</span><span class="sxs-lookup"><span data-stu-id="8a2ec-120">String</span></span> | <span data-ttu-id="8a2ec-121">Расположение, в котором находится соответствующее событие.</span><span class="sxs-lookup"><span data-stu-id="8a2ec-121">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="8a2ec-122">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8a2ec-122">Optional.</span></span>|
|<span data-ttu-id="8a2ec-123">начать</span><span class="sxs-lookup"><span data-stu-id="8a2ec-123">start</span></span> |[<span data-ttu-id="8a2ec-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8a2ec-124">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="8a2ec-125">Дата, время и часовой пояс, в котором начинается соответствующее событие.</span><span class="sxs-lookup"><span data-stu-id="8a2ec-125">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="8a2ec-126">status</span><span class="sxs-lookup"><span data-stu-id="8a2ec-126">status</span></span> |<span data-ttu-id="8a2ec-127">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="8a2ec-127">freeBusyStatus</span></span> | <span data-ttu-id="8a2ec-128">Состояние доступности пользователя или ресурса во время соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="8a2ec-128">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="8a2ec-129">Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="8a2ec-129">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="8a2ec-130">subject</span><span class="sxs-lookup"><span data-stu-id="8a2ec-130">subject</span></span> |<span data-ttu-id="8a2ec-131">String</span><span class="sxs-lookup"><span data-stu-id="8a2ec-131">String</span></span> | <span data-ttu-id="8a2ec-132">Строка темы соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="8a2ec-132">The corresponding event's subject line.</span></span> <span data-ttu-id="8a2ec-133">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8a2ec-133">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8a2ec-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a2ec-134">JSON representation</span></span>

<span data-ttu-id="8a2ec-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a2ec-135">The following is a JSON representation of the resource.</span></span>

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
