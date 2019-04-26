---
title: Тип ресурса Тимеоффитем
description: Представляет версию объекта Тимеофф.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3b5b819b9179d266064d7ddf0f6636b9027591af
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345506"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="c7dfe-103">Тип ресурса Тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="c7dfe-103">timeOffItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7dfe-104">Представляет версию объекта [тимеофф](timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="c7dfe-104">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c7dfe-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7dfe-105">Properties</span></span>
| <span data-ttu-id="c7dfe-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7dfe-106">Property</span></span>                         | <span data-ttu-id="c7dfe-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c7dfe-107">Type</span></span>                    | <span data-ttu-id="c7dfe-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c7dfe-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="c7dfe-109">Тимеоффреасонид</span><span class="sxs-lookup"><span data-stu-id="c7dfe-109">timeOffReasonId</span></span>               | <span data-ttu-id="c7dfe-110">строка</span><span class="sxs-lookup"><span data-stu-id="c7dfe-110">string</span></span>                  | <span data-ttu-id="c7dfe-111">Идентификатор объекта `timeOffReason` для этого `timeOffItem`параметра.</span><span class="sxs-lookup"><span data-stu-id="c7dfe-111">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="c7dfe-112">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7dfe-112">Required.</span></span>     |
| <span data-ttu-id="c7dfe-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c7dfe-113">startDateTime</span></span>               | <span data-ttu-id="c7dfe-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7dfe-114">DateTimeOffset</span></span>                  | <span data-ttu-id="c7dfe-115">Дата и время начала для `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="c7dfe-115">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="c7dfe-116">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7dfe-116">Required.</span></span> <span data-ttu-id="c7dfe-117">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c7dfe-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c7dfe-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="c7dfe-118">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="c7dfe-119">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c7dfe-119">endDateTime</span></span>               | <span data-ttu-id="c7dfe-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7dfe-120">DateTimeOffset</span></span>                  | <span data-ttu-id="c7dfe-121">Дата и время окончания для `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="c7dfe-121">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="c7dfe-122">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7dfe-122">Required.</span></span> <span data-ttu-id="c7dfe-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c7dfe-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c7dfe-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="c7dfe-124">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="c7dfe-125">theme</span><span class="sxs-lookup"><span data-stu-id="c7dfe-125">theme</span></span> | <span data-ttu-id="c7dfe-126">Счедулинтитисеме</span><span class="sxs-lookup"><span data-stu-id="c7dfe-126">scheduleEntityTheme</span></span>   | <span data-ttu-id="c7dfe-127">Поддерживаемые цвета: белый; компонентов Интенсив цвет Розов желтый участка Даркблуе; Даркгрин; Даркпурпле; Даркпинк; Даркеллов.</span><span class="sxs-lookup"><span data-stu-id="c7dfe-127">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c7dfe-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c7dfe-128">JSON representation</span></span>

<span data-ttu-id="c7dfe-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7dfe-129">Here is a JSON representation of the resource.</span></span>

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
