---
title: Тип ресурсов timeSlot
description: Период времени.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 874b587db2bb9e2234fcacca9b3e3b0cf5c2f89b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090755"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="6dae2-103">Тип ресурсов timeSlot</span><span class="sxs-lookup"><span data-stu-id="6dae2-103">timeSlot resource type</span></span>

<span data-ttu-id="6dae2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dae2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6dae2-105">Представляет интервал времени для собрания.</span><span class="sxs-lookup"><span data-stu-id="6dae2-105">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6dae2-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6dae2-106">JSON representation</span></span>

<span data-ttu-id="6dae2-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="6dae2-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="6dae2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6dae2-108">Properties</span></span>
| <span data-ttu-id="6dae2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6dae2-109">Property</span></span>     | <span data-ttu-id="6dae2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6dae2-110">Type</span></span>   |<span data-ttu-id="6dae2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6dae2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6dae2-112">end</span><span class="sxs-lookup"><span data-stu-id="6dae2-112">end</span></span>|[<span data-ttu-id="6dae2-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6dae2-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6dae2-114">Дата, время и часовой пояс, с которого начинается период.</span><span class="sxs-lookup"><span data-stu-id="6dae2-114">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="6dae2-115">начать</span><span class="sxs-lookup"><span data-stu-id="6dae2-115">start</span></span>|[<span data-ttu-id="6dae2-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6dae2-116">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6dae2-117">Дата, время и часовой пояс, в течение которого заканчивается срок.</span><span class="sxs-lookup"><span data-stu-id="6dae2-117">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

