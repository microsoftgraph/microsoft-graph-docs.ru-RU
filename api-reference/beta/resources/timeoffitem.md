---
title: Тип ресурса Тимеоффитем
description: Представляет версию объекта Тимеофф.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c83a8725a0048a622ed88ec8265be76c30e46cc0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582883"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="fcc66-103">Тип ресурса Тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="fcc66-103">timeOffItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcc66-104">Представляет версию объекта [тимеофф](timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="fcc66-104">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fcc66-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fcc66-105">Properties</span></span>
| <span data-ttu-id="fcc66-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcc66-106">Property</span></span>                         | <span data-ttu-id="fcc66-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fcc66-107">Type</span></span>                    | <span data-ttu-id="fcc66-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fcc66-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="fcc66-109">Тимеоффреасонид</span><span class="sxs-lookup"><span data-stu-id="fcc66-109">timeOffReasonId</span></span>               | `string`                  | <span data-ttu-id="fcc66-110">Идентификатор объекта `timeOffReason` для этого `timeOffItem`параметра.</span><span class="sxs-lookup"><span data-stu-id="fcc66-110">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="fcc66-111">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcc66-111">Required.</span></span>     |
| <span data-ttu-id="fcc66-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fcc66-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="fcc66-113">Дата и время начала для `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="fcc66-113">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="fcc66-114">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcc66-114">Required.</span></span> <span data-ttu-id="fcc66-115">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fcc66-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fcc66-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="fcc66-116">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="fcc66-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="fcc66-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="fcc66-118">Дата и время окончания для `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="fcc66-118">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="fcc66-119">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcc66-119">Required.</span></span> <span data-ttu-id="fcc66-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fcc66-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fcc66-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="fcc66-121">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="fcc66-122">theme</span><span class="sxs-lookup"><span data-stu-id="fcc66-122">theme</span></span> | `enum`   | <span data-ttu-id="fcc66-123">Поддерживаемые цвета: белый; компонентов Интенсив цвет Розов желтый участка Даркблуе; Даркгрин; Даркпурпле; Даркпинк; Даркеллов.</span><span class="sxs-lookup"><span data-stu-id="fcc66-123">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fcc66-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fcc66-124">JSON representation</span></span>

<span data-ttu-id="fcc66-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcc66-125">Here is a JSON representation of the resource.</span></span>

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
