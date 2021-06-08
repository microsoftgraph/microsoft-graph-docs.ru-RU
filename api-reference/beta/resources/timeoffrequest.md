---
title: тип ресурса timeOffRequest
description: Представляет тип запроса на смену, чтобы занять время.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 31d855f21164f933fe27acc824759cee08e16c16
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786070"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="adbd9-103">тип ресурса timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="adbd9-103">timeOffRequest resource type</span></span>

<span data-ttu-id="adbd9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adbd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adbd9-105">Представляет тип запроса на перенос, чтобы занять [timeOff](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="adbd9-105">Represents a type of shift request to take [timeOff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="adbd9-106">Методы</span><span class="sxs-lookup"><span data-stu-id="adbd9-106">Methods</span></span>

| <span data-ttu-id="adbd9-107">Метод</span><span class="sxs-lookup"><span data-stu-id="adbd9-107">Method</span></span>       | <span data-ttu-id="adbd9-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="adbd9-108">Return type</span></span> | <span data-ttu-id="adbd9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="adbd9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="adbd9-110">Список</span><span class="sxs-lookup"><span data-stu-id="adbd9-110">List</span></span>](../api/timeoffrequest-list.md) | <span data-ttu-id="adbd9-111">[коллекция timeOffRequest](timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="adbd9-111">[timeOffRequest](timeoffrequest.md) collection</span></span> | <span data-ttu-id="adbd9-112">Получите список объектов **timeOffRequest** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="adbd9-112">Get the list of **timeOffRequest** objects in this schedule.</span></span>|
| <span data-ttu-id="adbd9-113">[получение](../api/timeoffrequest-get.md);</span><span class="sxs-lookup"><span data-stu-id="adbd9-113">[Get](../api/timeoffrequest-get.md)</span></span> | [<span data-ttu-id="adbd9-114">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="adbd9-114">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="adbd9-115">Ознакомьтесь с свойствами и отношениями объекта **timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="adbd9-115">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="adbd9-116">Delete</span><span class="sxs-lookup"><span data-stu-id="adbd9-116">Delete</span></span>](../api/timeoffrequest-delete.md) | <span data-ttu-id="adbd9-117">Нет</span><span class="sxs-lookup"><span data-stu-id="adbd9-117">None</span></span> | <span data-ttu-id="adbd9-118">Удаление **объекта timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="adbd9-118">Delete a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="adbd9-119">Утвердить</span><span class="sxs-lookup"><span data-stu-id="adbd9-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="adbd9-120">Нет</span><span class="sxs-lookup"><span data-stu-id="adbd9-120">None</span></span>|<span data-ttu-id="adbd9-121">Утверждение запроса на время.</span><span class="sxs-lookup"><span data-stu-id="adbd9-121">Approve a time off request.</span></span>|
| [<span data-ttu-id="adbd9-122">Отклонение</span><span class="sxs-lookup"><span data-stu-id="adbd9-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="adbd9-123">Нет</span><span class="sxs-lookup"><span data-stu-id="adbd9-123">None</span></span>|<span data-ttu-id="adbd9-124">Отклонение запроса на время.</span><span class="sxs-lookup"><span data-stu-id="adbd9-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="adbd9-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="adbd9-125">Properties</span></span>

| <span data-ttu-id="adbd9-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="adbd9-126">Property</span></span>     | <span data-ttu-id="adbd9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="adbd9-127">Type</span></span>        | <span data-ttu-id="adbd9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="adbd9-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="adbd9-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="adbd9-129">endDateTime</span></span>|<span data-ttu-id="adbd9-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adbd9-130">DateTimeOffset</span></span>|<span data-ttu-id="adbd9-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="adbd9-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="adbd9-132">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="adbd9-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="adbd9-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="adbd9-133">startDateTime</span></span>|<span data-ttu-id="adbd9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adbd9-134">DateTimeOffset</span></span>|<span data-ttu-id="adbd9-135">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="adbd9-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="adbd9-136">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="adbd9-136">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="adbd9-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="adbd9-137">timeOffReasonId</span></span>|<span data-ttu-id="adbd9-138">String</span><span class="sxs-lookup"><span data-stu-id="adbd9-138">String</span></span>|<span data-ttu-id="adbd9-139">Причина простоя.</span><span class="sxs-lookup"><span data-stu-id="adbd9-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="adbd9-140">Связи</span><span class="sxs-lookup"><span data-stu-id="adbd9-140">Relationships</span></span>

<span data-ttu-id="adbd9-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="adbd9-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="adbd9-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="adbd9-142">JSON representation</span></span>

<span data-ttu-id="adbd9-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adbd9-143">The following is a JSON representation of the resource.</span></span>

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


