---
title: Тип ресурсов timeSlot
description: Период времени.
localization_priority: Normal
doc_type: resourcePageType
author: vrod9429
ms.prod: outlook
ms.openlocfilehash: f531add7d16fc5d1922a40e7341894b7fedd6535
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472057"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="31110-103">Тип ресурсов timeSlot</span><span class="sxs-lookup"><span data-stu-id="31110-103">timeSlot resource type</span></span>

<span data-ttu-id="31110-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31110-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31110-105">Представляет интервал времени для собрания.</span><span class="sxs-lookup"><span data-stu-id="31110-105">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31110-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31110-106">JSON representation</span></span>

<span data-ttu-id="31110-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="31110-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="31110-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="31110-108">Properties</span></span>
| <span data-ttu-id="31110-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="31110-109">Property</span></span>     | <span data-ttu-id="31110-110">Тип</span><span class="sxs-lookup"><span data-stu-id="31110-110">Type</span></span>   |<span data-ttu-id="31110-111">Описание</span><span class="sxs-lookup"><span data-stu-id="31110-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31110-112">end</span><span class="sxs-lookup"><span data-stu-id="31110-112">end</span></span>|[<span data-ttu-id="31110-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="31110-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="31110-114">Дата, время и часовой пояс, который начинается.</span><span class="sxs-lookup"><span data-stu-id="31110-114">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="31110-115">начать</span><span class="sxs-lookup"><span data-stu-id="31110-115">start</span></span>|[<span data-ttu-id="31110-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="31110-116">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="31110-117">Дата, время и часовой пояс, который заканчивается.</span><span class="sxs-lookup"><span data-stu-id="31110-117">The date, time, and time zone that a period ends.</span></span>|

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


