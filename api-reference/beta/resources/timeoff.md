---
title: Тип ресурса Тимеофф
description: Единица измерения, которая не работает в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 848365a812053b7788db37395bee8662d69cda37
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342037"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="da98b-103">Тип ресурса Тимеофф</span><span class="sxs-lookup"><span data-stu-id="da98b-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da98b-104">Единица измерения, которая не работает в расписании.</span><span class="sxs-lookup"><span data-stu-id="da98b-104">A unit of non-work in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="da98b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="da98b-105">Methods</span></span>

| <span data-ttu-id="da98b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="da98b-106">Method</span></span>       | <span data-ttu-id="da98b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="da98b-107">Return Type</span></span>  |<span data-ttu-id="da98b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="da98b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="da98b-109">Создание Тимеофф</span><span class="sxs-lookup"><span data-stu-id="da98b-109">Create timeOff</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="da98b-110">Тимеофф</span><span class="sxs-lookup"><span data-stu-id="da98b-110">timeOff</span></span>](timeOff.md) | <span data-ttu-id="da98b-111">Создание нового объекта `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="da98b-111">Create a new `timeOff` object.</span></span>|
|[<span data-ttu-id="da98b-112">Список Тимеоффс</span><span class="sxs-lookup"><span data-stu-id="da98b-112">List timeOffs</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="da98b-113">Коллекция [тимеофф](timeOff.md)</span><span class="sxs-lookup"><span data-stu-id="da98b-113">[timeOff](timeOff.md) collection</span></span> | <span data-ttu-id="da98b-114">Получение списка `timeOff` объектов в расписании.</span><span class="sxs-lookup"><span data-stu-id="da98b-114">Get the list of `timeOff` objects in this schedule.</span></span>|
|[<span data-ttu-id="da98b-115">Получение Тимеофф</span><span class="sxs-lookup"><span data-stu-id="da98b-115">Get timeOff</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="da98b-116">Тимеофф</span><span class="sxs-lookup"><span data-stu-id="da98b-116">timeOff</span></span>](timeOff.md) | <span data-ttu-id="da98b-117">Получение `timeOff` по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="da98b-117">Get a `timeOff` by ID.</span></span>|
|[<span data-ttu-id="da98b-118">Замена Тимеофф</span><span class="sxs-lookup"><span data-stu-id="da98b-118">Replace timeOff</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="da98b-119">Тимеофф</span><span class="sxs-lookup"><span data-stu-id="da98b-119">timeOff</span></span>](timeOff.md) | <span data-ttu-id="da98b-120">Замена объекта `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="da98b-120">Replace a `timeOff`.</span></span>|
|[<span data-ttu-id="da98b-121">Удаление Тимеофф</span><span class="sxs-lookup"><span data-stu-id="da98b-121">Delete timeOff</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="da98b-122">Нет</span><span class="sxs-lookup"><span data-stu-id="da98b-122">None</span></span> | <span data-ttu-id="da98b-123">Удаление `timeOff` из расписания.</span><span class="sxs-lookup"><span data-stu-id="da98b-123">Delete a `timeOff` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="da98b-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="da98b-124">Properties</span></span>
|<span data-ttu-id="da98b-125">Имя</span><span class="sxs-lookup"><span data-stu-id="da98b-125">Name</span></span>          |<span data-ttu-id="da98b-126">Тип</span><span class="sxs-lookup"><span data-stu-id="da98b-126">Type</span></span>           |<span data-ttu-id="da98b-127">Описание</span><span class="sxs-lookup"><span data-stu-id="da98b-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="da98b-128">id</span><span class="sxs-lookup"><span data-stu-id="da98b-128">id</span></span>            |`string`      |<span data-ttu-id="da98b-129">Идентификатор объекта `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="da98b-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="da98b-130">userId</span><span class="sxs-lookup"><span data-stu-id="da98b-130">userId</span></span>            |`string`      |<span data-ttu-id="da98b-131">Идентификатор пользователя, `timeOff`назначенный.</span><span class="sxs-lookup"><span data-stu-id="da98b-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="da98b-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da98b-132">Required.</span></span>|
| <span data-ttu-id="da98b-133">Шаредтимеофф</span><span class="sxs-lookup"><span data-stu-id="da98b-133">sharedTimeOff</span></span>     | [<span data-ttu-id="da98b-134">Тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="da98b-134">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="da98b-135">Общая версия этого `timeOff` объекта доступна как для сотрудников, так и для руководителей.</span><span class="sxs-lookup"><span data-stu-id="da98b-135">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="da98b-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da98b-136">Required.</span></span>|
| <span data-ttu-id="da98b-137">Драфттимеофф</span><span class="sxs-lookup"><span data-stu-id="da98b-137">draftTimeOff</span></span>      | [<span data-ttu-id="da98b-138">Тимеоффитем</span><span class="sxs-lookup"><span data-stu-id="da98b-138">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="da98b-139">Черновая версия этого `timeOff` элемента, просматриваемая руководителями.</span><span class="sxs-lookup"><span data-stu-id="da98b-139">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="da98b-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da98b-140">Required.</span></span>|
| <span data-ttu-id="da98b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da98b-141">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="da98b-142">Отметка `timeOff` времени первоначального создания.</span><span class="sxs-lookup"><span data-stu-id="da98b-142">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="da98b-143">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="da98b-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="da98b-144">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="da98b-144">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="da98b-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da98b-145">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="da98b-146">Отметка `timeOff` времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="da98b-146">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="da98b-147">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="da98b-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="da98b-148">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="da98b-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="da98b-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="da98b-149">lastModifiedBy</span></span>        | [<span data-ttu-id="da98b-150">identitySet</span><span class="sxs-lookup"><span data-stu-id="da98b-150">identitySet</span></span>](identityset.md)        |<span data-ttu-id="da98b-151">Учетная запись, которая последней обновила этот объект `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="da98b-151">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="da98b-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="da98b-152">JSON representation</span></span>

<span data-ttu-id="da98b-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da98b-153">Here is a JSON representation of the resource.</span></span>

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
