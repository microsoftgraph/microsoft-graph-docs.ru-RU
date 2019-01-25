---
title: Тип ресурса outlookTaskGroup
description: 'Группа папок (outlookTaskFolder), которые содержат задачи Outlook (коллекцию объектов outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 486261d80b8faad7a5969f8f1ce198479e39583c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524620"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="52fc5-103">Тип ресурса outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="52fc5-103">outlookTaskGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52fc5-104">Группа папок ([outlookTaskFolder](outlooktaskfolder.md)), которые содержат задачи Outlook (коллекцию объектов [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="52fc5-104">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="52fc5-105">В программе Outlook является группу задач по умолчанию `My Tasks` которого невозможно переименование или удаление.</span><span class="sxs-lookup"><span data-stu-id="52fc5-105">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="52fc5-106">Тем не менее, можно создать дополнительные группы задач.</span><span class="sxs-lookup"><span data-stu-id="52fc5-106">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="52fc5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="52fc5-107">Methods</span></span>

| <span data-ttu-id="52fc5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="52fc5-108">Method</span></span>           | <span data-ttu-id="52fc5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="52fc5-109">Return Type</span></span>    |<span data-ttu-id="52fc5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="52fc5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52fc5-111">Получение outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="52fc5-111">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="52fc5-112">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="52fc5-112">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="52fc5-113">Получите свойства и связи в указанную группу задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="52fc5-113">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="52fc5-114">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="52fc5-114">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="52fc5-115">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="52fc5-115">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="52fc5-116">Создайте папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="52fc5-116">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="52fc5-117">Список taskFolders</span><span class="sxs-lookup"><span data-stu-id="52fc5-117">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="52fc5-118">[outlookTaskFolder](outlooktaskfolder.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="52fc5-118">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="52fc5-119">Получите коллекцию папок задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="52fc5-119">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="52fc5-120">Update</span><span class="sxs-lookup"><span data-stu-id="52fc5-120">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="52fc5-121">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="52fc5-121">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="52fc5-122">Обновление для записи свойств группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="52fc5-122">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="52fc5-123">Delete</span><span class="sxs-lookup"><span data-stu-id="52fc5-123">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="52fc5-124">Нет</span><span class="sxs-lookup"><span data-stu-id="52fc5-124">None</span></span> |<span data-ttu-id="52fc5-125">Удаление указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="52fc5-125">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="52fc5-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="52fc5-126">Properties</span></span>
| <span data-ttu-id="52fc5-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="52fc5-127">Property</span></span>     | <span data-ttu-id="52fc5-128">Тип</span><span class="sxs-lookup"><span data-stu-id="52fc5-128">Type</span></span>   |<span data-ttu-id="52fc5-129">Описание</span><span class="sxs-lookup"><span data-stu-id="52fc5-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52fc5-130">changeKey</span><span class="sxs-lookup"><span data-stu-id="52fc5-130">changeKey</span></span>|<span data-ttu-id="52fc5-131">String</span><span class="sxs-lookup"><span data-stu-id="52fc5-131">String</span></span>|<span data-ttu-id="52fc5-132">Версия групповой задачи.</span><span class="sxs-lookup"><span data-stu-id="52fc5-132">The version of the task group.</span></span>|
|<span data-ttu-id="52fc5-133">groupKey</span><span class="sxs-lookup"><span data-stu-id="52fc5-133">groupKey</span></span>|<span data-ttu-id="52fc5-134">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="52fc5-134">Edm.Guid</span></span>|<span data-ttu-id="52fc5-135">Уникальный идентификатор GUID для группы задач.</span><span class="sxs-lookup"><span data-stu-id="52fc5-135">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="52fc5-136">id</span><span class="sxs-lookup"><span data-stu-id="52fc5-136">id</span></span>|<span data-ttu-id="52fc5-137">String</span><span class="sxs-lookup"><span data-stu-id="52fc5-137">String</span></span>|<span data-ttu-id="52fc5-138">Уникальная строка идентификатор группы задач.</span><span class="sxs-lookup"><span data-stu-id="52fc5-138">The unique string identifier of the task group.</span></span> <span data-ttu-id="52fc5-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="52fc5-139">Read-only.</span></span>|
|<span data-ttu-id="52fc5-140">isDefaultGroup</span><span class="sxs-lookup"><span data-stu-id="52fc5-140">isDefaultGroup</span></span>|<span data-ttu-id="52fc5-141">Логическое</span><span class="sxs-lookup"><span data-stu-id="52fc5-141">Boolean</span></span>|<span data-ttu-id="52fc5-142">Значение true, если группа задач является группу задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="52fc5-142">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="52fc5-143">name</span><span class="sxs-lookup"><span data-stu-id="52fc5-143">name</span></span>|<span data-ttu-id="52fc5-144">String</span><span class="sxs-lookup"><span data-stu-id="52fc5-144">String</span></span>|<span data-ttu-id="52fc5-145">Имя группы задач.</span><span class="sxs-lookup"><span data-stu-id="52fc5-145">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52fc5-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="52fc5-146">Relationships</span></span>
| <span data-ttu-id="52fc5-147">Связь</span><span class="sxs-lookup"><span data-stu-id="52fc5-147">Relationship</span></span> | <span data-ttu-id="52fc5-148">Тип</span><span class="sxs-lookup"><span data-stu-id="52fc5-148">Type</span></span>   |<span data-ttu-id="52fc5-149">Описание</span><span class="sxs-lookup"><span data-stu-id="52fc5-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52fc5-150">taskFolders</span><span class="sxs-lookup"><span data-stu-id="52fc5-150">taskFolders</span></span>|<span data-ttu-id="52fc5-151">[outlookTaskFolder](outlooktaskfolder.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="52fc5-151">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="52fc5-152">Коллекция папок задач в группе задач.</span><span class="sxs-lookup"><span data-stu-id="52fc5-152">The collection of task folders in the task group.</span></span> <span data-ttu-id="52fc5-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="52fc5-153">Read-only.</span></span> <span data-ttu-id="52fc5-154">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="52fc5-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52fc5-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52fc5-155">JSON representation</span></span>
<span data-ttu-id="52fc5-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52fc5-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookTaskGroup"
}-->

```json
{
  "changeKey": "String",
  "groupKey": "Guid",
  "id": "String (identifier)",
  "isDefaultGroup": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlooktaskgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
