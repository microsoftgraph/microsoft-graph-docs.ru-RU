---
title: Тип ресурса Shift
description: Смена — это единица запланированной работы в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: f76cd25a36ba070d9fa8281f31a1520a0d7b4435
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008350"
---
# <a name="shift-resource-type"></a><span data-ttu-id="9034f-103">Тип ресурса Shift</span><span class="sxs-lookup"><span data-stu-id="9034f-103">shift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9034f-104">Единица запланированной работы по [расписанию](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="9034f-104">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="9034f-105">Методы</span><span class="sxs-lookup"><span data-stu-id="9034f-105">Methods</span></span>

| <span data-ttu-id="9034f-106">Метод</span><span class="sxs-lookup"><span data-stu-id="9034f-106">Method</span></span>       | <span data-ttu-id="9034f-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9034f-107">Return Type</span></span>  |<span data-ttu-id="9034f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9034f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9034f-109">Создание смены</span><span class="sxs-lookup"><span data-stu-id="9034f-109">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="9034f-110">перемещен</span><span class="sxs-lookup"><span data-stu-id="9034f-110">shift</span></span>](shift.md) | <span data-ttu-id="9034f-111">Создание объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="9034f-111">Create a new `shift`.</span></span>|
|[<span data-ttu-id="9034f-112">Перечисление смещений</span><span class="sxs-lookup"><span data-stu-id="9034f-112">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="9034f-113">Коллекция " [SHIFT](shift.md) "</span><span class="sxs-lookup"><span data-stu-id="9034f-113">[shift](shift.md) collection</span></span> | <span data-ttu-id="9034f-114">Получение списка `shifts` по данному расписанию.</span><span class="sxs-lookup"><span data-stu-id="9034f-114">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="9034f-115">Получение Shift</span><span class="sxs-lookup"><span data-stu-id="9034f-115">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="9034f-116">перемещен</span><span class="sxs-lookup"><span data-stu-id="9034f-116">shift</span></span>](shift.md) | <span data-ttu-id="9034f-117">Получение `shift` по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="9034f-117">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="9034f-118">Замена Shift</span><span class="sxs-lookup"><span data-stu-id="9034f-118">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="9034f-119">перемещен</span><span class="sxs-lookup"><span data-stu-id="9034f-119">shift</span></span>](shift.md) | <span data-ttu-id="9034f-120">Замена объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="9034f-120">Replace a `shift`.</span></span>|
|[<span data-ttu-id="9034f-121">Удаление смены</span><span class="sxs-lookup"><span data-stu-id="9034f-121">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="9034f-122">Нет</span><span class="sxs-lookup"><span data-stu-id="9034f-122">None</span></span> | <span data-ttu-id="9034f-123">Удаление `shift` из расписания.</span><span class="sxs-lookup"><span data-stu-id="9034f-123">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="9034f-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="9034f-124">Properties</span></span>
|<span data-ttu-id="9034f-125">Имя</span><span class="sxs-lookup"><span data-stu-id="9034f-125">Name</span></span>          |<span data-ttu-id="9034f-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9034f-126">Type</span></span>           |<span data-ttu-id="9034f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9034f-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9034f-128">id</span><span class="sxs-lookup"><span data-stu-id="9034f-128">id</span></span>            |`string`      |<span data-ttu-id="9034f-129">Идентификатор объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="9034f-129">ID of the `shift`.</span></span>|
| <span data-ttu-id="9034f-130">userId</span><span class="sxs-lookup"><span data-stu-id="9034f-130">userId</span></span>            |`string`      |<span data-ttu-id="9034f-131">Идентификатор пользователя, `shift`назначенный.</span><span class="sxs-lookup"><span data-stu-id="9034f-131">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="9034f-132">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9034f-132">Required.</span></span> |
| <span data-ttu-id="9034f-133">Счедулингграупид</span><span class="sxs-lookup"><span data-stu-id="9034f-133">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="9034f-134">Идентификатор группы планирования, в которой `shift` входит.</span><span class="sxs-lookup"><span data-stu-id="9034f-134">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="9034f-135">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9034f-135">Required.</span></span> |
| <span data-ttu-id="9034f-136">Шаредшифт</span><span class="sxs-lookup"><span data-stu-id="9034f-136">sharedShift</span></span>   |[<span data-ttu-id="9034f-137">Шифтитем</span><span class="sxs-lookup"><span data-stu-id="9034f-137">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="9034f-138">Общая версия этого `shift` объекта доступна как для сотрудников, так и для руководителей.</span><span class="sxs-lookup"><span data-stu-id="9034f-138">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="9034f-139">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9034f-139">Required.</span></span> |
| <span data-ttu-id="9034f-140">Драфтшифт</span><span class="sxs-lookup"><span data-stu-id="9034f-140">draftShift</span></span>        |[<span data-ttu-id="9034f-141">Шифтитем</span><span class="sxs-lookup"><span data-stu-id="9034f-141">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="9034f-142">Черновая версия этого `shift` элемента, просматриваемая руководителями.</span><span class="sxs-lookup"><span data-stu-id="9034f-142">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="9034f-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9034f-143">Required.</span></span> |
| <span data-ttu-id="9034f-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9034f-144">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="9034f-145">Временная метка, на которую `shift` был создан впервые.</span><span class="sxs-lookup"><span data-stu-id="9034f-145">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="9034f-146">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9034f-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9034f-147">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="9034f-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="9034f-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9034f-148">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="9034f-149">Отметка времени `shift` последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="9034f-149">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="9034f-150">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9034f-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9034f-151">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="9034f-151">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="9034f-152">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="9034f-152">lastModifiedBy</span></span>        | [<span data-ttu-id="9034f-153">identitySet</span><span class="sxs-lookup"><span data-stu-id="9034f-153">identitySet</span></span>](identityset.md)        |<span data-ttu-id="9034f-154">Учетная запись, которая последней обновила этот объект `shift`.</span><span class="sxs-lookup"><span data-stu-id="9034f-154">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9034f-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9034f-155">JSON representation</span></span>

<span data-ttu-id="9034f-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9034f-156">Here is a JSON representation of the resource.</span></span>

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
