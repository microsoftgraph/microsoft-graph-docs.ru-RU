---
title: Тип ресурса Тимеоффрекуест
description: Представляет тип запроса на сдвиг для получения тимеофф.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 73fa72d403bd20e6a966b01a0529d09689e5ed66
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519717"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="d9003-103">Тип ресурса Тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="d9003-103">timeOffRequest resource type</span></span>

<span data-ttu-id="d9003-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d9003-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9003-105">Представляет тип запроса на сдвиг для получения [тимеофф](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="d9003-105">Represents a type of shift request to take [timeoff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d9003-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d9003-106">Methods</span></span>

| <span data-ttu-id="d9003-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d9003-107">Method</span></span>       | <span data-ttu-id="d9003-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d9003-108">Return Type</span></span> | <span data-ttu-id="d9003-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d9003-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d9003-110">[получение](../api/timeoffrequest-get.md);</span><span class="sxs-lookup"><span data-stu-id="d9003-110">[Get](../api/timeoffrequest-get.md)</span></span> | [<span data-ttu-id="d9003-111">тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="d9003-111">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="d9003-112">Чтение свойств и связей объекта **тимеоффрекуест** .</span><span class="sxs-lookup"><span data-stu-id="d9003-112">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| <span data-ttu-id="d9003-113">[обновление](../api/timeoffrequest-update.md).</span><span class="sxs-lookup"><span data-stu-id="d9003-113">[Update](../api/timeoffrequest-update.md)</span></span> | [<span data-ttu-id="d9003-114">тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="d9003-114">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="d9003-115">Обновление объекта **тимеоффрекуест** .</span><span class="sxs-lookup"><span data-stu-id="d9003-115">Update a **timeOffRequest** object.</span></span> |
| <span data-ttu-id="d9003-116">[удаление](../api/timeoffrequest-delete.md);</span><span class="sxs-lookup"><span data-stu-id="d9003-116">[Delete](../api/timeoffrequest-delete.md)</span></span> | <span data-ttu-id="d9003-117">Нет</span><span class="sxs-lookup"><span data-stu-id="d9003-117">None</span></span> | <span data-ttu-id="d9003-118">Удаление объекта **тимеоффрекуест** .</span><span class="sxs-lookup"><span data-stu-id="d9003-118">Delete a **timeOffRequest** object.</span></span> |
|[<span data-ttu-id="d9003-119">Утвердить</span><span class="sxs-lookup"><span data-stu-id="d9003-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="d9003-120">Нет</span><span class="sxs-lookup"><span data-stu-id="d9003-120">None</span></span>|<span data-ttu-id="d9003-121">Утверждение запроса на нерабочее время.</span><span class="sxs-lookup"><span data-stu-id="d9003-121">Approve a time off request.</span></span>|
|[<span data-ttu-id="d9003-122">Отклоня</span><span class="sxs-lookup"><span data-stu-id="d9003-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="d9003-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d9003-123">None</span></span>|<span data-ttu-id="d9003-124">Отклонить запрос времени ожидания.</span><span class="sxs-lookup"><span data-stu-id="d9003-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="d9003-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9003-125">Properties</span></span>

| <span data-ttu-id="d9003-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9003-126">Property</span></span>     | <span data-ttu-id="d9003-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d9003-127">Type</span></span>        | <span data-ttu-id="d9003-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d9003-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9003-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d9003-129">endDateTime</span></span>|<span data-ttu-id="d9003-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9003-130">DateTimeOffset</span></span>|<span data-ttu-id="d9003-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d9003-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d9003-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d9003-133">startDateTime</span></span>|<span data-ttu-id="d9003-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9003-134">DateTimeOffset</span></span>|<span data-ttu-id="d9003-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d9003-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d9003-137">тимеоффреасонид</span><span class="sxs-lookup"><span data-stu-id="d9003-137">timeOffReasonId</span></span>|<span data-ttu-id="d9003-138">String</span><span class="sxs-lookup"><span data-stu-id="d9003-138">String</span></span>|<span data-ttu-id="d9003-139">Причина невыходного времени.</span><span class="sxs-lookup"><span data-stu-id="d9003-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9003-140">Связи</span><span class="sxs-lookup"><span data-stu-id="d9003-140">Relationships</span></span>

<span data-ttu-id="d9003-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d9003-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9003-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d9003-142">JSON representation</span></span>

<span data-ttu-id="d9003-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9003-143">The following is a JSON representation of the resource.</span></span>

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
