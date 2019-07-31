---
title: Тип ресурса Тимеоффреасон
description: Допустимая причина для выполнения времени ожидания в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 62943670a0c87d34fd849e988ef5bf827aa6d72a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964293"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="3861f-103">Тип ресурса Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="3861f-103">timeOffReason resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3861f-104">Допустимая причина для экземпляра [тимеофф](timeoff.md) по расписанию. [](schedule.md)</span><span class="sxs-lookup"><span data-stu-id="3861f-104">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3861f-105">Методы</span><span class="sxs-lookup"><span data-stu-id="3861f-105">Methods</span></span>

| <span data-ttu-id="3861f-106">Метод</span><span class="sxs-lookup"><span data-stu-id="3861f-106">Method</span></span>       | <span data-ttu-id="3861f-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3861f-107">Return Type</span></span>  |<span data-ttu-id="3861f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3861f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3861f-109">Создание Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="3861f-109">Create timeOffReason</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="3861f-110">Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="3861f-110">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="3861f-111">Создание объекта `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="3861f-111">Create a new `timeOffReason`.</span></span>|
|[<span data-ttu-id="3861f-112">Список Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="3861f-112">List timeOffReason</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="3861f-113">Коллекция [тимеоффреасон](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="3861f-113">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="3861f-114">Получение списка объектов `timeOffReasons` в расписании.</span><span class="sxs-lookup"><span data-stu-id="3861f-114">Get the list of `timeOffReasons` in a schedule.</span></span>|
|[<span data-ttu-id="3861f-115">Получение Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="3861f-115">Get timeOffReason</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="3861f-116">Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="3861f-116">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="3861f-117">Получение `timeOffReason` по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="3861f-117">Get a `timeOffReason` by ID.</span></span>|
|[<span data-ttu-id="3861f-118">Замена Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="3861f-118">Replace timeOffReason</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="3861f-119">Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="3861f-119">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="3861f-120">Замена объекта `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="3861f-120">Replace a `timeOffReason`.</span></span>|
|[<span data-ttu-id="3861f-121">Удаление Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="3861f-121">Delete timeOffReason</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="3861f-122">Нет</span><span class="sxs-lookup"><span data-stu-id="3861f-122">None</span></span> | <span data-ttu-id="3861f-123">Объект `timeOffReason` помечается как неактивный.</span><span class="sxs-lookup"><span data-stu-id="3861f-123">Mark `timeOffReason` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="3861f-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="3861f-124">Properties</span></span>
|<span data-ttu-id="3861f-125">Имя</span><span class="sxs-lookup"><span data-stu-id="3861f-125">Name</span></span>          |<span data-ttu-id="3861f-126">Тип</span><span class="sxs-lookup"><span data-stu-id="3861f-126">Type</span></span>           |<span data-ttu-id="3861f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="3861f-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="3861f-128">id</span><span class="sxs-lookup"><span data-stu-id="3861f-128">id</span></span>            |`string`      |<span data-ttu-id="3861f-129">Идентификатор объекта `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="3861f-129">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="3861f-130">displayName</span><span class="sxs-lookup"><span data-stu-id="3861f-130">displayName</span></span>               | `string`                  | <span data-ttu-id="3861f-131">Имя файла `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="3861f-131">The name of the `timeOffReason`.</span></span> <span data-ttu-id="3861f-132">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3861f-132">Required.</span></span> |
| <span data-ttu-id="3861f-133">Иконтипе</span><span class="sxs-lookup"><span data-stu-id="3861f-133">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="3861f-134">Поддерживаемые типы значков: нет; Мойка ведения запускается ходил Фирстаид; врача Нотворкинг; регистрации Журидути; любой кружк звонков Погода Общий Пиггибанк; Dog очень Траффикконе; крепления Веселая.</span><span class="sxs-lookup"><span data-stu-id="3861f-134">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="3861f-135">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3861f-135">Required.</span></span> |
| <span data-ttu-id="3861f-136">isActive</span><span class="sxs-lookup"><span data-stu-id="3861f-136">isActive</span></span>          |`Boolean`      | <span data-ttu-id="3861f-137">Указывает, можно ли использовать объект `timeOffReason` при создании новых сущностей или обновлении существующих.</span><span class="sxs-lookup"><span data-stu-id="3861f-137">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="3861f-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3861f-138">Required.</span></span> |
| <span data-ttu-id="3861f-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3861f-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="3861f-140">Отметка `timeOffReason` времени первоначального создания.</span><span class="sxs-lookup"><span data-stu-id="3861f-140">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="3861f-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3861f-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3861f-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="3861f-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="3861f-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3861f-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="3861f-144">Отметка `timeOffReason` времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="3861f-144">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="3861f-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3861f-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3861f-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="3861f-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="3861f-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3861f-147">lastModifiedBy</span></span>        | [<span data-ttu-id="3861f-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="3861f-148">identitySet</span></span>](identityset.md)        |<span data-ttu-id="3861f-149">Учетная запись, которая последней обновила этот объект `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="3861f-149">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3861f-150">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3861f-150">JSON representation</span></span>

<span data-ttu-id="3861f-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3861f-151">Here is a JSON representation of the resource.</span></span>

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
