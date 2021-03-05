---
title: Тип ресурсов timeSlot
description: Период времени.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 378a7ac71058ec80c9ce20ee0959c1dc5c3ce091
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474685"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="da263-103">Тип ресурсов timeSlot</span><span class="sxs-lookup"><span data-stu-id="da263-103">timeSlot resource type</span></span>

<span data-ttu-id="da263-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da263-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da263-105">Представляет интервал времени для собрания.</span><span class="sxs-lookup"><span data-stu-id="da263-105">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da263-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da263-106">JSON representation</span></span>

<span data-ttu-id="da263-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="da263-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="da263-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="da263-108">Properties</span></span>
| <span data-ttu-id="da263-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="da263-109">Property</span></span>     | <span data-ttu-id="da263-110">Тип</span><span class="sxs-lookup"><span data-stu-id="da263-110">Type</span></span>   |<span data-ttu-id="da263-111">Описание</span><span class="sxs-lookup"><span data-stu-id="da263-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da263-112">end</span><span class="sxs-lookup"><span data-stu-id="da263-112">end</span></span>|[<span data-ttu-id="da263-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="da263-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="da263-114">Дата, время и часовой пояс, который начинается.</span><span class="sxs-lookup"><span data-stu-id="da263-114">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="da263-115">начать</span><span class="sxs-lookup"><span data-stu-id="da263-115">start</span></span>|[<span data-ttu-id="da263-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="da263-116">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="da263-117">Дата, время и часовой пояс, который заканчивается.</span><span class="sxs-lookup"><span data-stu-id="da263-117">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

