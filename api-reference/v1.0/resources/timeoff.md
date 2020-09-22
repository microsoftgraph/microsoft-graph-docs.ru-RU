---
title: Тип ресурса Тимеофф
description: Единица измерения, которая не работает в расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 1c33ed74b52983b9adc3ce0d1c729caaa35dce09
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090832"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="2c115-103">Тип ресурса Тимеофф</span><span class="sxs-lookup"><span data-stu-id="2c115-103">timeOff resource type</span></span>

<span data-ttu-id="2c115-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c115-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2c115-105">Единица измерения "не работает" в расписании.</span><span class="sxs-lookup"><span data-stu-id="2c115-105">A unit of non-work in a schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="2c115-106">Методы</span><span class="sxs-lookup"><span data-stu-id="2c115-106">Methods</span></span>

| <span data-ttu-id="2c115-107">Метод</span><span class="sxs-lookup"><span data-stu-id="2c115-107">Method</span></span>       | <span data-ttu-id="2c115-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2c115-108">Return Type</span></span>  |<span data-ttu-id="2c115-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2c115-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2c115-110">Перечисление</span><span class="sxs-lookup"><span data-stu-id="2c115-110">List</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="2c115-111">Коллекция [тимеофф](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="2c115-111">[timeOff](timeoff.md) collection</span></span> | <span data-ttu-id="2c115-112">Получение списка объектов **тимеофф** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="2c115-112">Get the list of **timeOff** objects in this schedule.</span></span>|
|[<span data-ttu-id="2c115-113">Создание</span><span class="sxs-lookup"><span data-stu-id="2c115-113">Create</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="2c115-114">timeOff</span><span class="sxs-lookup"><span data-stu-id="2c115-114">timeOff</span></span>](timeoff.md) | <span data-ttu-id="2c115-115">Создание нового объекта **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="2c115-115">Create a new **timeOff** object.</span></span>|
|[<span data-ttu-id="2c115-116">Получение</span><span class="sxs-lookup"><span data-stu-id="2c115-116">Get</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="2c115-117">timeOff</span><span class="sxs-lookup"><span data-stu-id="2c115-117">timeOff</span></span>](timeoff.md) | <span data-ttu-id="2c115-118">Получение объекта **тимеофф** по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="2c115-118">Get a **timeOff** object by ID.</span></span>|
|[<span data-ttu-id="2c115-119">Replace</span><span class="sxs-lookup"><span data-stu-id="2c115-119">Replace</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="2c115-120">timeOff</span><span class="sxs-lookup"><span data-stu-id="2c115-120">timeOff</span></span>](timeoff.md) | <span data-ttu-id="2c115-121">Замена объекта **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="2c115-121">Replace a **timeOff** object.</span></span>|
|<span data-ttu-id="2c115-122">[удаление](../api/timeoff-delete.md);</span><span class="sxs-lookup"><span data-stu-id="2c115-122">[Delete](../api/timeoff-delete.md)</span></span> | <span data-ttu-id="2c115-123">Нет</span><span class="sxs-lookup"><span data-stu-id="2c115-123">None</span></span> | <span data-ttu-id="2c115-124">Удаление объекта **тимеофф** из расписания.</span><span class="sxs-lookup"><span data-stu-id="2c115-124">Delete a **timeOff** object from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="2c115-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c115-125">Properties</span></span>
|<span data-ttu-id="2c115-126">Имя</span><span class="sxs-lookup"><span data-stu-id="2c115-126">Name</span></span>          |<span data-ttu-id="2c115-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2c115-127">Type</span></span>           |<span data-ttu-id="2c115-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2c115-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2c115-129">id</span><span class="sxs-lookup"><span data-stu-id="2c115-129">id</span></span>            |`string`      |<span data-ttu-id="2c115-130">Идентификатор объекта **тимеофф**.</span><span class="sxs-lookup"><span data-stu-id="2c115-130">ID of the **timeOff**.</span></span>|
| <span data-ttu-id="2c115-131">userId</span><span class="sxs-lookup"><span data-stu-id="2c115-131">userId</span></span>            |`string`      |<span data-ttu-id="2c115-132">Идентификатор пользователя, назначенный **тимеофф**.</span><span class="sxs-lookup"><span data-stu-id="2c115-132">ID of the user assigned to the **timeOff**.</span></span> <span data-ttu-id="2c115-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c115-133">Required.</span></span>|
| <span data-ttu-id="2c115-134">шаредтимеофф</span><span class="sxs-lookup"><span data-stu-id="2c115-134">sharedTimeOff</span></span>     | [<span data-ttu-id="2c115-135">тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="2c115-135">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="2c115-136">Общая версия этого **тимеофф** , которая доступна для сотрудников и руководителей.</span><span class="sxs-lookup"><span data-stu-id="2c115-136">The shared version of this **timeOff** that is viewable by both employees and managers.</span></span> <span data-ttu-id="2c115-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c115-137">Required.</span></span>|
| <span data-ttu-id="2c115-138">драфттимеофф</span><span class="sxs-lookup"><span data-stu-id="2c115-138">draftTimeOff</span></span>      | [<span data-ttu-id="2c115-139">тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="2c115-139">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="2c115-140">Черновая версия этого **тимеофф** , которая отображается руководителями.</span><span class="sxs-lookup"><span data-stu-id="2c115-140">The draft version of this **timeOff** that is viewable by managers.</span></span> <span data-ttu-id="2c115-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c115-141">Required.</span></span>|
| <span data-ttu-id="2c115-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c115-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="2c115-143">Отметка времени первоначального создания **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="2c115-143">The time stamp at which this **timeOff** was first created.</span></span> <span data-ttu-id="2c115-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="2c115-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2c115-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="2c115-145">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="2c115-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c115-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="2c115-147">Отметка времени последнего обновления **тимеофф** .</span><span class="sxs-lookup"><span data-stu-id="2c115-147">The time stamp at which this **timeOff** was last updated.</span></span> <span data-ttu-id="2c115-148">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="2c115-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2c115-149">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="2c115-149">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="2c115-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2c115-150">lastModifiedBy</span></span>        | [<span data-ttu-id="2c115-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="2c115-151">identitySet</span></span>](identityset.md)        |<span data-ttu-id="2c115-152">Удостоверение, которое последним обновило этот **тимеофф**.</span><span class="sxs-lookup"><span data-stu-id="2c115-152">The identity that last updated this **timeOff**.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2c115-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c115-153">JSON representation</span></span>

<span data-ttu-id="2c115-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c115-154">The following is a JSON representation of the resource.</span></span>

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

