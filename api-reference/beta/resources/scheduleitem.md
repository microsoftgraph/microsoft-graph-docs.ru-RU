---
title: Тип ресурса Счедулеитем
description: Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию. Этот элемент также применяется к ресурсу.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: ''
ms.openlocfilehash: fd71cd95d676ea226e03a15324cda01e41b6d2c1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520972"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="8da4b-104">Тип ресурса Счедулеитем</span><span class="sxs-lookup"><span data-stu-id="8da4b-104">scheduleItem resource type</span></span>

<span data-ttu-id="8da4b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8da4b-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="8da4b-106">Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8da4b-106">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="8da4b-107">Этот элемент также применяется к ресурсу (комнате или оборудованию).</span><span class="sxs-lookup"><span data-stu-id="8da4b-107">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="8da4b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8da4b-108">Properties</span></span>
| <span data-ttu-id="8da4b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8da4b-109">Property</span></span>     | <span data-ttu-id="8da4b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8da4b-110">Type</span></span>   |<span data-ttu-id="8da4b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8da4b-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8da4b-112">end</span><span class="sxs-lookup"><span data-stu-id="8da4b-112">end</span></span> |[<span data-ttu-id="8da4b-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8da4b-113">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="8da4b-114">Дата, время и часовой пояс, в течение которого заканчивается соответствующее событие.</span><span class="sxs-lookup"><span data-stu-id="8da4b-114">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="8da4b-115">Частный</span><span class="sxs-lookup"><span data-stu-id="8da4b-115">isPrivate</span></span> |<span data-ttu-id="8da4b-116">Логическое</span><span class="sxs-lookup"><span data-stu-id="8da4b-116">Boolean</span></span> |<span data-ttu-id="8da4b-117">Чувствительность соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="8da4b-117">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="8da4b-118">Значение true, если событие помечено `private` , в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="8da4b-118">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="8da4b-119">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8da4b-119">Optional.</span></span> |
|<span data-ttu-id="8da4b-120">location</span><span class="sxs-lookup"><span data-stu-id="8da4b-120">location</span></span> |<span data-ttu-id="8da4b-121">Строка</span><span class="sxs-lookup"><span data-stu-id="8da4b-121">String</span></span> | <span data-ttu-id="8da4b-122">Расположение, в котором находится соответствующее событие.</span><span class="sxs-lookup"><span data-stu-id="8da4b-122">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="8da4b-123">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8da4b-123">Optional.</span></span>|
|<span data-ttu-id="8da4b-124">начать</span><span class="sxs-lookup"><span data-stu-id="8da4b-124">start</span></span> |[<span data-ttu-id="8da4b-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8da4b-125">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="8da4b-126">Дата, время и часовой пояс, в котором начинается соответствующее событие.</span><span class="sxs-lookup"><span data-stu-id="8da4b-126">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="8da4b-127">status</span><span class="sxs-lookup"><span data-stu-id="8da4b-127">status</span></span> |<span data-ttu-id="8da4b-128">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="8da4b-128">freeBusyStatus</span></span> | <span data-ttu-id="8da4b-129">Состояние доступности пользователя или ресурса во время соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="8da4b-129">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="8da4b-130">Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="8da4b-130">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="8da4b-131">subject</span><span class="sxs-lookup"><span data-stu-id="8da4b-131">subject</span></span> |<span data-ttu-id="8da4b-132">String</span><span class="sxs-lookup"><span data-stu-id="8da4b-132">String</span></span> | <span data-ttu-id="8da4b-133">Строка темы соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="8da4b-133">The corresponding event's subject line.</span></span> <span data-ttu-id="8da4b-134">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8da4b-134">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8da4b-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8da4b-135">JSON representation</span></span>

<span data-ttu-id="8da4b-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8da4b-136">The following is a JSON representation of the resource.</span></span>

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
