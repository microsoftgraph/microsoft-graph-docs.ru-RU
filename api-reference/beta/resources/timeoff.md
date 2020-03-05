---
title: Тип ресурса Тимеофф
description: Единица измерения, которая не работает в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 3ff9edf6bf3834faf5d91773b6c94ecbc4158d79
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519738"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="aefbf-103">Тип ресурса Тимеофф</span><span class="sxs-lookup"><span data-stu-id="aefbf-103">timeOff resource type</span></span>

<span data-ttu-id="aefbf-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="aefbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aefbf-105">Единица измерения "не работает" в расписании.</span><span class="sxs-lookup"><span data-stu-id="aefbf-105">A unit of non-work in a schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="aefbf-106">Методы</span><span class="sxs-lookup"><span data-stu-id="aefbf-106">Methods</span></span>

| <span data-ttu-id="aefbf-107">Метод</span><span class="sxs-lookup"><span data-stu-id="aefbf-107">Method</span></span>       | <span data-ttu-id="aefbf-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="aefbf-108">Return Type</span></span>  |<span data-ttu-id="aefbf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aefbf-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aefbf-110">Создание</span><span class="sxs-lookup"><span data-stu-id="aefbf-110">Create</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="aefbf-111">тимеофф</span><span class="sxs-lookup"><span data-stu-id="aefbf-111">timeOff</span></span>](timeoff.md) | <span data-ttu-id="aefbf-112">Создание нового объекта **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="aefbf-112">Create a new **timeOff** object.</span></span>|
|[<span data-ttu-id="aefbf-113">List</span><span class="sxs-lookup"><span data-stu-id="aefbf-113">List</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="aefbf-114">Коллекция [тимеофф](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="aefbf-114">[timeOff](timeoff.md) collection</span></span> | <span data-ttu-id="aefbf-115">Получение списка объектов **тимеофф** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="aefbf-115">Get the list of **timeOff** objects in this schedule.</span></span>|
|<span data-ttu-id="aefbf-116">[Get (.. /АПИ/тимеофф-жет.МД)</span><span class="sxs-lookup"><span data-stu-id="aefbf-116">[Get (../api/timeoff-get.md)</span></span> | [<span data-ttu-id="aefbf-117">тимеофф</span><span class="sxs-lookup"><span data-stu-id="aefbf-117">timeOff</span></span>](timeoff.md) | <span data-ttu-id="aefbf-118">Получение объекта **тимеофф** по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="aefbf-118">Get a **timeOff** object by ID.</span></span>|
|[<span data-ttu-id="aefbf-119">Replace</span><span class="sxs-lookup"><span data-stu-id="aefbf-119">Replace</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="aefbf-120">тимеофф</span><span class="sxs-lookup"><span data-stu-id="aefbf-120">timeOff</span></span>](timeoff.md) | <span data-ttu-id="aefbf-121">Замена объекта **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="aefbf-121">Replace a **timeOff** object.</span></span>|
|<span data-ttu-id="aefbf-122">[удаление](../api/timeoff-delete.md);</span><span class="sxs-lookup"><span data-stu-id="aefbf-122">[Delete](../api/timeoff-delete.md)</span></span> | <span data-ttu-id="aefbf-123">Нет</span><span class="sxs-lookup"><span data-stu-id="aefbf-123">None</span></span> | <span data-ttu-id="aefbf-124">Удаление объекта **тимеофф** из расписания.</span><span class="sxs-lookup"><span data-stu-id="aefbf-124">Delete a **timeOff** object from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="aefbf-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="aefbf-125">Properties</span></span>
|<span data-ttu-id="aefbf-126">Имя</span><span class="sxs-lookup"><span data-stu-id="aefbf-126">Name</span></span>          |<span data-ttu-id="aefbf-127">Тип</span><span class="sxs-lookup"><span data-stu-id="aefbf-127">Type</span></span>           |<span data-ttu-id="aefbf-128">Описание</span><span class="sxs-lookup"><span data-stu-id="aefbf-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="aefbf-129">id</span><span class="sxs-lookup"><span data-stu-id="aefbf-129">id</span></span>            |`string`      |<span data-ttu-id="aefbf-130">Идентификатор объекта `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="aefbf-130">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="aefbf-131">userId</span><span class="sxs-lookup"><span data-stu-id="aefbf-131">userId</span></span>            |`string`      |<span data-ttu-id="aefbf-132">Идентификатор пользователя, назначенного объекту `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="aefbf-132">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="aefbf-133">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="aefbf-133">Required.</span></span>|
| <span data-ttu-id="aefbf-134">шаредтимеофф</span><span class="sxs-lookup"><span data-stu-id="aefbf-134">sharedTimeOff</span></span>     | [<span data-ttu-id="aefbf-135">тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="aefbf-135">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="aefbf-136">Общая версия объекта `timeOff`, доступная для просмотра как сотрудникам, так и руководителям.</span><span class="sxs-lookup"><span data-stu-id="aefbf-136">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="aefbf-137">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="aefbf-137">Required.</span></span>|
| <span data-ttu-id="aefbf-138">драфттимеофф</span><span class="sxs-lookup"><span data-stu-id="aefbf-138">draftTimeOff</span></span>      | [<span data-ttu-id="aefbf-139">тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="aefbf-139">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="aefbf-140">Черновая версия объекта `timeOff`, доступная для просмотра руководителями.</span><span class="sxs-lookup"><span data-stu-id="aefbf-140">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="aefbf-141">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="aefbf-141">Required.</span></span>|
| <span data-ttu-id="aefbf-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aefbf-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="aefbf-143">Отметка `timeOff` времени первоначального создания.</span><span class="sxs-lookup"><span data-stu-id="aefbf-143">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="aefbf-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="aefbf-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aefbf-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="aefbf-145">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="aefbf-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aefbf-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="aefbf-147">Отметка `timeOff` времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="aefbf-147">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="aefbf-148">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="aefbf-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aefbf-149">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="aefbf-149">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="aefbf-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="aefbf-150">lastModifiedBy</span></span>        | [<span data-ttu-id="aefbf-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="aefbf-151">identitySet</span></span>](identityset.md)        |<span data-ttu-id="aefbf-152">Учетная запись, которая последней обновила этот объект `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="aefbf-152">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aefbf-153">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="aefbf-153">JSON representation</span></span>

<span data-ttu-id="aefbf-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aefbf-154">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff",
   "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "userId": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"},
  "draftTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"}
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
  "suppressions": []
}
-->
