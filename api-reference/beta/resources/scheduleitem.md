---
title: Тип ресурса Счедулеитем
description: Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию. Этот элемент также применяется к ресурсу.
localization_priority: Normal
ms.openlocfilehash: a39f45598ab3c427a741659aa93615317c3c57a7
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869311"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="6ca4c-104">Тип ресурса Счедулеитем</span><span class="sxs-lookup"><span data-stu-id="6ca4c-104">scheduleItem resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="6ca4c-105">Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6ca4c-105">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="6ca4c-106">Этот элемент также применяется к ресурсу (комнате или оборудованию).</span><span class="sxs-lookup"><span data-stu-id="6ca4c-106">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="6ca4c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ca4c-107">Properties</span></span>
| <span data-ttu-id="6ca4c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ca4c-108">Property</span></span>     | <span data-ttu-id="6ca4c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6ca4c-109">Type</span></span>   |<span data-ttu-id="6ca4c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6ca4c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ca4c-111">end</span><span class="sxs-lookup"><span data-stu-id="6ca4c-111">end</span></span> |[<span data-ttu-id="6ca4c-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6ca4c-112">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="6ca4c-113">Дата, время и часовой пояс, в течение которого заканчивается соответствующее событие.</span><span class="sxs-lookup"><span data-stu-id="6ca4c-113">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="6ca4c-114">Частный</span><span class="sxs-lookup"><span data-stu-id="6ca4c-114">isPrivate</span></span> |<span data-ttu-id="6ca4c-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ca4c-115">Boolean</span></span> |<span data-ttu-id="6ca4c-116">Чувствительность соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="6ca4c-116">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="6ca4c-117">Значение true, если событие помечено `private`, в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="6ca4c-117">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="6ca4c-118">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="6ca4c-118">Optional.</span></span> |
|<span data-ttu-id="6ca4c-119">location</span><span class="sxs-lookup"><span data-stu-id="6ca4c-119">location</span></span> |<span data-ttu-id="6ca4c-120">String</span><span class="sxs-lookup"><span data-stu-id="6ca4c-120">String</span></span> | <span data-ttu-id="6ca4c-121">Расположение, в котором находится соответствующее событие.</span><span class="sxs-lookup"><span data-stu-id="6ca4c-121">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="6ca4c-122">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="6ca4c-122">Optional.</span></span>|
|<span data-ttu-id="6ca4c-123">start</span><span class="sxs-lookup"><span data-stu-id="6ca4c-123">start</span></span> |[<span data-ttu-id="6ca4c-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6ca4c-124">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="6ca4c-125">Дата, время и часовой пояс, в котором начинается соответствующее событие.</span><span class="sxs-lookup"><span data-stu-id="6ca4c-125">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="6ca4c-126">status</span><span class="sxs-lookup"><span data-stu-id="6ca4c-126">status</span></span> |<span data-ttu-id="6ca4c-127">Фрибусистатус</span><span class="sxs-lookup"><span data-stu-id="6ca4c-127">freeBusyStatus</span></span> | <span data-ttu-id="6ca4c-128">Состояние доступности пользователя или ресурса во время соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="6ca4c-128">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="6ca4c-129">Возможные `free`значения:, `tentative`, `busy`, `oof`, `workingElsewhere`,. `unknown`</span><span class="sxs-lookup"><span data-stu-id="6ca4c-129">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="6ca4c-130">subject</span><span class="sxs-lookup"><span data-stu-id="6ca4c-130">subject</span></span> |<span data-ttu-id="6ca4c-131">String</span><span class="sxs-lookup"><span data-stu-id="6ca4c-131">String</span></span> | <span data-ttu-id="6ca4c-132">Строка темы соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="6ca4c-132">The corresponding event's subject line.</span></span> <span data-ttu-id="6ca4c-133">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="6ca4c-133">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6ca4c-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6ca4c-134">JSON representation</span></span>

<span data-ttu-id="6ca4c-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ca4c-135">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
