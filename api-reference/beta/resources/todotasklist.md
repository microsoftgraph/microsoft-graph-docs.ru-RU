---
title: Тип ресурса todoTaskList
description: Список в Microsoft To Do, содержащий один или несколько ресурсов todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d34f90329fc6ca4d5e12ff2f2b191819b88f895b
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850045"
---
# <a name="todotasklist-resource-type"></a><span data-ttu-id="9753c-103">Тип ресурса todoTaskList</span><span class="sxs-lookup"><span data-stu-id="9753c-103">todoTaskList resource type</span></span>

<span data-ttu-id="9753c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9753c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9753c-105">Список в Microsoft To Do, содержащий один или несколько [ресурсов todoTask.](./todotask.md)</span><span class="sxs-lookup"><span data-stu-id="9753c-105">A list in Microsoft To Do that contains one or more [todoTask](./todotask.md) resources.</span></span> 

<span data-ttu-id="9753c-106">В задачах есть встроенные списки задач, такие как отмеченные **сообщения электронной** почты и **задачи,** которые нельзя переименовать или удалить.</span><span class="sxs-lookup"><span data-stu-id="9753c-106">In To Do, there are built-in task lists such as **Flagged emails** and **Tasks** which cannot be renamed or deleted.</span></span>  <span data-ttu-id="9753c-107">Однако можно создавать дополнительные списки задач.</span><span class="sxs-lookup"><span data-stu-id="9753c-107">You can, however, create additional task lists.</span></span>

<span data-ttu-id="9753c-108">Этот ресурс поддерживает</span><span class="sxs-lookup"><span data-stu-id="9753c-108">This resource supports</span></span>
* <span data-ttu-id="9753c-109">Добавление данных к настраиваемым свойствам в качестве [открытых расширений](/graph/extensibility-overview)</span><span class="sxs-lookup"><span data-stu-id="9753c-109">Adding your data to custom properties as [open extensions](/graph/extensibility-overview)</span></span>
* <span data-ttu-id="9753c-110">Использование [разностного запроса](/graph/delta-query-overview) для отслеживания добавлений, удалений и обновлений.</span><span class="sxs-lookup"><span data-stu-id="9753c-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>

