---
title: Тип ресурса Тимеофф
description: Единица измерения, которая не работает в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 64ef8a07d3190ad2a54e9e3e5c68f3ffb0335acc
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866527"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="7dd8d-103">Тип ресурса Тимеофф</span><span class="sxs-lookup"><span data-stu-id="7dd8d-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dd8d-104">Единица измерения "не работает" в расписании.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-104">A unit of non-work in a schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="7dd8d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="7dd8d-105">Methods</span></span>

| <span data-ttu-id="7dd8d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="7dd8d-106">Method</span></span>       | <span data-ttu-id="7dd8d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7dd8d-107">Return Type</span></span>  |<span data-ttu-id="7dd8d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7dd8d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7dd8d-109">Создание</span><span class="sxs-lookup"><span data-stu-id="7dd8d-109">Create</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="7dd8d-110">тимеофф</span><span class="sxs-lookup"><span data-stu-id="7dd8d-110">timeOff</span></span>](timeoff.md) | <span data-ttu-id="7dd8d-111">Создание нового объекта **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="7dd8d-111">Create a new **timeOff** object.</span></span>|
|[<span data-ttu-id="7dd8d-112">List</span><span class="sxs-lookup"><span data-stu-id="7dd8d-112">List</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="7dd8d-113">Коллекция [тимеофф](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="7dd8d-113">[timeOff](timeoff.md) collection</span></span> | <span data-ttu-id="7dd8d-114">Получение списка объектов **тимеофф** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-114">Get the list of **timeOff** objects in this schedule.</span></span>|
|<span data-ttu-id="7dd8d-115">[Get (.. /АПИ/тимеофф-жет.МД)</span><span class="sxs-lookup"><span data-stu-id="7dd8d-115">[Get (../api/timeoff-get.md)</span></span> | [<span data-ttu-id="7dd8d-116">тимеофф</span><span class="sxs-lookup"><span data-stu-id="7dd8d-116">timeOff</span></span>](timeoff.md) | <span data-ttu-id="7dd8d-117">Получение объекта **тимеофф** по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-117">Get a **timeOff** object by ID.</span></span>|
|[<span data-ttu-id="7dd8d-118">Replace</span><span class="sxs-lookup"><span data-stu-id="7dd8d-118">Replace</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="7dd8d-119">тимеофф</span><span class="sxs-lookup"><span data-stu-id="7dd8d-119">timeOff</span></span>](timeoff.md) | <span data-ttu-id="7dd8d-120">Замена объекта **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="7dd8d-120">Replace a **timeOff** object.</span></span>|
|<span data-ttu-id="7dd8d-121">[удаление](../api/timeoff-delete.md);</span><span class="sxs-lookup"><span data-stu-id="7dd8d-121">[Delete](../api/timeoff-delete.md)</span></span> | <span data-ttu-id="7dd8d-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-122">None</span></span> | <span data-ttu-id="7dd8d-123">Удаление объекта **тимеофф** из расписания.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-123">Delete a **timeOff** object from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="7dd8d-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="7dd8d-124">Properties</span></span>
|<span data-ttu-id="7dd8d-125">Имя</span><span class="sxs-lookup"><span data-stu-id="7dd8d-125">Name</span></span>          |<span data-ttu-id="7dd8d-126">Тип</span><span class="sxs-lookup"><span data-stu-id="7dd8d-126">Type</span></span>           |<span data-ttu-id="7dd8d-127">Описание</span><span class="sxs-lookup"><span data-stu-id="7dd8d-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7dd8d-128">id</span><span class="sxs-lookup"><span data-stu-id="7dd8d-128">id</span></span>            |`string`      |<span data-ttu-id="7dd8d-129">Идентификатор объекта `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="7dd8d-130">userId</span><span class="sxs-lookup"><span data-stu-id="7dd8d-130">userId</span></span>            |`string`      |<span data-ttu-id="7dd8d-131">Идентификатор пользователя, назначенного объекту `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="7dd8d-132">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-132">Required.</span></span>|
| <span data-ttu-id="7dd8d-133">шаредтимеофф</span><span class="sxs-lookup"><span data-stu-id="7dd8d-133">sharedTimeOff</span></span>     | [<span data-ttu-id="7dd8d-134">тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="7dd8d-134">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="7dd8d-135">Общая версия объекта `timeOff`, доступная для просмотра как сотрудникам, так и руководителям.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-135">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="7dd8d-136">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-136">Required.</span></span>|
| <span data-ttu-id="7dd8d-137">драфттимеофф</span><span class="sxs-lookup"><span data-stu-id="7dd8d-137">draftTimeOff</span></span>      | [<span data-ttu-id="7dd8d-138">тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="7dd8d-138">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="7dd8d-139">Черновая версия объекта `timeOff`, доступная для просмотра руководителями.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-139">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="7dd8d-140">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-140">Required.</span></span>|
| <span data-ttu-id="7dd8d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7dd8d-141">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="7dd8d-142">Отметка `timeOff` времени первоначального создания.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-142">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="7dd8d-143">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="7dd8d-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7dd8d-144">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="7dd8d-144">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="7dd8d-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7dd8d-145">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="7dd8d-146">Отметка `timeOff` времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-146">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="7dd8d-147">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="7dd8d-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7dd8d-148">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="7dd8d-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="7dd8d-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="7dd8d-149">lastModifiedBy</span></span>        | [<span data-ttu-id="7dd8d-150">identitySet</span><span class="sxs-lookup"><span data-stu-id="7dd8d-150">identitySet</span></span>](identityset.md)        |<span data-ttu-id="7dd8d-151">Учетная запись, которая последней обновила этот объект `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-151">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7dd8d-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7dd8d-152">JSON representation</span></span>

<span data-ttu-id="7dd8d-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7dd8d-153">Here is a JSON representation of the resource.</span></span>

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
