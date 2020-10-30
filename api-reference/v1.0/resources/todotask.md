---
title: Тип ресурса Тодотаск
description: Ресурс Тодотаск отслеживает рабочий элемент.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f578df4189d70e6fc9c82d4cd5c038e3cd2de7a2
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797314"
---
# <a name="todotask-resource-type"></a><span data-ttu-id="aa919-103">Тип ресурса Тодотаск</span><span class="sxs-lookup"><span data-stu-id="aa919-103">todoTask resource type</span></span>

<span data-ttu-id="aa919-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa919-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aa919-105">**Тодотаск** представляет задачу, например фрагмент рабочего или личного элемента, которые можно отслеживать и заполнять.</span><span class="sxs-lookup"><span data-stu-id="aa919-105">A **todoTask** represents a task, such as a piece of work or personal item, that can be tracked and completed.</span></span> 

<span data-ttu-id="aa919-106">**Тодотаск** всегда находится в [тодотасклист](todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="aa919-106">A **todoTask** is always contained in a [todoTaskList](todotasklist.md).</span></span> <span data-ttu-id="aa919-107">Он включает связь с коллекцией объектов [линкедресаурце](./linkedResource.md) , отслеживая один или несколько источников задачи.</span><span class="sxs-lookup"><span data-stu-id="aa919-107">It includes a relationship to a collection of [linkedResource](./linkedResource.md) objects, tracking one or more sources of the task.</span></span>

<span data-ttu-id="aa919-108">Этот ресурс поддерживает следующие компоненты:</span><span class="sxs-lookup"><span data-stu-id="aa919-108">This resource supports the following:</span></span>
* <span data-ttu-id="aa919-109">Добавление данных в качестве настраиваемых свойств в [открытые расширения](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="aa919-109">Adding your data as custom properties in [open extensions](/graph/extensibility-overview).</span></span>
* <span data-ttu-id="aa919-110">Использование [запроса изменений](/graph/delta-query-overview) для отслеживания добавочных дополнений, удалений и обновлений.</span><span class="sxs-lookup"><span data-stu-id="aa919-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>

## <a name="methods"></a><span data-ttu-id="aa919-111">Методы</span><span class="sxs-lookup"><span data-stu-id="aa919-111">Methods</span></span>
|<span data-ttu-id="aa919-112">Метод</span><span class="sxs-lookup"><span data-stu-id="aa919-112">Method</span></span>|<span data-ttu-id="aa919-113">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="aa919-113">Return type</span></span>|<span data-ttu-id="aa919-114">Описание</span><span class="sxs-lookup"><span data-stu-id="aa919-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aa919-115">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="aa919-115">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="aa919-116">Коллекция [todoTask](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="aa919-116">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="aa919-117">Получение всех ресурсов [todoTask](todotask.md) в указанном списке.</span><span class="sxs-lookup"><span data-stu-id="aa919-117">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="aa919-118">Создание задачи</span><span class="sxs-lookup"><span data-stu-id="aa919-118">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="aa919-119">todoTask</span><span class="sxs-lookup"><span data-stu-id="aa919-119">todoTask</span></span>](todotask.md)| <span data-ttu-id="aa919-120">Создание объекта [тодотаск](todotask.md) в указанном списке задач</span><span class="sxs-lookup"><span data-stu-id="aa919-120">Create a [todoTask](todotask.md) in the specified task list</span></span>|
|[<span data-ttu-id="aa919-121">Вывод задачи</span><span class="sxs-lookup"><span data-stu-id="aa919-121">Get task</span></span>](../api/todotask-get.md)|[<span data-ttu-id="aa919-122">todoTask</span><span class="sxs-lookup"><span data-stu-id="aa919-122">todoTask</span></span>](../resources/todotask.md)|<span data-ttu-id="aa919-123">Чтение свойств и связей объекта [тодотаск](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="aa919-123">Read the properties and relationships of a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="aa919-124">Обновление задачи</span><span class="sxs-lookup"><span data-stu-id="aa919-124">Update task</span></span>](../api/todotask-update.md)|[<span data-ttu-id="aa919-125">todoTask</span><span class="sxs-lookup"><span data-stu-id="aa919-125">todoTask</span></span>](../resources/todotask.md)|<span data-ttu-id="aa919-126">Обновление свойств объекта [тодотаск](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="aa919-126">Update the properties of a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="aa919-127">Удаление задачи</span><span class="sxs-lookup"><span data-stu-id="aa919-127">Delete task</span></span>](../api/todotask-delete.md)|<span data-ttu-id="aa919-128">Нет</span><span class="sxs-lookup"><span data-stu-id="aa919-128">None</span></span>|<span data-ttu-id="aa919-129">Удаляет объект [тодотаск](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="aa919-129">Deletes a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="aa919-130">Список Линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="aa919-130">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="aa919-131">Коллекция [линкедресаурце](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="aa919-131">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="aa919-132">Получение Линкедресаурцес из свойства навигации Линкедресаурцес.</span><span class="sxs-lookup"><span data-stu-id="aa919-132">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="aa919-133">Создание Линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="aa919-133">Create linkedResources</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="aa919-134">линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="aa919-134">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="aa919-135">Создание нового объекта Линкедресаурцес.</span><span class="sxs-lookup"><span data-stu-id="aa919-135">Create a new linkedResources object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa919-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa919-136">Properties</span></span>
|<span data-ttu-id="aa919-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa919-137">Property</span></span>|<span data-ttu-id="aa919-138">Тип</span><span class="sxs-lookup"><span data-stu-id="aa919-138">Type</span></span>|<span data-ttu-id="aa919-139">Описание</span><span class="sxs-lookup"><span data-stu-id="aa919-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa919-140">body</span><span class="sxs-lookup"><span data-stu-id="aa919-140">body</span></span>|[<span data-ttu-id="aa919-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="aa919-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="aa919-142">Текст задачи, который обычно содержит сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="aa919-142">The task body that typically contains information about the task.</span></span>|
|<span data-ttu-id="aa919-143">бодиластмодифиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="aa919-143">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="aa919-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa919-144">DateTimeOffset</span></span>|<span data-ttu-id="aa919-145">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="aa919-145">The date and time when the task was last modified.</span></span> <span data-ttu-id="aa919-146">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="aa919-146">By default, it is in UTC.</span></span> <span data-ttu-id="aa919-147">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="aa919-147">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="aa919-148">Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="aa919-148">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aa919-149">Например, полночь UTC 1 января 2020: ' 2020 – 01 – 01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="aa919-149">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="aa919-150">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa919-150">completedDateTime</span></span>|[<span data-ttu-id="aa919-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="aa919-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="aa919-152">Дата в указанном часовом поясе, когда задача была завершена.</span><span class="sxs-lookup"><span data-stu-id="aa919-152">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="aa919-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa919-153">createdDateTime</span></span>|<span data-ttu-id="aa919-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa919-154">DateTimeOffset</span></span>|<span data-ttu-id="aa919-155">Дата и время создания задачи.</span><span class="sxs-lookup"><span data-stu-id="aa919-155">The date and time when the task was created.</span></span> <span data-ttu-id="aa919-156">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="aa919-156">By default, it is in UTC.</span></span> <span data-ttu-id="aa919-157">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="aa919-157">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="aa919-158">Значение свойства представлено в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="aa919-158">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="aa919-159">Например, полночь UTC 1 января 2020: ' 2020 – 01 – 01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="aa919-159">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="aa919-160">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="aa919-160">dueDateTime</span></span>|[<span data-ttu-id="aa919-161">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="aa919-161">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="aa919-162">Дата в указанном часовом поясе, когда задача должна быть завершена.</span><span class="sxs-lookup"><span data-stu-id="aa919-162">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="aa919-163">id</span><span class="sxs-lookup"><span data-stu-id="aa919-163">id</span></span>|<span data-ttu-id="aa919-164">String</span><span class="sxs-lookup"><span data-stu-id="aa919-164">String</span></span>|<span data-ttu-id="aa919-165">Уникальный идентификатор задачи.</span><span class="sxs-lookup"><span data-stu-id="aa919-165">Unique identifier for the task.</span></span> <span data-ttu-id="aa919-166">По умолчанию это значение изменяется при перемещении элемента из одного списка в другой.</span><span class="sxs-lookup"><span data-stu-id="aa919-166">By default, this value changes when the item is moved from one list to another.</span></span>|
|<span data-ttu-id="aa919-167">importance</span><span class="sxs-lookup"><span data-stu-id="aa919-167">importance</span></span>|<span data-ttu-id="aa919-168">importance</span><span class="sxs-lookup"><span data-stu-id="aa919-168">importance</span></span>|<span data-ttu-id="aa919-169">Важность задачи.</span><span class="sxs-lookup"><span data-stu-id="aa919-169">The importance of the task.</span></span> <span data-ttu-id="aa919-170">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="aa919-170">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="aa919-171">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="aa919-171">isReminderOn</span></span>|<span data-ttu-id="aa919-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa919-172">Boolean</span></span>|<span data-ttu-id="aa919-173">Присвоено значение true, если установлено напоминание пользователю о задаче.</span><span class="sxs-lookup"><span data-stu-id="aa919-173">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="aa919-174">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa919-174">lastModifiedDateTime</span></span>|<span data-ttu-id="aa919-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa919-175">DateTimeOffset</span></span>|<span data-ttu-id="aa919-176">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="aa919-176">The date and time when the task was last modified.</span></span> <span data-ttu-id="aa919-177">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="aa919-177">By default, it is in UTC.</span></span> <span data-ttu-id="aa919-178">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="aa919-178">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="aa919-179">Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="aa919-179">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aa919-180">Например, полночь UTC 1 января 2020: ' 2020 – 01 – 01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="aa919-180">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="aa919-181">recurrence</span><span class="sxs-lookup"><span data-stu-id="aa919-181">recurrence</span></span>|[<span data-ttu-id="aa919-182">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="aa919-182">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="aa919-183">Расписание повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="aa919-183">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="aa919-184">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="aa919-184">reminderDateTime</span></span>|[<span data-ttu-id="aa919-185">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="aa919-185">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="aa919-186">Дата и время появления напоминания о задаче.</span><span class="sxs-lookup"><span data-stu-id="aa919-186">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="aa919-187">status</span><span class="sxs-lookup"><span data-stu-id="aa919-187">status</span></span>|<span data-ttu-id="aa919-188">таскстатус</span><span class="sxs-lookup"><span data-stu-id="aa919-188">taskStatus</span></span>|<span data-ttu-id="aa919-189">Указывает состояние или ход выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="aa919-189">Indicates the state or progress of the task.</span></span> <span data-ttu-id="aa919-190">Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="aa919-190">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="aa919-191">title</span><span class="sxs-lookup"><span data-stu-id="aa919-191">title</span></span>|<span data-ttu-id="aa919-192">String</span><span class="sxs-lookup"><span data-stu-id="aa919-192">String</span></span>|<span data-ttu-id="aa919-193">Краткое описание задачи.</span><span class="sxs-lookup"><span data-stu-id="aa919-193">A brief description of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa919-194">Связи</span><span class="sxs-lookup"><span data-stu-id="aa919-194">Relationships</span></span>
|<span data-ttu-id="aa919-195">Связь</span><span class="sxs-lookup"><span data-stu-id="aa919-195">Relationship</span></span>|<span data-ttu-id="aa919-196">Тип</span><span class="sxs-lookup"><span data-stu-id="aa919-196">Type</span></span>|<span data-ttu-id="aa919-197">Описание</span><span class="sxs-lookup"><span data-stu-id="aa919-197">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa919-198">extensions</span><span class="sxs-lookup"><span data-stu-id="aa919-198">extensions</span></span>|<span data-ttu-id="aa919-199">Коллекция объектов [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="aa919-199">[extension](extension.md) collection</span></span>| <span data-ttu-id="aa919-200">Коллекция открытых расширений, определенных для задачи.</span><span class="sxs-lookup"><span data-stu-id="aa919-200">The collection of open extensions defined for the task.</span></span> <span data-ttu-id="aa919-201">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="aa919-201">Nullable.</span></span>|
|<span data-ttu-id="aa919-202">линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="aa919-202">linkedResources</span></span>|<span data-ttu-id="aa919-203">Коллекция [линкедресаурце](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="aa919-203">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="aa919-204">Коллекция ресурсов, связанных с задачей.</span><span class="sxs-lookup"><span data-stu-id="aa919-204">A collection of resources linked to the task.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="aa919-205">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa919-205">JSON representation</span></span>
<span data-ttu-id="aa919-206">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa919-206">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todoTask",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todoTask",
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "completedDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "importance": "String",
  "isReminderOn": "Boolean",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "reminderDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "status": "String",
  "title": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "bodyLastModifiedDateTime": "String (timestamp)"
}
```



