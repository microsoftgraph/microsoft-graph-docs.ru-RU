---
title: Тип ресурса Тодотаск
description: Ресурс Тодотаск отслеживает рабочий элемент.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ffcd3da43b7ae165045b545c656035e47d291419
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597202"
---
# <a name="todotask-resource-type"></a><span data-ttu-id="bc670-103">Тип ресурса Тодотаск</span><span class="sxs-lookup"><span data-stu-id="bc670-103">todoTask resource type</span></span>

<span data-ttu-id="bc670-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc670-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc670-105">**Тодотаск** представляет задачу, например фрагмент рабочего или личного элемента, которые можно отслеживать и заполнять.</span><span class="sxs-lookup"><span data-stu-id="bc670-105">A **todoTask** represents a task, such as a piece of work or personal item, that can be tracked and completed.</span></span> 

<span data-ttu-id="bc670-106">**Тодотаск** всегда находится в [тодотасклист](todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="bc670-106">A **todoTask** is always contained in a [todoTaskList](todotasklist.md).</span></span> <span data-ttu-id="bc670-107">Он включает связь с коллекцией объектов [линкедресаурце](./linkedResource.md) , отслеживая один или несколько источников задачи.</span><span class="sxs-lookup"><span data-stu-id="bc670-107">It includes a relationship to a collection of [linkedResource](./linkedResource.md) objects, tracking one or more sources of the task.</span></span>

<span data-ttu-id="bc670-108">Этот ресурс поддерживает следующие компоненты:</span><span class="sxs-lookup"><span data-stu-id="bc670-108">This resource supports the following:</span></span>
* <span data-ttu-id="bc670-109">Добавление данных в качестве настраиваемых свойств в [открытые расширения](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="bc670-109">Adding your data as custom properties in [open extensions](/graph/extensibility-overview).</span></span>
* <span data-ttu-id="bc670-110">подписку на [уведомления об изменениях](/graph/webhooks);</span><span class="sxs-lookup"><span data-stu-id="bc670-110">Subscribing to [change notifications](/graph/webhooks).</span></span>
* <span data-ttu-id="bc670-111">Использование [запроса изменений](/graph/delta-query-overview) для отслеживания добавочных дополнений, удалений и обновлений.</span><span class="sxs-lookup"><span data-stu-id="bc670-111">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>


## <a name="methods"></a><span data-ttu-id="bc670-112">Методы</span><span class="sxs-lookup"><span data-stu-id="bc670-112">Methods</span></span>
|<span data-ttu-id="bc670-113">Метод</span><span class="sxs-lookup"><span data-stu-id="bc670-113">Method</span></span>|<span data-ttu-id="bc670-114">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="bc670-114">Return type</span></span>|<span data-ttu-id="bc670-115">Описание</span><span class="sxs-lookup"><span data-stu-id="bc670-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc670-116">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="bc670-116">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="bc670-117">Коллекция [тодотаск](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="bc670-117">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="bc670-118">Получение всех ресурсов [тодотаск](todotask.md) в указанном списке.</span><span class="sxs-lookup"><span data-stu-id="bc670-118">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="bc670-119">Создание задачи</span><span class="sxs-lookup"><span data-stu-id="bc670-119">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="bc670-120">тодотаск</span><span class="sxs-lookup"><span data-stu-id="bc670-120">todoTask</span></span>](todotask.md)| <span data-ttu-id="bc670-121">Создание объекта [тодотаск](todotask.md) в указанном списке задач</span><span class="sxs-lookup"><span data-stu-id="bc670-121">Create a [todoTask](todotask.md) in the specified task list</span></span>|
|[<span data-ttu-id="bc670-122">Вывод задачи</span><span class="sxs-lookup"><span data-stu-id="bc670-122">Get task</span></span>](../api/todotask-get.md)|[<span data-ttu-id="bc670-123">тодотаск</span><span class="sxs-lookup"><span data-stu-id="bc670-123">todoTask</span></span>](../resources/todotask.md)|<span data-ttu-id="bc670-124">Чтение свойств и связей объекта [тодотаск](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="bc670-124">Read the properties and relationships of a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="bc670-125">Обновление задачи</span><span class="sxs-lookup"><span data-stu-id="bc670-125">Update task</span></span>](../api/todotask-update.md)|[<span data-ttu-id="bc670-126">тодотаск</span><span class="sxs-lookup"><span data-stu-id="bc670-126">todoTask</span></span>](../resources/todotask.md)|<span data-ttu-id="bc670-127">Обновление свойств объекта [тодотаск](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="bc670-127">Update the properties of a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="bc670-128">Удаление задачи</span><span class="sxs-lookup"><span data-stu-id="bc670-128">Delete task</span></span>](../api/todotask-delete.md)|<span data-ttu-id="bc670-129">Нет</span><span class="sxs-lookup"><span data-stu-id="bc670-129">None</span></span>|<span data-ttu-id="bc670-130">Удаляет объект [тодотаск](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="bc670-130">Deletes a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="bc670-131">Список Линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="bc670-131">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="bc670-132">Коллекция [линкедресаурце](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="bc670-132">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="bc670-133">Получение Линкедресаурцес из свойства навигации Линкедресаурцес.</span><span class="sxs-lookup"><span data-stu-id="bc670-133">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="bc670-134">Создание Линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="bc670-134">Create linkedResources</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="bc670-135">линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="bc670-135">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="bc670-136">Создание нового объекта Линкедресаурцес.</span><span class="sxs-lookup"><span data-stu-id="bc670-136">Create a new linkedResources object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc670-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc670-137">Properties</span></span>
|<span data-ttu-id="bc670-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc670-138">Property</span></span>|<span data-ttu-id="bc670-139">Тип</span><span class="sxs-lookup"><span data-stu-id="bc670-139">Type</span></span>|<span data-ttu-id="bc670-140">Описание</span><span class="sxs-lookup"><span data-stu-id="bc670-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc670-141">body</span><span class="sxs-lookup"><span data-stu-id="bc670-141">body</span></span>|[<span data-ttu-id="bc670-142">itemBody</span><span class="sxs-lookup"><span data-stu-id="bc670-142">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="bc670-143">Текст задачи, который обычно содержит сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="bc670-143">The task body that typically contains information about the task.</span></span>|
|<span data-ttu-id="bc670-144">бодиластмодифиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="bc670-144">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="bc670-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc670-145">DateTimeOffset</span></span>|<span data-ttu-id="bc670-146">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="bc670-146">The date and time when the task was last modified.</span></span> <span data-ttu-id="bc670-147">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="bc670-147">By default, it is in UTC.</span></span> <span data-ttu-id="bc670-148">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="bc670-148">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="bc670-149">Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bc670-149">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bc670-150">Например, полночь UTC 1 января 2020: ' 2020 – 01 – 01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="bc670-150">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="bc670-151">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc670-151">completedDateTime</span></span>|[<span data-ttu-id="bc670-152">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bc670-152">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="bc670-153">Дата в указанном часовом поясе, когда задача была завершена.</span><span class="sxs-lookup"><span data-stu-id="bc670-153">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="bc670-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc670-154">createdDateTime</span></span>|<span data-ttu-id="bc670-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc670-155">DateTimeOffset</span></span>|<span data-ttu-id="bc670-156">Дата и время создания задачи.</span><span class="sxs-lookup"><span data-stu-id="bc670-156">The date and time when the task was created.</span></span> <span data-ttu-id="bc670-157">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="bc670-157">By default, it is in UTC.</span></span> <span data-ttu-id="bc670-158">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="bc670-158">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="bc670-159">Значение свойства представлено в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="bc670-159">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="bc670-160">Например, полночь UTC 1 января 2020: ' 2020 – 01 – 01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="bc670-160">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="bc670-161">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="bc670-161">dueDateTime</span></span>|[<span data-ttu-id="bc670-162">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bc670-162">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="bc670-163">Дата в указанном часовом поясе, когда задача должна быть завершена.</span><span class="sxs-lookup"><span data-stu-id="bc670-163">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="bc670-164">id</span><span class="sxs-lookup"><span data-stu-id="bc670-164">id</span></span>|<span data-ttu-id="bc670-165">String</span><span class="sxs-lookup"><span data-stu-id="bc670-165">String</span></span>|<span data-ttu-id="bc670-166">Уникальный идентификатор задачи.</span><span class="sxs-lookup"><span data-stu-id="bc670-166">Unique identifier for the task.</span></span> <span data-ttu-id="bc670-167">По умолчанию это значение изменяется при перемещении элемента из одного списка в другой.</span><span class="sxs-lookup"><span data-stu-id="bc670-167">By default, this value changes when the item is moved from one list to another.</span></span>|
|<span data-ttu-id="bc670-168">importance</span><span class="sxs-lookup"><span data-stu-id="bc670-168">importance</span></span>|<span data-ttu-id="bc670-169">importance</span><span class="sxs-lookup"><span data-stu-id="bc670-169">importance</span></span>|<span data-ttu-id="bc670-170">Важность задачи.</span><span class="sxs-lookup"><span data-stu-id="bc670-170">The importance of the task.</span></span> <span data-ttu-id="bc670-171">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="bc670-171">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="bc670-172">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="bc670-172">isReminderOn</span></span>|<span data-ttu-id="bc670-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc670-173">Boolean</span></span>|<span data-ttu-id="bc670-174">Присвоено значение true, если установлено напоминание пользователю о задаче.</span><span class="sxs-lookup"><span data-stu-id="bc670-174">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="bc670-175">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc670-175">lastModifiedDateTime</span></span>|<span data-ttu-id="bc670-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc670-176">DateTimeOffset</span></span>|<span data-ttu-id="bc670-177">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="bc670-177">The date and time when the task was last modified.</span></span> <span data-ttu-id="bc670-178">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="bc670-178">By default, it is in UTC.</span></span> <span data-ttu-id="bc670-179">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="bc670-179">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="bc670-180">Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bc670-180">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bc670-181">Например, полночь UTC 1 января 2020: ' 2020 – 01 – 01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="bc670-181">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="bc670-182">recurrence</span><span class="sxs-lookup"><span data-stu-id="bc670-182">recurrence</span></span>|[<span data-ttu-id="bc670-183">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="bc670-183">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="bc670-184">Расписание повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="bc670-184">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="bc670-185">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="bc670-185">reminderDateTime</span></span>|[<span data-ttu-id="bc670-186">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bc670-186">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="bc670-187">Дата и время появления напоминания о задаче.</span><span class="sxs-lookup"><span data-stu-id="bc670-187">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="bc670-188">status</span><span class="sxs-lookup"><span data-stu-id="bc670-188">status</span></span>|<span data-ttu-id="bc670-189">таскстатус</span><span class="sxs-lookup"><span data-stu-id="bc670-189">taskStatus</span></span>|<span data-ttu-id="bc670-190">Указывает состояние или ход выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="bc670-190">Indicates the state or progress of the task.</span></span> <span data-ttu-id="bc670-191">Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="bc670-191">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="bc670-192">title</span><span class="sxs-lookup"><span data-stu-id="bc670-192">title</span></span>|<span data-ttu-id="bc670-193">String</span><span class="sxs-lookup"><span data-stu-id="bc670-193">String</span></span>|<span data-ttu-id="bc670-194">Краткое описание задачи.</span><span class="sxs-lookup"><span data-stu-id="bc670-194">A brief description of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc670-195">Связи</span><span class="sxs-lookup"><span data-stu-id="bc670-195">Relationships</span></span>
|<span data-ttu-id="bc670-196">Связь</span><span class="sxs-lookup"><span data-stu-id="bc670-196">Relationship</span></span>|<span data-ttu-id="bc670-197">Тип</span><span class="sxs-lookup"><span data-stu-id="bc670-197">Type</span></span>|<span data-ttu-id="bc670-198">Описание</span><span class="sxs-lookup"><span data-stu-id="bc670-198">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc670-199">extensions</span><span class="sxs-lookup"><span data-stu-id="bc670-199">extensions</span></span>|<span data-ttu-id="bc670-200">Коллекция [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="bc670-200">[extension](extension.md) collection</span></span>| <span data-ttu-id="bc670-201">Коллекция открытых расширений, определенных для задачи.</span><span class="sxs-lookup"><span data-stu-id="bc670-201">The collection of open extensions defined for the task.</span></span> <span data-ttu-id="bc670-202">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bc670-202">Nullable.</span></span>|
|<span data-ttu-id="bc670-203">линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="bc670-203">linkedResources</span></span>|<span data-ttu-id="bc670-204">Коллекция [линкедресаурце](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="bc670-204">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="bc670-205">Коллекция ресурсов, связанных с задачей.</span><span class="sxs-lookup"><span data-stu-id="bc670-205">A collection of resources linked to the task.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="bc670-206">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc670-206">JSON representation</span></span>
<span data-ttu-id="bc670-207">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc670-207">The following is a JSON representation of the resource.</span></span>
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



