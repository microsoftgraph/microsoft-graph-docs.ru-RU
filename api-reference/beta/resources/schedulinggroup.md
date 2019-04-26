---
title: Тип ресурса schedulingGroup
description: Логическая группа участников расписания (как правило, по роли).
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 644a9492e47979241ccab3f0e69eb90407eb2647
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562956"
---
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="12ee8-103">Тип ресурса schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="12ee8-103">schedulingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12ee8-104">Логическая группа участников [расписания](schedule.md) (как правило, по роли).</span><span class="sxs-lookup"><span data-stu-id="12ee8-104">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="12ee8-105">Методы</span><span class="sxs-lookup"><span data-stu-id="12ee8-105">Methods</span></span>

| <span data-ttu-id="12ee8-106">Метод</span><span class="sxs-lookup"><span data-stu-id="12ee8-106">Method</span></span>       | <span data-ttu-id="12ee8-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="12ee8-107">Return Type</span></span>  |<span data-ttu-id="12ee8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="12ee8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="12ee8-109">Создание объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="12ee8-109">Create schedulingGroup</span></span>](../api/schedule-post-schedulinggroups.md) | [<span data-ttu-id="12ee8-110">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="12ee8-110">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="12ee8-111">Создание объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="12ee8-111">Create a new `schedulingGroup`.</span></span>|
|[<span data-ttu-id="12ee8-112">Список объектов schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="12ee8-112">List schedulingGroups</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="12ee8-113">Коллекция [schedulingGroup](schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="12ee8-113">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="12ee8-114">Получение списка объектов `schedulingGroups` в расписании.</span><span class="sxs-lookup"><span data-stu-id="12ee8-114">Get the list of `schedulingGroups` in a schedule.</span></span>|
|[<span data-ttu-id="12ee8-115">Получение объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="12ee8-115">Get schedulingGroup</span></span>](../api/schedulinggroup-get.md) | [<span data-ttu-id="12ee8-116">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="12ee8-116">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="12ee8-117">Получение `schedulingGroup` по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="12ee8-117">Get a `schedulingGroup` by ID.</span></span>|
|[<span data-ttu-id="12ee8-118">Замена объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="12ee8-118">Replace schedulingGroup</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="12ee8-119">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="12ee8-119">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="12ee8-120">Замена объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="12ee8-120">Replace a `schedulingGroup`.</span></span>|
|[<span data-ttu-id="12ee8-121">Удаление объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="12ee8-121">Delete schedulingGroup</span></span>](../api/schedulinggroup-delete.md) | <span data-ttu-id="12ee8-122">Нет</span><span class="sxs-lookup"><span data-stu-id="12ee8-122">None</span></span> | <span data-ttu-id="12ee8-123">Объект `schedulingGroup` помечается как неактивный.</span><span class="sxs-lookup"><span data-stu-id="12ee8-123">Mark `schedulingGroup` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="12ee8-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="12ee8-124">Properties</span></span>
|<span data-ttu-id="12ee8-125">Имя</span><span class="sxs-lookup"><span data-stu-id="12ee8-125">Name</span></span>          |<span data-ttu-id="12ee8-126">Тип</span><span class="sxs-lookup"><span data-stu-id="12ee8-126">Type</span></span>           |<span data-ttu-id="12ee8-127">Описание</span><span class="sxs-lookup"><span data-stu-id="12ee8-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="12ee8-128">id</span><span class="sxs-lookup"><span data-stu-id="12ee8-128">id</span></span>            | `string`      |<span data-ttu-id="12ee8-129">Идентификатор объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="12ee8-129">ID of the `schedulingGroup`.</span></span>|
| <span data-ttu-id="12ee8-130">displayName</span><span class="sxs-lookup"><span data-stu-id="12ee8-130">displayName</span></span>   | `string`      | <span data-ttu-id="12ee8-131">Отображаемое имя объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="12ee8-131">The display name for the `schedulingGroup`.</span></span> <span data-ttu-id="12ee8-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12ee8-132">Required.</span></span> |
| <span data-ttu-id="12ee8-133">isActive</span><span class="sxs-lookup"><span data-stu-id="12ee8-133">isActive</span></span>          |`bool`      | <span data-ttu-id="12ee8-134">Указывает, можно ли использовать объект `schedulingGroup` при создании новых сущностей или обновлении существующих.</span><span class="sxs-lookup"><span data-stu-id="12ee8-134">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="12ee8-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12ee8-135">Required.</span></span> |
| <span data-ttu-id="12ee8-136">userIds</span><span class="sxs-lookup"><span data-stu-id="12ee8-136">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="12ee8-137">Список идентификаторов пользователей, являющихся участниками группы `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="12ee8-137">The list of user IDs that are a member of the `schedulingGroup`.</span></span> <span data-ttu-id="12ee8-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12ee8-138">Required.</span></span> |
| <span data-ttu-id="12ee8-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12ee8-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="12ee8-140">Метка времени создания объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="12ee8-140">The time stamp in which this `schedulingGroup` was first created.</span></span> <span data-ttu-id="12ee8-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="12ee8-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="12ee8-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="12ee8-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="12ee8-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12ee8-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="12ee8-144">Метка времени последнего обновления объекта `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="12ee8-144">The time stamp in which this `schedulingGroup` was last updated.</span></span> <span data-ttu-id="12ee8-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="12ee8-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="12ee8-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="12ee8-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="12ee8-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="12ee8-147">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="12ee8-148">Учетная запись, которая последней обновила этот объект `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="12ee8-148">The identity that last updated this `schedulingGroup`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12ee8-149">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="12ee8-149">JSON representation</span></span>

<span data-ttu-id="12ee8-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12ee8-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup"
}-->

```json
{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
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
  "suppressions": [
    "Error: /api-reference/beta/resources/schedulinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
