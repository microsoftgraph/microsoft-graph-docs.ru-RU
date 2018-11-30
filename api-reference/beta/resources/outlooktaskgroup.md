---
title: Тип ресурса outlookTaskGroup
description: 'Группа папок (outlookTaskFolder), которые содержат задачи Outlook (коллекцию объектов outlookTask). '
ms.openlocfilehash: 4896b114bf04b7e1703886453f21a4e015c9e7d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081610"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="f59b6-103">Тип ресурса outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="f59b6-103">outlookTaskGroup resource type</span></span>

> <span data-ttu-id="f59b6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f59b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f59b6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f59b6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f59b6-106">Группа папок ([outlookTaskFolder](outlooktaskfolder.md)), которые содержат задачи Outlook (коллекцию объектов [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="f59b6-106">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="f59b6-107">В программе Outlook является группу задач по умолчанию `My Tasks` которого невозможно переименование или удаление.</span><span class="sxs-lookup"><span data-stu-id="f59b6-107">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="f59b6-108">Тем не менее, можно создать дополнительные группы задач.</span><span class="sxs-lookup"><span data-stu-id="f59b6-108">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="f59b6-109">Методы</span><span class="sxs-lookup"><span data-stu-id="f59b6-109">Methods</span></span>

| <span data-ttu-id="f59b6-110">Метод</span><span class="sxs-lookup"><span data-stu-id="f59b6-110">Method</span></span>           | <span data-ttu-id="f59b6-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f59b6-111">Return Type</span></span>    |<span data-ttu-id="f59b6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f59b6-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f59b6-113">Получение outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="f59b6-113">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="f59b6-114">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="f59b6-114">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="f59b6-115">Получите свойства и связи в указанную группу задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="f59b6-115">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="f59b6-116">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="f59b6-116">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="f59b6-117">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="f59b6-117">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="f59b6-118">Создайте папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="f59b6-118">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="f59b6-119">Список taskFolders</span><span class="sxs-lookup"><span data-stu-id="f59b6-119">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="f59b6-120">[outlookTaskFolder](outlooktaskfolder.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f59b6-120">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="f59b6-121">Получите коллекцию папок задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="f59b6-121">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="f59b6-122">Update</span><span class="sxs-lookup"><span data-stu-id="f59b6-122">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="f59b6-123">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="f59b6-123">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="f59b6-124">Обновление для записи свойств группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="f59b6-124">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="f59b6-125">Delete</span><span class="sxs-lookup"><span data-stu-id="f59b6-125">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="f59b6-126">Нет</span><span class="sxs-lookup"><span data-stu-id="f59b6-126">None</span></span> |<span data-ttu-id="f59b6-127">Удаление указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="f59b6-127">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="f59b6-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="f59b6-128">Properties</span></span>
| <span data-ttu-id="f59b6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f59b6-129">Property</span></span>     | <span data-ttu-id="f59b6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f59b6-130">Type</span></span>   |<span data-ttu-id="f59b6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f59b6-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f59b6-132">changeKey</span><span class="sxs-lookup"><span data-stu-id="f59b6-132">changeKey</span></span>|<span data-ttu-id="f59b6-133">String</span><span class="sxs-lookup"><span data-stu-id="f59b6-133">String</span></span>|<span data-ttu-id="f59b6-134">Версия групповой задачи.</span><span class="sxs-lookup"><span data-stu-id="f59b6-134">The version of the task group.</span></span>|
|<span data-ttu-id="f59b6-135">groupKey</span><span class="sxs-lookup"><span data-stu-id="f59b6-135">groupKey</span></span>|<span data-ttu-id="f59b6-136">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="f59b6-136">Edm.Guid</span></span>|<span data-ttu-id="f59b6-137">Уникальный идентификатор GUID для группы задач.</span><span class="sxs-lookup"><span data-stu-id="f59b6-137">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="f59b6-138">id</span><span class="sxs-lookup"><span data-stu-id="f59b6-138">id</span></span>|<span data-ttu-id="f59b6-139">String</span><span class="sxs-lookup"><span data-stu-id="f59b6-139">String</span></span>|<span data-ttu-id="f59b6-140">Уникальная строка идентификатор группы задач.</span><span class="sxs-lookup"><span data-stu-id="f59b6-140">The unique string identifier of the task group.</span></span> <span data-ttu-id="f59b6-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f59b6-141">Read-only.</span></span>|
|<span data-ttu-id="f59b6-142">isDefaultGroup</span><span class="sxs-lookup"><span data-stu-id="f59b6-142">isDefaultGroup</span></span>|<span data-ttu-id="f59b6-143">Логический</span><span class="sxs-lookup"><span data-stu-id="f59b6-143">Boolean</span></span>|<span data-ttu-id="f59b6-144">Значение true, если группа задач является группу задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f59b6-144">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="f59b6-145">name</span><span class="sxs-lookup"><span data-stu-id="f59b6-145">name</span></span>|<span data-ttu-id="f59b6-146">String</span><span class="sxs-lookup"><span data-stu-id="f59b6-146">String</span></span>|<span data-ttu-id="f59b6-147">Имя группы задач.</span><span class="sxs-lookup"><span data-stu-id="f59b6-147">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f59b6-148">Связи</span><span class="sxs-lookup"><span data-stu-id="f59b6-148">Relationships</span></span>
| <span data-ttu-id="f59b6-149">Связь</span><span class="sxs-lookup"><span data-stu-id="f59b6-149">Relationship</span></span> | <span data-ttu-id="f59b6-150">Тип</span><span class="sxs-lookup"><span data-stu-id="f59b6-150">Type</span></span>   |<span data-ttu-id="f59b6-151">Description</span><span class="sxs-lookup"><span data-stu-id="f59b6-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f59b6-152">taskFolders</span><span class="sxs-lookup"><span data-stu-id="f59b6-152">taskFolders</span></span>|<span data-ttu-id="f59b6-153">[outlookTaskFolder](outlooktaskfolder.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f59b6-153">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="f59b6-154">Коллекция папок задач в группе задач.</span><span class="sxs-lookup"><span data-stu-id="f59b6-154">The collection of task folders in the task group.</span></span> <span data-ttu-id="f59b6-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f59b6-155">Read-only.</span></span> <span data-ttu-id="f59b6-156">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f59b6-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f59b6-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f59b6-157">JSON representation</span></span>
<span data-ttu-id="f59b6-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f59b6-158">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->