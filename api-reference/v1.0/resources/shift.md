---
title: Тип ресурса shift
description: Представляет блок запланированных работ в расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e8c871e580818d96edcb0eae244c88c7edcc128c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721840"
---
# <a name="shift-resource-type"></a><span data-ttu-id="4e86f-103">Тип ресурса shift</span><span class="sxs-lookup"><span data-stu-id="4e86f-103">shift resource type</span></span>

<span data-ttu-id="4e86f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e86f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e86f-105">Представляет единицу запланированных работ в [расписании.](schedule.md)</span><span class="sxs-lookup"><span data-stu-id="4e86f-105">Represents a unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="4e86f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4e86f-106">Methods</span></span>

| <span data-ttu-id="4e86f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4e86f-107">Method</span></span>       | <span data-ttu-id="4e86f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4e86f-108">Return Type</span></span>  |<span data-ttu-id="4e86f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4e86f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4e86f-110">Перечисление смен</span><span class="sxs-lookup"><span data-stu-id="4e86f-110">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="4e86f-111">Коллекция [shift](shift.md)</span><span class="sxs-lookup"><span data-stu-id="4e86f-111">[shift](shift.md) collection</span></span> | <span data-ttu-id="4e86f-112">Получите список **сдвигов в** этом расписании.</span><span class="sxs-lookup"><span data-stu-id="4e86f-112">Get the list of **shifts** in this schedule.</span></span>|
|[<span data-ttu-id="4e86f-113">Создание смены</span><span class="sxs-lookup"><span data-stu-id="4e86f-113">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="4e86f-114">shift</span><span class="sxs-lookup"><span data-stu-id="4e86f-114">shift</span></span>](shift.md) | <span data-ttu-id="4e86f-115">Создайте новую **смену.**</span><span class="sxs-lookup"><span data-stu-id="4e86f-115">Create a new **shift**.</span></span>|
|[<span data-ttu-id="4e86f-116">Получение смены</span><span class="sxs-lookup"><span data-stu-id="4e86f-116">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="4e86f-117">shift</span><span class="sxs-lookup"><span data-stu-id="4e86f-117">shift</span></span>](shift.md) | <span data-ttu-id="4e86f-118">Получите **смену** по ID.</span><span class="sxs-lookup"><span data-stu-id="4e86f-118">Get a **shift** by ID.</span></span>|
|[<span data-ttu-id="4e86f-119">Замена смены</span><span class="sxs-lookup"><span data-stu-id="4e86f-119">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="4e86f-120">shift</span><span class="sxs-lookup"><span data-stu-id="4e86f-120">shift</span></span>](shift.md) | <span data-ttu-id="4e86f-121">Замените **смену**.</span><span class="sxs-lookup"><span data-stu-id="4e86f-121">Replace a **shift**.</span></span>|
|[<span data-ttu-id="4e86f-122">Удаление смены</span><span class="sxs-lookup"><span data-stu-id="4e86f-122">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="4e86f-123">Нет</span><span class="sxs-lookup"><span data-stu-id="4e86f-123">None</span></span> | <span data-ttu-id="4e86f-124">Удаление **переноса** из расписания.</span><span class="sxs-lookup"><span data-stu-id="4e86f-124">Delete a **shift** from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="4e86f-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e86f-125">Properties</span></span>
|<span data-ttu-id="4e86f-126">Имя</span><span class="sxs-lookup"><span data-stu-id="4e86f-126">Name</span></span>          |<span data-ttu-id="4e86f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4e86f-127">Type</span></span>           |<span data-ttu-id="4e86f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4e86f-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4e86f-129">id</span><span class="sxs-lookup"><span data-stu-id="4e86f-129">id</span></span>            |`string`      |<span data-ttu-id="4e86f-130">ID **смены**.</span><span class="sxs-lookup"><span data-stu-id="4e86f-130">ID of the **shift**.</span></span>|
| <span data-ttu-id="4e86f-131">userId</span><span class="sxs-lookup"><span data-stu-id="4e86f-131">userId</span></span>            |`string`      |<span data-ttu-id="4e86f-132">ID пользователя, назначенного на **смену.**</span><span class="sxs-lookup"><span data-stu-id="4e86f-132">ID of the user assigned to the **shift**.</span></span> <span data-ttu-id="4e86f-133">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="4e86f-133">Required.</span></span> |
| <span data-ttu-id="4e86f-134">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="4e86f-134">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="4e86f-135">ID группы планирования **является** частью смены.</span><span class="sxs-lookup"><span data-stu-id="4e86f-135">ID of the scheduling group the **shift** is part of.</span></span> <span data-ttu-id="4e86f-136">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="4e86f-136">Required.</span></span> |
| <span data-ttu-id="4e86f-137">sharedShift</span><span class="sxs-lookup"><span data-stu-id="4e86f-137">sharedShift</span></span>   |[<span data-ttu-id="4e86f-138">shiftItem</span><span class="sxs-lookup"><span data-stu-id="4e86f-138">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="4e86f-139">Общая версия этого **изменения,** которая просматривается как сотрудниками, так и руководителями.</span><span class="sxs-lookup"><span data-stu-id="4e86f-139">The shared version of this **shift** that is viewable by both employees and managers.</span></span> <span data-ttu-id="4e86f-140">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="4e86f-140">Required.</span></span> |
| <span data-ttu-id="4e86f-141">draftShift</span><span class="sxs-lookup"><span data-stu-id="4e86f-141">draftShift</span></span>        |[<span data-ttu-id="4e86f-142">shiftItem</span><span class="sxs-lookup"><span data-stu-id="4e86f-142">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="4e86f-143">Черновик версии этого **изменения,** который просматривается руководителями.</span><span class="sxs-lookup"><span data-stu-id="4e86f-143">The draft version of this **shift** that is viewable by managers.</span></span> <span data-ttu-id="4e86f-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e86f-144">Required.</span></span> |
| <span data-ttu-id="4e86f-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e86f-145">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="4e86f-146">Время создания этой смены. </span><span class="sxs-lookup"><span data-stu-id="4e86f-146">The timestamp on which this **shift** was first created.</span></span> <span data-ttu-id="4e86f-147">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4e86f-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4e86f-148">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="4e86f-148">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="4e86f-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e86f-149">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="4e86f-150">Время последнего обновления  этого переноса.</span><span class="sxs-lookup"><span data-stu-id="4e86f-150">The timestamp on which this **shift** was last updated.</span></span> <span data-ttu-id="4e86f-151">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4e86f-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4e86f-152">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="4e86f-152">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="4e86f-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4e86f-153">lastModifiedBy</span></span>        | [<span data-ttu-id="4e86f-154">identitySet</span><span class="sxs-lookup"><span data-stu-id="4e86f-154">identitySet</span></span>](identityset.md)        |<span data-ttu-id="4e86f-155">Удостоверение, которое в последний раз обновило этот **сдвиг.**</span><span class="sxs-lookup"><span data-stu-id="4e86f-155">The identity that last updated this **shift**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e86f-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e86f-156">JSON representation</span></span>

<span data-ttu-id="4e86f-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e86f-157">The following is a JSON representation of the resource.</span></span>

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

