---
title: Тип ресурса schedulingGroup
description: Логическая группа участников расписания (как правило, по роли).
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: fb8ed65991d87780b6250841df8bdbdb089b7992
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343465"
---
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="fc1a1-103">Тип ресурса schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="fc1a1-103">schedulingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc1a1-104">Логическая группа участников [расписания](schedule.md) (как правило, по роли).</span><span class="sxs-lookup"><span data-stu-id="fc1a1-104">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="fc1a1-105">Методы</span><span class="sxs-lookup"><span data-stu-id="fc1a1-105">Methods</span></span>

| <span data-ttu-id="fc1a1-106">Метод</span><span class="sxs-lookup"><span data-stu-id="fc1a1-106">Method</span></span>       | <span data-ttu-id="fc1a1-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fc1a1-107">Return Type</span></span>  |<span data-ttu-id="fc1a1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fc1a1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fc1a1-109">Создание объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="fc1a1-109">Create schedulingGroup</span></span>](../api/schedule-post-schedulinggroups.md) | [<span data-ttu-id="fc1a1-110">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="fc1a1-110">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="fc1a1-111">Создание объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-111">Create a new `schedulingGroup`.</span></span>|
|[<span data-ttu-id="fc1a1-112">Список объектов schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="fc1a1-112">List schedulingGroups</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="fc1a1-113">Коллекция [schedulingGroup](schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="fc1a1-113">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="fc1a1-114">Получение списка объектов `schedulingGroups` в расписании.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-114">Get the list of `schedulingGroups` in a schedule.</span></span>|
|[<span data-ttu-id="fc1a1-115">Получение объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="fc1a1-115">Get schedulingGroup</span></span>](../api/schedulinggroup-get.md) | [<span data-ttu-id="fc1a1-116">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="fc1a1-116">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="fc1a1-117">Получение `schedulingGroup` по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-117">Get a `schedulingGroup` by ID.</span></span>|
|[<span data-ttu-id="fc1a1-118">Замена объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="fc1a1-118">Replace schedulingGroup</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="fc1a1-119">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="fc1a1-119">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="fc1a1-120">Замена объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-120">Replace a `schedulingGroup`.</span></span>|
|[<span data-ttu-id="fc1a1-121">Удаление объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="fc1a1-121">Delete schedulingGroup</span></span>](../api/schedulinggroup-delete.md) | <span data-ttu-id="fc1a1-122">Нет</span><span class="sxs-lookup"><span data-stu-id="fc1a1-122">None</span></span> | <span data-ttu-id="fc1a1-123">Объект `schedulingGroup` помечается как неактивный.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-123">Mark `schedulingGroup` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="fc1a1-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc1a1-124">Properties</span></span>
|<span data-ttu-id="fc1a1-125">Имя</span><span class="sxs-lookup"><span data-stu-id="fc1a1-125">Name</span></span>          |<span data-ttu-id="fc1a1-126">Тип</span><span class="sxs-lookup"><span data-stu-id="fc1a1-126">Type</span></span>           |<span data-ttu-id="fc1a1-127">Описание</span><span class="sxs-lookup"><span data-stu-id="fc1a1-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="fc1a1-128">id</span><span class="sxs-lookup"><span data-stu-id="fc1a1-128">id</span></span>            | `string`      |<span data-ttu-id="fc1a1-129">Идентификатор объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-129">ID of the `schedulingGroup`.</span></span>|
| <span data-ttu-id="fc1a1-130">displayName</span><span class="sxs-lookup"><span data-stu-id="fc1a1-130">displayName</span></span>   | `string`      | <span data-ttu-id="fc1a1-131">Отображаемое имя объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-131">The display name for the `schedulingGroup`.</span></span> <span data-ttu-id="fc1a1-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-132">Required.</span></span> |
| <span data-ttu-id="fc1a1-133">isActive</span><span class="sxs-lookup"><span data-stu-id="fc1a1-133">isActive</span></span>          |`bool`      | <span data-ttu-id="fc1a1-134">Указывает, можно ли использовать объект `schedulingGroup` при создании новых сущностей или обновлении существующих.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-134">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="fc1a1-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-135">Required.</span></span> |
| <span data-ttu-id="fc1a1-136">userIds</span><span class="sxs-lookup"><span data-stu-id="fc1a1-136">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="fc1a1-137">Список идентификаторов пользователей, являющихся участниками группы `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-137">The list of user IDs that are a member of the `schedulingGroup`.</span></span> <span data-ttu-id="fc1a1-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-138">Required.</span></span> |
| <span data-ttu-id="fc1a1-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc1a1-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="fc1a1-140">Метка времени создания объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-140">The time stamp in which this `schedulingGroup` was first created.</span></span> <span data-ttu-id="fc1a1-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fc1a1-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fc1a1-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="fc1a1-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="fc1a1-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc1a1-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="fc1a1-144">Метка времени последнего обновления объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-144">The time stamp in which this `schedulingGroup` was last updated.</span></span> <span data-ttu-id="fc1a1-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fc1a1-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fc1a1-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="fc1a1-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="fc1a1-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="fc1a1-147">lastModifiedBy</span></span>        | [<span data-ttu-id="fc1a1-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="fc1a1-148">identitySet</span></span>](identityset.md) |<span data-ttu-id="fc1a1-149">Учетная запись, которая последней обновила этот объект `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-149">The identity that last updated this `schedulingGroup`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc1a1-150">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fc1a1-150">JSON representation</span></span>

<span data-ttu-id="fc1a1-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc1a1-151">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup",
  "baseType": "microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "isActive": true,
  "userIds": ["String (identifier)"],
  "lastModifiedBy":{"@odata.type":"microsoft.graph.identitySet"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedulingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
