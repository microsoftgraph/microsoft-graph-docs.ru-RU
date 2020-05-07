---
title: Тип ресурса Тимеоффреасон
description: Представляет допустимую причину для выполнения времени ожидания в расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: ef852fa92217b32812340fd17b14465a5f4cbba3
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154908"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="64d25-103">Тип ресурса Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="64d25-103">timeOffReason resource type</span></span>

<span data-ttu-id="64d25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64d25-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64d25-105">Представляет допустимую причину для экземпляра [тимеофф](timeoff.md) по [расписанию](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="64d25-105">Represents a valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="64d25-106">Методы</span><span class="sxs-lookup"><span data-stu-id="64d25-106">Methods</span></span>

| <span data-ttu-id="64d25-107">Метод</span><span class="sxs-lookup"><span data-stu-id="64d25-107">Method</span></span>       | <span data-ttu-id="64d25-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="64d25-108">Return Type</span></span>  |<span data-ttu-id="64d25-109">Описание</span><span class="sxs-lookup"><span data-stu-id="64d25-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="64d25-110">List</span><span class="sxs-lookup"><span data-stu-id="64d25-110">List</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="64d25-111">Коллекция [тимеоффреасон](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="64d25-111">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="64d25-112">Получение списка **тимеоффреасон** по расписанию.</span><span class="sxs-lookup"><span data-stu-id="64d25-112">Get the list of **timeOffReason** in a schedule.</span></span>|
|<span data-ttu-id="64d25-113">[создание](../api/schedule-post-timeoffreasons.md);</span><span class="sxs-lookup"><span data-stu-id="64d25-113">[Create](../api/schedule-post-timeoffreasons.md)</span></span> | [<span data-ttu-id="64d25-114">тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="64d25-114">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="64d25-115">Создание нового **тимеоффреасон**.</span><span class="sxs-lookup"><span data-stu-id="64d25-115">Create a new **timeOffReason**.</span></span>|
|<span data-ttu-id="64d25-116">[получение](../api/timeoffreason-get.md);</span><span class="sxs-lookup"><span data-stu-id="64d25-116">[Get](../api/timeoffreason-get.md)</span></span> | [<span data-ttu-id="64d25-117">тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="64d25-117">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="64d25-118">Получение **тимеоффреасон** по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="64d25-118">Get a **timeOffReason** by ID.</span></span>|
|[<span data-ttu-id="64d25-119">Replace</span><span class="sxs-lookup"><span data-stu-id="64d25-119">Replace</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="64d25-120">тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="64d25-120">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="64d25-121">Замените **тимеоффреасон**.</span><span class="sxs-lookup"><span data-stu-id="64d25-121">Replace a **timeOffReason**.</span></span>|
|<span data-ttu-id="64d25-122">[удаление](../api/timeoffreason-delete.md);</span><span class="sxs-lookup"><span data-stu-id="64d25-122">[Delete](../api/timeoffreason-delete.md)</span></span> | <span data-ttu-id="64d25-123">Нет</span><span class="sxs-lookup"><span data-stu-id="64d25-123">None</span></span> | <span data-ttu-id="64d25-124">Пометка **тимеоффреасон** как неактивной.</span><span class="sxs-lookup"><span data-stu-id="64d25-124">Mark a **timeOffReason** as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="64d25-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="64d25-125">Properties</span></span>
|<span data-ttu-id="64d25-126">Имя</span><span class="sxs-lookup"><span data-stu-id="64d25-126">Name</span></span>          |<span data-ttu-id="64d25-127">Тип</span><span class="sxs-lookup"><span data-stu-id="64d25-127">Type</span></span>           |<span data-ttu-id="64d25-128">Описание</span><span class="sxs-lookup"><span data-stu-id="64d25-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="64d25-129">id</span><span class="sxs-lookup"><span data-stu-id="64d25-129">id</span></span>            |`string`      |<span data-ttu-id="64d25-130">Идентификатор объекта `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="64d25-130">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="64d25-131">displayName</span><span class="sxs-lookup"><span data-stu-id="64d25-131">displayName</span></span>               | `string`                  | <span data-ttu-id="64d25-132">Имя **тимеоффреасон**.</span><span class="sxs-lookup"><span data-stu-id="64d25-132">The name of the **timeOffReason**.</span></span> <span data-ttu-id="64d25-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64d25-133">Required.</span></span> |
| <span data-ttu-id="64d25-134">иконтипе</span><span class="sxs-lookup"><span data-stu-id="64d25-134">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="64d25-135">Поддерживаемые типы значков: нет; Мойка ведения запускается ходил Фирстаид; врача Нотворкинг; регистрации Журидути; любой кружк звонков Погода Общий Пиггибанк; Dog очень Траффикконе; крепления Веселая.</span><span class="sxs-lookup"><span data-stu-id="64d25-135">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="64d25-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64d25-136">Required.</span></span> |
| <span data-ttu-id="64d25-137">isActive</span><span class="sxs-lookup"><span data-stu-id="64d25-137">isActive</span></span>          |`Boolean`      | <span data-ttu-id="64d25-138">Указывает, можно ли использовать **тимеоффреасон** при создании новых сущностей или обновлении существующих.</span><span class="sxs-lookup"><span data-stu-id="64d25-138">Indicates whether the **timeOffReason** can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="64d25-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64d25-139">Required.</span></span> |
| <span data-ttu-id="64d25-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64d25-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="64d25-141">Отметка времени первоначального создания **тимеоффреасон** .</span><span class="sxs-lookup"><span data-stu-id="64d25-141">The time stamp on which this **timeOffReason** was first created.</span></span> <span data-ttu-id="64d25-142">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="64d25-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="64d25-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="64d25-143">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="64d25-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64d25-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="64d25-145">Отметка времени последнего обновления **тимеоффреасон** .</span><span class="sxs-lookup"><span data-stu-id="64d25-145">The time stamp on which this **timeOffReason** was last updated.</span></span> <span data-ttu-id="64d25-146">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="64d25-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="64d25-147">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="64d25-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="64d25-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="64d25-148">lastModifiedBy</span></span>        | [<span data-ttu-id="64d25-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="64d25-149">identitySet</span></span>](identityset.md)        |<span data-ttu-id="64d25-150">Удостоверение, которое последним обновило этот **тимеоффреасон**.</span><span class="sxs-lookup"><span data-stu-id="64d25-150">The identity that last updated this **timeOffReason**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64d25-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64d25-151">JSON representation</span></span>

<span data-ttu-id="64d25-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64d25-152">The following is a JSON representation of the resource.</span></span>

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
