---
title: Тип ресурса Тимеофф
description: Единица измерения, которая не работает в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4ad289b745fcd26adea3cbe2698f01dde3d87d30
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075499"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="ab677-103">Тип ресурса Тимеофф</span><span class="sxs-lookup"><span data-stu-id="ab677-103">timeOff resource type</span></span>

<span data-ttu-id="ab677-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab677-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab677-105">Единица измерения "не работает" в расписании.</span><span class="sxs-lookup"><span data-stu-id="ab677-105">A unit of non-work in a schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="ab677-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ab677-106">Methods</span></span>

| <span data-ttu-id="ab677-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ab677-107">Method</span></span>       | <span data-ttu-id="ab677-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ab677-108">Return Type</span></span>  |<span data-ttu-id="ab677-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ab677-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab677-110">Создание</span><span class="sxs-lookup"><span data-stu-id="ab677-110">Create</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="ab677-111">timeOff</span><span class="sxs-lookup"><span data-stu-id="ab677-111">timeOff</span></span>](timeoff.md) | <span data-ttu-id="ab677-112">Создание нового объекта **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="ab677-112">Create a new **timeOff** object.</span></span>|
|[<span data-ttu-id="ab677-113">Список</span><span class="sxs-lookup"><span data-stu-id="ab677-113">List</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="ab677-114">Коллекция [тимеофф](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="ab677-114">[timeOff](timeoff.md) collection</span></span> | <span data-ttu-id="ab677-115">Получение списка объектов **тимеофф** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="ab677-115">Get the list of **timeOff** objects in this schedule.</span></span>|
|<span data-ttu-id="ab677-116">[получение](../api/timeoff-get.md);</span><span class="sxs-lookup"><span data-stu-id="ab677-116">[Get](../api/timeoff-get.md)</span></span> | [<span data-ttu-id="ab677-117">timeOff</span><span class="sxs-lookup"><span data-stu-id="ab677-117">timeOff</span></span>](timeoff.md) | <span data-ttu-id="ab677-118">Получение объекта **тимеофф** по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="ab677-118">Get a **timeOff** object by ID.</span></span>|
|[<span data-ttu-id="ab677-119">Replace</span><span class="sxs-lookup"><span data-stu-id="ab677-119">Replace</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="ab677-120">timeOff</span><span class="sxs-lookup"><span data-stu-id="ab677-120">timeOff</span></span>](timeoff.md) | <span data-ttu-id="ab677-121">Замена объекта **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="ab677-121">Replace a **timeOff** object.</span></span>|
|[<span data-ttu-id="ab677-122">Удаление</span><span class="sxs-lookup"><span data-stu-id="ab677-122">Delete</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="ab677-123">Нет</span><span class="sxs-lookup"><span data-stu-id="ab677-123">None</span></span> | <span data-ttu-id="ab677-124">Удаление объекта **тимеофф** из расписания.</span><span class="sxs-lookup"><span data-stu-id="ab677-124">Delete a **timeOff** object from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="ab677-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab677-125">Properties</span></span>
|<span data-ttu-id="ab677-126">Имя</span><span class="sxs-lookup"><span data-stu-id="ab677-126">Name</span></span>          |<span data-ttu-id="ab677-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ab677-127">Type</span></span>           |<span data-ttu-id="ab677-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ab677-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ab677-129">id</span><span class="sxs-lookup"><span data-stu-id="ab677-129">id</span></span>            |`string`      |<span data-ttu-id="ab677-130">Идентификатор объекта `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="ab677-130">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="ab677-131">userId</span><span class="sxs-lookup"><span data-stu-id="ab677-131">userId</span></span>            |`string`      |<span data-ttu-id="ab677-132">Идентификатор пользователя, назначенного объекту `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="ab677-132">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="ab677-133">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="ab677-133">Required.</span></span>|
| <span data-ttu-id="ab677-134">шаредтимеофф</span><span class="sxs-lookup"><span data-stu-id="ab677-134">sharedTimeOff</span></span>     | [<span data-ttu-id="ab677-135">тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="ab677-135">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="ab677-136">Общая версия объекта `timeOff`, доступная для просмотра как сотрудникам, так и руководителям.</span><span class="sxs-lookup"><span data-stu-id="ab677-136">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="ab677-137">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="ab677-137">Required.</span></span>|
| <span data-ttu-id="ab677-138">драфттимеофф</span><span class="sxs-lookup"><span data-stu-id="ab677-138">draftTimeOff</span></span>      | [<span data-ttu-id="ab677-139">тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="ab677-139">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="ab677-140">Черновая версия объекта `timeOff`, доступная для просмотра руководителями.</span><span class="sxs-lookup"><span data-stu-id="ab677-140">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="ab677-141">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="ab677-141">Required.</span></span>|
| <span data-ttu-id="ab677-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab677-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="ab677-143">Отметка времени `timeOff` первоначального создания.</span><span class="sxs-lookup"><span data-stu-id="ab677-143">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="ab677-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ab677-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ab677-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="ab677-145">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="ab677-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab677-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="ab677-147">Отметка времени `timeOff` последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="ab677-147">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="ab677-148">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ab677-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ab677-149">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="ab677-149">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="ab677-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ab677-150">lastModifiedBy</span></span>        | [<span data-ttu-id="ab677-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="ab677-151">identitySet</span></span>](identityset.md)        |<span data-ttu-id="ab677-152">Учетная запись, которая последней обновила этот объект `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="ab677-152">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ab677-153">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ab677-153">JSON representation</span></span>

<span data-ttu-id="ab677-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab677-154">Here is a JSON representation of the resource.</span></span>

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


