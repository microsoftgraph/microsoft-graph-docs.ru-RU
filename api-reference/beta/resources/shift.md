---
title: Тип ресурса shift
description: Смена — это единица запланированных трудозатрат в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 49d877859202ca9d8dc5c7b414368a63d2fcf8ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058104"
---
# <a name="shift-resource-type"></a><span data-ttu-id="fa060-103">Тип ресурса shift</span><span class="sxs-lookup"><span data-stu-id="fa060-103">shift resource type</span></span>

<span data-ttu-id="fa060-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa060-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa060-105">Единица запланированных трудозатрат в [расписании](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="fa060-105">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="fa060-106">Методы</span><span class="sxs-lookup"><span data-stu-id="fa060-106">Methods</span></span>

| <span data-ttu-id="fa060-107">Метод</span><span class="sxs-lookup"><span data-stu-id="fa060-107">Method</span></span>       | <span data-ttu-id="fa060-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fa060-108">Return Type</span></span>  |<span data-ttu-id="fa060-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fa060-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fa060-110">Создание смены</span><span class="sxs-lookup"><span data-stu-id="fa060-110">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="fa060-111">shift</span><span class="sxs-lookup"><span data-stu-id="fa060-111">shift</span></span>](shift.md) | <span data-ttu-id="fa060-112">Создание объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="fa060-112">Create a new `shift`.</span></span>|
|[<span data-ttu-id="fa060-113">Перечисление смен</span><span class="sxs-lookup"><span data-stu-id="fa060-113">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="fa060-114">Коллекция [shift](shift.md)</span><span class="sxs-lookup"><span data-stu-id="fa060-114">[shift](shift.md) collection</span></span> | <span data-ttu-id="fa060-115">Получение списка объектов `shifts` в расписании.</span><span class="sxs-lookup"><span data-stu-id="fa060-115">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="fa060-116">Получение смены</span><span class="sxs-lookup"><span data-stu-id="fa060-116">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="fa060-117">shift</span><span class="sxs-lookup"><span data-stu-id="fa060-117">shift</span></span>](shift.md) | <span data-ttu-id="fa060-118">Получение `shift` по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="fa060-118">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="fa060-119">Замена смены</span><span class="sxs-lookup"><span data-stu-id="fa060-119">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="fa060-120">shift</span><span class="sxs-lookup"><span data-stu-id="fa060-120">shift</span></span>](shift.md) | <span data-ttu-id="fa060-121">Замена объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="fa060-121">Replace a `shift`.</span></span>|
|[<span data-ttu-id="fa060-122">Удаление смены</span><span class="sxs-lookup"><span data-stu-id="fa060-122">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="fa060-123">Нет</span><span class="sxs-lookup"><span data-stu-id="fa060-123">None</span></span> | <span data-ttu-id="fa060-124">Удаление объекта `shift` из расписания.</span><span class="sxs-lookup"><span data-stu-id="fa060-124">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="fa060-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa060-125">Properties</span></span>
|<span data-ttu-id="fa060-126">Имя</span><span class="sxs-lookup"><span data-stu-id="fa060-126">Name</span></span>          |<span data-ttu-id="fa060-127">Тип</span><span class="sxs-lookup"><span data-stu-id="fa060-127">Type</span></span>           |<span data-ttu-id="fa060-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fa060-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fa060-129">id</span><span class="sxs-lookup"><span data-stu-id="fa060-129">id</span></span>            |`string`      |<span data-ttu-id="fa060-130">Идентификатор объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="fa060-130">ID of the `shift`.</span></span>|
| <span data-ttu-id="fa060-131">userId</span><span class="sxs-lookup"><span data-stu-id="fa060-131">userId</span></span>            |`string`      |<span data-ttu-id="fa060-132">Идентификатор пользователя, назначенного объекту `shift`.</span><span class="sxs-lookup"><span data-stu-id="fa060-132">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="fa060-133">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="fa060-133">Required.</span></span> |
| <span data-ttu-id="fa060-134">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="fa060-134">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="fa060-135">Идентификатор группы планирования, частью которой является объект `shift`.</span><span class="sxs-lookup"><span data-stu-id="fa060-135">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="fa060-136">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="fa060-136">Required.</span></span> |
| <span data-ttu-id="fa060-137">sharedShift</span><span class="sxs-lookup"><span data-stu-id="fa060-137">sharedShift</span></span>   |[<span data-ttu-id="fa060-138">shiftItem</span><span class="sxs-lookup"><span data-stu-id="fa060-138">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="fa060-139">Общая версия объекта `shift`, доступная для просмотра как сотрудникам, так и руководителям.</span><span class="sxs-lookup"><span data-stu-id="fa060-139">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="fa060-140">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="fa060-140">Required.</span></span> |
| <span data-ttu-id="fa060-141">draftShift</span><span class="sxs-lookup"><span data-stu-id="fa060-141">draftShift</span></span>        |[<span data-ttu-id="fa060-142">shiftItem</span><span class="sxs-lookup"><span data-stu-id="fa060-142">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="fa060-143">Черновая версия объекта `shift`, доступная для просмотра руководителями.</span><span class="sxs-lookup"><span data-stu-id="fa060-143">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="fa060-144">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="fa060-144">Required.</span></span> |
| <span data-ttu-id="fa060-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa060-145">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="fa060-146">Метка времени создания объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="fa060-146">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="fa060-147">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fa060-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fa060-148">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="fa060-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="fa060-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa060-149">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="fa060-150">Метка времени последнего обновления объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="fa060-150">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="fa060-151">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fa060-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fa060-152">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="fa060-152">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="fa060-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="fa060-153">lastModifiedBy</span></span>        | [<span data-ttu-id="fa060-154">identitySet</span><span class="sxs-lookup"><span data-stu-id="fa060-154">identitySet</span></span>](identityset.md)        |<span data-ttu-id="fa060-155">Учетная запись, которая последней обновила этот объект `shift`.</span><span class="sxs-lookup"><span data-stu-id="fa060-155">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa060-156">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fa060-156">JSON representation</span></span>

<span data-ttu-id="fa060-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa060-157">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shift"
}-->

```json
{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedShift": {"@odata.type":"microsoft.graph.shiftItem"},
  "draftShift": {"@odata.type":"microsoft.graph.shiftItem"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


