---
title: Тип ресурса outlookTaskGroup
description: 'Группа папок (outlookTaskFolder), которая содержит задачи Outlook (Коллекция объектов outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: af5599773c6a4edef97356e99daa522760d9b37a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345541"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="95851-103">Тип ресурса outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="95851-103">outlookTaskGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95851-104">Группа папок ([outlookTaskFolder](outlooktaskfolder.md)), которая содержит задачи Outlook (Коллекция объектов [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="95851-104">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="95851-105">В Outlook существует группа `My Tasks` задач по умолчанию, которую нельзя переименовать или удалить.</span><span class="sxs-lookup"><span data-stu-id="95851-105">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="95851-106">Тем не менее, вы можете создать дополнительные группы задач.</span><span class="sxs-lookup"><span data-stu-id="95851-106">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="95851-107">Методы</span><span class="sxs-lookup"><span data-stu-id="95851-107">Methods</span></span>

| <span data-ttu-id="95851-108">Метод</span><span class="sxs-lookup"><span data-stu-id="95851-108">Method</span></span>           | <span data-ttu-id="95851-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="95851-109">Return Type</span></span>    |<span data-ttu-id="95851-110">Описание</span><span class="sxs-lookup"><span data-stu-id="95851-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="95851-111">Получение outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="95851-111">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="95851-112">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="95851-112">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="95851-113">Получение свойств и связей указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="95851-113">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="95851-114">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="95851-114">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="95851-115">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="95851-115">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="95851-116">Создайте папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="95851-116">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="95851-117">Список Таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="95851-117">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="95851-118">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="95851-118">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="95851-119">Получение коллекции папок задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="95851-119">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="95851-120">Обновление</span><span class="sxs-lookup"><span data-stu-id="95851-120">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="95851-121">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="95851-121">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="95851-122">Обновление свойств, доступных для записи, для группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="95851-122">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="95851-123">Удаление</span><span class="sxs-lookup"><span data-stu-id="95851-123">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="95851-124">Нет</span><span class="sxs-lookup"><span data-stu-id="95851-124">None</span></span> |<span data-ttu-id="95851-125">Удаление указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="95851-125">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="95851-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="95851-126">Properties</span></span>
| <span data-ttu-id="95851-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="95851-127">Property</span></span>     | <span data-ttu-id="95851-128">Тип</span><span class="sxs-lookup"><span data-stu-id="95851-128">Type</span></span>   |<span data-ttu-id="95851-129">Описание</span><span class="sxs-lookup"><span data-stu-id="95851-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95851-130">changeKey</span><span class="sxs-lookup"><span data-stu-id="95851-130">changeKey</span></span>|<span data-ttu-id="95851-131">String</span><span class="sxs-lookup"><span data-stu-id="95851-131">String</span></span>|<span data-ttu-id="95851-132">Версия группы задач.</span><span class="sxs-lookup"><span data-stu-id="95851-132">The version of the task group.</span></span>|
|<span data-ttu-id="95851-133">Граупкэй</span><span class="sxs-lookup"><span data-stu-id="95851-133">groupKey</span></span>|<span data-ttu-id="95851-134">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="95851-134">Edm.Guid</span></span>|<span data-ttu-id="95851-135">Уникальный идентификатор GUID для группы задач.</span><span class="sxs-lookup"><span data-stu-id="95851-135">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="95851-136">id</span><span class="sxs-lookup"><span data-stu-id="95851-136">id</span></span>|<span data-ttu-id="95851-137">String</span><span class="sxs-lookup"><span data-stu-id="95851-137">String</span></span>|<span data-ttu-id="95851-138">Уникальный строковый идентификатор группы задач.</span><span class="sxs-lookup"><span data-stu-id="95851-138">The unique string identifier of the task group.</span></span> <span data-ttu-id="95851-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95851-139">Read-only.</span></span>|
|<span data-ttu-id="95851-140">Исдефаултграуп</span><span class="sxs-lookup"><span data-stu-id="95851-140">isDefaultGroup</span></span>|<span data-ttu-id="95851-141">Логический</span><span class="sxs-lookup"><span data-stu-id="95851-141">Boolean</span></span>|<span data-ttu-id="95851-142">Значение true, если группа задач является группой задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="95851-142">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="95851-143">name</span><span class="sxs-lookup"><span data-stu-id="95851-143">name</span></span>|<span data-ttu-id="95851-144">String</span><span class="sxs-lookup"><span data-stu-id="95851-144">String</span></span>|<span data-ttu-id="95851-145">Имя группы задач.</span><span class="sxs-lookup"><span data-stu-id="95851-145">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95851-146">Связи</span><span class="sxs-lookup"><span data-stu-id="95851-146">Relationships</span></span>
| <span data-ttu-id="95851-147">Отношение</span><span class="sxs-lookup"><span data-stu-id="95851-147">Relationship</span></span> | <span data-ttu-id="95851-148">Тип</span><span class="sxs-lookup"><span data-stu-id="95851-148">Type</span></span>   |<span data-ttu-id="95851-149">Описание</span><span class="sxs-lookup"><span data-stu-id="95851-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95851-150">Таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="95851-150">taskFolders</span></span>|<span data-ttu-id="95851-151">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="95851-151">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="95851-152">Коллекция папок задач в группе задач.</span><span class="sxs-lookup"><span data-stu-id="95851-152">The collection of task folders in the task group.</span></span> <span data-ttu-id="95851-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95851-153">Read-only.</span></span> <span data-ttu-id="95851-154">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="95851-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95851-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95851-155">JSON representation</span></span>
<span data-ttu-id="95851-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95851-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
  "suppressions": []
}
-->
