---
title: Тип ресурса Тодотаск
description: Ресурс Тодотаск отслеживает рабочий элемент.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 58859f2781ecec713e547340606411302232ec06
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003495"
---
# <a name="todotask-resource-type"></a><span data-ttu-id="6d80a-103">Тип ресурса Тодотаск</span><span class="sxs-lookup"><span data-stu-id="6d80a-103">todoTask resource type</span></span>

<span data-ttu-id="6d80a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d80a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d80a-105">**Тодотаск** представляет задачу, например фрагмент рабочего или личного элемента, которые можно отслеживать и заполнять.</span><span class="sxs-lookup"><span data-stu-id="6d80a-105">A **todoTask** represents a task, such as a piece of work or personal item, that can be tracked and completed.</span></span> 

<span data-ttu-id="6d80a-106">**Тодотаск** всегда находится в [тодотасклист](todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="6d80a-106">A **todoTask** is always contained in a [todoTaskList](todotasklist.md).</span></span> <span data-ttu-id="6d80a-107">Он включает связь с коллекцией объектов [линкедресаурце](./linkedResource.md) , отслеживая один или несколько источников задачи.</span><span class="sxs-lookup"><span data-stu-id="6d80a-107">It includes a relationship to a collection of [linkedResource](./linkedResource.md) objects, tracking one or more sources of the task.</span></span>

<span data-ttu-id="6d80a-108">Этот ресурс поддерживает следующие компоненты:</span><span class="sxs-lookup"><span data-stu-id="6d80a-108">This resource supports the following:</span></span>
* <span data-ttu-id="6d80a-109">Добавление данных в качестве настраиваемых свойств в [открытые расширения](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="6d80a-109">Adding your data as custom properties in [open extensions](/graph/extensibility-overview).</span></span>
* <span data-ttu-id="6d80a-110">Использование [запроса изменений](/graph/delta-query-overview) для отслеживания добавочных дополнений, удалений и обновлений.</span><span class="sxs-lookup"><span data-stu-id="6d80a-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>

## <a name="methods"></a><span data-ttu-id="6d80a-111">Методы</span><span class="sxs-lookup"><span data-stu-id="6d80a-111">Methods</span></span>
|<span data-ttu-id="6d80a-112">Метод</span><span class="sxs-lookup"><span data-stu-id="6d80a-112">Method</span></span>|<span data-ttu-id="6d80a-113">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="6d80a-113">Return type</span></span>|<span data-ttu-id="6d80a-114">Описание</span><span class="sxs-lookup"><span data-stu-id="6d80a-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6d80a-115">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="6d80a-115">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="6d80a-116">Коллекция [тодотаск](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="6d80a-116">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="6d80a-117">Получение всех ресурсов [тодотаск](todotask.md) в указанном списке.</span><span class="sxs-lookup"><span data-stu-id="6d80a-117">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="6d80a-118">Создание задачи</span><span class="sxs-lookup"><span data-stu-id="6d80a-118">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="6d80a-119">тодотаск</span><span class="sxs-lookup"><span data-stu-id="6d80a-119">todoTask</span></span>](todotask.md)| <span data-ttu-id="6d80a-120">Создание объекта [тодотаск](todotask.md) в указанном списке задач</span><span class="sxs-lookup"><span data-stu-id="6d80a-120">Create a [todoTask](todotask.md) in the specified task list</span></span>|
|[<span data-ttu-id="6d80a-121">Вывод задачи</span><span class="sxs-lookup"><span data-stu-id="6d80a-121">Get task</span></span>](../api/todotask-get.md)|[<span data-ttu-id="6d80a-122">тодотаск</span><span class="sxs-lookup"><span data-stu-id="6d80a-122">todoTask</span></span>](../resources/todotask.md)|<span data-ttu-id="6d80a-123">Чтение свойств и связей объекта [тодотаск](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="6d80a-123">Read the properties and relationships of a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="6d80a-124">Обновление задачи</span><span class="sxs-lookup"><span data-stu-id="6d80a-124">Update task</span></span>](../api/todotask-update.md)|[<span data-ttu-id="6d80a-125">тодотаск</span><span class="sxs-lookup"><span data-stu-id="6d80a-125">todoTask</span></span>](../resources/todotask.md)|<span data-ttu-id="6d80a-126">Обновление свойств объекта [тодотаск](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="6d80a-126">Update the properties of a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="6d80a-127">Удаление задачи</span><span class="sxs-lookup"><span data-stu-id="6d80a-127">Delete task</span></span>](../api/todotask-delete.md)|<span data-ttu-id="6d80a-128">Нет</span><span class="sxs-lookup"><span data-stu-id="6d80a-128">None</span></span>|<span data-ttu-id="6d80a-129">Удаляет объект [тодотаск](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="6d80a-129">Deletes a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="6d80a-130">Список Линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="6d80a-130">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="6d80a-131">Коллекция [линкедресаурце](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="6d80a-131">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="6d80a-132">Получение Линкедресаурцес из свойства навигации Линкедресаурцес.</span><span class="sxs-lookup"><span data-stu-id="6d80a-132">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="6d80a-133">Создание Линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="6d80a-133">Create linkedResources</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="6d80a-134">линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="6d80a-134">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="6d80a-135">Создание нового объекта Линкедресаурцес.</span><span class="sxs-lookup"><span data-stu-id="6d80a-135">Create a new linkedResources object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6d80a-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d80a-136">Properties</span></span>
|<span data-ttu-id="6d80a-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d80a-137">Property</span></span>|<span data-ttu-id="6d80a-138">Тип</span><span class="sxs-lookup"><span data-stu-id="6d80a-138">Type</span></span>|<span data-ttu-id="6d80a-139">Описание</span><span class="sxs-lookup"><span data-stu-id="6d80a-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d80a-140">body</span><span class="sxs-lookup"><span data-stu-id="6d80a-140">body</span></span>|[<span data-ttu-id="6d80a-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="6d80a-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="6d80a-142">Текст задачи, который обычно содержит сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="6d80a-142">The task body that typically contains information about the task.</span></span>|
|<span data-ttu-id="6d80a-143">бодиластмодифиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="6d80a-143">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="6d80a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d80a-144">DateTimeOffset</span></span>|<span data-ttu-id="6d80a-145">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="6d80a-145">The date and time when the task was last modified.</span></span> <span data-ttu-id="6d80a-146">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="6d80a-146">By default, it is in UTC.</span></span> <span data-ttu-id="6d80a-147">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="6d80a-147">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="6d80a-148">Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6d80a-148">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d80a-149">Например, полночь UTC 1 января 2020: ' 2020 – 01 – 01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="6d80a-149">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="6d80a-150">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d80a-150">completedDateTime</span></span>|[<span data-ttu-id="6d80a-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6d80a-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="6d80a-152">Дата в указанном часовом поясе, когда задача была завершена.</span><span class="sxs-lookup"><span data-stu-id="6d80a-152">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="6d80a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d80a-153">createdDateTime</span></span>|<span data-ttu-id="6d80a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d80a-154">DateTimeOffset</span></span>|<span data-ttu-id="6d80a-155">Дата и время создания задачи.</span><span class="sxs-lookup"><span data-stu-id="6d80a-155">The date and time when the task was created.</span></span> <span data-ttu-id="6d80a-156">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="6d80a-156">By default, it is in UTC.</span></span> <span data-ttu-id="6d80a-157">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="6d80a-157">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="6d80a-158">Значение свойства представлено в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="6d80a-158">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="6d80a-159">Например, полночь UTC 1 января 2020: ' 2020 – 01 – 01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="6d80a-159">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="6d80a-160">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="6d80a-160">dueDateTime</span></span>|[<span data-ttu-id="6d80a-161">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6d80a-161">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="6d80a-162">Дата в указанном часовом поясе, когда задача должна быть завершена.</span><span class="sxs-lookup"><span data-stu-id="6d80a-162">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="6d80a-163">id</span><span class="sxs-lookup"><span data-stu-id="6d80a-163">id</span></span>|<span data-ttu-id="6d80a-164">String</span><span class="sxs-lookup"><span data-stu-id="6d80a-164">String</span></span>|<span data-ttu-id="6d80a-165">Уникальный идентификатор задачи.</span><span class="sxs-lookup"><span data-stu-id="6d80a-165">Unique identifier for the task.</span></span> <span data-ttu-id="6d80a-166">По умолчанию это значение изменяется при перемещении элемента из одного списка в другой.</span><span class="sxs-lookup"><span data-stu-id="6d80a-166">By default, this value changes when the item is moved from one list to another.</span></span>|
|<span data-ttu-id="6d80a-167">importance</span><span class="sxs-lookup"><span data-stu-id="6d80a-167">importance</span></span>|<span data-ttu-id="6d80a-168">importance</span><span class="sxs-lookup"><span data-stu-id="6d80a-168">importance</span></span>|<span data-ttu-id="6d80a-169">Важность задачи.</span><span class="sxs-lookup"><span data-stu-id="6d80a-169">The importance of the task.</span></span> <span data-ttu-id="6d80a-170">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="6d80a-170">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="6d80a-171">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="6d80a-171">isReminderOn</span></span>|<span data-ttu-id="6d80a-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d80a-172">Boolean</span></span>|<span data-ttu-id="6d80a-173">Присвоено значение true, если установлено напоминание пользователю о задаче.</span><span class="sxs-lookup"><span data-stu-id="6d80a-173">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="6d80a-174">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d80a-174">lastModifiedDateTime</span></span>|<span data-ttu-id="6d80a-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d80a-175">DateTimeOffset</span></span>|<span data-ttu-id="6d80a-176">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="6d80a-176">The date and time when the task was last modified.</span></span> <span data-ttu-id="6d80a-177">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="6d80a-177">By default, it is in UTC.</span></span> <span data-ttu-id="6d80a-178">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="6d80a-178">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="6d80a-179">Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6d80a-179">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d80a-180">Например, полночь UTC 1 января 2020: ' 2020 – 01 – 01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="6d80a-180">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="6d80a-181">recurrence</span><span class="sxs-lookup"><span data-stu-id="6d80a-181">recurrence</span></span>|[<span data-ttu-id="6d80a-182">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="6d80a-182">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="6d80a-183">Расписание повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="6d80a-183">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="6d80a-184">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="6d80a-184">reminderDateTime</span></span>|[<span data-ttu-id="6d80a-185">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6d80a-185">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="6d80a-186">Дата и время появления напоминания о задаче.</span><span class="sxs-lookup"><span data-stu-id="6d80a-186">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="6d80a-187">status</span><span class="sxs-lookup"><span data-stu-id="6d80a-187">status</span></span>|<span data-ttu-id="6d80a-188">таскстатус</span><span class="sxs-lookup"><span data-stu-id="6d80a-188">taskStatus</span></span>|<span data-ttu-id="6d80a-189">Указывает состояние или ход выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="6d80a-189">Indicates the state or progress of the task.</span></span> <span data-ttu-id="6d80a-190">Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="6d80a-190">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="6d80a-191">title</span><span class="sxs-lookup"><span data-stu-id="6d80a-191">title</span></span>|<span data-ttu-id="6d80a-192">String</span><span class="sxs-lookup"><span data-stu-id="6d80a-192">String</span></span>|<span data-ttu-id="6d80a-193">Краткое описание задачи.</span><span class="sxs-lookup"><span data-stu-id="6d80a-193">A brief description of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d80a-194">Связи</span><span class="sxs-lookup"><span data-stu-id="6d80a-194">Relationships</span></span>
|<span data-ttu-id="6d80a-195">Связь</span><span class="sxs-lookup"><span data-stu-id="6d80a-195">Relationship</span></span>|<span data-ttu-id="6d80a-196">Тип</span><span class="sxs-lookup"><span data-stu-id="6d80a-196">Type</span></span>|<span data-ttu-id="6d80a-197">Описание</span><span class="sxs-lookup"><span data-stu-id="6d80a-197">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d80a-198">extensions</span><span class="sxs-lookup"><span data-stu-id="6d80a-198">extensions</span></span>|<span data-ttu-id="6d80a-199">Коллекция [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="6d80a-199">[extension](extension.md) collection</span></span>| <span data-ttu-id="6d80a-200">Коллекция открытых расширений, определенных для задачи.</span><span class="sxs-lookup"><span data-stu-id="6d80a-200">The collection of open extensions defined for the task.</span></span> <span data-ttu-id="6d80a-201">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6d80a-201">Nullable.</span></span>|
|<span data-ttu-id="6d80a-202">линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="6d80a-202">linkedResources</span></span>|<span data-ttu-id="6d80a-203">Коллекция [линкедресаурце](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="6d80a-203">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="6d80a-204">Коллекция ресурсов, связанных с задачей.</span><span class="sxs-lookup"><span data-stu-id="6d80a-204">A collection of resources linked to the task.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6d80a-205">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d80a-205">JSON representation</span></span>
<span data-ttu-id="6d80a-206">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d80a-206">The following is a JSON representation of the resource.</span></span>
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



