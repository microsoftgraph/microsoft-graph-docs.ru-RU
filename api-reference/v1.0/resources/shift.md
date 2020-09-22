---
title: Тип ресурса shift
description: Представляет единицу измерения трудозатрат по расписанию.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 52c83c8052725e99d1136df8b0c14d8d3c24ffe4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086433"
---
# <a name="shift-resource-type"></a><span data-ttu-id="07628-103">Тип ресурса shift</span><span class="sxs-lookup"><span data-stu-id="07628-103">shift resource type</span></span>

<span data-ttu-id="07628-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07628-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="07628-105">Представляет единицу измерения запланированной работы по [расписанию](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="07628-105">Represents a unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="07628-106">Методы</span><span class="sxs-lookup"><span data-stu-id="07628-106">Methods</span></span>

| <span data-ttu-id="07628-107">Метод</span><span class="sxs-lookup"><span data-stu-id="07628-107">Method</span></span>       | <span data-ttu-id="07628-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="07628-108">Return Type</span></span>  |<span data-ttu-id="07628-109">Описание</span><span class="sxs-lookup"><span data-stu-id="07628-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="07628-110">Перечисление смен</span><span class="sxs-lookup"><span data-stu-id="07628-110">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="07628-111">Коллекция [shift](shift.md)</span><span class="sxs-lookup"><span data-stu-id="07628-111">[shift](shift.md) collection</span></span> | <span data-ttu-id="07628-112">Получение списка **смен** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="07628-112">Get the list of **shifts** in this schedule.</span></span>|
|[<span data-ttu-id="07628-113">Создание смены</span><span class="sxs-lookup"><span data-stu-id="07628-113">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="07628-114">shift</span><span class="sxs-lookup"><span data-stu-id="07628-114">shift</span></span>](shift.md) | <span data-ttu-id="07628-115">Создайте новую **смену**.</span><span class="sxs-lookup"><span data-stu-id="07628-115">Create a new **shift**.</span></span>|
|[<span data-ttu-id="07628-116">Получение смены</span><span class="sxs-lookup"><span data-stu-id="07628-116">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="07628-117">shift</span><span class="sxs-lookup"><span data-stu-id="07628-117">shift</span></span>](shift.md) | <span data-ttu-id="07628-118">Получение **сдвига** по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="07628-118">Get a **shift** by ID.</span></span>|
|[<span data-ttu-id="07628-119">Замена смены</span><span class="sxs-lookup"><span data-stu-id="07628-119">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="07628-120">shift</span><span class="sxs-lookup"><span data-stu-id="07628-120">shift</span></span>](shift.md) | <span data-ttu-id="07628-121">Замените **смену**.</span><span class="sxs-lookup"><span data-stu-id="07628-121">Replace a **shift**.</span></span>|
|[<span data-ttu-id="07628-122">Удаление смены</span><span class="sxs-lookup"><span data-stu-id="07628-122">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="07628-123">Нет</span><span class="sxs-lookup"><span data-stu-id="07628-123">None</span></span> | <span data-ttu-id="07628-124">Удалить **смену** из расписания.</span><span class="sxs-lookup"><span data-stu-id="07628-124">Delete a **shift** from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="07628-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="07628-125">Properties</span></span>
|<span data-ttu-id="07628-126">Имя</span><span class="sxs-lookup"><span data-stu-id="07628-126">Name</span></span>          |<span data-ttu-id="07628-127">Тип</span><span class="sxs-lookup"><span data-stu-id="07628-127">Type</span></span>           |<span data-ttu-id="07628-128">Описание</span><span class="sxs-lookup"><span data-stu-id="07628-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="07628-129">id</span><span class="sxs-lookup"><span data-stu-id="07628-129">id</span></span>            |`string`      |<span data-ttu-id="07628-130">Идентификатор **смены**.</span><span class="sxs-lookup"><span data-stu-id="07628-130">ID of the **shift**.</span></span>|
| <span data-ttu-id="07628-131">userId</span><span class="sxs-lookup"><span data-stu-id="07628-131">userId</span></span>            |`string`      |<span data-ttu-id="07628-132">Идентификатор пользователя, назначенный **смене**.</span><span class="sxs-lookup"><span data-stu-id="07628-132">ID of the user assigned to the **shift**.</span></span> <span data-ttu-id="07628-133">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="07628-133">Required.</span></span> |
| <span data-ttu-id="07628-134">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="07628-134">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="07628-135">Идентификатор группы планирования, частью которой является **Смена** .</span><span class="sxs-lookup"><span data-stu-id="07628-135">ID of the scheduling group the **shift** is part of.</span></span> <span data-ttu-id="07628-136">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="07628-136">Required.</span></span> |
| <span data-ttu-id="07628-137">sharedShift</span><span class="sxs-lookup"><span data-stu-id="07628-137">sharedShift</span></span>   |[<span data-ttu-id="07628-138">shiftItem</span><span class="sxs-lookup"><span data-stu-id="07628-138">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="07628-139">Общая версия этой **смены** , отображаемая как для сотрудников, так и для руководителей.</span><span class="sxs-lookup"><span data-stu-id="07628-139">The shared version of this **shift** that is viewable by both employees and managers.</span></span> <span data-ttu-id="07628-140">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="07628-140">Required.</span></span> |
| <span data-ttu-id="07628-141">draftShift</span><span class="sxs-lookup"><span data-stu-id="07628-141">draftShift</span></span>        |[<span data-ttu-id="07628-142">shiftItem</span><span class="sxs-lookup"><span data-stu-id="07628-142">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="07628-143">Черновая версия этой **смены** , которая отображается руководителями.</span><span class="sxs-lookup"><span data-stu-id="07628-143">The draft version of this **shift** that is viewable by managers.</span></span> <span data-ttu-id="07628-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07628-144">Required.</span></span> |
| <span data-ttu-id="07628-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07628-145">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="07628-146">Временная метка, на которую было впервые создана эта **Смена** .</span><span class="sxs-lookup"><span data-stu-id="07628-146">The timestamp on which this **shift** was first created.</span></span> <span data-ttu-id="07628-147">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="07628-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="07628-148">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="07628-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="07628-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07628-149">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="07628-150">Временная метка, на которую было Последнее обновление этой **смены** .</span><span class="sxs-lookup"><span data-stu-id="07628-150">The timestamp on which this **shift** was last updated.</span></span> <span data-ttu-id="07628-151">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="07628-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="07628-152">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="07628-152">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="07628-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="07628-153">lastModifiedBy</span></span>        | [<span data-ttu-id="07628-154">identitySet</span><span class="sxs-lookup"><span data-stu-id="07628-154">identitySet</span></span>](identityset.md)        |<span data-ttu-id="07628-155">Идентификатор, который последним обновил этот **сдвиг**.</span><span class="sxs-lookup"><span data-stu-id="07628-155">The identity that last updated this **shift**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07628-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07628-156">JSON representation</span></span>

<span data-ttu-id="07628-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07628-157">The following is a JSON representation of the resource.</span></span>

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

