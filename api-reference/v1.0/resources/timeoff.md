---
title: Тип ресурса timeOff
description: Единица, не работая в расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: a3060b9fcd47bddc2d589d2ffdfc249146ee4dca
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720853"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="ffa4c-103">Тип ресурса timeOff</span><span class="sxs-lookup"><span data-stu-id="ffa4c-103">timeOff resource type</span></span>

<span data-ttu-id="ffa4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffa4c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ffa4c-105">Единица не работает в расписании.</span><span class="sxs-lookup"><span data-stu-id="ffa4c-105">A unit of non-work in a schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="ffa4c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ffa4c-106">Methods</span></span>

| <span data-ttu-id="ffa4c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ffa4c-107">Method</span></span>       | <span data-ttu-id="ffa4c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ffa4c-108">Return Type</span></span>  |<span data-ttu-id="ffa4c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ffa4c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ffa4c-110">Список</span><span class="sxs-lookup"><span data-stu-id="ffa4c-110">List</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="ffa4c-111">[коллекция timeOff](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="ffa4c-111">[timeOff](timeoff.md) collection</span></span> | <span data-ttu-id="ffa4c-112">Получите список объектов **timeOff** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="ffa4c-112">Get the list of **timeOff** objects in this schedule.</span></span>|
|[<span data-ttu-id="ffa4c-113">Создание</span><span class="sxs-lookup"><span data-stu-id="ffa4c-113">Create</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="ffa4c-114">timeOff</span><span class="sxs-lookup"><span data-stu-id="ffa4c-114">timeOff</span></span>](timeoff.md) | <span data-ttu-id="ffa4c-115">Создание нового **объекта timeOff.**</span><span class="sxs-lookup"><span data-stu-id="ffa4c-115">Create a new **timeOff** object.</span></span>|
|<span data-ttu-id="ffa4c-116">[получение](../api/timeoff-get.md);</span><span class="sxs-lookup"><span data-stu-id="ffa4c-116">[Get](../api/timeoff-get.md)</span></span> | [<span data-ttu-id="ffa4c-117">timeOff</span><span class="sxs-lookup"><span data-stu-id="ffa4c-117">timeOff</span></span>](timeoff.md) | <span data-ttu-id="ffa4c-118">Получите объект **timeOff** по ID.</span><span class="sxs-lookup"><span data-stu-id="ffa4c-118">Get a **timeOff** object by ID.</span></span>|
|[<span data-ttu-id="ffa4c-119">Replace</span><span class="sxs-lookup"><span data-stu-id="ffa4c-119">Replace</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="ffa4c-120">timeOff</span><span class="sxs-lookup"><span data-stu-id="ffa4c-120">timeOff</span></span>](timeoff.md) | <span data-ttu-id="ffa4c-121">Замените **объект timeOff.**</span><span class="sxs-lookup"><span data-stu-id="ffa4c-121">Replace a **timeOff** object.</span></span>|
|<span data-ttu-id="ffa4c-122">[удаление](../api/timeoff-delete.md);</span><span class="sxs-lookup"><span data-stu-id="ffa4c-122">[Delete](../api/timeoff-delete.md)</span></span> | <span data-ttu-id="ffa4c-123">Нет</span><span class="sxs-lookup"><span data-stu-id="ffa4c-123">None</span></span> | <span data-ttu-id="ffa4c-124">Удаление объекта **timeOff** из расписания.</span><span class="sxs-lookup"><span data-stu-id="ffa4c-124">Delete a **timeOff** object from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="ffa4c-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="ffa4c-125">Properties</span></span>
|<span data-ttu-id="ffa4c-126">Имя</span><span class="sxs-lookup"><span data-stu-id="ffa4c-126">Name</span></span>          |<span data-ttu-id="ffa4c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ffa4c-127">Type</span></span>           |<span data-ttu-id="ffa4c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ffa4c-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ffa4c-129">id</span><span class="sxs-lookup"><span data-stu-id="ffa4c-129">id</span></span>            |`string`      |<span data-ttu-id="ffa4c-130">ID **timeOff**.</span><span class="sxs-lookup"><span data-stu-id="ffa4c-130">ID of the **timeOff**.</span></span>|
| <span data-ttu-id="ffa4c-131">userId</span><span class="sxs-lookup"><span data-stu-id="ffa4c-131">userId</span></span>            |`string`      |<span data-ttu-id="ffa4c-132">ID пользователя, назначенного **timeOff**.</span><span class="sxs-lookup"><span data-stu-id="ffa4c-132">ID of the user assigned to the **timeOff**.</span></span> <span data-ttu-id="ffa4c-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffa4c-133">Required.</span></span>|
| <span data-ttu-id="ffa4c-134">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="ffa4c-134">sharedTimeOff</span></span>     | [<span data-ttu-id="ffa4c-135">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="ffa4c-135">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="ffa4c-136">Общая версия этого **timeOff,** которая просматривается как сотрудниками, так и руководителями.</span><span class="sxs-lookup"><span data-stu-id="ffa4c-136">The shared version of this **timeOff** that is viewable by both employees and managers.</span></span> <span data-ttu-id="ffa4c-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffa4c-137">Required.</span></span>|
| <span data-ttu-id="ffa4c-138">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="ffa4c-138">draftTimeOff</span></span>      | [<span data-ttu-id="ffa4c-139">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="ffa4c-139">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="ffa4c-140">Черновик версии этого **timeOff,** который просматривается руководителями.</span><span class="sxs-lookup"><span data-stu-id="ffa4c-140">The draft version of this **timeOff** that is viewable by managers.</span></span> <span data-ttu-id="ffa4c-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffa4c-141">Required.</span></span>|
| <span data-ttu-id="ffa4c-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffa4c-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="ffa4c-143">Отметка времени, на которой впервые был создан **этот timeOff.**</span><span class="sxs-lookup"><span data-stu-id="ffa4c-143">The time stamp at which this **timeOff** was first created.</span></span> <span data-ttu-id="ffa4c-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ffa4c-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ffa4c-145">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ffa4c-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="ffa4c-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffa4c-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="ffa4c-147">Отпечаток времени, на котором в этот **раз был** обновлен последний раз.</span><span class="sxs-lookup"><span data-stu-id="ffa4c-147">The time stamp at which this **timeOff** was last updated.</span></span> <span data-ttu-id="ffa4c-148">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ffa4c-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ffa4c-149">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ffa4c-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="ffa4c-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ffa4c-150">lastModifiedBy</span></span>        | [<span data-ttu-id="ffa4c-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="ffa4c-151">identitySet</span></span>](identityset.md)        |<span data-ttu-id="ffa4c-152">Удостоверение, которое в последний раз обновлялось **в этот раз.**</span><span class="sxs-lookup"><span data-stu-id="ffa4c-152">The identity that last updated this **timeOff**.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ffa4c-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ffa4c-153">JSON representation</span></span>

<span data-ttu-id="ffa4c-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffa4c-154">The following is a JSON representation of the resource.</span></span>

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

