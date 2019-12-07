---
title: Тип ресурса Тимеоффрекуест
description: Представляет тип запроса на сдвиг для получения тимеофф.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 28be6904b64b89c6386bd25a4ced71f76fdc4088
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895844"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="53e39-103">Тип ресурса Тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="53e39-103">timeOffRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53e39-104">Представляет тип запроса на сдвиг для получения [тимеофф](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="53e39-104">Represents a type of shift request to take [timeoff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="53e39-105">Методы</span><span class="sxs-lookup"><span data-stu-id="53e39-105">Methods</span></span>

| <span data-ttu-id="53e39-106">Метод</span><span class="sxs-lookup"><span data-stu-id="53e39-106">Method</span></span>       | <span data-ttu-id="53e39-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="53e39-107">Return Type</span></span> | <span data-ttu-id="53e39-108">Описание</span><span class="sxs-lookup"><span data-stu-id="53e39-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="53e39-109">[получение](../api/timeoffrequest-get.md);</span><span class="sxs-lookup"><span data-stu-id="53e39-109">[Get](../api/timeoffrequest-get.md)</span></span> | [<span data-ttu-id="53e39-110">тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="53e39-110">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="53e39-111">Чтение свойств и связей объекта **тимеоффрекуест** .</span><span class="sxs-lookup"><span data-stu-id="53e39-111">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| <span data-ttu-id="53e39-112">[обновление](../api/timeoffrequest-update.md).</span><span class="sxs-lookup"><span data-stu-id="53e39-112">[Update](../api/timeoffrequest-update.md)</span></span> | [<span data-ttu-id="53e39-113">тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="53e39-113">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="53e39-114">Обновление объекта **тимеоффрекуест** .</span><span class="sxs-lookup"><span data-stu-id="53e39-114">Update a **timeOffRequest** object.</span></span> |
| <span data-ttu-id="53e39-115">[удаление](../api/timeoffrequest-delete.md);</span><span class="sxs-lookup"><span data-stu-id="53e39-115">[Delete](../api/timeoffrequest-delete.md)</span></span> | <span data-ttu-id="53e39-116">Нет</span><span class="sxs-lookup"><span data-stu-id="53e39-116">None</span></span> | <span data-ttu-id="53e39-117">Удаление объекта **тимеоффрекуест** .</span><span class="sxs-lookup"><span data-stu-id="53e39-117">Delete a **timeOffRequest** object.</span></span> |
|[<span data-ttu-id="53e39-118">Утвердить</span><span class="sxs-lookup"><span data-stu-id="53e39-118">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="53e39-119">Нет</span><span class="sxs-lookup"><span data-stu-id="53e39-119">None</span></span>|<span data-ttu-id="53e39-120">Утверждение запроса на нерабочее время.</span><span class="sxs-lookup"><span data-stu-id="53e39-120">Approve a time off request.</span></span>|
|[<span data-ttu-id="53e39-121">Отклоня</span><span class="sxs-lookup"><span data-stu-id="53e39-121">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="53e39-122">Нет</span><span class="sxs-lookup"><span data-stu-id="53e39-122">None</span></span>|<span data-ttu-id="53e39-123">Отклонить запрос времени ожидания.</span><span class="sxs-lookup"><span data-stu-id="53e39-123">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="53e39-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="53e39-124">Properties</span></span>

| <span data-ttu-id="53e39-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="53e39-125">Property</span></span>     | <span data-ttu-id="53e39-126">Тип</span><span class="sxs-lookup"><span data-stu-id="53e39-126">Type</span></span>        | <span data-ttu-id="53e39-127">Описание</span><span class="sxs-lookup"><span data-stu-id="53e39-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="53e39-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="53e39-128">endDateTime</span></span>|<span data-ttu-id="53e39-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53e39-129">DateTimeOffset</span></span>|<span data-ttu-id="53e39-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="53e39-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="53e39-132">startDateTime</span><span class="sxs-lookup"><span data-stu-id="53e39-132">startDateTime</span></span>|<span data-ttu-id="53e39-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53e39-133">DateTimeOffset</span></span>|<span data-ttu-id="53e39-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="53e39-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="53e39-136">тимеоффреасонид</span><span class="sxs-lookup"><span data-stu-id="53e39-136">timeOffReasonId</span></span>|<span data-ttu-id="53e39-137">String</span><span class="sxs-lookup"><span data-stu-id="53e39-137">String</span></span>|<span data-ttu-id="53e39-138">Причина невыходного времени.</span><span class="sxs-lookup"><span data-stu-id="53e39-138">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53e39-139">Связи</span><span class="sxs-lookup"><span data-stu-id="53e39-139">Relationships</span></span>

<span data-ttu-id="53e39-140">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="53e39-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="53e39-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="53e39-141">JSON representation</span></span>

<span data-ttu-id="53e39-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53e39-142">The following is a JSON representation of the resource.</span></span>

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
