---
title: Тип ресурсов timeSlot
description: Период времени.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5dbde12e63a5e48863f1353f4d4d22df5ba41091
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033595"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="e6439-103">Тип ресурсов timeSlot</span><span class="sxs-lookup"><span data-stu-id="e6439-103">timeSlot resource type</span></span>

<span data-ttu-id="e6439-104">Представляет интервал времени для собрания.</span><span class="sxs-lookup"><span data-stu-id="e6439-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6439-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6439-105">JSON representation</span></span>

<span data-ttu-id="e6439-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e6439-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a><span data-ttu-id="e6439-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6439-107">Properties</span></span>
| <span data-ttu-id="e6439-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6439-108">Property</span></span>     | <span data-ttu-id="e6439-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e6439-109">Type</span></span>   |<span data-ttu-id="e6439-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e6439-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6439-111">end</span><span class="sxs-lookup"><span data-stu-id="e6439-111">end</span></span>|[<span data-ttu-id="e6439-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e6439-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e6439-113">Дата, время и часовой пояс, с которого начинается период.</span><span class="sxs-lookup"><span data-stu-id="e6439-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="e6439-114">начать</span><span class="sxs-lookup"><span data-stu-id="e6439-114">start</span></span>|[<span data-ttu-id="e6439-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e6439-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e6439-116">Дата, время и часовой пояс, в течение которого заканчивается срок.</span><span class="sxs-lookup"><span data-stu-id="e6439-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
