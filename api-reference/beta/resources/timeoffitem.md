---
title: Тип ресурса Тимеоффитем
description: Представляет версию объекта Тимеофф.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 6b240f587e20e2da178f9afa3e8d712cf2ae114d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964307"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="bfab4-103">Тип ресурса Тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="bfab4-103">timeOffItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfab4-104">Представляет версию объекта [тимеофф](timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="bfab4-104">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bfab4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="bfab4-105">Properties</span></span>
| <span data-ttu-id="bfab4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfab4-106">Property</span></span>                         | <span data-ttu-id="bfab4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="bfab4-107">Type</span></span>                    | <span data-ttu-id="bfab4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bfab4-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="bfab4-109">Тимеоффреасонид</span><span class="sxs-lookup"><span data-stu-id="bfab4-109">timeOffReasonId</span></span>               | <span data-ttu-id="bfab4-110">string</span><span class="sxs-lookup"><span data-stu-id="bfab4-110">string</span></span>                  | <span data-ttu-id="bfab4-111">Идентификатор объекта `timeOffReason` для этого `timeOffItem`параметра.</span><span class="sxs-lookup"><span data-stu-id="bfab4-111">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="bfab4-112">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="bfab4-112">Required.</span></span>     |
| <span data-ttu-id="bfab4-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bfab4-113">startDateTime</span></span>               | <span data-ttu-id="bfab4-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfab4-114">DateTimeOffset</span></span>                  | <span data-ttu-id="bfab4-115">Дата и время начала для `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="bfab4-115">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="bfab4-116">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="bfab4-116">Required.</span></span> <span data-ttu-id="bfab4-117">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bfab4-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bfab4-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="bfab4-118">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="bfab4-119">endDateTime</span><span class="sxs-lookup"><span data-stu-id="bfab4-119">endDateTime</span></span>               | <span data-ttu-id="bfab4-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfab4-120">DateTimeOffset</span></span>                  | <span data-ttu-id="bfab4-121">Дата и время окончания для `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="bfab4-121">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="bfab4-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="bfab4-122">Required.</span></span> <span data-ttu-id="bfab4-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bfab4-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bfab4-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="bfab4-124">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="bfab4-125">theme</span><span class="sxs-lookup"><span data-stu-id="bfab4-125">theme</span></span> | <span data-ttu-id="bfab4-126">Счедулинтитисеме</span><span class="sxs-lookup"><span data-stu-id="bfab4-126">scheduleEntityTheme</span></span>   | <span data-ttu-id="bfab4-127">Поддерживаемые цвета: белый; компонентов Интенсив цвет Розов желтый участка Даркблуе; Даркгрин; Даркпурпле; Даркпинк; Даркеллов.</span><span class="sxs-lookup"><span data-stu-id="bfab4-127">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bfab4-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bfab4-128">JSON representation</span></span>

<span data-ttu-id="bfab4-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfab4-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffItem"
}-->
```json
{
  "timeOffReasonId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
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
  "suppressions": []
}
-->
