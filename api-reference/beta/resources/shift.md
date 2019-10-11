---
title: Тип ресурса shift
description: Смена — это единица запланированных трудозатрат в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d3a91cd7b4f2b4d8e32219514d1190599ac416de
ms.sourcegitcommit: a700f1c283a5d847cd1697e26bcd47bc8625384e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2019
ms.locfileid: "36049633"
---
# <a name="shift-resource-type"></a><span data-ttu-id="d38be-103">Тип ресурса shift</span><span class="sxs-lookup"><span data-stu-id="d38be-103">shift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d38be-104">Единица запланированных трудозатрат в [расписании](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="d38be-104">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="d38be-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d38be-105">Methods</span></span>

| <span data-ttu-id="d38be-106">Метод</span><span class="sxs-lookup"><span data-stu-id="d38be-106">Method</span></span>       | <span data-ttu-id="d38be-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d38be-107">Return Type</span></span>  |<span data-ttu-id="d38be-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d38be-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d38be-109">Создание смены</span><span class="sxs-lookup"><span data-stu-id="d38be-109">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="d38be-110">shift</span><span class="sxs-lookup"><span data-stu-id="d38be-110">Shift</span></span>](shift.md) | <span data-ttu-id="d38be-111">Создание объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="d38be-111">Create a new `shift`.</span></span>|
|[<span data-ttu-id="d38be-112">Перечисление смен</span><span class="sxs-lookup"><span data-stu-id="d38be-112">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="d38be-113">Коллекция [shift](shift.md)</span><span class="sxs-lookup"><span data-stu-id="d38be-113">[shift](shift.md) collection</span></span> | <span data-ttu-id="d38be-114">Получение списка объектов `shifts` в расписании.</span><span class="sxs-lookup"><span data-stu-id="d38be-114">Get the list of `shifts` in a schedule.</span></span>|
|[<span data-ttu-id="d38be-115">Получение смены</span><span class="sxs-lookup"><span data-stu-id="d38be-115">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="d38be-116">shift</span><span class="sxs-lookup"><span data-stu-id="d38be-116">Shift</span></span>](shift.md) | <span data-ttu-id="d38be-117">Получение `shift` по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="d38be-117">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="d38be-118">Замена смены</span><span class="sxs-lookup"><span data-stu-id="d38be-118">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="d38be-119">shift</span><span class="sxs-lookup"><span data-stu-id="d38be-119">Shift</span></span>](shift.md) | <span data-ttu-id="d38be-120">Замена объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="d38be-120">Replace a `shift`.</span></span>|
|[<span data-ttu-id="d38be-121">Удаление смены</span><span class="sxs-lookup"><span data-stu-id="d38be-121">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="d38be-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d38be-122">None</span></span> | <span data-ttu-id="d38be-123">Удаление объекта `shift` из расписания.</span><span class="sxs-lookup"><span data-stu-id="d38be-123">Delete a theme from the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="d38be-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="d38be-124">Properties</span></span>
|<span data-ttu-id="d38be-125">Имя</span><span class="sxs-lookup"><span data-stu-id="d38be-125">Name</span></span>          |<span data-ttu-id="d38be-126">Тип</span><span class="sxs-lookup"><span data-stu-id="d38be-126">Type</span></span>           |<span data-ttu-id="d38be-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d38be-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d38be-128">id</span><span class="sxs-lookup"><span data-stu-id="d38be-128">id</span></span>            |`string`      |<span data-ttu-id="d38be-129">Идентификатор объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="d38be-129">ID of the `shift`.</span></span>|
| <span data-ttu-id="d38be-130">userId</span><span class="sxs-lookup"><span data-stu-id="d38be-130">userId</span></span>            |`string`      |<span data-ttu-id="d38be-131">Идентификатор пользователя, назначенного объекту `shift`.</span><span class="sxs-lookup"><span data-stu-id="d38be-131">Integer specifying the ID of the user to whom the task is assigned.</span></span> <span data-ttu-id="d38be-132">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d38be-132">Required.</span></span> |
| <span data-ttu-id="d38be-133">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="d38be-133">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="d38be-134">Идентификатор группы планирования, частью которой является объект `shift`.</span><span class="sxs-lookup"><span data-stu-id="d38be-134">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="d38be-135">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d38be-135">Required.</span></span> |
| <span data-ttu-id="d38be-136">sharedShift</span><span class="sxs-lookup"><span data-stu-id="d38be-136">sharedShift</span></span>   |[<span data-ttu-id="d38be-137">shiftItem</span><span class="sxs-lookup"><span data-stu-id="d38be-137">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="d38be-138">Общая версия объекта `shift`, доступная для просмотра как сотрудникам, так и руководителям.</span><span class="sxs-lookup"><span data-stu-id="d38be-138">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="d38be-139">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d38be-139">Required.</span></span> |
| <span data-ttu-id="d38be-140">draftShift</span><span class="sxs-lookup"><span data-stu-id="d38be-140">draftShift</span></span>        |[<span data-ttu-id="d38be-141">shiftItem</span><span class="sxs-lookup"><span data-stu-id="d38be-141">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="d38be-142">Черновая версия объекта `shift`, доступная для просмотра руководителями.</span><span class="sxs-lookup"><span data-stu-id="d38be-142">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="d38be-143">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d38be-143">Required.</span></span> |
| <span data-ttu-id="d38be-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d38be-144">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="d38be-145">Метка времени создания объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="d38be-145">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="d38be-146">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d38be-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d38be-147">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="d38be-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="d38be-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d38be-148">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="d38be-149">Метка времени последнего обновления объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="d38be-149">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="d38be-150">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d38be-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d38be-151">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="d38be-151">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="d38be-152">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d38be-152">lastModifiedBy</span></span>        | [<span data-ttu-id="d38be-153">identitySet</span><span class="sxs-lookup"><span data-stu-id="d38be-153">identitySet</span></span>](identityset.md)        |<span data-ttu-id="d38be-154">Учетная запись, которая последней обновила этот объект `shift`.</span><span class="sxs-lookup"><span data-stu-id="d38be-154">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d38be-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d38be-155">JSON representation</span></span>

<span data-ttu-id="d38be-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d38be-156">Here is a JSON representation of the resource.</span></span>

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
