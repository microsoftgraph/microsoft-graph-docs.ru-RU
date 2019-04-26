---
title: Тип ресурса Тимеоффреасон
description: Допустимая причина для выполнения времени ожидания в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8ba1e4bd596b82643ecbfa4b842e60232c182a4b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341976"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="48753-103">Тип ресурса Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="48753-103">timeOffReason resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48753-104">Допустимая причина для экземпляра [тимеофф](timeoff.md) по расписанию. [](schedule.md)</span><span class="sxs-lookup"><span data-stu-id="48753-104">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="48753-105">Методы</span><span class="sxs-lookup"><span data-stu-id="48753-105">Methods</span></span>

| <span data-ttu-id="48753-106">Метод</span><span class="sxs-lookup"><span data-stu-id="48753-106">Method</span></span>       | <span data-ttu-id="48753-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="48753-107">Return Type</span></span>  |<span data-ttu-id="48753-108">Описание</span><span class="sxs-lookup"><span data-stu-id="48753-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48753-109">Создание Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="48753-109">Create timeOffReason</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="48753-110">Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="48753-110">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="48753-111">Создание объекта `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="48753-111">Create a new `timeOffReason`.</span></span>|
|[<span data-ttu-id="48753-112">Список Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="48753-112">List timeOffReason</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="48753-113">Коллекция [тимеоффреасон](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="48753-113">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="48753-114">Получение списка объектов `timeOffReasons` в расписании.</span><span class="sxs-lookup"><span data-stu-id="48753-114">Get the list of `timeOffReasons` in a schedule.</span></span>|
|[<span data-ttu-id="48753-115">Получение Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="48753-115">Get timeOffReason</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="48753-116">Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="48753-116">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="48753-117">Получение `timeOffReason` по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="48753-117">Get a `timeOffReason` by ID.</span></span>|
|[<span data-ttu-id="48753-118">Замена Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="48753-118">Replace timeOffReason</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="48753-119">Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="48753-119">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="48753-120">Замена объекта `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="48753-120">Replace a `timeOffReason`.</span></span>|
|[<span data-ttu-id="48753-121">Удаление Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="48753-121">Delete timeOffReason</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="48753-122">Нет</span><span class="sxs-lookup"><span data-stu-id="48753-122">None</span></span> | <span data-ttu-id="48753-123">Объект `timeOffReason` помечается как неактивный.</span><span class="sxs-lookup"><span data-stu-id="48753-123">Mark `timeOffReason` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="48753-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="48753-124">Properties</span></span>
|<span data-ttu-id="48753-125">Имя</span><span class="sxs-lookup"><span data-stu-id="48753-125">Name</span></span>          |<span data-ttu-id="48753-126">Тип</span><span class="sxs-lookup"><span data-stu-id="48753-126">Type</span></span>           |<span data-ttu-id="48753-127">Описание</span><span class="sxs-lookup"><span data-stu-id="48753-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="48753-128">id</span><span class="sxs-lookup"><span data-stu-id="48753-128">id</span></span>            |`string`      |<span data-ttu-id="48753-129">Идентификатор объекта `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="48753-129">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="48753-130">displayName</span><span class="sxs-lookup"><span data-stu-id="48753-130">displayName</span></span>               | `string`                  | <span data-ttu-id="48753-131">Имя файла `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="48753-131">The name of the `timeOffReason`.</span></span> <span data-ttu-id="48753-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48753-132">Required.</span></span> |
| <span data-ttu-id="48753-133">Иконтипе</span><span class="sxs-lookup"><span data-stu-id="48753-133">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="48753-134">Поддерживаемые типы значков: нет; Мойка ведения запускается ходил Фирстаид; врача Нотворкинг; регистрации Журидути; любой кружк звонков Погода Общий Пиггибанк; Dog очень Траффикконе; крепления Веселая.</span><span class="sxs-lookup"><span data-stu-id="48753-134">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="48753-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48753-135">Required.</span></span> |
| <span data-ttu-id="48753-136">isActive</span><span class="sxs-lookup"><span data-stu-id="48753-136">isActive</span></span>          |`Boolean`      | <span data-ttu-id="48753-137">Указывает, можно ли использовать объект `timeOffReason` при создании новых сущностей или обновлении существующих.</span><span class="sxs-lookup"><span data-stu-id="48753-137">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="48753-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48753-138">Required.</span></span> |
| <span data-ttu-id="48753-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48753-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="48753-140">Отметка `timeOffReason` времени первоначального создания.</span><span class="sxs-lookup"><span data-stu-id="48753-140">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="48753-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="48753-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="48753-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="48753-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="48753-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48753-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="48753-144">Отметка `timeOffReason` времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="48753-144">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="48753-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="48753-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="48753-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="48753-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="48753-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="48753-147">lastModifiedBy</span></span>        | [<span data-ttu-id="48753-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="48753-148">identitySet</span></span>](identityset.md)        |<span data-ttu-id="48753-149">Учетная запись, которая последней обновила этот объект `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="48753-149">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48753-150">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="48753-150">JSON representation</span></span>

<span data-ttu-id="48753-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48753-151">Here is a JSON representation of the resource.</span></span>

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
