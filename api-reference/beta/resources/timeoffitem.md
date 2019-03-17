---
title: Тип ресурса Тимеоффитем
description: Представляет версию объекта Тимеофф.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c83a8725a0048a622ed88ec8265be76c30e46cc0
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657856"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="465de-103">Тип ресурса Тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="465de-103">timeOffItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="465de-104">Представляет версию объекта [тимеофф](timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="465de-104">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="465de-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="465de-105">Properties</span></span>
| <span data-ttu-id="465de-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="465de-106">Property</span></span>                         | <span data-ttu-id="465de-107">Тип</span><span class="sxs-lookup"><span data-stu-id="465de-107">Type</span></span>                    | <span data-ttu-id="465de-108">Описание</span><span class="sxs-lookup"><span data-stu-id="465de-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="465de-109">Тимеоффреасонид</span><span class="sxs-lookup"><span data-stu-id="465de-109">timeOffReasonId</span></span>               | `string`                  | <span data-ttu-id="465de-110">Идентификатор объекта `timeOffReason` для этого `timeOffItem`параметра.</span><span class="sxs-lookup"><span data-stu-id="465de-110">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="465de-111">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="465de-111">Required.</span></span>     |
| <span data-ttu-id="465de-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="465de-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="465de-113">Дата и время начала для `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="465de-113">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="465de-114">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="465de-114">Required.</span></span> <span data-ttu-id="465de-115">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="465de-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="465de-116">Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="465de-116">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="465de-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="465de-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="465de-118">Дата и время окончания для `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="465de-118">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="465de-119">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="465de-119">Required.</span></span> <span data-ttu-id="465de-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="465de-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="465de-121">Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="465de-121">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="465de-122">theme</span><span class="sxs-lookup"><span data-stu-id="465de-122">theme</span></span> | `enum`   | <span data-ttu-id="465de-123">Поддерживаемые цвета: белый; компонентов Интенсив цвет Розов желтый участка Даркблуе; Даркгрин; Даркпурпле; Даркпинк; Даркеллов.</span><span class="sxs-lookup"><span data-stu-id="465de-123">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="465de-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="465de-124">JSON representation</span></span>

<span data-ttu-id="465de-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="465de-125">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffItem"
}-->
```json
{
  "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "startDateTime": "2019-03-11T07:00:00Z",
  "endDateTime": "2019-03-12T07:00:00Z",
  "theme": "pink"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoffitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
