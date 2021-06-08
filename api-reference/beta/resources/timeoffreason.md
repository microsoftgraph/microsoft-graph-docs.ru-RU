---
title: тип ресурса timeOffReason
description: Веские причины для того, чтобы взять время в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b236fa6bd55e0af294955286e1443310196688a8
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52784978"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="f0c35-103">тип ресурса timeOffReason</span><span class="sxs-lookup"><span data-stu-id="f0c35-103">timeOffReason resource type</span></span>

<span data-ttu-id="f0c35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0c35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0c35-105">Веские основания для [экземпляра timeOff](timeoff.md) в [расписании](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="f0c35-105">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f0c35-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f0c35-106">Methods</span></span>

| <span data-ttu-id="f0c35-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f0c35-107">Method</span></span>       | <span data-ttu-id="f0c35-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="f0c35-108">Return type</span></span>  |<span data-ttu-id="f0c35-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f0c35-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f0c35-110">Создание</span><span class="sxs-lookup"><span data-stu-id="f0c35-110">Create</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="f0c35-111">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="f0c35-111">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="f0c35-112">Создание нового **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="f0c35-112">Create a new **timeOffReason**.</span></span>|
|[<span data-ttu-id="f0c35-113">List</span><span class="sxs-lookup"><span data-stu-id="f0c35-113">List</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="f0c35-114">[коллекция timeOffReason](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="f0c35-114">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="f0c35-115">Получите список **timeOffReason в** расписании.</span><span class="sxs-lookup"><span data-stu-id="f0c35-115">Get the list of **timeOffReason** in a schedule.</span></span>|
|<span data-ttu-id="f0c35-116">[получение](../api/timeoffreason-get.md);</span><span class="sxs-lookup"><span data-stu-id="f0c35-116">[Get](../api/timeoffreason-get.md)</span></span> | [<span data-ttu-id="f0c35-117">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="f0c35-117">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="f0c35-118">Получите **timeOffReason по** ID.</span><span class="sxs-lookup"><span data-stu-id="f0c35-118">Get a **timeOffReason** by ID.</span></span>|
|[<span data-ttu-id="f0c35-119">Replace</span><span class="sxs-lookup"><span data-stu-id="f0c35-119">Replace</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="f0c35-120">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="f0c35-120">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="f0c35-121">Замените **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="f0c35-121">Replace a **timeOffReason**.</span></span>|
|[<span data-ttu-id="f0c35-122">Delete</span><span class="sxs-lookup"><span data-stu-id="f0c35-122">Delete</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="f0c35-123">Нет</span><span class="sxs-lookup"><span data-stu-id="f0c35-123">None</span></span> | <span data-ttu-id="f0c35-124">**Пометить timeOffReason** как неактивное.</span><span class="sxs-lookup"><span data-stu-id="f0c35-124">Mark a **timeOffReason** as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="f0c35-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0c35-125">Properties</span></span>
|<span data-ttu-id="f0c35-126">Имя</span><span class="sxs-lookup"><span data-stu-id="f0c35-126">Name</span></span>          |<span data-ttu-id="f0c35-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f0c35-127">Type</span></span>           |<span data-ttu-id="f0c35-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f0c35-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="f0c35-129">id</span><span class="sxs-lookup"><span data-stu-id="f0c35-129">id</span></span>            |`string`      |<span data-ttu-id="f0c35-130">ID **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="f0c35-130">ID of the **timeOffReason**.</span></span>|
| <span data-ttu-id="f0c35-131">displayName</span><span class="sxs-lookup"><span data-stu-id="f0c35-131">displayName</span></span>               | `string`                  | <span data-ttu-id="f0c35-132">Имя **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="f0c35-132">The name of the **timeOffReason**.</span></span> <span data-ttu-id="f0c35-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0c35-133">Required.</span></span> |
| <span data-ttu-id="f0c35-134">iconType</span><span class="sxs-lookup"><span data-stu-id="f0c35-134">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="f0c35-135">Поддерживаемые типы значков: нет; автомобиль; календарь; запуск; плоскости; firstAid; врач; notWorking; часы; juryDuty; глобус; чашка; телефон; погода; зонт; piggyBank; собака; торт; trafficCone; пин-код; солнечный.</span><span class="sxs-lookup"><span data-stu-id="f0c35-135">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="f0c35-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0c35-136">Required.</span></span> |
| <span data-ttu-id="f0c35-137">isActive</span><span class="sxs-lookup"><span data-stu-id="f0c35-137">isActive</span></span>          |`Boolean`      | <span data-ttu-id="f0c35-138">Указывает, можно ли **использовать timeOffReason** при создании новых сущностям или обновлении существующих.</span><span class="sxs-lookup"><span data-stu-id="f0c35-138">Indicates whether the **timeOffReason** can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="f0c35-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0c35-139">Required.</span></span> |
| <span data-ttu-id="f0c35-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0c35-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="f0c35-141">Штамп времени, на котором на **этот раз был созданOffReason.**</span><span class="sxs-lookup"><span data-stu-id="f0c35-141">The time stamp on which this **timeOffReason** was first created.</span></span> <span data-ttu-id="f0c35-142">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f0c35-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f0c35-143">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="f0c35-143">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="f0c35-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0c35-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="f0c35-145">Штамп времени, на котором **в этот раз был обновленOffReason.**</span><span class="sxs-lookup"><span data-stu-id="f0c35-145">The time stamp on which this **timeOffReason** was last updated.</span></span> <span data-ttu-id="f0c35-146">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f0c35-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f0c35-147">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="f0c35-147">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="f0c35-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f0c35-148">lastModifiedBy</span></span>        | [<span data-ttu-id="f0c35-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="f0c35-149">identitySet</span></span>](identityset.md)        |<span data-ttu-id="f0c35-150">Удостоверение, которое в последний раз обновлялось **на этот разOffReason**.</span><span class="sxs-lookup"><span data-stu-id="f0c35-150">The identity that last updated this **timeOffReason**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0c35-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0c35-151">JSON representation</span></span>

<span data-ttu-id="f0c35-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0c35-152">Here is a JSON representation of the resource.</span></span>

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


