---
title: Тип ресурса Тимеоффитем
description: Представляет версию объекта Тимеофф.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 166f1fe569301f6c2805867ff85b3c6354377128
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075492"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="4d5d9-103">Тип ресурса Тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="4d5d9-103">timeOffItem resource type</span></span>

<span data-ttu-id="4d5d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d5d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d5d9-105">Представляет версию объекта [тимеофф](timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="4d5d9-105">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4d5d9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d5d9-106">Properties</span></span>
| <span data-ttu-id="4d5d9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d5d9-107">Property</span></span>                         | <span data-ttu-id="4d5d9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4d5d9-108">Type</span></span>                    | <span data-ttu-id="4d5d9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4d5d9-109">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="4d5d9-110">тимеоффреасонид</span><span class="sxs-lookup"><span data-stu-id="4d5d9-110">timeOffReasonId</span></span>               | <span data-ttu-id="4d5d9-111">string</span><span class="sxs-lookup"><span data-stu-id="4d5d9-111">string</span></span>                  | <span data-ttu-id="4d5d9-112">Идентификатор объекта `timeOffReason` для этого параметра `timeOffItem` .</span><span class="sxs-lookup"><span data-stu-id="4d5d9-112">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="4d5d9-113">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4d5d9-113">Required.</span></span>     |
| <span data-ttu-id="4d5d9-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4d5d9-114">startDateTime</span></span>               | <span data-ttu-id="4d5d9-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d5d9-115">DateTimeOffset</span></span>                  | <span data-ttu-id="4d5d9-116">Дата и время начала для ресурса `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="4d5d9-116">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="4d5d9-117">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="4d5d9-117">Required.</span></span> <span data-ttu-id="4d5d9-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4d5d9-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4d5d9-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="4d5d9-119">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="4d5d9-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4d5d9-120">endDateTime</span></span>               | <span data-ttu-id="4d5d9-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d5d9-121">DateTimeOffset</span></span>                  | <span data-ttu-id="4d5d9-122">Дата и время окончания для ресурса `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="4d5d9-122">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="4d5d9-123">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="4d5d9-123">Required.</span></span> <span data-ttu-id="4d5d9-124">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4d5d9-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4d5d9-125">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="4d5d9-125">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="4d5d9-126">theme</span><span class="sxs-lookup"><span data-stu-id="4d5d9-126">theme</span></span> | <span data-ttu-id="4d5d9-127">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="4d5d9-127">scheduleEntityTheme</span></span>   | <span data-ttu-id="4d5d9-128">Поддерживаемые цвета: белый, синий, зеленый, фиолетовый, розовый, желтый, серый, темно-синий, темно-зеленый, темно-фиолетовый, темно-розовый, темно-желтый.</span><span class="sxs-lookup"><span data-stu-id="4d5d9-128">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4d5d9-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d5d9-129">JSON representation</span></span>

<span data-ttu-id="4d5d9-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d5d9-130">Here is a JSON representation of the resource.</span></span>

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


