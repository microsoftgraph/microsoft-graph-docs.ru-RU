---
title: Тип ресурса Shift
description: Смена — это единица запланированной работы в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd80cd36bd32ea9efba9e565aabd2da963c51ec8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583797"
---
# <a name="shift-resource-type"></a><span data-ttu-id="93bf4-103">Тип ресурса Shift</span><span class="sxs-lookup"><span data-stu-id="93bf4-103">shift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93bf4-104">Единица запланированной работы по [расписанию](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="93bf4-104">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="93bf4-105">Методы</span><span class="sxs-lookup"><span data-stu-id="93bf4-105">Methods</span></span>

| <span data-ttu-id="93bf4-106">Метод</span><span class="sxs-lookup"><span data-stu-id="93bf4-106">Method</span></span>       | <span data-ttu-id="93bf4-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="93bf4-107">Return Type</span></span>  |<span data-ttu-id="93bf4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="93bf4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="93bf4-109">Создание смены</span><span class="sxs-lookup"><span data-stu-id="93bf4-109">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="93bf4-110">перемещен</span><span class="sxs-lookup"><span data-stu-id="93bf4-110">shift</span></span>](shift.md) | <span data-ttu-id="93bf4-111">Создание объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="93bf4-111">Create a new `shift`.</span></span>|
|[<span data-ttu-id="93bf4-112">ПереЧисление смещений</span><span class="sxs-lookup"><span data-stu-id="93bf4-112">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="93bf4-113">Коллекция " [SHIFT](shift.md) "</span><span class="sxs-lookup"><span data-stu-id="93bf4-113">[shift](shift.md) collection</span></span> | <span data-ttu-id="93bf4-114">Получение списка `shifts` по данному расписанию.</span><span class="sxs-lookup"><span data-stu-id="93bf4-114">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="93bf4-115">Получение Shift</span><span class="sxs-lookup"><span data-stu-id="93bf4-115">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="93bf4-116">перемещен</span><span class="sxs-lookup"><span data-stu-id="93bf4-116">shift</span></span>](shift.md) | <span data-ttu-id="93bf4-117">Получение `shift` по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="93bf4-117">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="93bf4-118">Замена Shift</span><span class="sxs-lookup"><span data-stu-id="93bf4-118">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="93bf4-119">перемещен</span><span class="sxs-lookup"><span data-stu-id="93bf4-119">shift</span></span>](shift.md) | <span data-ttu-id="93bf4-120">Замена объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="93bf4-120">Replace a `shift`.</span></span>|
|[<span data-ttu-id="93bf4-121">Удаление смены</span><span class="sxs-lookup"><span data-stu-id="93bf4-121">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="93bf4-122">Нет</span><span class="sxs-lookup"><span data-stu-id="93bf4-122">None</span></span> | <span data-ttu-id="93bf4-123">Удаление `shift` из расписания.</span><span class="sxs-lookup"><span data-stu-id="93bf4-123">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="93bf4-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="93bf4-124">Properties</span></span>
|<span data-ttu-id="93bf4-125">Имя</span><span class="sxs-lookup"><span data-stu-id="93bf4-125">Name</span></span>          |<span data-ttu-id="93bf4-126">Тип</span><span class="sxs-lookup"><span data-stu-id="93bf4-126">Type</span></span>           |<span data-ttu-id="93bf4-127">Описание</span><span class="sxs-lookup"><span data-stu-id="93bf4-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="93bf4-128">id</span><span class="sxs-lookup"><span data-stu-id="93bf4-128">id</span></span>            |`string`      |<span data-ttu-id="93bf4-129">Идентификатор объекта `shift`.</span><span class="sxs-lookup"><span data-stu-id="93bf4-129">ID of the `shift`.</span></span>|
| <span data-ttu-id="93bf4-130">userId</span><span class="sxs-lookup"><span data-stu-id="93bf4-130">userId</span></span>            |`string`      |<span data-ttu-id="93bf4-131">Идентификатор пользователя, `shift`назначенный.</span><span class="sxs-lookup"><span data-stu-id="93bf4-131">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="93bf4-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93bf4-132">Required.</span></span> |
| <span data-ttu-id="93bf4-133">Счедулингграупид</span><span class="sxs-lookup"><span data-stu-id="93bf4-133">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="93bf4-134">Идентификатор группы планирования, в которой `shift` входит.</span><span class="sxs-lookup"><span data-stu-id="93bf4-134">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="93bf4-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93bf4-135">Required.</span></span> |
| <span data-ttu-id="93bf4-136">Шаредшифт</span><span class="sxs-lookup"><span data-stu-id="93bf4-136">sharedShift</span></span>   |[<span data-ttu-id="93bf4-137">Шифтитем</span><span class="sxs-lookup"><span data-stu-id="93bf4-137">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="93bf4-138">Общая версия этого `shift` объекта доступна как для сотрудников, так и для руководителей.</span><span class="sxs-lookup"><span data-stu-id="93bf4-138">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="93bf4-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93bf4-139">Required.</span></span> |
| <span data-ttu-id="93bf4-140">Драфтшифт</span><span class="sxs-lookup"><span data-stu-id="93bf4-140">draftShift</span></span>        |[<span data-ttu-id="93bf4-141">Шифтитем</span><span class="sxs-lookup"><span data-stu-id="93bf4-141">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="93bf4-142">Черновая версия этого `shift` элемента, просматриваемая руководителями.</span><span class="sxs-lookup"><span data-stu-id="93bf4-142">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="93bf4-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93bf4-143">Required.</span></span> |
| <span data-ttu-id="93bf4-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93bf4-144">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="93bf4-145">Временная метка, на которую `shift` был создан впервые.</span><span class="sxs-lookup"><span data-stu-id="93bf4-145">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="93bf4-146">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="93bf4-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="93bf4-147">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="93bf4-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="93bf4-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93bf4-148">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="93bf4-149">Отметка времени `shift` последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="93bf4-149">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="93bf4-150">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="93bf4-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="93bf4-151">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="93bf4-151">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="93bf4-152">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="93bf4-152">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="93bf4-153">Учетная запись, которая последней обновила этот объект `shift`.</span><span class="sxs-lookup"><span data-stu-id="93bf4-153">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93bf4-154">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="93bf4-154">JSON representation</span></span>

<span data-ttu-id="93bf4-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93bf4-155">Here is a JSON representation of the resource.</span></span>

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
