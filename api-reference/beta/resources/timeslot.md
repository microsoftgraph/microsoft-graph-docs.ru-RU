---
title: Тип ресурсов timeSlot
description: Период времени.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ee8746d1278f4c9422fa2803895a20c359d5f1e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555299"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="e0e07-103">Тип ресурсов timeSlot</span><span class="sxs-lookup"><span data-stu-id="e0e07-103">timeSlot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0e07-104">Представляет интервал времени для собрания.</span><span class="sxs-lookup"><span data-stu-id="e0e07-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0e07-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0e07-105">JSON representation</span></span>

<span data-ttu-id="e0e07-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e0e07-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="e0e07-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0e07-107">Properties</span></span>
| <span data-ttu-id="e0e07-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0e07-108">Property</span></span>     | <span data-ttu-id="e0e07-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e0e07-109">Type</span></span>   |<span data-ttu-id="e0e07-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e0e07-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0e07-111">end</span><span class="sxs-lookup"><span data-stu-id="e0e07-111">end</span></span>|[<span data-ttu-id="e0e07-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e0e07-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e0e07-113">Дата, время и часовой пояс, с которого начинается период.</span><span class="sxs-lookup"><span data-stu-id="e0e07-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="e0e07-114">start</span><span class="sxs-lookup"><span data-stu-id="e0e07-114">start</span></span>|[<span data-ttu-id="e0e07-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e0e07-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e0e07-116">Дата, время и часовой пояс, в течение которого заканчивается срок.</span><span class="sxs-lookup"><span data-stu-id="e0e07-116">The date, time, and time zone that a period ends.</span></span>|

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
