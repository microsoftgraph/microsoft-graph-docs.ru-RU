---
title: тип ресурса timeOffRequest
description: Представляет тип запроса на перенос, чтобы занять время.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 76eea937b03f3eb117e6b5f870a316f268df615c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721699"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="b694c-103">тип ресурса timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="b694c-103">timeOffRequest resource type</span></span>

<span data-ttu-id="b694c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b694c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b694c-105">Представляет тип запроса на перенос, чтобы занять [timeOff](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="b694c-105">Represents a type of shift request to take [timeOff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b694c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b694c-106">Methods</span></span>

| <span data-ttu-id="b694c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b694c-107">Method</span></span>       | <span data-ttu-id="b694c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b694c-108">Return Type</span></span> | <span data-ttu-id="b694c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b694c-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b694c-110">[получение](../api/timeoffrequest-get.md);</span><span class="sxs-lookup"><span data-stu-id="b694c-110">[Get](../api/timeoffrequest-get.md)</span></span> | [<span data-ttu-id="b694c-111">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="b694c-111">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="b694c-112">Ознакомьтесь с свойствами и отношениями объекта **timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="b694c-112">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="b694c-113">List</span><span class="sxs-lookup"><span data-stu-id="b694c-113">List</span></span>](../api/timeoffrequest-list.md) | <span data-ttu-id="b694c-114">[коллекция timeOffRequest](timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="b694c-114">[timeOffRequest](timeoffrequest.md) collection</span></span> | <span data-ttu-id="b694c-115">Получите список объектов **timeOffRequest** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="b694c-115">Get the list of **timeOffRequest** objects in this schedule.</span></span>|
| <span data-ttu-id="b694c-116">[удаление](../api/timeoffrequest-delete.md);</span><span class="sxs-lookup"><span data-stu-id="b694c-116">[Delete](../api/timeoffrequest-delete.md)</span></span> | <span data-ttu-id="b694c-117">Нет</span><span class="sxs-lookup"><span data-stu-id="b694c-117">None</span></span> | <span data-ttu-id="b694c-118">Удаление **объекта timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="b694c-118">Delete a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="b694c-119">Утвердить</span><span class="sxs-lookup"><span data-stu-id="b694c-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="b694c-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b694c-120">None</span></span>|<span data-ttu-id="b694c-121">Утверждение запроса на время.</span><span class="sxs-lookup"><span data-stu-id="b694c-121">Approve a time off request.</span></span>|
| [<span data-ttu-id="b694c-122">Отклонение</span><span class="sxs-lookup"><span data-stu-id="b694c-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="b694c-123">Нет</span><span class="sxs-lookup"><span data-stu-id="b694c-123">None</span></span>|<span data-ttu-id="b694c-124">Отклонение запроса на время.</span><span class="sxs-lookup"><span data-stu-id="b694c-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="b694c-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="b694c-125">Properties</span></span>

| <span data-ttu-id="b694c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b694c-126">Property</span></span>     | <span data-ttu-id="b694c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b694c-127">Type</span></span>        | <span data-ttu-id="b694c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b694c-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b694c-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b694c-129">endDateTime</span></span>|<span data-ttu-id="b694c-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b694c-130">DateTimeOffset</span></span>|<span data-ttu-id="b694c-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b694c-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b694c-132">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b694c-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b694c-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b694c-133">startDateTime</span></span>|<span data-ttu-id="b694c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b694c-134">DateTimeOffset</span></span>|<span data-ttu-id="b694c-135">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b694c-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b694c-136">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b694c-136">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b694c-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="b694c-137">timeOffReasonId</span></span>|<span data-ttu-id="b694c-138">String</span><span class="sxs-lookup"><span data-stu-id="b694c-138">String</span></span>|<span data-ttu-id="b694c-139">Причина простоя.</span><span class="sxs-lookup"><span data-stu-id="b694c-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b694c-140">Связи</span><span class="sxs-lookup"><span data-stu-id="b694c-140">Relationships</span></span>

<span data-ttu-id="b694c-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b694c-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b694c-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b694c-142">JSON representation</span></span>

<span data-ttu-id="b694c-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b694c-143">The following is a JSON representation of the resource.</span></span>

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

