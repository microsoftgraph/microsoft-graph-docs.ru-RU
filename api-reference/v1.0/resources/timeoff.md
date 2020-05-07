---
title: Тип ресурса Тимеофф
description: Единица измерения, которая не работает в расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 508ace24bc15eda6f722153d4e55f12699c461bb
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44153867"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="71527-103">Тип ресурса Тимеофф</span><span class="sxs-lookup"><span data-stu-id="71527-103">timeOff resource type</span></span>

<span data-ttu-id="71527-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71527-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71527-105">Единица измерения "не работает" в расписании.</span><span class="sxs-lookup"><span data-stu-id="71527-105">A unit of non-work in a schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="71527-106">Методы</span><span class="sxs-lookup"><span data-stu-id="71527-106">Methods</span></span>

| <span data-ttu-id="71527-107">Метод</span><span class="sxs-lookup"><span data-stu-id="71527-107">Method</span></span>       | <span data-ttu-id="71527-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="71527-108">Return Type</span></span>  |<span data-ttu-id="71527-109">Описание</span><span class="sxs-lookup"><span data-stu-id="71527-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="71527-110">List</span><span class="sxs-lookup"><span data-stu-id="71527-110">List</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="71527-111">Коллекция [тимеофф](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="71527-111">[timeOff](timeoff.md) collection</span></span> | <span data-ttu-id="71527-112">Получение списка объектов **тимеофф** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="71527-112">Get the list of **timeOff** objects in this schedule.</span></span>|
|<span data-ttu-id="71527-113">[создание](../api/schedule-post-timesoff.md);</span><span class="sxs-lookup"><span data-stu-id="71527-113">[Create](../api/schedule-post-timesoff.md)</span></span> | [<span data-ttu-id="71527-114">тимеофф</span><span class="sxs-lookup"><span data-stu-id="71527-114">timeOff</span></span>](timeoff.md) | <span data-ttu-id="71527-115">Создание нового объекта **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="71527-115">Create a new **timeOff** object.</span></span>|
|<span data-ttu-id="71527-116">[получение](../api/timeoff-get.md);</span><span class="sxs-lookup"><span data-stu-id="71527-116">[Get](../api/timeoff-get.md)</span></span> | [<span data-ttu-id="71527-117">тимеофф</span><span class="sxs-lookup"><span data-stu-id="71527-117">timeOff</span></span>](timeoff.md) | <span data-ttu-id="71527-118">Получение объекта **тимеофф** по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="71527-118">Get a **timeOff** object by ID.</span></span>|
|[<span data-ttu-id="71527-119">Replace</span><span class="sxs-lookup"><span data-stu-id="71527-119">Replace</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="71527-120">тимеофф</span><span class="sxs-lookup"><span data-stu-id="71527-120">timeOff</span></span>](timeoff.md) | <span data-ttu-id="71527-121">Замена объекта **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="71527-121">Replace a **timeOff** object.</span></span>|
|<span data-ttu-id="71527-122">[удаление](../api/timeoff-delete.md);</span><span class="sxs-lookup"><span data-stu-id="71527-122">[Delete](../api/timeoff-delete.md)</span></span> | <span data-ttu-id="71527-123">Нет</span><span class="sxs-lookup"><span data-stu-id="71527-123">None</span></span> | <span data-ttu-id="71527-124">Удаление объекта **тимеофф** из расписания.</span><span class="sxs-lookup"><span data-stu-id="71527-124">Delete a **timeOff** object from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="71527-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="71527-125">Properties</span></span>
|<span data-ttu-id="71527-126">Имя</span><span class="sxs-lookup"><span data-stu-id="71527-126">Name</span></span>          |<span data-ttu-id="71527-127">Тип</span><span class="sxs-lookup"><span data-stu-id="71527-127">Type</span></span>           |<span data-ttu-id="71527-128">Описание</span><span class="sxs-lookup"><span data-stu-id="71527-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="71527-129">id</span><span class="sxs-lookup"><span data-stu-id="71527-129">id</span></span>            |`string`      |<span data-ttu-id="71527-130">Идентификатор объекта **тимеофф**.</span><span class="sxs-lookup"><span data-stu-id="71527-130">ID of the **timeOff**.</span></span>|
| <span data-ttu-id="71527-131">userId</span><span class="sxs-lookup"><span data-stu-id="71527-131">userId</span></span>            |`string`      |<span data-ttu-id="71527-132">Идентификатор пользователя, назначенный **тимеофф**.</span><span class="sxs-lookup"><span data-stu-id="71527-132">ID of the user assigned to the **timeOff**.</span></span> <span data-ttu-id="71527-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71527-133">Required.</span></span>|
| <span data-ttu-id="71527-134">шаредтимеофф</span><span class="sxs-lookup"><span data-stu-id="71527-134">sharedTimeOff</span></span>     | [<span data-ttu-id="71527-135">тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="71527-135">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="71527-136">Общая версия этого **тимеофф** , которая доступна для сотрудников и руководителей.</span><span class="sxs-lookup"><span data-stu-id="71527-136">The shared version of this **timeOff** that is viewable by both employees and managers.</span></span> <span data-ttu-id="71527-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71527-137">Required.</span></span>|
| <span data-ttu-id="71527-138">драфттимеофф</span><span class="sxs-lookup"><span data-stu-id="71527-138">draftTimeOff</span></span>      | [<span data-ttu-id="71527-139">тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="71527-139">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="71527-140">Черновая версия этого **тимеофф** , которая отображается руководителями.</span><span class="sxs-lookup"><span data-stu-id="71527-140">The draft version of this **timeOff** that is viewable by managers.</span></span> <span data-ttu-id="71527-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71527-141">Required.</span></span>|
| <span data-ttu-id="71527-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71527-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="71527-143">Отметка времени первоначального создания **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="71527-143">The time stamp at which this **timeOff** was first created.</span></span> <span data-ttu-id="71527-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="71527-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="71527-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="71527-145">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="71527-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71527-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="71527-147">Отметка времени последнего обновления **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="71527-147">The time stamp at which this **timeOff** was last updated.</span></span> <span data-ttu-id="71527-148">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="71527-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="71527-149">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="71527-149">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="71527-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="71527-150">lastModifiedBy</span></span>        | [<span data-ttu-id="71527-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="71527-151">identitySet</span></span>](identityset.md)        |<span data-ttu-id="71527-152">Удостоверение, которое последним обновило этот **тимеофф**.</span><span class="sxs-lookup"><span data-stu-id="71527-152">The identity that last updated this **timeOff**.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="71527-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71527-153">JSON representation</span></span>

<span data-ttu-id="71527-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71527-154">The following is a JSON representation of the resource.</span></span>

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
