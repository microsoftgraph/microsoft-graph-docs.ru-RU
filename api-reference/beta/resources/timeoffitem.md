---
title: тип ресурса timeOffItem
description: Представляет версию timeOff.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8fbe535fcbc63f94a50e65c62c694ffaac1a9aed
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786084"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="35d5e-103">тип ресурса timeOffItem</span><span class="sxs-lookup"><span data-stu-id="35d5e-103">timeOffItem resource type</span></span>

<span data-ttu-id="35d5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35d5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35d5e-105">Представляет версию [timeOff](timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="35d5e-105">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="35d5e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="35d5e-106">Properties</span></span>
| <span data-ttu-id="35d5e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="35d5e-107">Property</span></span>                         | <span data-ttu-id="35d5e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="35d5e-108">Type</span></span>                    | <span data-ttu-id="35d5e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="35d5e-109">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="35d5e-110">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="35d5e-110">timeOffReasonId</span></span>               | <span data-ttu-id="35d5e-111">Строка</span><span class="sxs-lookup"><span data-stu-id="35d5e-111">string</span></span>                  | <span data-ttu-id="35d5e-112">ID этого `timeOffReason` **времениOffItem**.</span><span class="sxs-lookup"><span data-stu-id="35d5e-112">ID of the `timeOffReason` for this **timeOffItem**.</span></span> <span data-ttu-id="35d5e-113">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35d5e-113">Required.</span></span>     |
| <span data-ttu-id="35d5e-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="35d5e-114">startDateTime</span></span>               | <span data-ttu-id="35d5e-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35d5e-115">DateTimeOffset</span></span>                  | <span data-ttu-id="35d5e-116">Дата начала и время **для timeOffItem**.</span><span class="sxs-lookup"><span data-stu-id="35d5e-116">The start date and time for the **timeOffItem**.</span></span> <span data-ttu-id="35d5e-117">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="35d5e-117">Required.</span></span> <span data-ttu-id="35d5e-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="35d5e-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="35d5e-119">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="35d5e-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="35d5e-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="35d5e-120">endDateTime</span></span>               | <span data-ttu-id="35d5e-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35d5e-121">DateTimeOffset</span></span>                  | <span data-ttu-id="35d5e-122">Дата окончания и время **для timeOffItem**.</span><span class="sxs-lookup"><span data-stu-id="35d5e-122">The end date and time for the **timeOffItem**.</span></span> <span data-ttu-id="35d5e-123">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="35d5e-123">Required.</span></span> <span data-ttu-id="35d5e-124">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="35d5e-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="35d5e-125">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="35d5e-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="35d5e-126">theme</span><span class="sxs-lookup"><span data-stu-id="35d5e-126">theme</span></span> | <span data-ttu-id="35d5e-127">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="35d5e-127">scheduleEntityTheme</span></span>   | <span data-ttu-id="35d5e-128">Поддерживаемые цвета: белый, синий, зеленый, фиолетовый, розовый, желтый, серый, темно-синий, темно-зеленый, темно-фиолетовый, темно-розовый, темно-желтый.</span><span class="sxs-lookup"><span data-stu-id="35d5e-128">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35d5e-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35d5e-129">JSON representation</span></span>

<span data-ttu-id="35d5e-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35d5e-130">Here is a JSON representation of the resource.</span></span>

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
  "theme": {"@odata.type": "microsoft.graph.scheduleEntityTheme"}
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


