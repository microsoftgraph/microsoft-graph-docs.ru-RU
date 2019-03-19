---
title: Тип ресурса Тимеофф
description: Единица измерения, которая не работает в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c15d65c6d0a5a9749654698a51996cb21c254a9d
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2019
ms.locfileid: "30676991"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="1ca1a-103">Тип ресурса Тимеофф</span><span class="sxs-lookup"><span data-stu-id="1ca1a-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ca1a-104">Единица измерения, которая не работает в расписании.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-104">A unit of non-work in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="1ca1a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="1ca1a-105">Methods</span></span>

| <span data-ttu-id="1ca1a-106">Метод</span><span class="sxs-lookup"><span data-stu-id="1ca1a-106">Method</span></span>       | <span data-ttu-id="1ca1a-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1ca1a-107">Return Type</span></span>  |<span data-ttu-id="1ca1a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1ca1a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1ca1a-109">Создание Тимеофф</span><span class="sxs-lookup"><span data-stu-id="1ca1a-109">Create timeOff</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="1ca1a-110">Тимеофф</span><span class="sxs-lookup"><span data-stu-id="1ca1a-110">timeOff</span></span>](timeOff.md) | <span data-ttu-id="1ca1a-111">Создание нового объекта `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-111">Create a new `timeOff` object.</span></span>|
|[<span data-ttu-id="1ca1a-112">Список Тимеоффс</span><span class="sxs-lookup"><span data-stu-id="1ca1a-112">List timeOffs</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="1ca1a-113">Коллекция [тимеофф](timeOff.md)</span><span class="sxs-lookup"><span data-stu-id="1ca1a-113">[timeOff](timeOff.md) collection</span></span> | <span data-ttu-id="1ca1a-114">Получение списка `timeOff` объектов в расписании.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-114">Get the list of `timeOff` objects in this schedule.</span></span>|
|[<span data-ttu-id="1ca1a-115">Получение Тимеофф</span><span class="sxs-lookup"><span data-stu-id="1ca1a-115">Get timeOff</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="1ca1a-116">Тимеофф</span><span class="sxs-lookup"><span data-stu-id="1ca1a-116">timeOff</span></span>](timeOff.md) | <span data-ttu-id="1ca1a-117">Получение `timeOff` по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-117">Get a `timeOff` by ID.</span></span>|
|[<span data-ttu-id="1ca1a-118">Замена Тимеофф</span><span class="sxs-lookup"><span data-stu-id="1ca1a-118">Replace timeOff</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="1ca1a-119">Тимеофф</span><span class="sxs-lookup"><span data-stu-id="1ca1a-119">timeOff</span></span>](timeOff.md) | <span data-ttu-id="1ca1a-120">Замените элемент `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-120">Replace a `timeOff`.</span></span>|
|[<span data-ttu-id="1ca1a-121">Удаление Тимеофф</span><span class="sxs-lookup"><span data-stu-id="1ca1a-121">Delete timeOff</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="1ca1a-122">Нет</span><span class="sxs-lookup"><span data-stu-id="1ca1a-122">None</span></span> | <span data-ttu-id="1ca1a-123">Удаление `timeOff` из расписания.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-123">Delete a `timeOff` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="1ca1a-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ca1a-124">Properties</span></span>
|<span data-ttu-id="1ca1a-125">Имя</span><span class="sxs-lookup"><span data-stu-id="1ca1a-125">Name</span></span>          |<span data-ttu-id="1ca1a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="1ca1a-126">Type</span></span>           |<span data-ttu-id="1ca1a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="1ca1a-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1ca1a-128">id</span><span class="sxs-lookup"><span data-stu-id="1ca1a-128">id</span></span>            |`string`      |<span data-ttu-id="1ca1a-129">Идентификатор объекта `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="1ca1a-130">userId</span><span class="sxs-lookup"><span data-stu-id="1ca1a-130">userId</span></span>            |`string`      |<span data-ttu-id="1ca1a-131">Идентификатор пользователя, `timeOff`назначенный.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="1ca1a-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-132">Required.</span></span>|
| <span data-ttu-id="1ca1a-133">Шаредтимеофф</span><span class="sxs-lookup"><span data-stu-id="1ca1a-133">sharedTimeOff</span></span>     |[<span data-ttu-id="1ca1a-134">Тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="1ca1a-134">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="1ca1a-135">Общая версия этого `timeOff` объекта доступна как для сотрудников, так и для руководителей.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-135">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="1ca1a-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-136">Required.</span></span>|
| <span data-ttu-id="1ca1a-137">Драфттимеофф</span><span class="sxs-lookup"><span data-stu-id="1ca1a-137">draftTimeOff</span></span>      |[<span data-ttu-id="1ca1a-138">Тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="1ca1a-138">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="1ca1a-139">Черновая версия этого `timeOff` элемента, просматриваемая руководителями.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-139">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="1ca1a-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-140">Required.</span></span>|
| <span data-ttu-id="1ca1a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ca1a-141">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="1ca1a-142">Отметка `timeOff` времени первоначального создания.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-142">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="1ca1a-143">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1ca1a-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1ca1a-144">Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="1ca1a-144">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="1ca1a-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ca1a-145">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="1ca1a-146">Отметка `timeOff` времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-146">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="1ca1a-147">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1ca1a-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1ca1a-148">Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="1ca1a-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="1ca1a-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1ca1a-149">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="1ca1a-150">Удостоверение, которое Последнее обновило `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-150">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1ca1a-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ca1a-151">JSON representation</span></span>

<span data-ttu-id="1ca1a-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ca1a-152">Here is a JSON representation of the resource.</span></span>

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
