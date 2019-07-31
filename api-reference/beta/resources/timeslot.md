---
title: Тип ресурсов timeSlot
description: Период времени.
localization_priority: Normal
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 8843b8418bff068564e5716d715a9ad11579f01b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007538"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="defe8-103">Тип ресурсов timeSlot</span><span class="sxs-lookup"><span data-stu-id="defe8-103">timeSlot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="defe8-104">Представляет интервал времени для собрания.</span><span class="sxs-lookup"><span data-stu-id="defe8-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="defe8-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="defe8-105">JSON representation</span></span>

<span data-ttu-id="defe8-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="defe8-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="defe8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="defe8-107">Properties</span></span>
| <span data-ttu-id="defe8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="defe8-108">Property</span></span>     | <span data-ttu-id="defe8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="defe8-109">Type</span></span>   |<span data-ttu-id="defe8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="defe8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="defe8-111">end</span><span class="sxs-lookup"><span data-stu-id="defe8-111">end</span></span>|[<span data-ttu-id="defe8-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="defe8-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="defe8-113">Дата, время и часовой пояс, с которого начинается период.</span><span class="sxs-lookup"><span data-stu-id="defe8-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="defe8-114">начать</span><span class="sxs-lookup"><span data-stu-id="defe8-114">start</span></span>|[<span data-ttu-id="defe8-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="defe8-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="defe8-116">Дата, время и часовой пояс, в течение которого заканчивается срок.</span><span class="sxs-lookup"><span data-stu-id="defe8-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
