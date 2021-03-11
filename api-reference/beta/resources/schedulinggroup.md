---
title: Тип ресурса schedulingGroup
description: Логическая группа участников расписания (как правило, по роли).
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c20fd79c9539ed2502960a63cb5b1de154c9693a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721476"
---
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="9419f-103">Тип ресурса schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9419f-103">schedulingGroup resource type</span></span>

<span data-ttu-id="9419f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9419f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9419f-105">Логическая группа участников [расписания](schedule.md) (как правило, по роли).</span><span class="sxs-lookup"><span data-stu-id="9419f-105">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="9419f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9419f-106">Methods</span></span>

| <span data-ttu-id="9419f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9419f-107">Method</span></span>       | <span data-ttu-id="9419f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9419f-108">Return Type</span></span>  |<span data-ttu-id="9419f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9419f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9419f-110">Создание объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9419f-110">Create schedulingGroup</span></span>](../api/schedule-post-schedulinggroups.md) | [<span data-ttu-id="9419f-111">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9419f-111">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="9419f-112">Создание объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="9419f-112">Create a new `schedulingGroup`.</span></span>|
|[<span data-ttu-id="9419f-113">Список объектов schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9419f-113">List schedulingGroups</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="9419f-114">Коллекция [schedulingGroup](schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="9419f-114">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="9419f-115">Получение списка объектов `schedulingGroups` в расписании.</span><span class="sxs-lookup"><span data-stu-id="9419f-115">Get the list of `schedulingGroups` in a schedule.</span></span>|
|[<span data-ttu-id="9419f-116">Получение объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9419f-116">Get schedulingGroup</span></span>](../api/schedulinggroup-get.md) | [<span data-ttu-id="9419f-117">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9419f-117">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="9419f-118">Получение `schedulingGroup` по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="9419f-118">Get a `schedulingGroup` by ID.</span></span>|
|[<span data-ttu-id="9419f-119">Замена объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9419f-119">Replace schedulingGroup</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="9419f-120">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9419f-120">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="9419f-121">Замена объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="9419f-121">Replace a `schedulingGroup`.</span></span>|
|[<span data-ttu-id="9419f-122">Удаление объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9419f-122">Delete schedulingGroup</span></span>](../api/schedulinggroup-delete.md) | <span data-ttu-id="9419f-123">Нет</span><span class="sxs-lookup"><span data-stu-id="9419f-123">None</span></span> | <span data-ttu-id="9419f-124">Объект `schedulingGroup` помечается как неактивный.</span><span class="sxs-lookup"><span data-stu-id="9419f-124">Mark `schedulingGroup` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="9419f-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="9419f-125">Properties</span></span>
|<span data-ttu-id="9419f-126">Имя</span><span class="sxs-lookup"><span data-stu-id="9419f-126">Name</span></span>          |<span data-ttu-id="9419f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="9419f-127">Type</span></span>           |<span data-ttu-id="9419f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9419f-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="9419f-129">id</span><span class="sxs-lookup"><span data-stu-id="9419f-129">id</span></span>            | `string`      |<span data-ttu-id="9419f-130">Идентификатор объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="9419f-130">ID of the `schedulingGroup`.</span></span>|
| <span data-ttu-id="9419f-131">displayName</span><span class="sxs-lookup"><span data-stu-id="9419f-131">displayName</span></span>   | `string`      | <span data-ttu-id="9419f-132">Отображаемое имя объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="9419f-132">The display name for the `schedulingGroup`.</span></span> <span data-ttu-id="9419f-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9419f-133">Required.</span></span> |
| <span data-ttu-id="9419f-134">isActive</span><span class="sxs-lookup"><span data-stu-id="9419f-134">isActive</span></span>          |`bool`      | <span data-ttu-id="9419f-135">Указывает, можно ли использовать объект `schedulingGroup` при создании новых сущностей или обновлении существующих.</span><span class="sxs-lookup"><span data-stu-id="9419f-135">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="9419f-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9419f-136">Required.</span></span> |
| <span data-ttu-id="9419f-137">userIds</span><span class="sxs-lookup"><span data-stu-id="9419f-137">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="9419f-138">Список идентификаторов пользователей, являющихся участниками группы `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="9419f-138">The list of user IDs that are a member of the `schedulingGroup`.</span></span> <span data-ttu-id="9419f-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9419f-139">Required.</span></span> |
| <span data-ttu-id="9419f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9419f-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="9419f-141">Метка времени создания объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="9419f-141">The time stamp in which this `schedulingGroup` was first created.</span></span> <span data-ttu-id="9419f-142">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9419f-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9419f-143">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="9419f-143">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="9419f-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9419f-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="9419f-145">Метка времени последнего обновления объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="9419f-145">The time stamp in which this `schedulingGroup` was last updated.</span></span> <span data-ttu-id="9419f-146">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9419f-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9419f-147">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="9419f-147">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="9419f-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="9419f-148">lastModifiedBy</span></span>        | [<span data-ttu-id="9419f-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="9419f-149">identitySet</span></span>](identityset.md) |<span data-ttu-id="9419f-150">Учетная запись, которая последней обновила этот объект `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="9419f-150">The identity that last updated this `schedulingGroup`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9419f-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9419f-151">JSON representation</span></span>

<span data-ttu-id="9419f-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9419f-152">Here is a JSON representation of the resource.</span></span>

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


