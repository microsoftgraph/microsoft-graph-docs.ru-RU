---
title: Тип ресурса Тимеофф
description: Единица измерения, которая не работает в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 933c940e25c772cede7918dabf62b52ee58f18d2
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657800"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="2a9d8-103">Тип ресурса Тимеофф</span><span class="sxs-lookup"><span data-stu-id="2a9d8-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a9d8-104">Единица измерения, которая не работает в расписании.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-104">A unit of non-work in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="2a9d8-105">Методы</span><span class="sxs-lookup"><span data-stu-id="2a9d8-105">Methods</span></span>

| <span data-ttu-id="2a9d8-106">Метод</span><span class="sxs-lookup"><span data-stu-id="2a9d8-106">Method</span></span>       | <span data-ttu-id="2a9d8-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2a9d8-107">Return Type</span></span>  |<span data-ttu-id="2a9d8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2a9d8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2a9d8-109">Создание Тимеофф</span><span class="sxs-lookup"><span data-stu-id="2a9d8-109">Create timeOff</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="2a9d8-110">Тимеофф</span><span class="sxs-lookup"><span data-stu-id="2a9d8-110">timeOff</span></span>](timeOff.md) | <span data-ttu-id="2a9d8-111">Создание нового объекта `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-111">Create a new `timeOff` object.</span></span>|
|[<span data-ttu-id="2a9d8-112">Список Тимеоффс</span><span class="sxs-lookup"><span data-stu-id="2a9d8-112">List timeOffs</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="2a9d8-113">Коллекция [тимеофф](timeOff.md)</span><span class="sxs-lookup"><span data-stu-id="2a9d8-113">[timeOff](timeOff.md) collection</span></span> | <span data-ttu-id="2a9d8-114">Получение списка `timeOff` объектов в расписании.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-114">Get the list of `timeOff` objects in this schedule.</span></span>|
|[<span data-ttu-id="2a9d8-115">Получение Тимеофф</span><span class="sxs-lookup"><span data-stu-id="2a9d8-115">Get timeOff</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="2a9d8-116">Тимеофф</span><span class="sxs-lookup"><span data-stu-id="2a9d8-116">timeOff</span></span>](timeOff.md) | <span data-ttu-id="2a9d8-117">Получение `timeOff` по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-117">Get a `timeOff` by ID.</span></span>|
|[<span data-ttu-id="2a9d8-118">Замена Тимеофф</span><span class="sxs-lookup"><span data-stu-id="2a9d8-118">Replace timeOff</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="2a9d8-119">Тимеофф</span><span class="sxs-lookup"><span data-stu-id="2a9d8-119">timeOff</span></span>](timeOff.md) | <span data-ttu-id="2a9d8-120">Замените элемент `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-120">Replace a `timeOff`.</span></span>|
|[<span data-ttu-id="2a9d8-121">Удаление Тимеофф</span><span class="sxs-lookup"><span data-stu-id="2a9d8-121">Delete timeOff</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="2a9d8-122">Нет</span><span class="sxs-lookup"><span data-stu-id="2a9d8-122">None</span></span> | <span data-ttu-id="2a9d8-123">Удаление `timeOff` из расписания.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-123">Delete a `timeOff` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a9d8-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a9d8-124">Properties</span></span>
|<span data-ttu-id="2a9d8-125">Имя</span><span class="sxs-lookup"><span data-stu-id="2a9d8-125">Name</span></span>          |<span data-ttu-id="2a9d8-126">Тип</span><span class="sxs-lookup"><span data-stu-id="2a9d8-126">Type</span></span>           |<span data-ttu-id="2a9d8-127">Описание</span><span class="sxs-lookup"><span data-stu-id="2a9d8-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2a9d8-128">id</span><span class="sxs-lookup"><span data-stu-id="2a9d8-128">id</span></span>            |`string`      |<span data-ttu-id="2a9d8-129">Идентификатор объекта `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="2a9d8-130">userId</span><span class="sxs-lookup"><span data-stu-id="2a9d8-130">userId</span></span>            |`string`      |<span data-ttu-id="2a9d8-131">Идентификатор пользователя, `timeOff`назначенный.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="2a9d8-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-132">Required.</span></span>|
| <span data-ttu-id="2a9d8-133">Шаредтимеофф</span><span class="sxs-lookup"><span data-stu-id="2a9d8-133">sharedTimeOff</span></span>     |`[timeOffItem](timeoffitem.md)`  |<span data-ttu-id="2a9d8-134">Общая версия этого `timeOff` объекта доступна как для сотрудников, так и для руководителей.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-134">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="2a9d8-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-135">Required.</span></span>|
| <span data-ttu-id="2a9d8-136">Драфттимеофф</span><span class="sxs-lookup"><span data-stu-id="2a9d8-136">draftTimeOff</span></span>      |`[timeOffItem](timeoffitem.md)`        |<span data-ttu-id="2a9d8-137">Черновая версия этого `timeOff` элемента, просматриваемая руководителями.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-137">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="2a9d8-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-138">Required.</span></span>|
| <span data-ttu-id="2a9d8-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a9d8-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="2a9d8-140">Отметка `timeOff` времени первоначального создания.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-140">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="2a9d8-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="2a9d8-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2a9d8-142">Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="2a9d8-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="2a9d8-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a9d8-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="2a9d8-144">Отметка `timeOff` времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-144">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="2a9d8-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="2a9d8-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2a9d8-146">Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="2a9d8-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="2a9d8-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2a9d8-147">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="2a9d8-148">Удостоверение, которое Последнее обновило `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-148">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2a9d8-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a9d8-149">JSON representation</span></span>

<span data-ttu-id="2a9d8-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a9d8-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff"
}-->

```json
{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOff resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoff.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
