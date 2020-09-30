---
title: Тип ресурса Тодотасклист
description: Список в Майкрософт для этого содержит один или несколько ресурсов Тодотаск.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: bddf0b72173b2f37b3fdd8544bc777c87bb33ee3
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314596"
---
# <a name="todotasklist-resource-type"></a><span data-ttu-id="88dd7-103">Тип ресурса Тодотасклист</span><span class="sxs-lookup"><span data-stu-id="88dd7-103">todoTaskList resource type</span></span>

<span data-ttu-id="88dd7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88dd7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88dd7-105">Список в Майкрософт для этого содержит один или несколько ресурсов [тодотаск](./todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="88dd7-105">A list in Microsoft To Do that contains one or more [todoTask](./todotask.md) resources.</span></span> 

<span data-ttu-id="88dd7-106">В этом случае есть встроенные списки задач, такие как **помеченные сообщения электронной почты** и **задачи** , которые не могут быть переименованы или удалены.</span><span class="sxs-lookup"><span data-stu-id="88dd7-106">In To Do, there are built-in task lists such as **Flagged emails** and **Tasks** which cannot be renamed or deleted.</span></span>  <span data-ttu-id="88dd7-107">Тем не менее, вы можете создавать дополнительные списки задач.</span><span class="sxs-lookup"><span data-stu-id="88dd7-107">You can, however, create additional task lists.</span></span>

<span data-ttu-id="88dd7-108">Этот ресурс поддерживает</span><span class="sxs-lookup"><span data-stu-id="88dd7-108">This resource supports</span></span>
* <span data-ttu-id="88dd7-109">Добавление данных к настраиваемым свойствам в виде [открытых расширений](/graph/extensibility-overview)</span><span class="sxs-lookup"><span data-stu-id="88dd7-109">Adding your data to custom properties as [open extensions](/graph/extensibility-overview)</span></span>
* <span data-ttu-id="88dd7-110">Использование [запроса изменений](/graph/delta-query-overview) для отслеживания добавочных дополнений, удалений и обновлений.</span><span class="sxs-lookup"><span data-stu-id="88dd7-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>

## <a name="methods"></a><span data-ttu-id="88dd7-111">Методы</span><span class="sxs-lookup"><span data-stu-id="88dd7-111">Methods</span></span>
|<span data-ttu-id="88dd7-112">Метод</span><span class="sxs-lookup"><span data-stu-id="88dd7-112">Method</span></span>|<span data-ttu-id="88dd7-113">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="88dd7-113">Return type</span></span>|<span data-ttu-id="88dd7-114">Описание</span><span class="sxs-lookup"><span data-stu-id="88dd7-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88dd7-115">Перечисление списков</span><span class="sxs-lookup"><span data-stu-id="88dd7-115">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="88dd7-116">Коллекция [todoTaskList](todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="88dd7-116">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="88dd7-117">Получение всех [тодотасклист](todotasklist.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="88dd7-117">Get all the [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="88dd7-118">Создание Тодотасклист</span><span class="sxs-lookup"><span data-stu-id="88dd7-118">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="88dd7-119">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="88dd7-119">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="88dd7-120">Создайте [тодотасклист](todotasklist.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="88dd7-120">Create a [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="88dd7-121">Получение списка задач</span><span class="sxs-lookup"><span data-stu-id="88dd7-121">Get task list</span></span>](../api/todotasklist-get.md)|[<span data-ttu-id="88dd7-122">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="88dd7-122">todoTaskList</span></span>](todotasklist.md)|<span data-ttu-id="88dd7-123">Чтение свойств и связей указанного [тодотасклист](todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="88dd7-123">Read the properties and relationships of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="88dd7-124">Обновление списка задач</span><span class="sxs-lookup"><span data-stu-id="88dd7-124">Update task list</span></span>](../api/todotasklist-update.md)|[<span data-ttu-id="88dd7-125">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="88dd7-125">todoTaskList</span></span>](todotasklist.md)| <span data-ttu-id="88dd7-126">Обновление свойств, доступных для записи, для указанного [тодотасклист](todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="88dd7-126">Update the writable properties of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="88dd7-127">Удаление списка задач</span><span class="sxs-lookup"><span data-stu-id="88dd7-127">Delete task list</span></span>](../api/todotasklist-delete.md)|<span data-ttu-id="88dd7-128">Нет</span><span class="sxs-lookup"><span data-stu-id="88dd7-128">None</span></span>| <span data-ttu-id="88dd7-129">Удаление указанного [тодотасклист](todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="88dd7-129">Delete the specified [todoTaskList](todotasklist.md) .</span></span>|
|[<span data-ttu-id="88dd7-130">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="88dd7-130">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="88dd7-131">Коллекция [тодотаск](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="88dd7-131">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="88dd7-132">Получение всех ресурсов [тодотаск](todotask.md) в указанном списке.</span><span class="sxs-lookup"><span data-stu-id="88dd7-132">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="88dd7-133">Создание задачи</span><span class="sxs-lookup"><span data-stu-id="88dd7-133">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="88dd7-134">тодотаск</span><span class="sxs-lookup"><span data-stu-id="88dd7-134">todoTask</span></span>](todotask.md)| <span data-ttu-id="88dd7-135">Создание [тодотаск](todotask.md) в указанном списке задач.</span><span class="sxs-lookup"><span data-stu-id="88dd7-135">Create a [todoTask](todotask.md) in the specified task list.</span></span>|

## <a name="properties"></a><span data-ttu-id="88dd7-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="88dd7-136">Properties</span></span>
|<span data-ttu-id="88dd7-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="88dd7-137">Property</span></span>|<span data-ttu-id="88dd7-138">Тип</span><span class="sxs-lookup"><span data-stu-id="88dd7-138">Type</span></span>|<span data-ttu-id="88dd7-139">Описание</span><span class="sxs-lookup"><span data-stu-id="88dd7-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88dd7-140">displayName</span><span class="sxs-lookup"><span data-stu-id="88dd7-140">displayName</span></span>|<span data-ttu-id="88dd7-141">String</span><span class="sxs-lookup"><span data-stu-id="88dd7-141">String</span></span>|<span data-ttu-id="88dd7-142">Имя списка задач.</span><span class="sxs-lookup"><span data-stu-id="88dd7-142">The name of the task list.</span></span>|
|<span data-ttu-id="88dd7-143">id</span><span class="sxs-lookup"><span data-stu-id="88dd7-143">id</span></span>|<span data-ttu-id="88dd7-144">String</span><span class="sxs-lookup"><span data-stu-id="88dd7-144">String</span></span>| <span data-ttu-id="88dd7-145">Идентификатор списка задач, уникальный в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="88dd7-145">The identifier of the task list, unique in the user's mailbox.</span></span> <span data-ttu-id="88dd7-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88dd7-146">Read-only.</span></span> <span data-ttu-id="88dd7-147">Наследуется от [объекта](entity.md)</span><span class="sxs-lookup"><span data-stu-id="88dd7-147">Inherited from [entity](entity.md)</span></span>|
|<span data-ttu-id="88dd7-148">Владелец</span><span class="sxs-lookup"><span data-stu-id="88dd7-148">isOwner</span></span>|<span data-ttu-id="88dd7-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="88dd7-149">Boolean</span></span>| <span data-ttu-id="88dd7-150">Значение true, если пользователь является владельцем данного списка задач.</span><span class="sxs-lookup"><span data-stu-id="88dd7-150">True if the user is owner of the given task list.</span></span>|
|<span data-ttu-id="88dd7-151">IsShared</span><span class="sxs-lookup"><span data-stu-id="88dd7-151">isShared</span></span>|<span data-ttu-id="88dd7-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="88dd7-152">Boolean</span></span>| <span data-ttu-id="88dd7-153">True, если список задач открыт для совместного использования с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="88dd7-153">True if the task list is shared with other users</span></span>|
|<span data-ttu-id="88dd7-154">веллкновнлистнаме</span><span class="sxs-lookup"><span data-stu-id="88dd7-154">wellknownListName</span></span>|<span data-ttu-id="88dd7-155">веллкновнлистнаме</span><span class="sxs-lookup"><span data-stu-id="88dd7-155">wellknownListName</span></span>| <span data-ttu-id="88dd7-156">Свойство, указывающее имя списка, если заданный список представляет собой известный список.</span><span class="sxs-lookup"><span data-stu-id="88dd7-156">Property indicating the list name if the given list is a well-known list.</span></span> <span data-ttu-id="88dd7-157">Возможные значения: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="88dd7-157">Possible values are: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span></span>|

### <a name="wellknownlistname-values"></a><span data-ttu-id="88dd7-158">значения Веллкновнлистнаме</span><span class="sxs-lookup"><span data-stu-id="88dd7-158">wellknownListName values</span></span>
|<span data-ttu-id="88dd7-159">Member</span><span class="sxs-lookup"><span data-stu-id="88dd7-159">Member</span></span>|<span data-ttu-id="88dd7-160">Описание</span><span class="sxs-lookup"><span data-stu-id="88dd7-160">Description</span></span>|
|:---|:---|
|<span data-ttu-id="88dd7-161">Нет</span><span class="sxs-lookup"><span data-stu-id="88dd7-161">none</span></span>| <span data-ttu-id="88dd7-162">Список, созданный пользователем.</span><span class="sxs-lookup"><span data-stu-id="88dd7-162">User created list.</span></span>|
|<span data-ttu-id="88dd7-163">дефаултлист</span><span class="sxs-lookup"><span data-stu-id="88dd7-163">defaultList</span></span>| <span data-ttu-id="88dd7-164">Встроенный список **задач** .</span><span class="sxs-lookup"><span data-stu-id="88dd7-164">Built-in **Tasks** list.</span></span>|
|<span data-ttu-id="88dd7-165">флагжедемаилс</span><span class="sxs-lookup"><span data-stu-id="88dd7-165">flaggedEmails</span></span>| <span data-ttu-id="88dd7-166">Встроенный список **электронной почты с пометкой** .</span><span class="sxs-lookup"><span data-stu-id="88dd7-166">Built-in **Flagged email** list.</span></span> <span data-ttu-id="88dd7-167">В этом списке представлены задачи с помеченными сообщениями электронной почты.</span><span class="sxs-lookup"><span data-stu-id="88dd7-167">Tasks from flagged emails are present in this list.</span></span>|
|<span data-ttu-id="88dd7-168">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="88dd7-168">unknownFutureValue</span></span>| <span data-ttu-id="88dd7-169">Значение Sentinel для перечисления расширяемые.</span><span class="sxs-lookup"><span data-stu-id="88dd7-169">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="88dd7-170">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="88dd7-170">Do not use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88dd7-171">Связи</span><span class="sxs-lookup"><span data-stu-id="88dd7-171">Relationships</span></span>
|<span data-ttu-id="88dd7-172">Связь</span><span class="sxs-lookup"><span data-stu-id="88dd7-172">Relationship</span></span>|<span data-ttu-id="88dd7-173">Тип</span><span class="sxs-lookup"><span data-stu-id="88dd7-173">Type</span></span>|<span data-ttu-id="88dd7-174">Описание</span><span class="sxs-lookup"><span data-stu-id="88dd7-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88dd7-175">extensions</span><span class="sxs-lookup"><span data-stu-id="88dd7-175">extensions</span></span>|<span data-ttu-id="88dd7-176">Коллекция [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="88dd7-176">[extension](extension.md) collection</span></span>| <span data-ttu-id="88dd7-177">Коллекция открытых расширений, определенных для списка задач.</span><span class="sxs-lookup"><span data-stu-id="88dd7-177">The collection of open extensions defined for the task list.</span></span> <span data-ttu-id="88dd7-178">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="88dd7-178">Nullable.</span></span>|
|<span data-ttu-id="88dd7-179">tasks</span><span class="sxs-lookup"><span data-stu-id="88dd7-179">tasks</span></span>|<span data-ttu-id="88dd7-180">Коллекция [тодотаск](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="88dd7-180">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="88dd7-181">Задачи в этом списке задач.</span><span class="sxs-lookup"><span data-stu-id="88dd7-181">The tasks in this task list.</span></span> <span data-ttu-id="88dd7-182">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88dd7-182">Read-only.</span></span> <span data-ttu-id="88dd7-183">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="88dd7-183">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88dd7-184">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88dd7-184">JSON representation</span></span>
<span data-ttu-id="88dd7-185">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88dd7-185">The following is a JSON representation of the resource.</span></span>
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



