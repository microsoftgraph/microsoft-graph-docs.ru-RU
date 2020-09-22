---
title: Тип ресурса shiftItem
description: shiftItem представляет версию ресурса shift.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7b1522ee4b1819b168d5e261a5e8a53138a69ea4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036970"
---
# <a name="shiftitem-resource-type"></a><span data-ttu-id="87e09-103">Тип ресурса shiftItem</span><span class="sxs-lookup"><span data-stu-id="87e09-103">shiftItem resource type</span></span>

<span data-ttu-id="87e09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87e09-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="87e09-105">Представляет версию ресурса [shift](shift.md).</span><span class="sxs-lookup"><span data-stu-id="87e09-105">Represents a version of a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="87e09-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="87e09-106">Properties</span></span>
| <span data-ttu-id="87e09-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="87e09-107">Property</span></span>                         | <span data-ttu-id="87e09-108">Тип</span><span class="sxs-lookup"><span data-stu-id="87e09-108">Type</span></span>                    | <span data-ttu-id="87e09-109">Описание</span><span class="sxs-lookup"><span data-stu-id="87e09-109">Description</span></span>                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="87e09-110">notes</span><span class="sxs-lookup"><span data-stu-id="87e09-110">notes</span></span>               | <span data-ttu-id="87e09-111">string</span><span class="sxs-lookup"><span data-stu-id="87e09-111">string</span></span>                  | <span data-ttu-id="87e09-112">Сдвиг заметок для `shiftItem` .</span><span class="sxs-lookup"><span data-stu-id="87e09-112">The shift notes for the `shiftItem`.</span></span>      |
| <span data-ttu-id="87e09-113">displayName</span><span class="sxs-lookup"><span data-stu-id="87e09-113">displayName</span></span>               | <span data-ttu-id="87e09-114">string</span><span class="sxs-lookup"><span data-stu-id="87e09-114">string</span></span>                  | <span data-ttu-id="87e09-115">Метка сдвига `shiftItem` .</span><span class="sxs-lookup"><span data-stu-id="87e09-115">The shift label of the `shiftItem`.</span></span> |
| <span data-ttu-id="87e09-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="87e09-116">startDateTime</span></span>               | <span data-ttu-id="87e09-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87e09-117">DateTimeOffset</span></span>                  | <span data-ttu-id="87e09-118">Дата и время начала для ресурса `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="87e09-118">The start date and time for the `shiftItem`.</span></span> <span data-ttu-id="87e09-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="87e09-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="87e09-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="87e09-120">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="87e09-121">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="87e09-121">Required.</span></span> |
| <span data-ttu-id="87e09-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="87e09-122">endDateTime</span></span>               | <span data-ttu-id="87e09-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87e09-123">DateTimeOffset</span></span>                 | <span data-ttu-id="87e09-124">Дата и время окончания для ресурса `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="87e09-124">The end date and time for the `shiftItem`.</span></span> <span data-ttu-id="87e09-125">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="87e09-125">Required.</span></span> <span data-ttu-id="87e09-126">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="87e09-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="87e09-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="87e09-127">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="87e09-128">theme</span><span class="sxs-lookup"><span data-stu-id="87e09-128">theme</span></span> | <span data-ttu-id="87e09-129">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="87e09-129">scheduleEntityTheme</span></span>   |  <span data-ttu-id="87e09-130">Поддерживаемые цвета: белый, синий, зеленый, фиолетовый, розовый, желтый, серый, темно-синий, темно-зеленый, темно-фиолетовый, темно-розовый, темно-желтый.</span><span class="sxs-lookup"><span data-stu-id="87e09-130">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |
| <span data-ttu-id="87e09-131">activities</span><span class="sxs-lookup"><span data-stu-id="87e09-131">activities</span></span>    | <span data-ttu-id="87e09-132">Коллекция [shiftActivity](shiftactivity.md)</span><span class="sxs-lookup"><span data-stu-id="87e09-132">[shiftActivity](shiftactivity.md) collection</span></span>   | <span data-ttu-id="87e09-133">Добавочная часть ресурса shift, содержащая сведения о том, где и когда находится сотрудник во время своей смены.</span><span class="sxs-lookup"><span data-stu-id="87e09-133">An incremental part of a shift which can cover details of when and where an employee is during their shift.</span></span> <span data-ttu-id="87e09-134">Например, выполняет задание, на плановом перерыве или на обеде.</span><span class="sxs-lookup"><span data-stu-id="87e09-134">For example, an assignment or a scheduled break or lunch.</span></span> <span data-ttu-id="87e09-135">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="87e09-135">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="87e09-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87e09-136">JSON representation</span></span>

<span data-ttu-id="87e09-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87e09-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "String",
  "notes": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "String",
  "activities": [{"@odata.type": "microsoft.graph.shiftActivity"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

