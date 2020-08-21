---
title: Тип ресурса outlookTaskGroup
description: 'Группа папок (outlookTaskFolder), содержащая задачи Outlook (коллекция объектов outlookTask). '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 112ffab7699a2c8812311ba0c21c2b0e47efff70
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849795"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="6cd26-103">Тип ресурса outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="6cd26-103">outlookTaskGroup resource type</span></span>

<span data-ttu-id="6cd26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cd26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="6cd26-105">Группа папок[(outlookTaskFolder),](outlooktaskfolder.md)которая содержит задачи Outlook (коллекция [объектов outlookTask).](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="6cd26-105">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="6cd26-106">В Outlook есть группа задач по умолчанию, `My Tasks` которую невозможно переименовать или удалить.</span><span class="sxs-lookup"><span data-stu-id="6cd26-106">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="6cd26-107">Однако можно создавать дополнительные группы задач.</span><span class="sxs-lookup"><span data-stu-id="6cd26-107">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="6cd26-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6cd26-108">Methods</span></span>

| <span data-ttu-id="6cd26-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6cd26-109">Method</span></span>           | <span data-ttu-id="6cd26-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6cd26-110">Return Type</span></span>    |<span data-ttu-id="6cd26-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6cd26-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6cd26-112">Get outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="6cd26-112">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="6cd26-113">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="6cd26-113">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="6cd26-114">Получение свойств и связей указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="6cd26-114">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="6cd26-115">Создание объекта outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="6cd26-115">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="6cd26-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="6cd26-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="6cd26-117">Создайте папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="6cd26-117">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="6cd26-118">Перечисление объектов taskFolder</span><span class="sxs-lookup"><span data-stu-id="6cd26-118">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="6cd26-119">[Коллекция outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="6cd26-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="6cd26-120">Получение коллекции папок задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="6cd26-120">Get a collection of Outlook task folders.</span></span>|
|<span data-ttu-id="6cd26-121">[обновление](../api/outlooktaskgroup-update.md).</span><span class="sxs-lookup"><span data-stu-id="6cd26-121">[Update](../api/outlooktaskgroup-update.md)</span></span> | [<span data-ttu-id="6cd26-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="6cd26-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="6cd26-123">Обновление записываемых свойств группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="6cd26-123">Update the writable properties of an Outlook task group.</span></span> |
|<span data-ttu-id="6cd26-124">[удаление](../api/outlooktaskgroup-delete.md);</span><span class="sxs-lookup"><span data-stu-id="6cd26-124">[Delete](../api/outlooktaskgroup-delete.md)</span></span> | <span data-ttu-id="6cd26-125">Нет</span><span class="sxs-lookup"><span data-stu-id="6cd26-125">None</span></span> |<span data-ttu-id="6cd26-126">Удаление указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="6cd26-126">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="6cd26-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="6cd26-127">Properties</span></span>
| <span data-ttu-id="6cd26-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cd26-128">Property</span></span>     | <span data-ttu-id="6cd26-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6cd26-129">Type</span></span>   |<span data-ttu-id="6cd26-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6cd26-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cd26-131">changeKey</span><span class="sxs-lookup"><span data-stu-id="6cd26-131">changeKey</span></span>|<span data-ttu-id="6cd26-132">String</span><span class="sxs-lookup"><span data-stu-id="6cd26-132">String</span></span>|<span data-ttu-id="6cd26-133">Версия группы задач.</span><span class="sxs-lookup"><span data-stu-id="6cd26-133">The version of the task group.</span></span>|
|<span data-ttu-id="6cd26-134">groupKey</span><span class="sxs-lookup"><span data-stu-id="6cd26-134">groupKey</span></span>|<span data-ttu-id="6cd26-135">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="6cd26-135">Edm.Guid</span></span>|<span data-ttu-id="6cd26-136">Уникальный идентификатор GUID группы задач.</span><span class="sxs-lookup"><span data-stu-id="6cd26-136">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="6cd26-137">id</span><span class="sxs-lookup"><span data-stu-id="6cd26-137">id</span></span>|<span data-ttu-id="6cd26-138">String</span><span class="sxs-lookup"><span data-stu-id="6cd26-138">String</span></span>|<span data-ttu-id="6cd26-139">Уникальный строковый идентификатор группы задач.</span><span class="sxs-lookup"><span data-stu-id="6cd26-139">The unique string identifier of the task group.</span></span> <span data-ttu-id="6cd26-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6cd26-140">Read-only.</span></span>|
|<span data-ttu-id="6cd26-141">isDefaultGroup</span><span class="sxs-lookup"><span data-stu-id="6cd26-141">isDefaultGroup</span></span>|<span data-ttu-id="6cd26-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cd26-142">Boolean</span></span>|<span data-ttu-id="6cd26-143">True, если группа задач является группой задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6cd26-143">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="6cd26-144">name</span><span class="sxs-lookup"><span data-stu-id="6cd26-144">name</span></span>|<span data-ttu-id="6cd26-145">String</span><span class="sxs-lookup"><span data-stu-id="6cd26-145">String</span></span>|<span data-ttu-id="6cd26-146">Имя группы задач.</span><span class="sxs-lookup"><span data-stu-id="6cd26-146">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6cd26-147">Связи</span><span class="sxs-lookup"><span data-stu-id="6cd26-147">Relationships</span></span>
| <span data-ttu-id="6cd26-148">Связь</span><span class="sxs-lookup"><span data-stu-id="6cd26-148">Relationship</span></span> | <span data-ttu-id="6cd26-149">Тип</span><span class="sxs-lookup"><span data-stu-id="6cd26-149">Type</span></span>   |<span data-ttu-id="6cd26-150">Описание</span><span class="sxs-lookup"><span data-stu-id="6cd26-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cd26-151">taskFolders</span><span class="sxs-lookup"><span data-stu-id="6cd26-151">taskFolders</span></span>|<span data-ttu-id="6cd26-152">[Коллекция outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="6cd26-152">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="6cd26-153">Коллекция папок задач в группе задач.</span><span class="sxs-lookup"><span data-stu-id="6cd26-153">The collection of task folders in the task group.</span></span> <span data-ttu-id="6cd26-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6cd26-154">Read-only.</span></span> <span data-ttu-id="6cd26-155">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6cd26-155">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6cd26-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6cd26-156">JSON representation</span></span>
<span data-ttu-id="6cd26-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6cd26-157">Here is a JSON representation of the resource.</span></span>

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
