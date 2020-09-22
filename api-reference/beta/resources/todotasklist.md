---
title: Тип ресурса Тодотасклист
description: Список в Майкрософт для этого содержит один или несколько ресурсов Тодотаск.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0523404e836223f8a59e191d1e7040a279433795
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073385"
---
# <a name="todotasklist-resource-type"></a><span data-ttu-id="94001-103">Тип ресурса Тодотасклист</span><span class="sxs-lookup"><span data-stu-id="94001-103">todoTaskList resource type</span></span>

<span data-ttu-id="94001-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94001-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94001-105">Список в Майкрософт для этого содержит один или несколько ресурсов [тодотаск](./todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="94001-105">A list in Microsoft To Do that contains one or more [todoTask](./todotask.md) resources.</span></span> 

<span data-ttu-id="94001-106">В этом случае есть встроенные списки задач, такие как **помеченные сообщения электронной почты** и **задачи** , которые не могут быть переименованы или удалены.</span><span class="sxs-lookup"><span data-stu-id="94001-106">In To Do, there are built-in task lists such as **Flagged emails** and **Tasks** which cannot be renamed or deleted.</span></span>  <span data-ttu-id="94001-107">Тем не менее, вы можете создавать дополнительные списки задач.</span><span class="sxs-lookup"><span data-stu-id="94001-107">You can, however, create additional task lists.</span></span>

<span data-ttu-id="94001-108">Этот ресурс поддерживает</span><span class="sxs-lookup"><span data-stu-id="94001-108">This resource supports</span></span>
* <span data-ttu-id="94001-109">Добавление данных к настраиваемым свойствам в виде [открытых расширений](/graph/extensibility-overview)</span><span class="sxs-lookup"><span data-stu-id="94001-109">Adding your data to custom properties as [open extensions](/graph/extensibility-overview)</span></span>
* <span data-ttu-id="94001-110">Использование [запроса изменений](/graph/delta-query-overview) для отслеживания добавочных дополнений, удалений и обновлений.</span><span class="sxs-lookup"><span data-stu-id="94001-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>

## <a name="methods"></a><span data-ttu-id="94001-111">Методы</span><span class="sxs-lookup"><span data-stu-id="94001-111">Methods</span></span>
|<span data-ttu-id="94001-112">Метод</span><span class="sxs-lookup"><span data-stu-id="94001-112">Method</span></span>|<span data-ttu-id="94001-113">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="94001-113">Return type</span></span>|<span data-ttu-id="94001-114">Описание</span><span class="sxs-lookup"><span data-stu-id="94001-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="94001-115">Перечисление списков</span><span class="sxs-lookup"><span data-stu-id="94001-115">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="94001-116">Коллекция [todoTaskList](todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="94001-116">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="94001-117">Получение всех [тодотасклист](todotasklist.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="94001-117">Get all the [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="94001-118">Создание Тодотасклист</span><span class="sxs-lookup"><span data-stu-id="94001-118">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="94001-119">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="94001-119">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="94001-120">Создайте [тодотасклист](todotasklist.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="94001-120">Create a [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="94001-121">Получение списка задач</span><span class="sxs-lookup"><span data-stu-id="94001-121">Get task list</span></span>](../api/todotasklist-get.md)|[<span data-ttu-id="94001-122">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="94001-122">todoTaskList</span></span>](todotasklist.md)|<span data-ttu-id="94001-123">Чтение свойств и связей указанного [тодотасклист](todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="94001-123">Read the properties and relationships of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="94001-124">Обновление списка задач</span><span class="sxs-lookup"><span data-stu-id="94001-124">Update task list</span></span>](../api/todotasklist-update.md)|[<span data-ttu-id="94001-125">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="94001-125">todoTaskList</span></span>](todotasklist.md)| <span data-ttu-id="94001-126">Обновление свойств, доступных для записи, для указанного [тодотасклист](todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="94001-126">Update the writable properties of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="94001-127">Удаление списка задач</span><span class="sxs-lookup"><span data-stu-id="94001-127">Delete task list</span></span>](../api/todotasklist-delete.md)|<span data-ttu-id="94001-128">Нет</span><span class="sxs-lookup"><span data-stu-id="94001-128">None</span></span>| <span data-ttu-id="94001-129">Удаление указанного [тодотасклист](todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="94001-129">Delete the specified [todoTaskList](todotasklist.md) .</span></span>|
|[<span data-ttu-id="94001-130">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="94001-130">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="94001-131">Коллекция [тодотаск](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="94001-131">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="94001-132">Получение всех ресурсов [тодотаск](todotask.md) в указанном списке.</span><span class="sxs-lookup"><span data-stu-id="94001-132">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="94001-133">Создание задачи</span><span class="sxs-lookup"><span data-stu-id="94001-133">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="94001-134">тодотаск</span><span class="sxs-lookup"><span data-stu-id="94001-134">todoTask</span></span>](todotask.md)| <span data-ttu-id="94001-135">Создание [тодотаск](todotask.md) в указанном списке задач.</span><span class="sxs-lookup"><span data-stu-id="94001-135">Create a [todoTask](todotask.md) in the specified task list.</span></span>|

## <a name="properties"></a><span data-ttu-id="94001-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="94001-136">Properties</span></span>
|<span data-ttu-id="94001-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="94001-137">Property</span></span>|<span data-ttu-id="94001-138">Тип</span><span class="sxs-lookup"><span data-stu-id="94001-138">Type</span></span>|<span data-ttu-id="94001-139">Описание</span><span class="sxs-lookup"><span data-stu-id="94001-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94001-140">displayName</span><span class="sxs-lookup"><span data-stu-id="94001-140">displayName</span></span>|<span data-ttu-id="94001-141">String</span><span class="sxs-lookup"><span data-stu-id="94001-141">String</span></span>|<span data-ttu-id="94001-142">Имя списка задач.</span><span class="sxs-lookup"><span data-stu-id="94001-142">The name of the task list.</span></span>|
|<span data-ttu-id="94001-143">id</span><span class="sxs-lookup"><span data-stu-id="94001-143">id</span></span>|<span data-ttu-id="94001-144">String</span><span class="sxs-lookup"><span data-stu-id="94001-144">String</span></span>| <span data-ttu-id="94001-145">Идентификатор списка задач, уникальный в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="94001-145">The identifier of the task list, unique in the user's mailbox.</span></span> <span data-ttu-id="94001-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94001-146">Read-only.</span></span> <span data-ttu-id="94001-147">Наследуется от [объекта](entity.md)</span><span class="sxs-lookup"><span data-stu-id="94001-147">Inherited from [entity](entity.md)</span></span>|
|<span data-ttu-id="94001-148">Владелец</span><span class="sxs-lookup"><span data-stu-id="94001-148">isOwner</span></span>|<span data-ttu-id="94001-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="94001-149">Boolean</span></span>| <span data-ttu-id="94001-150">Значение true, если пользователь является владельцем данного списка задач.</span><span class="sxs-lookup"><span data-stu-id="94001-150">True if the user is owner of the given task list.</span></span>|
|<span data-ttu-id="94001-151">IsShared</span><span class="sxs-lookup"><span data-stu-id="94001-151">isShared</span></span>|<span data-ttu-id="94001-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="94001-152">Boolean</span></span>| <span data-ttu-id="94001-153">True, если список задач открыт для совместного использования с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="94001-153">True if the task list is shared with other users</span></span>|
|<span data-ttu-id="94001-154">веллкновнлистнаме</span><span class="sxs-lookup"><span data-stu-id="94001-154">wellknownListName</span></span>|<span data-ttu-id="94001-155">веллкновнлистнаме</span><span class="sxs-lookup"><span data-stu-id="94001-155">wellknownListName</span></span>| <span data-ttu-id="94001-156">Свойство, указывающее известное имя списка, если заданный список представляет собой известный список.</span><span class="sxs-lookup"><span data-stu-id="94001-156">Property indicating the well-known list name if the given list is a well-known list.</span></span> <span data-ttu-id="94001-157">Возможные значения: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="94001-157">Possible values are: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94001-158">Отношения</span><span class="sxs-lookup"><span data-stu-id="94001-158">Relationships</span></span>
|<span data-ttu-id="94001-159">Связь</span><span class="sxs-lookup"><span data-stu-id="94001-159">Relationship</span></span>|<span data-ttu-id="94001-160">Тип</span><span class="sxs-lookup"><span data-stu-id="94001-160">Type</span></span>|<span data-ttu-id="94001-161">Описание</span><span class="sxs-lookup"><span data-stu-id="94001-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94001-162">extensions</span><span class="sxs-lookup"><span data-stu-id="94001-162">extensions</span></span>|<span data-ttu-id="94001-163">Коллекция [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="94001-163">[extension](extension.md) collection</span></span>| <span data-ttu-id="94001-164">Коллекция открытых расширений, определенных для списка задач.</span><span class="sxs-lookup"><span data-stu-id="94001-164">The collection of open extensions defined for the task list.</span></span> <span data-ttu-id="94001-165">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="94001-165">Nullable.</span></span>|
|<span data-ttu-id="94001-166">tasks</span><span class="sxs-lookup"><span data-stu-id="94001-166">tasks</span></span>|<span data-ttu-id="94001-167">Коллекция [тодотаск](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="94001-167">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="94001-168">Задачи в этом списке задач.</span><span class="sxs-lookup"><span data-stu-id="94001-168">The tasks in this task list.</span></span> <span data-ttu-id="94001-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94001-169">Read-only.</span></span> <span data-ttu-id="94001-170">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="94001-170">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94001-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94001-171">JSON representation</span></span>
<span data-ttu-id="94001-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94001-172">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todoTaskList",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todoTaskList",
  "id": "String (identifier)",
  "displayName": "String",
  "isOwner": "Boolean",
  "isShared": "Boolean",
  "wellknownListName": "String"
}
```



