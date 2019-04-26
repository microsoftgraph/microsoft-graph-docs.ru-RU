---
title: Тип ресурса Shift
description: Смена — это единица запланированной работы в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f5c66d0f555ae6e5740883ed72964a8fa36df303
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343053"
---
# <a name="shift-resource-type"></a><span data-ttu-id="bb20d-103">Тип ресурса Shift</span><span class="sxs-lookup"><span data-stu-id="bb20d-103">shift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb20d-104">Единица запланированной работы по [расписанию](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="bb20d-104">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="bb20d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="bb20d-105">Methods</span></span>

| <span data-ttu-id="bb20d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="bb20d-106">Method</span></span>       | <span data-ttu-id="bb20d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bb20d-107">Return Type</span></span>  |<span data-ttu-id="bb20d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bb20d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bb20d-109">Создание смены</span><span class="sxs-lookup"><span data-stu-id="bb20d-109">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="bb20d-110">перемещен</span><span class="sxs-lookup"><span data-stu-id="bb20d-110">shift</span></span>](shift.md) | <span data-ttu-id="bb20d-111">Создание объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="bb20d-111">Create a new `shift`.</span></span>|
|[<span data-ttu-id="bb20d-112">ПереЧисление смещений</span><span class="sxs-lookup"><span data-stu-id="bb20d-112">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="bb20d-113">Коллекция " [SHIFT](shift.md) "</span><span class="sxs-lookup"><span data-stu-id="bb20d-113">[shift](shift.md) collection</span></span> | <span data-ttu-id="bb20d-114">Получение списка `shifts` по данному расписанию.</span><span class="sxs-lookup"><span data-stu-id="bb20d-114">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="bb20d-115">Получение Shift</span><span class="sxs-lookup"><span data-stu-id="bb20d-115">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="bb20d-116">перемещен</span><span class="sxs-lookup"><span data-stu-id="bb20d-116">shift</span></span>](shift.md) | <span data-ttu-id="bb20d-117">Получение `shift` по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="bb20d-117">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="bb20d-118">Замена Shift</span><span class="sxs-lookup"><span data-stu-id="bb20d-118">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="bb20d-119">перемещен</span><span class="sxs-lookup"><span data-stu-id="bb20d-119">shift</span></span>](shift.md) | <span data-ttu-id="bb20d-120">Замена объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="bb20d-120">Replace a `shift`.</span></span>|
|[<span data-ttu-id="bb20d-121">Удаление смены</span><span class="sxs-lookup"><span data-stu-id="bb20d-121">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="bb20d-122">Нет</span><span class="sxs-lookup"><span data-stu-id="bb20d-122">None</span></span> | <span data-ttu-id="bb20d-123">Удаление `shift` из расписания.</span><span class="sxs-lookup"><span data-stu-id="bb20d-123">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="bb20d-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb20d-124">Properties</span></span>
|<span data-ttu-id="bb20d-125">Имя</span><span class="sxs-lookup"><span data-stu-id="bb20d-125">Name</span></span>          |<span data-ttu-id="bb20d-126">Тип</span><span class="sxs-lookup"><span data-stu-id="bb20d-126">Type</span></span>           |<span data-ttu-id="bb20d-127">Описание</span><span class="sxs-lookup"><span data-stu-id="bb20d-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="bb20d-128">id</span><span class="sxs-lookup"><span data-stu-id="bb20d-128">id</span></span>            |`string`      |<span data-ttu-id="bb20d-129">Идентификатор объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="bb20d-129">ID of the `shift`.</span></span>|
| <span data-ttu-id="bb20d-130">userId</span><span class="sxs-lookup"><span data-stu-id="bb20d-130">userId</span></span>            |`string`      |<span data-ttu-id="bb20d-131">Идентификатор пользователя, `shift`назначенный.</span><span class="sxs-lookup"><span data-stu-id="bb20d-131">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="bb20d-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb20d-132">Required.</span></span> |
| <span data-ttu-id="bb20d-133">Счедулингграупид</span><span class="sxs-lookup"><span data-stu-id="bb20d-133">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="bb20d-134">Идентификатор группы планирования, в которой `shift` входит.</span><span class="sxs-lookup"><span data-stu-id="bb20d-134">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="bb20d-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb20d-135">Required.</span></span> |
| <span data-ttu-id="bb20d-136">Шаредшифт</span><span class="sxs-lookup"><span data-stu-id="bb20d-136">sharedShift</span></span>   |[<span data-ttu-id="bb20d-137">Шифтитем</span><span class="sxs-lookup"><span data-stu-id="bb20d-137">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="bb20d-138">Общая версия этого `shift` объекта доступна как для сотрудников, так и для руководителей.</span><span class="sxs-lookup"><span data-stu-id="bb20d-138">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="bb20d-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb20d-139">Required.</span></span> |
| <span data-ttu-id="bb20d-140">Драфтшифт</span><span class="sxs-lookup"><span data-stu-id="bb20d-140">draftShift</span></span>        |[<span data-ttu-id="bb20d-141">Шифтитем</span><span class="sxs-lookup"><span data-stu-id="bb20d-141">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="bb20d-142">Черновая версия этого `shift` элемента, просматриваемая руководителями.</span><span class="sxs-lookup"><span data-stu-id="bb20d-142">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="bb20d-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb20d-143">Required.</span></span> |
| <span data-ttu-id="bb20d-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb20d-144">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="bb20d-145">Временная метка, на которую `shift` был создан впервые.</span><span class="sxs-lookup"><span data-stu-id="bb20d-145">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="bb20d-146">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bb20d-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bb20d-147">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="bb20d-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="bb20d-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb20d-148">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="bb20d-149">Отметка времени `shift` последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="bb20d-149">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="bb20d-150">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bb20d-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bb20d-151">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="bb20d-151">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="bb20d-152">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="bb20d-152">lastModifiedBy</span></span>        | [<span data-ttu-id="bb20d-153">identitySet</span><span class="sxs-lookup"><span data-stu-id="bb20d-153">identitySet</span></span>](identityset.md)        |<span data-ttu-id="bb20d-154">Учетная запись, которая последней обновила этот объект `shift`.</span><span class="sxs-lookup"><span data-stu-id="bb20d-154">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb20d-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bb20d-155">JSON representation</span></span>

<span data-ttu-id="bb20d-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb20d-156">Here is a JSON representation of the resource.</span></span>

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
