---
title: тип ресурса timeOffReason
description: Веские причины для того, чтобы взять время в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b449f2cb4dcfcd73208d58f8e1e969b9a701e54b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720188"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="d267b-103">тип ресурса timeOffReason</span><span class="sxs-lookup"><span data-stu-id="d267b-103">timeOffReason resource type</span></span>

<span data-ttu-id="d267b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d267b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d267b-105">Веские основания для [экземпляра timeOff](timeoff.md) в [расписании](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="d267b-105">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d267b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d267b-106">Methods</span></span>

| <span data-ttu-id="d267b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d267b-107">Method</span></span>       | <span data-ttu-id="d267b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d267b-108">Return Type</span></span>  |<span data-ttu-id="d267b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d267b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d267b-110">Создание</span><span class="sxs-lookup"><span data-stu-id="d267b-110">Create</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="d267b-111">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="d267b-111">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="d267b-112">Создание нового **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="d267b-112">Create a new **timeOffReason**.</span></span>|
|[<span data-ttu-id="d267b-113">List</span><span class="sxs-lookup"><span data-stu-id="d267b-113">List</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="d267b-114">[коллекция timeOffReason](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="d267b-114">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="d267b-115">Получите список **timeOffReason в** расписании.</span><span class="sxs-lookup"><span data-stu-id="d267b-115">Get the list of **timeOffReason** in a schedule.</span></span>|
|<span data-ttu-id="d267b-116">[получение](../api/timeoffreason-get.md);</span><span class="sxs-lookup"><span data-stu-id="d267b-116">[Get](../api/timeoffreason-get.md)</span></span> | [<span data-ttu-id="d267b-117">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="d267b-117">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="d267b-118">Получите **timeOffReason по** ID.</span><span class="sxs-lookup"><span data-stu-id="d267b-118">Get a **timeOffReason** by ID.</span></span>|
|[<span data-ttu-id="d267b-119">Replace</span><span class="sxs-lookup"><span data-stu-id="d267b-119">Replace</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="d267b-120">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="d267b-120">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="d267b-121">Замените **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="d267b-121">Replace a **timeOffReason**.</span></span>|
|[<span data-ttu-id="d267b-122">Удаление</span><span class="sxs-lookup"><span data-stu-id="d267b-122">Delete</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="d267b-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d267b-123">None</span></span> | <span data-ttu-id="d267b-124">**Пометить timeOffReason** как неактивное.</span><span class="sxs-lookup"><span data-stu-id="d267b-124">Mark a **timeOffReason** as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="d267b-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="d267b-125">Properties</span></span>
|<span data-ttu-id="d267b-126">Имя</span><span class="sxs-lookup"><span data-stu-id="d267b-126">Name</span></span>          |<span data-ttu-id="d267b-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d267b-127">Type</span></span>           |<span data-ttu-id="d267b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d267b-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="d267b-129">id</span><span class="sxs-lookup"><span data-stu-id="d267b-129">id</span></span>            |`string`      |<span data-ttu-id="d267b-130">Идентификатор объекта `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="d267b-130">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="d267b-131">displayName</span><span class="sxs-lookup"><span data-stu-id="d267b-131">displayName</span></span>               | `string`                  | <span data-ttu-id="d267b-132">Имя ресурса `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="d267b-132">The name of the `timeOffReason`.</span></span> <span data-ttu-id="d267b-133">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="d267b-133">Required.</span></span> |
| <span data-ttu-id="d267b-134">iconType</span><span class="sxs-lookup"><span data-stu-id="d267b-134">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="d267b-135">Поддерживаемые типы значков: нет; автомобиль; календарь; запуск; плоскости; firstAid; врач; notWorking; часы; juryDuty; глобус; чашка; телефон; погода; зонт; piggyBank; собака; торт; trafficCone; пин-код; солнечный.</span><span class="sxs-lookup"><span data-stu-id="d267b-135">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="d267b-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d267b-136">Required.</span></span> |
| <span data-ttu-id="d267b-137">isActive</span><span class="sxs-lookup"><span data-stu-id="d267b-137">isActive</span></span>          |`Boolean`      | <span data-ttu-id="d267b-138">Указывает, можно ли использовать объект `timeOffReason` при создании новых сущностей или обновлении существующих.</span><span class="sxs-lookup"><span data-stu-id="d267b-138">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="d267b-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d267b-139">Required.</span></span> |
| <span data-ttu-id="d267b-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d267b-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="d267b-141">Штамп времени, на котором `timeOffReason` это было впервые создано.</span><span class="sxs-lookup"><span data-stu-id="d267b-141">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="d267b-142">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d267b-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d267b-143">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="d267b-143">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="d267b-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d267b-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="d267b-145">Отпечаток времени, на котором `timeOffReason` это было обновлено в последний раз.</span><span class="sxs-lookup"><span data-stu-id="d267b-145">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="d267b-146">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d267b-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d267b-147">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="d267b-147">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="d267b-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d267b-148">lastModifiedBy</span></span>        | [<span data-ttu-id="d267b-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="d267b-149">identitySet</span></span>](identityset.md)        |<span data-ttu-id="d267b-150">Учетная запись, которая последней обновила этот объект `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="d267b-150">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d267b-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d267b-151">JSON representation</span></span>

<span data-ttu-id="d267b-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d267b-152">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason",
  "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "iconType": "String",
  "isActive": true,
  "lastModifiedBy": { "@odata.type":"microsoft.graph.identitySet"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffReason resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


