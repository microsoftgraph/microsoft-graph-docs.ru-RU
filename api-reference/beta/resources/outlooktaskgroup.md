---
title: Тип ресурса outlookTaskGroup
description: 'Группа папок (outlookTaskFolder), которая содержит задачи Outlook (Коллекция объектов outlookTask). '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8018863ed7fd142b99e0008f860495a4d13d4e01
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463212"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="a4ff8-103">Тип ресурса outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="a4ff8-103">outlookTaskGroup resource type</span></span>

<span data-ttu-id="a4ff8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4ff8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4ff8-105">Группа папок ([outlookTaskFolder](outlooktaskfolder.md)), которая содержит задачи Outlook (Коллекция объектов [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="a4ff8-105">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="a4ff8-106">В Outlook существует группа `My Tasks` задач по умолчанию, которую нельзя переименовать или удалить.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-106">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="a4ff8-107">Тем не менее, вы можете создать дополнительные группы задач.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-107">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="a4ff8-108">Методы</span><span class="sxs-lookup"><span data-stu-id="a4ff8-108">Methods</span></span>

| <span data-ttu-id="a4ff8-109">Метод</span><span class="sxs-lookup"><span data-stu-id="a4ff8-109">Method</span></span>           | <span data-ttu-id="a4ff8-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a4ff8-110">Return Type</span></span>    |<span data-ttu-id="a4ff8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a4ff8-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a4ff8-112">Получение outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="a4ff8-112">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="a4ff8-113">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="a4ff8-113">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="a4ff8-114">Получение свойств и связей указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-114">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="a4ff8-115">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="a4ff8-115">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="a4ff8-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="a4ff8-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="a4ff8-117">Создайте папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-117">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="a4ff8-118">Список Таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="a4ff8-118">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="a4ff8-119">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="a4ff8-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="a4ff8-120">Получение коллекции папок задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-120">Get a collection of Outlook task folders.</span></span>|
|<span data-ttu-id="a4ff8-121">[обновление](../api/outlooktaskgroup-update.md).</span><span class="sxs-lookup"><span data-stu-id="a4ff8-121">[Update](../api/outlooktaskgroup-update.md)</span></span> | [<span data-ttu-id="a4ff8-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="a4ff8-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="a4ff8-123">Обновление свойств, доступных для записи, для группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-123">Update the writable properties of an Outlook task group.</span></span> |
|<span data-ttu-id="a4ff8-124">[удаление](../api/outlooktaskgroup-delete.md);</span><span class="sxs-lookup"><span data-stu-id="a4ff8-124">[Delete](../api/outlooktaskgroup-delete.md)</span></span> | <span data-ttu-id="a4ff8-125">Нет</span><span class="sxs-lookup"><span data-stu-id="a4ff8-125">None</span></span> |<span data-ttu-id="a4ff8-126">Удаление указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-126">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="a4ff8-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4ff8-127">Properties</span></span>
| <span data-ttu-id="a4ff8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4ff8-128">Property</span></span>     | <span data-ttu-id="a4ff8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a4ff8-129">Type</span></span>   |<span data-ttu-id="a4ff8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a4ff8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4ff8-131">changeKey</span><span class="sxs-lookup"><span data-stu-id="a4ff8-131">changeKey</span></span>|<span data-ttu-id="a4ff8-132">String</span><span class="sxs-lookup"><span data-stu-id="a4ff8-132">String</span></span>|<span data-ttu-id="a4ff8-133">Версия группы задач.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-133">The version of the task group.</span></span>|
|<span data-ttu-id="a4ff8-134">граупкэй</span><span class="sxs-lookup"><span data-stu-id="a4ff8-134">groupKey</span></span>|<span data-ttu-id="a4ff8-135">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="a4ff8-135">Edm.Guid</span></span>|<span data-ttu-id="a4ff8-136">Уникальный идентификатор GUID для группы задач.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-136">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="a4ff8-137">id</span><span class="sxs-lookup"><span data-stu-id="a4ff8-137">id</span></span>|<span data-ttu-id="a4ff8-138">String</span><span class="sxs-lookup"><span data-stu-id="a4ff8-138">String</span></span>|<span data-ttu-id="a4ff8-139">Уникальный строковый идентификатор группы задач.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-139">The unique string identifier of the task group.</span></span> <span data-ttu-id="a4ff8-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-140">Read-only.</span></span>|
|<span data-ttu-id="a4ff8-141">исдефаултграуп</span><span class="sxs-lookup"><span data-stu-id="a4ff8-141">isDefaultGroup</span></span>|<span data-ttu-id="a4ff8-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4ff8-142">Boolean</span></span>|<span data-ttu-id="a4ff8-143">Значение true, если группа задач является группой задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-143">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="a4ff8-144">name</span><span class="sxs-lookup"><span data-stu-id="a4ff8-144">name</span></span>|<span data-ttu-id="a4ff8-145">String</span><span class="sxs-lookup"><span data-stu-id="a4ff8-145">String</span></span>|<span data-ttu-id="a4ff8-146">Имя группы задач.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-146">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4ff8-147">Связи</span><span class="sxs-lookup"><span data-stu-id="a4ff8-147">Relationships</span></span>
| <span data-ttu-id="a4ff8-148">Связь</span><span class="sxs-lookup"><span data-stu-id="a4ff8-148">Relationship</span></span> | <span data-ttu-id="a4ff8-149">Тип</span><span class="sxs-lookup"><span data-stu-id="a4ff8-149">Type</span></span>   |<span data-ttu-id="a4ff8-150">Описание</span><span class="sxs-lookup"><span data-stu-id="a4ff8-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4ff8-151">таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="a4ff8-151">taskFolders</span></span>|<span data-ttu-id="a4ff8-152">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="a4ff8-152">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="a4ff8-153">Коллекция папок задач в группе задач.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-153">The collection of task folders in the task group.</span></span> <span data-ttu-id="a4ff8-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-154">Read-only.</span></span> <span data-ttu-id="a4ff8-155">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-155">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4ff8-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4ff8-156">JSON representation</span></span>
<span data-ttu-id="a4ff8-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4ff8-157">Here is a JSON representation of the resource.</span></span>

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
