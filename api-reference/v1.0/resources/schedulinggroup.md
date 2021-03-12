---
title: Тип ресурса schedulingGroup
description: Логическая группа участников расписания (как правило, по роли).
author: akumar39
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 018359ab0dd6702a2fda40bf5f0b29c639211f4a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719306"
---
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="a914a-103">Тип ресурса schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="a914a-103">schedulingGroup resource type</span></span>

<span data-ttu-id="a914a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a914a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a914a-105">Логическая группа участников [расписания](schedule.md) (как правило, по роли).</span><span class="sxs-lookup"><span data-stu-id="a914a-105">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="a914a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a914a-106">Methods</span></span>

| <span data-ttu-id="a914a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a914a-107">Method</span></span>       | <span data-ttu-id="a914a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a914a-108">Return Type</span></span>  |<span data-ttu-id="a914a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a914a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a914a-110">Список</span><span class="sxs-lookup"><span data-stu-id="a914a-110">List</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="a914a-111">Коллекция объектов [schedulingGroup](schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="a914a-111">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="a914a-112">Вы можете просмотреть список объектов **schedulingGroups** в расписании.</span><span class="sxs-lookup"><span data-stu-id="a914a-112">Get the list of **schedulingGroups** in a schedule.</span></span>|
|<span data-ttu-id="a914a-113">[Создание](../api/schedule-post-schedulinggroups.md);</span><span class="sxs-lookup"><span data-stu-id="a914a-113">[Create](../api/schedule-post-schedulinggroups.md)</span></span> | [<span data-ttu-id="a914a-114">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="a914a-114">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="a914a-115">Создание нового объекта **schedulingGroup**</span><span class="sxs-lookup"><span data-stu-id="a914a-115">Create a new **schedulingGroup**.</span></span>|
|<span data-ttu-id="a914a-116">[Получение](../api/schedulinggroup-get.md);</span><span class="sxs-lookup"><span data-stu-id="a914a-116">[Get](../api/schedulinggroup-get.md)</span></span> | [<span data-ttu-id="a914a-117">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="a914a-117">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="a914a-118">Получение объекта **schedulingGroup** по ИД</span><span class="sxs-lookup"><span data-stu-id="a914a-118">Get a **schedulingGroup** by ID.</span></span>|
|<span data-ttu-id="a914a-119">[удаление](../api/schedulinggroup-delete.md);</span><span class="sxs-lookup"><span data-stu-id="a914a-119">[Delete](../api/schedulinggroup-delete.md)</span></span> | <span data-ttu-id="a914a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="a914a-120">None</span></span> | <span data-ttu-id="a914a-121">Обозначение объекта **schedulingGroup** как неактивного.</span><span class="sxs-lookup"><span data-stu-id="a914a-121">Mark **schedulingGroup** as inactive.</span></span>|
|[<span data-ttu-id="a914a-122">Замена</span><span class="sxs-lookup"><span data-stu-id="a914a-122">Replace</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="a914a-123">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="a914a-123">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="a914a-124">Замена объекта **schedulingGroup**.</span><span class="sxs-lookup"><span data-stu-id="a914a-124">Replace a **schedulingGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="a914a-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="a914a-125">Properties</span></span>
|<span data-ttu-id="a914a-126">Имя</span><span class="sxs-lookup"><span data-stu-id="a914a-126">Name</span></span>          |<span data-ttu-id="a914a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a914a-127">Type</span></span>           |<span data-ttu-id="a914a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a914a-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="a914a-129">id</span><span class="sxs-lookup"><span data-stu-id="a914a-129">id</span></span>            | `string`      |<span data-ttu-id="a914a-130">ИД объекта **schedulingGroup**</span><span class="sxs-lookup"><span data-stu-id="a914a-130">ID of the **schedulingGroup**.</span></span>|
| <span data-ttu-id="a914a-131">displayName</span><span class="sxs-lookup"><span data-stu-id="a914a-131">displayName</span></span>   | `string`      | <span data-ttu-id="a914a-132">Отображаемое имя для объекта **schedulingGroup**.</span><span class="sxs-lookup"><span data-stu-id="a914a-132">The display name for the **schedulingGroup**.</span></span> <span data-ttu-id="a914a-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a914a-133">Required.</span></span> |
| <span data-ttu-id="a914a-134">isActive</span><span class="sxs-lookup"><span data-stu-id="a914a-134">isActive</span></span>          |`bool`      | <span data-ttu-id="a914a-135">Указывает, можно ли использовать объект `schedulingGroup` при создании новых сущностей или обновлении существующих.</span><span class="sxs-lookup"><span data-stu-id="a914a-135">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="a914a-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a914a-136">Required.</span></span> |
| <span data-ttu-id="a914a-137">userIds</span><span class="sxs-lookup"><span data-stu-id="a914a-137">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="a914a-138">Список ИД пользователей, являющихся участниками **schedulingGroup**.</span><span class="sxs-lookup"><span data-stu-id="a914a-138">The list of user IDs that are a member of the **schedulingGroup**.</span></span> <span data-ttu-id="a914a-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a914a-139">Required.</span></span> |
| <span data-ttu-id="a914a-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a914a-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="a914a-141">Метка времени первоначального создания объекта **schedulingGroup**.</span><span class="sxs-lookup"><span data-stu-id="a914a-141">The time stamp in which this **schedulingGroup** was first created.</span></span> <span data-ttu-id="a914a-142">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a914a-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a914a-143">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="a914a-143">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="a914a-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a914a-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="a914a-145">Метка времени последнего обновления объекта **schedulingGroup**.</span><span class="sxs-lookup"><span data-stu-id="a914a-145">The time stamp in which this **schedulingGroup** was last updated.</span></span> <span data-ttu-id="a914a-146">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a914a-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a914a-147">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="a914a-147">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="a914a-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a914a-148">lastModifiedBy</span></span>        | [<span data-ttu-id="a914a-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="a914a-149">identitySet</span></span>](identityset.md) |<span data-ttu-id="a914a-150">Учетная запись, которая последней обновила этот объект **schedulingGroup**.</span><span class="sxs-lookup"><span data-stu-id="a914a-150">The identity that last updated this **schedulingGroup**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a914a-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a914a-151">JSON representation</span></span>

<span data-ttu-id="a914a-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a914a-152">The following is a JSON representation of the resource.</span></span>

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

