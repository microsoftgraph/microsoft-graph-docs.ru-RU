---
title: Тип ресурса Тимеоффреасон
description: Допустимая причина для выполнения времени ожидания в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: f9d84ae6b86d7d97af5ec2376879a5961da7367b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519724"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="eee35-103">Тип ресурса Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="eee35-103">timeOffReason resource type</span></span>

<span data-ttu-id="eee35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eee35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eee35-105">Допустимая причина для экземпляра [тимеофф](timeoff.md) по [расписанию](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="eee35-105">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="eee35-106">Методы</span><span class="sxs-lookup"><span data-stu-id="eee35-106">Methods</span></span>

| <span data-ttu-id="eee35-107">Метод</span><span class="sxs-lookup"><span data-stu-id="eee35-107">Method</span></span>       | <span data-ttu-id="eee35-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eee35-108">Return Type</span></span>  |<span data-ttu-id="eee35-109">Описание</span><span class="sxs-lookup"><span data-stu-id="eee35-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eee35-110">Создание</span><span class="sxs-lookup"><span data-stu-id="eee35-110">Create</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="eee35-111">тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="eee35-111">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="eee35-112">Создание нового **тимеоффреасон**.</span><span class="sxs-lookup"><span data-stu-id="eee35-112">Create a new **timeOffReason**.</span></span>|
|[<span data-ttu-id="eee35-113">List</span><span class="sxs-lookup"><span data-stu-id="eee35-113">List</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="eee35-114">Коллекция [тимеоффреасон](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="eee35-114">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="eee35-115">Получение списка **тимеоффреасон** по расписанию.</span><span class="sxs-lookup"><span data-stu-id="eee35-115">Get the list of **timeOffReason** in a schedule.</span></span>|
|<span data-ttu-id="eee35-116">[получение](../api/timeoffreason-get.md);</span><span class="sxs-lookup"><span data-stu-id="eee35-116">[Get](../api/timeoffreason-get.md)</span></span> | [<span data-ttu-id="eee35-117">тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="eee35-117">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="eee35-118">Получение **тимеоффреасон** по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="eee35-118">Get a **timeOffReason** by ID.</span></span>|
|[<span data-ttu-id="eee35-119">Replace</span><span class="sxs-lookup"><span data-stu-id="eee35-119">Replace</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="eee35-120">тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="eee35-120">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="eee35-121">Замените **тимеоффреасон**.</span><span class="sxs-lookup"><span data-stu-id="eee35-121">Replace a **timeOffReason**.</span></span>|
|<span data-ttu-id="eee35-122">[удаление](../api/timeoffreason-delete.md);</span><span class="sxs-lookup"><span data-stu-id="eee35-122">[Delete](../api/timeoffreason-delete.md)</span></span> | <span data-ttu-id="eee35-123">Нет</span><span class="sxs-lookup"><span data-stu-id="eee35-123">None</span></span> | <span data-ttu-id="eee35-124">Пометка **тимеоффреасон** как неактивной.</span><span class="sxs-lookup"><span data-stu-id="eee35-124">Mark a **timeOffReason** as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="eee35-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="eee35-125">Properties</span></span>
|<span data-ttu-id="eee35-126">Имя</span><span class="sxs-lookup"><span data-stu-id="eee35-126">Name</span></span>          |<span data-ttu-id="eee35-127">Тип</span><span class="sxs-lookup"><span data-stu-id="eee35-127">Type</span></span>           |<span data-ttu-id="eee35-128">Описание</span><span class="sxs-lookup"><span data-stu-id="eee35-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="eee35-129">id</span><span class="sxs-lookup"><span data-stu-id="eee35-129">id</span></span>            |`string`      |<span data-ttu-id="eee35-130">Идентификатор объекта `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="eee35-130">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="eee35-131">displayName</span><span class="sxs-lookup"><span data-stu-id="eee35-131">displayName</span></span>               | `string`                  | <span data-ttu-id="eee35-132">Имя ресурса `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="eee35-132">The name of the `timeOffReason`.</span></span> <span data-ttu-id="eee35-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eee35-133">Required.</span></span> |
| <span data-ttu-id="eee35-134">иконтипе</span><span class="sxs-lookup"><span data-stu-id="eee35-134">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="eee35-135">Поддерживаемые типы значков: нет; Мойка ведения запускается ходил Фирстаид; врача Нотворкинг; регистрации Журидути; любой кружк звонков Погода Общий Пиггибанк; Dog очень Траффикконе; крепления Веселая.</span><span class="sxs-lookup"><span data-stu-id="eee35-135">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="eee35-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eee35-136">Required.</span></span> |
| <span data-ttu-id="eee35-137">isActive</span><span class="sxs-lookup"><span data-stu-id="eee35-137">isActive</span></span>          |`Boolean`      | <span data-ttu-id="eee35-138">Указывает, можно ли использовать объект `timeOffReason` при создании новых сущностей или обновлении существующих.</span><span class="sxs-lookup"><span data-stu-id="eee35-138">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="eee35-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eee35-139">Required.</span></span> |
| <span data-ttu-id="eee35-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eee35-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="eee35-141">Отметка `timeOffReason` времени первоначального создания.</span><span class="sxs-lookup"><span data-stu-id="eee35-141">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="eee35-142">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="eee35-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eee35-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="eee35-143">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="eee35-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eee35-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="eee35-145">Отметка `timeOffReason` времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="eee35-145">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="eee35-146">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="eee35-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eee35-147">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="eee35-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="eee35-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="eee35-148">lastModifiedBy</span></span>        | [<span data-ttu-id="eee35-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="eee35-149">identitySet</span></span>](identityset.md)        |<span data-ttu-id="eee35-150">Учетная запись, которая последней обновила этот объект `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="eee35-150">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eee35-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="eee35-151">JSON representation</span></span>

<span data-ttu-id="eee35-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eee35-152">Here is a JSON representation of the resource.</span></span>

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
