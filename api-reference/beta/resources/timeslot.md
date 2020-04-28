---
title: Тип ресурсов timeSlot
description: Период времени.
localization_priority: Normal
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ff02706768feed52eaf6b85294e496211d9d711f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519703"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="e94f6-103">Тип ресурсов timeSlot</span><span class="sxs-lookup"><span data-stu-id="e94f6-103">timeSlot resource type</span></span>

<span data-ttu-id="e94f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e94f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e94f6-105">Представляет интервал времени для собрания.</span><span class="sxs-lookup"><span data-stu-id="e94f6-105">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e94f6-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e94f6-106">JSON representation</span></span>

<span data-ttu-id="e94f6-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e94f6-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="e94f6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e94f6-108">Properties</span></span>
| <span data-ttu-id="e94f6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e94f6-109">Property</span></span>     | <span data-ttu-id="e94f6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e94f6-110">Type</span></span>   |<span data-ttu-id="e94f6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e94f6-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e94f6-112">end</span><span class="sxs-lookup"><span data-stu-id="e94f6-112">end</span></span>|[<span data-ttu-id="e94f6-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e94f6-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e94f6-114">Дата, время и часовой пояс, с которого начинается период.</span><span class="sxs-lookup"><span data-stu-id="e94f6-114">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="e94f6-115">начать</span><span class="sxs-lookup"><span data-stu-id="e94f6-115">start</span></span>|[<span data-ttu-id="e94f6-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e94f6-116">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e94f6-117">Дата, время и часовой пояс, в течение которого заканчивается срок.</span><span class="sxs-lookup"><span data-stu-id="e94f6-117">The date, time, and time zone that a period ends.</span></span>|

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
