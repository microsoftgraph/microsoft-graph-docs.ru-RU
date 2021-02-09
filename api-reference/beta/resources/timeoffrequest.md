---
title: Тип ресурса timeOffRequest
description: Представляет тип запроса на смену для отключки.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6d94f90ca0c77fc0e97de94027a4bf5b591820f4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159446"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="87529-103">Тип ресурса timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="87529-103">timeOffRequest resource type</span></span>

<span data-ttu-id="87529-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87529-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87529-105">Представляет тип запроса на смену для [отключки.](../resources/timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="87529-105">Represents a type of shift request to take [timeoff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="87529-106">Методы</span><span class="sxs-lookup"><span data-stu-id="87529-106">Methods</span></span>

| <span data-ttu-id="87529-107">Метод</span><span class="sxs-lookup"><span data-stu-id="87529-107">Method</span></span>       | <span data-ttu-id="87529-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="87529-108">Return Type</span></span> | <span data-ttu-id="87529-109">Описание</span><span class="sxs-lookup"><span data-stu-id="87529-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="87529-110">Список</span><span class="sxs-lookup"><span data-stu-id="87529-110">List</span></span>](../api/timeoffrequest-list.md) | <span data-ttu-id="87529-111">[Коллекция timeOffRequest](timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="87529-111">[timeOffRequest](timeoffrequest.md) collection</span></span> | <span data-ttu-id="87529-112">Получите список объектов **timeOffRequest** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="87529-112">Get the list of **timeOffRequest** objects in this schedule.</span></span>|
| [<span data-ttu-id="87529-113">Получение</span><span class="sxs-lookup"><span data-stu-id="87529-113">Get</span></span>](../api/timeoffrequest-get.md) | [<span data-ttu-id="87529-114">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="87529-114">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="87529-115">Чтение свойств и связей объекта **timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="87529-115">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| <span data-ttu-id="87529-116">[удаление](../api/timeoffrequest-delete.md);</span><span class="sxs-lookup"><span data-stu-id="87529-116">[Delete](../api/timeoffrequest-delete.md)</span></span> | <span data-ttu-id="87529-117">Нет</span><span class="sxs-lookup"><span data-stu-id="87529-117">None</span></span> | <span data-ttu-id="87529-118">Удаление объекта **timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="87529-118">Delete a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="87529-119">Утвердить</span><span class="sxs-lookup"><span data-stu-id="87529-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="87529-120">Нет</span><span class="sxs-lookup"><span data-stu-id="87529-120">None</span></span>|<span data-ttu-id="87529-121">Утверждение запроса на неавключие.</span><span class="sxs-lookup"><span data-stu-id="87529-121">Approve a time off request.</span></span>|
| [<span data-ttu-id="87529-122">Отклонение</span><span class="sxs-lookup"><span data-stu-id="87529-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="87529-123">Нет</span><span class="sxs-lookup"><span data-stu-id="87529-123">None</span></span>|<span data-ttu-id="87529-124">Отклонение запроса на отключение.</span><span class="sxs-lookup"><span data-stu-id="87529-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="87529-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="87529-125">Properties</span></span>

| <span data-ttu-id="87529-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="87529-126">Property</span></span>     | <span data-ttu-id="87529-127">Тип</span><span class="sxs-lookup"><span data-stu-id="87529-127">Type</span></span>        | <span data-ttu-id="87529-128">Описание</span><span class="sxs-lookup"><span data-stu-id="87529-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="87529-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="87529-129">endDateTime</span></span>|<span data-ttu-id="87529-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87529-130">DateTimeOffset</span></span>|<span data-ttu-id="87529-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="87529-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="87529-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="87529-133">startDateTime</span></span>|<span data-ttu-id="87529-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87529-134">DateTimeOffset</span></span>|<span data-ttu-id="87529-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="87529-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="87529-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="87529-137">timeOffReasonId</span></span>|<span data-ttu-id="87529-138">String</span><span class="sxs-lookup"><span data-stu-id="87529-138">String</span></span>|<span data-ttu-id="87529-139">Причина простоя.</span><span class="sxs-lookup"><span data-stu-id="87529-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87529-140">Связи</span><span class="sxs-lookup"><span data-stu-id="87529-140">Relationships</span></span>

<span data-ttu-id="87529-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="87529-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87529-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="87529-142">JSON representation</span></span>

<span data-ttu-id="87529-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87529-143">The following is a JSON representation of the resource.</span></span>

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


