---
title: Тип ресурса Тимеофф
description: Единица измерения, которая не работает в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 04cdadefd9c784c07d4b93c02bf7c9f51e7e3e73
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154453"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="d4519-103">Тип ресурса Тимеофф</span><span class="sxs-lookup"><span data-stu-id="d4519-103">timeOff resource type</span></span>

<span data-ttu-id="d4519-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4519-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4519-105">Единица измерения "не работает" в расписании.</span><span class="sxs-lookup"><span data-stu-id="d4519-105">A unit of non-work in a schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="d4519-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d4519-106">Methods</span></span>

| <span data-ttu-id="d4519-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d4519-107">Method</span></span>       | <span data-ttu-id="d4519-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d4519-108">Return Type</span></span>  |<span data-ttu-id="d4519-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d4519-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4519-110">Создание</span><span class="sxs-lookup"><span data-stu-id="d4519-110">Create</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="d4519-111">тимеофф</span><span class="sxs-lookup"><span data-stu-id="d4519-111">timeOff</span></span>](timeoff.md) | <span data-ttu-id="d4519-112">Создание нового объекта **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="d4519-112">Create a new **timeOff** object.</span></span>|
|[<span data-ttu-id="d4519-113">List</span><span class="sxs-lookup"><span data-stu-id="d4519-113">List</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="d4519-114">Коллекция [тимеофф](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="d4519-114">[timeOff](timeoff.md) collection</span></span> | <span data-ttu-id="d4519-115">Получение списка объектов **тимеофф** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="d4519-115">Get the list of **timeOff** objects in this schedule.</span></span>|
|<span data-ttu-id="d4519-116">[получение](../api/timeoff-get.md);</span><span class="sxs-lookup"><span data-stu-id="d4519-116">[Get](../api/timeoff-get.md)</span></span> | [<span data-ttu-id="d4519-117">тимеофф</span><span class="sxs-lookup"><span data-stu-id="d4519-117">timeOff</span></span>](timeoff.md) | <span data-ttu-id="d4519-118">Получение объекта **тимеофф** по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="d4519-118">Get a **timeOff** object by ID.</span></span>|
|[<span data-ttu-id="d4519-119">Replace</span><span class="sxs-lookup"><span data-stu-id="d4519-119">Replace</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="d4519-120">тимеофф</span><span class="sxs-lookup"><span data-stu-id="d4519-120">timeOff</span></span>](timeoff.md) | <span data-ttu-id="d4519-121">Замена объекта **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="d4519-121">Replace a **timeOff** object.</span></span>|
|<span data-ttu-id="d4519-122">[удаление](../api/timeoff-delete.md);</span><span class="sxs-lookup"><span data-stu-id="d4519-122">[Delete](../api/timeoff-delete.md)</span></span> | <span data-ttu-id="d4519-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d4519-123">None</span></span> | <span data-ttu-id="d4519-124">Удаление объекта **тимеофф** из расписания.</span><span class="sxs-lookup"><span data-stu-id="d4519-124">Delete a **timeOff** object from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4519-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4519-125">Properties</span></span>
|<span data-ttu-id="d4519-126">Имя</span><span class="sxs-lookup"><span data-stu-id="d4519-126">Name</span></span>          |<span data-ttu-id="d4519-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d4519-127">Type</span></span>           |<span data-ttu-id="d4519-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d4519-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d4519-129">id</span><span class="sxs-lookup"><span data-stu-id="d4519-129">id</span></span>            |`string`      |<span data-ttu-id="d4519-130">Идентификатор объекта `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="d4519-130">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="d4519-131">userId</span><span class="sxs-lookup"><span data-stu-id="d4519-131">userId</span></span>            |`string`      |<span data-ttu-id="d4519-132">Идентификатор пользователя, назначенного объекту `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="d4519-132">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="d4519-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4519-133">Required.</span></span>|
| <span data-ttu-id="d4519-134">шаредтимеофф</span><span class="sxs-lookup"><span data-stu-id="d4519-134">sharedTimeOff</span></span>     | [<span data-ttu-id="d4519-135">тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="d4519-135">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="d4519-136">Общая версия объекта `timeOff`, доступная для просмотра как сотрудникам, так и руководителям.</span><span class="sxs-lookup"><span data-stu-id="d4519-136">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="d4519-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4519-137">Required.</span></span>|
| <span data-ttu-id="d4519-138">драфттимеофф</span><span class="sxs-lookup"><span data-stu-id="d4519-138">draftTimeOff</span></span>      | [<span data-ttu-id="d4519-139">тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="d4519-139">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="d4519-140">Черновая версия объекта `timeOff`, доступная для просмотра руководителями.</span><span class="sxs-lookup"><span data-stu-id="d4519-140">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="d4519-141">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d4519-141">Required.</span></span>|
| <span data-ttu-id="d4519-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4519-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="d4519-143">Отметка `timeOff` времени первоначального создания.</span><span class="sxs-lookup"><span data-stu-id="d4519-143">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="d4519-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d4519-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d4519-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="d4519-145">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="d4519-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4519-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="d4519-147">Отметка `timeOff` времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="d4519-147">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="d4519-148">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d4519-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d4519-149">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="d4519-149">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="d4519-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d4519-150">lastModifiedBy</span></span>        | [<span data-ttu-id="d4519-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="d4519-151">identitySet</span></span>](identityset.md)        |<span data-ttu-id="d4519-152">Учетная запись, которая последней обновила этот объект `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="d4519-152">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d4519-153">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d4519-153">JSON representation</span></span>

<span data-ttu-id="d4519-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4519-154">Here is a JSON representation of the resource.</span></span>

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
