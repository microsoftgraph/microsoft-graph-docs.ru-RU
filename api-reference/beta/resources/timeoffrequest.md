---
title: Тип ресурса Тимеоффрекуест
description: Представляет тип запроса на сдвиг для получения тимеофф.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1b1e6c3f55b716590a399c9324ea759ff93810d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073392"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="3ba66-103">Тип ресурса Тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="3ba66-103">timeOffRequest resource type</span></span>

<span data-ttu-id="3ba66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ba66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ba66-105">Представляет тип запроса на сдвиг для получения [тимеофф](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="3ba66-105">Represents a type of shift request to take [timeoff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3ba66-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3ba66-106">Methods</span></span>

| <span data-ttu-id="3ba66-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3ba66-107">Method</span></span>       | <span data-ttu-id="3ba66-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3ba66-108">Return Type</span></span> | <span data-ttu-id="3ba66-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3ba66-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3ba66-110">Список</span><span class="sxs-lookup"><span data-stu-id="3ba66-110">List</span></span>](../api/timeoffrequest-list.md) | <span data-ttu-id="3ba66-111">Коллекция [тимеоффрекуест](timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="3ba66-111">[timeOffRequest](timeoffrequest.md) collection</span></span> | <span data-ttu-id="3ba66-112">Получение списка объектов **тимеоффрекуест** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="3ba66-112">Get the list of **timeOffRequest** objects in this schedule.</span></span>|
| <span data-ttu-id="3ba66-113">[получение](../api/timeoffrequest-get.md);</span><span class="sxs-lookup"><span data-stu-id="3ba66-113">[Get](../api/timeoffrequest-get.md)</span></span> | [<span data-ttu-id="3ba66-114">тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="3ba66-114">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="3ba66-115">Чтение свойств и связей объекта **тимеоффрекуест** .</span><span class="sxs-lookup"><span data-stu-id="3ba66-115">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="3ba66-116">Удаление</span><span class="sxs-lookup"><span data-stu-id="3ba66-116">Delete</span></span>](../api/timeoffrequest-delete.md) | <span data-ttu-id="3ba66-117">Нет</span><span class="sxs-lookup"><span data-stu-id="3ba66-117">None</span></span> | <span data-ttu-id="3ba66-118">Удаление объекта **тимеоффрекуест** .</span><span class="sxs-lookup"><span data-stu-id="3ba66-118">Delete a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="3ba66-119">Утвердить</span><span class="sxs-lookup"><span data-stu-id="3ba66-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="3ba66-120">Нет</span><span class="sxs-lookup"><span data-stu-id="3ba66-120">None</span></span>|<span data-ttu-id="3ba66-121">Утверждение запроса на нерабочее время.</span><span class="sxs-lookup"><span data-stu-id="3ba66-121">Approve a time off request.</span></span>|
| [<span data-ttu-id="3ba66-122">Отклоня</span><span class="sxs-lookup"><span data-stu-id="3ba66-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="3ba66-123">Нет</span><span class="sxs-lookup"><span data-stu-id="3ba66-123">None</span></span>|<span data-ttu-id="3ba66-124">Отклонить запрос времени ожидания.</span><span class="sxs-lookup"><span data-stu-id="3ba66-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="3ba66-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ba66-125">Properties</span></span>

| <span data-ttu-id="3ba66-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ba66-126">Property</span></span>     | <span data-ttu-id="3ba66-127">Тип</span><span class="sxs-lookup"><span data-stu-id="3ba66-127">Type</span></span>        | <span data-ttu-id="3ba66-128">Описание</span><span class="sxs-lookup"><span data-stu-id="3ba66-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3ba66-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3ba66-129">endDateTime</span></span>|<span data-ttu-id="3ba66-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ba66-130">DateTimeOffset</span></span>|<span data-ttu-id="3ba66-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3ba66-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3ba66-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3ba66-133">startDateTime</span></span>|<span data-ttu-id="3ba66-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ba66-134">DateTimeOffset</span></span>|<span data-ttu-id="3ba66-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3ba66-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3ba66-137">тимеоффреасонид</span><span class="sxs-lookup"><span data-stu-id="3ba66-137">timeOffReasonId</span></span>|<span data-ttu-id="3ba66-138">String</span><span class="sxs-lookup"><span data-stu-id="3ba66-138">String</span></span>|<span data-ttu-id="3ba66-139">Причина невыходного времени.</span><span class="sxs-lookup"><span data-stu-id="3ba66-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ba66-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="3ba66-140">Relationships</span></span>

<span data-ttu-id="3ba66-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3ba66-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ba66-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3ba66-142">JSON representation</span></span>

<span data-ttu-id="3ba66-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ba66-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeOffRequest",
  "baseType": ""
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


