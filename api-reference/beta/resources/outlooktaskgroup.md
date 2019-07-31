---
title: Тип ресурса outlookTaskGroup
description: 'Группа папок (outlookTaskFolder), которая содержит задачи Outlook (Коллекция объектов outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d519e18723ac9fbd38e7cec64a6758b0c9396bc2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966281"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="35261-103">Тип ресурса outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="35261-103">outlookTaskGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35261-104">Группа папок ([outlookTaskFolder](outlooktaskfolder.md)), которая содержит задачи Outlook (Коллекция объектов [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="35261-104">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="35261-105">В Outlook существует группа `My Tasks` задач по умолчанию, которую нельзя переименовать или удалить.</span><span class="sxs-lookup"><span data-stu-id="35261-105">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="35261-106">Тем не менее, вы можете создать дополнительные группы задач.</span><span class="sxs-lookup"><span data-stu-id="35261-106">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="35261-107">Методы</span><span class="sxs-lookup"><span data-stu-id="35261-107">Methods</span></span>

| <span data-ttu-id="35261-108">Метод</span><span class="sxs-lookup"><span data-stu-id="35261-108">Method</span></span>           | <span data-ttu-id="35261-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="35261-109">Return Type</span></span>    |<span data-ttu-id="35261-110">Описание</span><span class="sxs-lookup"><span data-stu-id="35261-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35261-111">Получение outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="35261-111">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="35261-112">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="35261-112">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="35261-113">Получение свойств и связей указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="35261-113">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="35261-114">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="35261-114">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="35261-115">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="35261-115">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="35261-116">Создайте папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="35261-116">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="35261-117">Список Таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="35261-117">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="35261-118">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="35261-118">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="35261-119">Получение коллекции папок задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="35261-119">Get a collection of Outlook task folders.</span></span>|
|<span data-ttu-id="35261-120">[обновление](../api/outlooktaskgroup-update.md);</span><span class="sxs-lookup"><span data-stu-id="35261-120">[Update](../api/outlooktaskgroup-update.md)</span></span> | [<span data-ttu-id="35261-121">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="35261-121">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="35261-122">Обновление свойств, доступных для записи, для группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="35261-122">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="35261-123">Удаление</span><span class="sxs-lookup"><span data-stu-id="35261-123">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="35261-124">Нет</span><span class="sxs-lookup"><span data-stu-id="35261-124">None</span></span> |<span data-ttu-id="35261-125">Удаление указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="35261-125">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="35261-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="35261-126">Properties</span></span>
| <span data-ttu-id="35261-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="35261-127">Property</span></span>     | <span data-ttu-id="35261-128">Тип</span><span class="sxs-lookup"><span data-stu-id="35261-128">Type</span></span>   |<span data-ttu-id="35261-129">Описание</span><span class="sxs-lookup"><span data-stu-id="35261-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35261-130">changeKey</span><span class="sxs-lookup"><span data-stu-id="35261-130">changeKey</span></span>|<span data-ttu-id="35261-131">String</span><span class="sxs-lookup"><span data-stu-id="35261-131">String</span></span>|<span data-ttu-id="35261-132">Версия группы задач.</span><span class="sxs-lookup"><span data-stu-id="35261-132">The version of the task group.</span></span>|
|<span data-ttu-id="35261-133">Граупкэй</span><span class="sxs-lookup"><span data-stu-id="35261-133">groupKey</span></span>|<span data-ttu-id="35261-134">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="35261-134">Edm.Guid</span></span>|<span data-ttu-id="35261-135">Уникальный идентификатор GUID для группы задач.</span><span class="sxs-lookup"><span data-stu-id="35261-135">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="35261-136">id</span><span class="sxs-lookup"><span data-stu-id="35261-136">id</span></span>|<span data-ttu-id="35261-137">String</span><span class="sxs-lookup"><span data-stu-id="35261-137">String</span></span>|<span data-ttu-id="35261-138">Уникальный строковый идентификатор группы задач.</span><span class="sxs-lookup"><span data-stu-id="35261-138">The unique string identifier of the task group.</span></span> <span data-ttu-id="35261-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35261-139">Read-only.</span></span>|
|<span data-ttu-id="35261-140">Исдефаултграуп</span><span class="sxs-lookup"><span data-stu-id="35261-140">isDefaultGroup</span></span>|<span data-ttu-id="35261-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="35261-141">Boolean</span></span>|<span data-ttu-id="35261-142">Значение true, если группа задач является группой задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="35261-142">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="35261-143">name</span><span class="sxs-lookup"><span data-stu-id="35261-143">name</span></span>|<span data-ttu-id="35261-144">String</span><span class="sxs-lookup"><span data-stu-id="35261-144">String</span></span>|<span data-ttu-id="35261-145">Имя группы задач.</span><span class="sxs-lookup"><span data-stu-id="35261-145">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35261-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="35261-146">Relationships</span></span>
| <span data-ttu-id="35261-147">Отношение</span><span class="sxs-lookup"><span data-stu-id="35261-147">Relationship</span></span> | <span data-ttu-id="35261-148">Тип</span><span class="sxs-lookup"><span data-stu-id="35261-148">Type</span></span>   |<span data-ttu-id="35261-149">Описание</span><span class="sxs-lookup"><span data-stu-id="35261-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35261-150">Таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="35261-150">taskFolders</span></span>|<span data-ttu-id="35261-151">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="35261-151">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="35261-152">Коллекция папок задач в группе задач.</span><span class="sxs-lookup"><span data-stu-id="35261-152">The collection of task folders in the task group.</span></span> <span data-ttu-id="35261-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35261-153">Read-only.</span></span> <span data-ttu-id="35261-154">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="35261-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35261-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35261-155">JSON representation</span></span>
<span data-ttu-id="35261-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35261-156">Here is a JSON representation of the resource.</span></span>

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
