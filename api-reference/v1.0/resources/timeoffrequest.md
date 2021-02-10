---
title: Тип ресурса timeOffRequest
description: Представляет тип запроса на смену для отключаемого времени.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e234873110f50ed66decaa04b5462a9ff6fcf9a2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154203"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="6556c-103">Тип ресурса timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="6556c-103">timeOffRequest resource type</span></span>

<span data-ttu-id="6556c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6556c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6556c-105">Представляет тип запроса на смену для [отключаемого времени.](../resources/timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="6556c-105">Represents a type of shift request to take [timeOff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6556c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6556c-106">Methods</span></span>

| <span data-ttu-id="6556c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6556c-107">Method</span></span>       | <span data-ttu-id="6556c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6556c-108">Return Type</span></span> | <span data-ttu-id="6556c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6556c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6556c-110">Получение</span><span class="sxs-lookup"><span data-stu-id="6556c-110">Get</span></span>](../api/timeoffrequest-get.md) | [<span data-ttu-id="6556c-111">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="6556c-111">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="6556c-112">Чтение свойств и связей объекта **timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="6556c-112">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="6556c-113">Список</span><span class="sxs-lookup"><span data-stu-id="6556c-113">List</span></span>](../api/timeoffrequest-list.md) | <span data-ttu-id="6556c-114">[Коллекция timeOffRequest](timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="6556c-114">[timeOffRequest](timeoffrequest.md) collection</span></span> | <span data-ttu-id="6556c-115">Получите список объектов **timeOffRequest** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="6556c-115">Get the list of **timeOffRequest** objects in this schedule.</span></span>|
| <span data-ttu-id="6556c-116">[удаление](../api/timeoffrequest-delete.md);</span><span class="sxs-lookup"><span data-stu-id="6556c-116">[Delete](../api/timeoffrequest-delete.md)</span></span> | <span data-ttu-id="6556c-117">Нет</span><span class="sxs-lookup"><span data-stu-id="6556c-117">None</span></span> | <span data-ttu-id="6556c-118">Удаление объекта **timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="6556c-118">Delete a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="6556c-119">Утвердить</span><span class="sxs-lookup"><span data-stu-id="6556c-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="6556c-120">Нет</span><span class="sxs-lookup"><span data-stu-id="6556c-120">None</span></span>|<span data-ttu-id="6556c-121">Утверждение запроса на неавключие.</span><span class="sxs-lookup"><span data-stu-id="6556c-121">Approve a time off request.</span></span>|
| [<span data-ttu-id="6556c-122">Отклонение</span><span class="sxs-lookup"><span data-stu-id="6556c-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="6556c-123">Нет</span><span class="sxs-lookup"><span data-stu-id="6556c-123">None</span></span>|<span data-ttu-id="6556c-124">Отклонение запроса на отключение.</span><span class="sxs-lookup"><span data-stu-id="6556c-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="6556c-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="6556c-125">Properties</span></span>

| <span data-ttu-id="6556c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="6556c-126">Property</span></span>     | <span data-ttu-id="6556c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="6556c-127">Type</span></span>        | <span data-ttu-id="6556c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6556c-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6556c-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6556c-129">endDateTime</span></span>|<span data-ttu-id="6556c-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6556c-130">DateTimeOffset</span></span>|<span data-ttu-id="6556c-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6556c-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6556c-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6556c-133">startDateTime</span></span>|<span data-ttu-id="6556c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6556c-134">DateTimeOffset</span></span>|<span data-ttu-id="6556c-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6556c-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6556c-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="6556c-137">timeOffReasonId</span></span>|<span data-ttu-id="6556c-138">String</span><span class="sxs-lookup"><span data-stu-id="6556c-138">String</span></span>|<span data-ttu-id="6556c-139">Причина простоя.</span><span class="sxs-lookup"><span data-stu-id="6556c-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6556c-140">Связи</span><span class="sxs-lookup"><span data-stu-id="6556c-140">Relationships</span></span>

<span data-ttu-id="6556c-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6556c-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6556c-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6556c-142">JSON representation</span></span>

<span data-ttu-id="6556c-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6556c-143">The following is a JSON representation of the resource.</span></span>

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

