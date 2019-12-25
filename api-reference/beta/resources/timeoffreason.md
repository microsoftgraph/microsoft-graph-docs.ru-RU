---
title: Тип ресурса Тимеоффреасон
description: Допустимая причина для выполнения времени ожидания в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 514ca74bb9826546e95f225e394e8fc07a0f674f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866520"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="ae22c-103">Тип ресурса Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="ae22c-103">timeOffReason resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae22c-104">Допустимая причина для экземпляра [тимеофф](timeoff.md) по [расписанию](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="ae22c-104">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ae22c-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ae22c-105">Methods</span></span>

| <span data-ttu-id="ae22c-106">Метод</span><span class="sxs-lookup"><span data-stu-id="ae22c-106">Method</span></span>       | <span data-ttu-id="ae22c-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ae22c-107">Return Type</span></span>  |<span data-ttu-id="ae22c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ae22c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ae22c-109">Создание</span><span class="sxs-lookup"><span data-stu-id="ae22c-109">Create</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="ae22c-110">тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="ae22c-110">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="ae22c-111">Создание нового **тимеоффреасон**.</span><span class="sxs-lookup"><span data-stu-id="ae22c-111">Create a new **timeOffReason**.</span></span>|
|[<span data-ttu-id="ae22c-112">List</span><span class="sxs-lookup"><span data-stu-id="ae22c-112">List</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="ae22c-113">Коллекция [тимеоффреасон](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="ae22c-113">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="ae22c-114">Получение списка **тимеоффреасон** по расписанию.</span><span class="sxs-lookup"><span data-stu-id="ae22c-114">Get the list of **timeOffReason** in a schedule.</span></span>|
|<span data-ttu-id="ae22c-115">[получение](../api/timeoffreason-get.md);</span><span class="sxs-lookup"><span data-stu-id="ae22c-115">[Get](../api/timeoffreason-get.md)</span></span> | [<span data-ttu-id="ae22c-116">тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="ae22c-116">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="ae22c-117">Получение **тимеоффреасон** по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="ae22c-117">Get a **timeOffReason** by ID.</span></span>|
|[<span data-ttu-id="ae22c-118">Replace</span><span class="sxs-lookup"><span data-stu-id="ae22c-118">Replace</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="ae22c-119">тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="ae22c-119">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="ae22c-120">Замените **тимеоффреасон**.</span><span class="sxs-lookup"><span data-stu-id="ae22c-120">Replace a **timeOffReason**.</span></span>|
|<span data-ttu-id="ae22c-121">[удаление](../api/timeoffreason-delete.md);</span><span class="sxs-lookup"><span data-stu-id="ae22c-121">[Delete](../api/timeoffreason-delete.md)</span></span> | <span data-ttu-id="ae22c-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="ae22c-122">None</span></span> | <span data-ttu-id="ae22c-123">Пометка **тимеоффреасон** как неактивной.</span><span class="sxs-lookup"><span data-stu-id="ae22c-123">Mark a **timeOffReason** as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="ae22c-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae22c-124">Properties</span></span>
|<span data-ttu-id="ae22c-125">Имя</span><span class="sxs-lookup"><span data-stu-id="ae22c-125">Name</span></span>          |<span data-ttu-id="ae22c-126">Тип</span><span class="sxs-lookup"><span data-stu-id="ae22c-126">Type</span></span>           |<span data-ttu-id="ae22c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ae22c-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="ae22c-128">id</span><span class="sxs-lookup"><span data-stu-id="ae22c-128">id</span></span>            |`string`      |<span data-ttu-id="ae22c-129">Идентификатор объекта `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="ae22c-129">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="ae22c-130">displayName</span><span class="sxs-lookup"><span data-stu-id="ae22c-130">displayName</span></span>               | `string`                  | <span data-ttu-id="ae22c-131">Имя ресурса `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="ae22c-131">The name of the `timeOffReason`.</span></span> <span data-ttu-id="ae22c-132">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="ae22c-132">Required.</span></span> |
| <span data-ttu-id="ae22c-133">иконтипе</span><span class="sxs-lookup"><span data-stu-id="ae22c-133">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="ae22c-134">Поддерживаемые типы значков: нет; Мойка ведения запускается ходил Фирстаид; врача Нотворкинг; регистрации Журидути; любой кружк звонков Погода Общий Пиггибанк; Dog очень Траффикконе; крепления Веселая.</span><span class="sxs-lookup"><span data-stu-id="ae22c-134">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="ae22c-135">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="ae22c-135">Required.</span></span> |
| <span data-ttu-id="ae22c-136">isActive</span><span class="sxs-lookup"><span data-stu-id="ae22c-136">isActive</span></span>          |`Boolean`      | <span data-ttu-id="ae22c-137">Указывает, можно ли использовать объект `timeOffReason` при создании новых сущностей или обновлении существующих.</span><span class="sxs-lookup"><span data-stu-id="ae22c-137">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="ae22c-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae22c-138">Required.</span></span> |
| <span data-ttu-id="ae22c-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae22c-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="ae22c-140">Отметка `timeOffReason` времени первоначального создания.</span><span class="sxs-lookup"><span data-stu-id="ae22c-140">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="ae22c-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ae22c-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ae22c-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="ae22c-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="ae22c-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae22c-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="ae22c-144">Отметка `timeOffReason` времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="ae22c-144">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="ae22c-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ae22c-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ae22c-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="ae22c-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="ae22c-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ae22c-147">lastModifiedBy</span></span>        | [<span data-ttu-id="ae22c-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="ae22c-148">identitySet</span></span>](identityset.md)        |<span data-ttu-id="ae22c-149">Учетная запись, которая последней обновила этот объект `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="ae22c-149">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae22c-150">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ae22c-150">JSON representation</span></span>

<span data-ttu-id="ae22c-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae22c-151">Here is a JSON representation of the resource.</span></span>

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
