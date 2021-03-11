---
title: тип ресурса timeOffRequest
description: Представляет тип запроса на смену, чтобы занять время.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 42ad70594dfc5f5c0491b88c95d88e19e226ec1c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720181"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="7257d-103">тип ресурса timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="7257d-103">timeOffRequest resource type</span></span>

<span data-ttu-id="7257d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7257d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7257d-105">Представляет тип запроса на смену, чтобы занять [время.](../resources/timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="7257d-105">Represents a type of shift request to take [timeoff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7257d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7257d-106">Methods</span></span>

| <span data-ttu-id="7257d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="7257d-107">Method</span></span>       | <span data-ttu-id="7257d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7257d-108">Return Type</span></span> | <span data-ttu-id="7257d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7257d-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7257d-110">Список</span><span class="sxs-lookup"><span data-stu-id="7257d-110">List</span></span>](../api/timeoffrequest-list.md) | <span data-ttu-id="7257d-111">[коллекция timeOffRequest](timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="7257d-111">[timeOffRequest](timeoffrequest.md) collection</span></span> | <span data-ttu-id="7257d-112">Получите список объектов **timeOffRequest** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="7257d-112">Get the list of **timeOffRequest** objects in this schedule.</span></span>|
| <span data-ttu-id="7257d-113">[получение](../api/timeoffrequest-get.md);</span><span class="sxs-lookup"><span data-stu-id="7257d-113">[Get](../api/timeoffrequest-get.md)</span></span> | [<span data-ttu-id="7257d-114">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="7257d-114">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="7257d-115">Ознакомьтесь с свойствами и отношениями объекта **timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="7257d-115">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="7257d-116">Удаление</span><span class="sxs-lookup"><span data-stu-id="7257d-116">Delete</span></span>](../api/timeoffrequest-delete.md) | <span data-ttu-id="7257d-117">Нет</span><span class="sxs-lookup"><span data-stu-id="7257d-117">None</span></span> | <span data-ttu-id="7257d-118">Удаление **объекта timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="7257d-118">Delete a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="7257d-119">Утвердить</span><span class="sxs-lookup"><span data-stu-id="7257d-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="7257d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="7257d-120">None</span></span>|<span data-ttu-id="7257d-121">Утверждение запроса на время.</span><span class="sxs-lookup"><span data-stu-id="7257d-121">Approve a time off request.</span></span>|
| [<span data-ttu-id="7257d-122">Отклонение</span><span class="sxs-lookup"><span data-stu-id="7257d-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="7257d-123">Нет</span><span class="sxs-lookup"><span data-stu-id="7257d-123">None</span></span>|<span data-ttu-id="7257d-124">Отклонение запроса на время.</span><span class="sxs-lookup"><span data-stu-id="7257d-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="7257d-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="7257d-125">Properties</span></span>

| <span data-ttu-id="7257d-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="7257d-126">Property</span></span>     | <span data-ttu-id="7257d-127">Тип</span><span class="sxs-lookup"><span data-stu-id="7257d-127">Type</span></span>        | <span data-ttu-id="7257d-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7257d-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7257d-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7257d-129">endDateTime</span></span>|<span data-ttu-id="7257d-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7257d-130">DateTimeOffset</span></span>|<span data-ttu-id="7257d-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="7257d-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7257d-132">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="7257d-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="7257d-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7257d-133">startDateTime</span></span>|<span data-ttu-id="7257d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7257d-134">DateTimeOffset</span></span>|<span data-ttu-id="7257d-135">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="7257d-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7257d-136">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="7257d-136">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="7257d-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="7257d-137">timeOffReasonId</span></span>|<span data-ttu-id="7257d-138">String</span><span class="sxs-lookup"><span data-stu-id="7257d-138">String</span></span>|<span data-ttu-id="7257d-139">Причина простоя.</span><span class="sxs-lookup"><span data-stu-id="7257d-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7257d-140">Связи</span><span class="sxs-lookup"><span data-stu-id="7257d-140">Relationships</span></span>

<span data-ttu-id="7257d-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7257d-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7257d-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7257d-142">JSON representation</span></span>

<span data-ttu-id="7257d-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7257d-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeOffRequest"
}-->

```json
{
  "endDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "timeOffReasonId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


