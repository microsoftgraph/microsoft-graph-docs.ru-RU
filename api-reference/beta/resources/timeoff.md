---
title: Тип ресурса timeOff
description: Единица, не работая в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9dc8d463e7015ffca2c2b49de503b9a0a3cb5709
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720202"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="8a20a-103">Тип ресурса timeOff</span><span class="sxs-lookup"><span data-stu-id="8a20a-103">timeOff resource type</span></span>

<span data-ttu-id="8a20a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a20a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a20a-105">Единица не работает в расписании.</span><span class="sxs-lookup"><span data-stu-id="8a20a-105">A unit of non-work in a schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="8a20a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8a20a-106">Methods</span></span>

| <span data-ttu-id="8a20a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8a20a-107">Method</span></span>       | <span data-ttu-id="8a20a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8a20a-108">Return Type</span></span>  |<span data-ttu-id="8a20a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8a20a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8a20a-110">Создание</span><span class="sxs-lookup"><span data-stu-id="8a20a-110">Create</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="8a20a-111">timeOff</span><span class="sxs-lookup"><span data-stu-id="8a20a-111">timeOff</span></span>](timeoff.md) | <span data-ttu-id="8a20a-112">Создание нового **объекта timeOff.**</span><span class="sxs-lookup"><span data-stu-id="8a20a-112">Create a new **timeOff** object.</span></span>|
|[<span data-ttu-id="8a20a-113">List</span><span class="sxs-lookup"><span data-stu-id="8a20a-113">List</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="8a20a-114">[коллекция timeOff](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="8a20a-114">[timeOff](timeoff.md) collection</span></span> | <span data-ttu-id="8a20a-115">Получите список объектов **timeOff** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="8a20a-115">Get the list of **timeOff** objects in this schedule.</span></span>|
|<span data-ttu-id="8a20a-116">[получение](../api/timeoff-get.md);</span><span class="sxs-lookup"><span data-stu-id="8a20a-116">[Get](../api/timeoff-get.md)</span></span> | [<span data-ttu-id="8a20a-117">timeOff</span><span class="sxs-lookup"><span data-stu-id="8a20a-117">timeOff</span></span>](timeoff.md) | <span data-ttu-id="8a20a-118">Получите объект **timeOff** по ID.</span><span class="sxs-lookup"><span data-stu-id="8a20a-118">Get a **timeOff** object by ID.</span></span>|
|[<span data-ttu-id="8a20a-119">Replace</span><span class="sxs-lookup"><span data-stu-id="8a20a-119">Replace</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="8a20a-120">timeOff</span><span class="sxs-lookup"><span data-stu-id="8a20a-120">timeOff</span></span>](timeoff.md) | <span data-ttu-id="8a20a-121">Замените **объект timeOff.**</span><span class="sxs-lookup"><span data-stu-id="8a20a-121">Replace a **timeOff** object.</span></span>|
|[<span data-ttu-id="8a20a-122">Удаление</span><span class="sxs-lookup"><span data-stu-id="8a20a-122">Delete</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="8a20a-123">Нет</span><span class="sxs-lookup"><span data-stu-id="8a20a-123">None</span></span> | <span data-ttu-id="8a20a-124">Удаление объекта **timeOff** из расписания.</span><span class="sxs-lookup"><span data-stu-id="8a20a-124">Delete a **timeOff** object from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="8a20a-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a20a-125">Properties</span></span>
|<span data-ttu-id="8a20a-126">Имя</span><span class="sxs-lookup"><span data-stu-id="8a20a-126">Name</span></span>          |<span data-ttu-id="8a20a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="8a20a-127">Type</span></span>           |<span data-ttu-id="8a20a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8a20a-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8a20a-129">id</span><span class="sxs-lookup"><span data-stu-id="8a20a-129">id</span></span>            |`string`      |<span data-ttu-id="8a20a-130">Идентификатор объекта `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="8a20a-130">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="8a20a-131">userId</span><span class="sxs-lookup"><span data-stu-id="8a20a-131">userId</span></span>            |`string`      |<span data-ttu-id="8a20a-132">Идентификатор пользователя, назначенного объекту `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="8a20a-132">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="8a20a-133">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="8a20a-133">Required.</span></span>|
| <span data-ttu-id="8a20a-134">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="8a20a-134">sharedTimeOff</span></span>     | [<span data-ttu-id="8a20a-135">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="8a20a-135">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="8a20a-136">Общая версия объекта `timeOff`, доступная для просмотра как сотрудникам, так и руководителям.</span><span class="sxs-lookup"><span data-stu-id="8a20a-136">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="8a20a-137">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="8a20a-137">Required.</span></span>|
| <span data-ttu-id="8a20a-138">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="8a20a-138">draftTimeOff</span></span>      | [<span data-ttu-id="8a20a-139">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="8a20a-139">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="8a20a-140">Черновая версия объекта `timeOff`, доступная для просмотра руководителями.</span><span class="sxs-lookup"><span data-stu-id="8a20a-140">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="8a20a-141">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="8a20a-141">Required.</span></span>|
| <span data-ttu-id="8a20a-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a20a-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="8a20a-143">Отметка времени, на которой `timeOff` это было впервые создано.</span><span class="sxs-lookup"><span data-stu-id="8a20a-143">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="8a20a-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8a20a-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8a20a-145">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8a20a-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="8a20a-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a20a-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="8a20a-147">Отпечаток времени, на котором `timeOff` это было в последний раз обновлено.</span><span class="sxs-lookup"><span data-stu-id="8a20a-147">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="8a20a-148">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8a20a-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8a20a-149">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8a20a-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="8a20a-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8a20a-150">lastModifiedBy</span></span>        | [<span data-ttu-id="8a20a-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="8a20a-151">identitySet</span></span>](identityset.md)        |<span data-ttu-id="8a20a-152">Учетная запись, которая последней обновила этот объект `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="8a20a-152">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8a20a-153">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8a20a-153">JSON representation</span></span>

<span data-ttu-id="8a20a-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a20a-154">Here is a JSON representation of the resource.</span></span>

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


