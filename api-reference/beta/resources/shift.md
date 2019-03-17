---
title: Тип ресурса Shift
description: Смена — это единица запланированной работы в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c392bfb4a1691ab99d852febdda27cdf1c3b8044
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657898"
---
# <a name="shift-resource-type"></a><span data-ttu-id="1d1ac-103">Тип ресурса Shift</span><span class="sxs-lookup"><span data-stu-id="1d1ac-103">shift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d1ac-104">Единица запланированной работы по [расписанию](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="1d1ac-104">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="1d1ac-105">Методы</span><span class="sxs-lookup"><span data-stu-id="1d1ac-105">Methods</span></span>

| <span data-ttu-id="1d1ac-106">Метод</span><span class="sxs-lookup"><span data-stu-id="1d1ac-106">Method</span></span>       | <span data-ttu-id="1d1ac-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1d1ac-107">Return Type</span></span>  |<span data-ttu-id="1d1ac-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1d1ac-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1d1ac-109">Создание смены</span><span class="sxs-lookup"><span data-stu-id="1d1ac-109">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="1d1ac-110">перемещен</span><span class="sxs-lookup"><span data-stu-id="1d1ac-110">shift</span></span>](shift.md) | <span data-ttu-id="1d1ac-111">Создание нового `shift`объекта.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-111">Create a new `shift`.</span></span>|
|[<span data-ttu-id="1d1ac-112">ПереЧисление смещений</span><span class="sxs-lookup"><span data-stu-id="1d1ac-112">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="1d1ac-113">Коллекция " [SHIFT](shift.md) "</span><span class="sxs-lookup"><span data-stu-id="1d1ac-113">[shift](shift.md) collection</span></span> | <span data-ttu-id="1d1ac-114">Получение списка `shifts` по данному расписанию.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-114">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="1d1ac-115">Получение Shift</span><span class="sxs-lookup"><span data-stu-id="1d1ac-115">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="1d1ac-116">перемещен</span><span class="sxs-lookup"><span data-stu-id="1d1ac-116">shift</span></span>](shift.md) | <span data-ttu-id="1d1ac-117">Получение `shift` по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-117">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="1d1ac-118">Замена Shift</span><span class="sxs-lookup"><span data-stu-id="1d1ac-118">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="1d1ac-119">перемещен</span><span class="sxs-lookup"><span data-stu-id="1d1ac-119">shift</span></span>](shift.md) | <span data-ttu-id="1d1ac-120">Замените элемент `shift`.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-120">Replace a `shift`.</span></span>|
|[<span data-ttu-id="1d1ac-121">Удаление смены</span><span class="sxs-lookup"><span data-stu-id="1d1ac-121">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="1d1ac-122">Нет</span><span class="sxs-lookup"><span data-stu-id="1d1ac-122">None</span></span> | <span data-ttu-id="1d1ac-123">Удаление `shift` из расписания.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-123">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="1d1ac-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d1ac-124">Properties</span></span>
|<span data-ttu-id="1d1ac-125">Имя</span><span class="sxs-lookup"><span data-stu-id="1d1ac-125">Name</span></span>          |<span data-ttu-id="1d1ac-126">Тип</span><span class="sxs-lookup"><span data-stu-id="1d1ac-126">Type</span></span>           |<span data-ttu-id="1d1ac-127">Описание</span><span class="sxs-lookup"><span data-stu-id="1d1ac-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1d1ac-128">id</span><span class="sxs-lookup"><span data-stu-id="1d1ac-128">id</span></span>            |`string`      |<span data-ttu-id="1d1ac-129">Идентификатор объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-129">ID of the `shift`.</span></span>|
| <span data-ttu-id="1d1ac-130">userId</span><span class="sxs-lookup"><span data-stu-id="1d1ac-130">userId</span></span>            |`string`      |<span data-ttu-id="1d1ac-131">Идентификатор пользователя, `shift`назначенный.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-131">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="1d1ac-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-132">Required.</span></span> |
| <span data-ttu-id="1d1ac-133">Счедулингграупид</span><span class="sxs-lookup"><span data-stu-id="1d1ac-133">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="1d1ac-134">Идентификатор группы планирования, в которой `shift` входит.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-134">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="1d1ac-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-135">Required.</span></span> |
| <span data-ttu-id="1d1ac-136">Шаредшифт</span><span class="sxs-lookup"><span data-stu-id="1d1ac-136">sharedShift</span></span>   |`[shiftItem](shiftitem.md)`  |<span data-ttu-id="1d1ac-137">Общая версия этого `shift` объекта доступна как для сотрудников, так и для руководителей.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-137">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="1d1ac-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-138">Required.</span></span> |
| <span data-ttu-id="1d1ac-139">Драфтшифт</span><span class="sxs-lookup"><span data-stu-id="1d1ac-139">draftShift</span></span>        |`[shiftItem](shiftitem.md)`        |<span data-ttu-id="1d1ac-140">Черновая версия этого `shift` элемента, просматриваемая руководителями.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-140">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="1d1ac-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-141">Required.</span></span> |
| <span data-ttu-id="1d1ac-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d1ac-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="1d1ac-143">Временная метка, на которую `shift` был создан впервые.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-143">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="1d1ac-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1d1ac-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1d1ac-145">Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="1d1ac-145">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="1d1ac-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d1ac-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="1d1ac-147">Отметка времени `shift` последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-147">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="1d1ac-148">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1d1ac-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1d1ac-149">Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="1d1ac-149">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="1d1ac-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1d1ac-150">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="1d1ac-151">Удостоверение, которое Последнее обновило `shift`.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-151">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d1ac-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d1ac-152">JSON representation</span></span>

<span data-ttu-id="1d1ac-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d1ac-153">Here is a JSON representation of the resource.</span></span>

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
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
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
  "suppressions": [
    "Error: /api-reference/beta/resources/shift.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
