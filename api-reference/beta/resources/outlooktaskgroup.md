---
title: Тип ресурса outlookTaskGroup
description: 'Группа папок (outlookTaskFolder), которая содержит задачи Outlook (Коллекция объектов outlookTask). '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: afd5da7663a9328a87b5df2616b0093a4208caeb
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312122"
---
# <a name="outlooktaskgroup-resource-type-deprecated"></a><span data-ttu-id="84523-103">Тип ресурса outlookTaskGroup (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="84523-103">outlookTaskGroup resource type (deprecated)</span></span>

<span data-ttu-id="84523-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84523-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="84523-105">Группа папок ([outlookTaskFolder](outlooktaskfolder.md)), которая содержит задачи Outlook (Коллекция объектов [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="84523-105">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="84523-106">В Outlook существует группа задач по умолчанию, `My Tasks` которую нельзя переименовать или удалить.</span><span class="sxs-lookup"><span data-stu-id="84523-106">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="84523-107">Тем не менее, вы можете создать дополнительные группы задач.</span><span class="sxs-lookup"><span data-stu-id="84523-107">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="84523-108">Методы</span><span class="sxs-lookup"><span data-stu-id="84523-108">Methods</span></span>

| <span data-ttu-id="84523-109">Метод</span><span class="sxs-lookup"><span data-stu-id="84523-109">Method</span></span>           | <span data-ttu-id="84523-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="84523-110">Return Type</span></span>    |<span data-ttu-id="84523-111">Описание</span><span class="sxs-lookup"><span data-stu-id="84523-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="84523-112">Получение outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="84523-112">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="84523-113">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="84523-113">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="84523-114">Получение свойств и связей указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="84523-114">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="84523-115">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="84523-115">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="84523-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="84523-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="84523-117">Создайте папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="84523-117">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="84523-118">Список Таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="84523-118">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="84523-119">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="84523-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="84523-120">Получение коллекции папок задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="84523-120">Get a collection of Outlook task folders.</span></span>|
|<span data-ttu-id="84523-121">[обновление](../api/outlooktaskgroup-update.md).</span><span class="sxs-lookup"><span data-stu-id="84523-121">[Update](../api/outlooktaskgroup-update.md)</span></span> | [<span data-ttu-id="84523-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="84523-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="84523-123">Обновление свойств, доступных для записи, для группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="84523-123">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="84523-124">Удаление</span><span class="sxs-lookup"><span data-stu-id="84523-124">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="84523-125">Нет</span><span class="sxs-lookup"><span data-stu-id="84523-125">None</span></span> |<span data-ttu-id="84523-126">Удаление указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="84523-126">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="84523-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="84523-127">Properties</span></span>
| <span data-ttu-id="84523-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="84523-128">Property</span></span>     | <span data-ttu-id="84523-129">Тип</span><span class="sxs-lookup"><span data-stu-id="84523-129">Type</span></span>   |<span data-ttu-id="84523-130">Описание</span><span class="sxs-lookup"><span data-stu-id="84523-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84523-131">changeKey</span><span class="sxs-lookup"><span data-stu-id="84523-131">changeKey</span></span>|<span data-ttu-id="84523-132">String</span><span class="sxs-lookup"><span data-stu-id="84523-132">String</span></span>|<span data-ttu-id="84523-133">Версия группы задач.</span><span class="sxs-lookup"><span data-stu-id="84523-133">The version of the task group.</span></span>|
|<span data-ttu-id="84523-134">граупкэй</span><span class="sxs-lookup"><span data-stu-id="84523-134">groupKey</span></span>|<span data-ttu-id="84523-135">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="84523-135">Edm.Guid</span></span>|<span data-ttu-id="84523-136">Уникальный идентификатор GUID для группы задач.</span><span class="sxs-lookup"><span data-stu-id="84523-136">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="84523-137">id</span><span class="sxs-lookup"><span data-stu-id="84523-137">id</span></span>|<span data-ttu-id="84523-138">String</span><span class="sxs-lookup"><span data-stu-id="84523-138">String</span></span>|<span data-ttu-id="84523-139">Уникальный строковый идентификатор группы задач.</span><span class="sxs-lookup"><span data-stu-id="84523-139">The unique string identifier of the task group.</span></span> <span data-ttu-id="84523-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84523-140">Read-only.</span></span>|
|<span data-ttu-id="84523-141">исдефаултграуп</span><span class="sxs-lookup"><span data-stu-id="84523-141">isDefaultGroup</span></span>|<span data-ttu-id="84523-142">Логический</span><span class="sxs-lookup"><span data-stu-id="84523-142">Boolean</span></span>|<span data-ttu-id="84523-143">Значение true, если группа задач является группой задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="84523-143">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="84523-144">name</span><span class="sxs-lookup"><span data-stu-id="84523-144">name</span></span>|<span data-ttu-id="84523-145">String</span><span class="sxs-lookup"><span data-stu-id="84523-145">String</span></span>|<span data-ttu-id="84523-146">Имя группы задач.</span><span class="sxs-lookup"><span data-stu-id="84523-146">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84523-147">Отношения</span><span class="sxs-lookup"><span data-stu-id="84523-147">Relationships</span></span>
| <span data-ttu-id="84523-148">Связь</span><span class="sxs-lookup"><span data-stu-id="84523-148">Relationship</span></span> | <span data-ttu-id="84523-149">Тип</span><span class="sxs-lookup"><span data-stu-id="84523-149">Type</span></span>   |<span data-ttu-id="84523-150">Описание</span><span class="sxs-lookup"><span data-stu-id="84523-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84523-151">таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="84523-151">taskFolders</span></span>|<span data-ttu-id="84523-152">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="84523-152">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="84523-153">Коллекция папок задач в группе задач.</span><span class="sxs-lookup"><span data-stu-id="84523-153">The collection of task folders in the task group.</span></span> <span data-ttu-id="84523-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84523-154">Read-only.</span></span> <span data-ttu-id="84523-155">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="84523-155">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84523-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84523-156">JSON representation</span></span>
<span data-ttu-id="84523-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84523-157">Here is a JSON representation of the resource.</span></span>

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