## <a name="methods"></a><span data-ttu-id="9753c-111">Методы</span><span class="sxs-lookup"><span data-stu-id="9753c-111">Methods</span></span>
|<span data-ttu-id="9753c-112">Метод</span><span class="sxs-lookup"><span data-stu-id="9753c-112">Method</span></span>|<span data-ttu-id="9753c-113">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="9753c-113">Return type</span></span>|<span data-ttu-id="9753c-114">Описание</span><span class="sxs-lookup"><span data-stu-id="9753c-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9753c-115">Списки</span><span class="sxs-lookup"><span data-stu-id="9753c-115">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="9753c-116">[Коллекция todoTaskList](todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="9753c-116">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="9753c-117">Получение [всех объектов todoTaskList](todotasklist.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="9753c-117">Get all the [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="9753c-118">Создание объекта todoTaskList</span><span class="sxs-lookup"><span data-stu-id="9753c-118">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="9753c-119">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="9753c-119">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="9753c-120">Создание [списка todoTaskList](todotasklist.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="9753c-120">Create a [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="9753c-121">Вывод списка задач</span><span class="sxs-lookup"><span data-stu-id="9753c-121">Get task list</span></span>](../api/todotasklist-get.md)|[<span data-ttu-id="9753c-122">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="9753c-122">todoTaskList</span></span>](todotasklist.md)|<span data-ttu-id="9753c-123">Чтение свойств и связей указанного [объекта todoTaskList.](todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="9753c-123">Read the properties and relationships of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="9753c-124">Обновление списка задач</span><span class="sxs-lookup"><span data-stu-id="9753c-124">Update task list</span></span>](../api/todotasklist-update.md)|[<span data-ttu-id="9753c-125">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="9753c-125">todoTaskList</span></span>](todotasklist.md)| <span data-ttu-id="9753c-126">Обновление записываемых свойств [указанного объекта todoTaskList.](todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="9753c-126">Update the writable properties of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="9753c-127">Удаление списка задач</span><span class="sxs-lookup"><span data-stu-id="9753c-127">Delete task list</span></span>](../api/todotasklist-delete.md)|<span data-ttu-id="9753c-128">Нет</span><span class="sxs-lookup"><span data-stu-id="9753c-128">None</span></span>| <span data-ttu-id="9753c-129">Удаление указанного [объекта todoTaskList.](todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="9753c-129">Delete the specified [todoTaskList](todotasklist.md) .</span></span>|
|[<span data-ttu-id="9753c-130">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="9753c-130">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="9753c-131">[Коллекция todoTask](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="9753c-131">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="9753c-132">Получение всех [ресурсов todoTask](todotask.md) в указанном списке.</span><span class="sxs-lookup"><span data-stu-id="9753c-132">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="9753c-133">Создание задачи</span><span class="sxs-lookup"><span data-stu-id="9753c-133">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="9753c-134">todoTask</span><span class="sxs-lookup"><span data-stu-id="9753c-134">todoTask</span></span>](todotask.md)| <span data-ttu-id="9753c-135">Создание объекта [todoTask](todotask.md) в указанном списке задач.</span><span class="sxs-lookup"><span data-stu-id="9753c-135">Create a [todoTask](todotask.md) in the specified task list.</span></span>|

## <a name="properties"></a><span data-ttu-id="9753c-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="9753c-136">Properties</span></span>
|<span data-ttu-id="9753c-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="9753c-137">Property</span></span>|<span data-ttu-id="9753c-138">Тип</span><span class="sxs-lookup"><span data-stu-id="9753c-138">Type</span></span>|<span data-ttu-id="9753c-139">Описание</span><span class="sxs-lookup"><span data-stu-id="9753c-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9753c-140">displayName</span><span class="sxs-lookup"><span data-stu-id="9753c-140">displayName</span></span>|<span data-ttu-id="9753c-141">String</span><span class="sxs-lookup"><span data-stu-id="9753c-141">String</span></span>|<span data-ttu-id="9753c-142">Имя списка задач.</span><span class="sxs-lookup"><span data-stu-id="9753c-142">The name of the task list.</span></span>|
|<span data-ttu-id="9753c-143">id</span><span class="sxs-lookup"><span data-stu-id="9753c-143">id</span></span>|<span data-ttu-id="9753c-144">String</span><span class="sxs-lookup"><span data-stu-id="9753c-144">String</span></span>| <span data-ttu-id="9753c-145">Идентификатор списка задач, уникальный в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="9753c-145">The identifier of the task list, unique in the user's mailbox.</span></span> <span data-ttu-id="9753c-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9753c-146">Read-only.</span></span> <span data-ttu-id="9753c-147">Наследуется от [сущности](entity.md)</span><span class="sxs-lookup"><span data-stu-id="9753c-147">Inherited from [entity](entity.md)</span></span>|
|<span data-ttu-id="9753c-148">isOwner</span><span class="sxs-lookup"><span data-stu-id="9753c-148">isOwner</span></span>|<span data-ttu-id="9753c-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="9753c-149">Boolean</span></span>| <span data-ttu-id="9753c-150">Имеет значение true, если пользователь является владельцем заданного списка задач.</span><span class="sxs-lookup"><span data-stu-id="9753c-150">True if the user is owner of the given task list.</span></span>|
|<span data-ttu-id="9753c-151">IsShared</span><span class="sxs-lookup"><span data-stu-id="9753c-151">isShared</span></span>|<span data-ttu-id="9753c-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="9753c-152">Boolean</span></span>| <span data-ttu-id="9753c-153">Имеет значение True, если доступ к списку задач предоставлен другим пользователям</span><span class="sxs-lookup"><span data-stu-id="9753c-153">True if the task list is shared with other users</span></span>|
|<span data-ttu-id="9753c-154">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="9753c-154">wellknownListName</span></span>|<span data-ttu-id="9753c-155">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="9753c-155">wellknownListName</span></span>| <span data-ttu-id="9753c-156">Свойство, указывающее имя известного списка, если данный список является известным.</span><span class="sxs-lookup"><span data-stu-id="9753c-156">Property indicating the well-known list name if the given list is a well-known list.</span></span> <span data-ttu-id="9753c-157">Возможные значения: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9753c-157">Possible values are: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9753c-158">Связи</span><span class="sxs-lookup"><span data-stu-id="9753c-158">Relationships</span></span>
|<span data-ttu-id="9753c-159">Связь</span><span class="sxs-lookup"><span data-stu-id="9753c-159">Relationship</span></span>|<span data-ttu-id="9753c-160">Тип</span><span class="sxs-lookup"><span data-stu-id="9753c-160">Type</span></span>|<span data-ttu-id="9753c-161">Описание</span><span class="sxs-lookup"><span data-stu-id="9753c-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9753c-162">extensions</span><span class="sxs-lookup"><span data-stu-id="9753c-162">extensions</span></span>|<span data-ttu-id="9753c-163">Коллекция объектов [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="9753c-163">[extension](extension.md) collection</span></span>| <span data-ttu-id="9753c-164">Коллекция открытых расширений, определенных для списка задач.</span><span class="sxs-lookup"><span data-stu-id="9753c-164">The collection of open extensions defined for the task list.</span></span> <span data-ttu-id="9753c-165">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9753c-165">Nullable.</span></span>|
|<span data-ttu-id="9753c-166">tasks</span><span class="sxs-lookup"><span data-stu-id="9753c-166">tasks</span></span>|<span data-ttu-id="9753c-167">[Коллекция todoTask](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="9753c-167">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="9753c-168">Задачи, перечисленные в этом списке задач.</span><span class="sxs-lookup"><span data-stu-id="9753c-168">The tasks in this task list.</span></span> <span data-ttu-id="9753c-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9753c-169">Read-only.</span></span> <span data-ttu-id="9753c-170">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9753c-170">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9753c-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9753c-171">JSON representation</span></span>
<span data-ttu-id="9753c-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9753c-172">The following is a JSON representation of the resource.</span></span>
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

