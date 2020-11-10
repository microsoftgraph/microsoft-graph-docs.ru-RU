---
title: Создание Тодотаск
description: Создание нового объекта Task в заданном Тодотасклист.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e42c65363f958aad92ea96a9cf913229fc4ead97
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972508"
---
# <a name="create-todotask"></a><span data-ttu-id="13d05-103">Создание Тодотаск</span><span class="sxs-lookup"><span data-stu-id="13d05-103">Create todoTask</span></span>
<span data-ttu-id="13d05-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="13d05-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="13d05-105">Создание нового объекта Task в заданном [тодотасклист](../resources/todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="13d05-105">Create a new task object in a specified [todoTaskList](../resources/todotasklist.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="13d05-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13d05-106">Permissions</span></span>
<span data-ttu-id="13d05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13d05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13d05-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13d05-109">Permission type</span></span>|<span data-ttu-id="13d05-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13d05-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13d05-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13d05-111">Delegated (work or school account)</span></span>|<span data-ttu-id="13d05-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13d05-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="13d05-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13d05-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13d05-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13d05-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="13d05-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13d05-115">Application</span></span>|<span data-ttu-id="13d05-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13d05-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13d05-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13d05-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="13d05-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13d05-118">Request headers</span></span>
|<span data-ttu-id="13d05-119">Имя</span><span class="sxs-lookup"><span data-stu-id="13d05-119">Name</span></span>|<span data-ttu-id="13d05-120">Описание</span><span class="sxs-lookup"><span data-stu-id="13d05-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="13d05-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13d05-121">Authorization</span></span>|<span data-ttu-id="13d05-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13d05-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="13d05-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="13d05-124">Content-Type</span></span>|<span data-ttu-id="13d05-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13d05-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="13d05-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13d05-127">Request body</span></span>
<span data-ttu-id="13d05-128">В тексте запроса добавьте представление объекта [тодотаск](../resources/todotask.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13d05-128">In the request body, supply a JSON representation of the [todoTask](../resources/todotask.md) object.</span></span>

<span data-ttu-id="13d05-129">В следующей таблице приведены свойства, необходимые при создании [тодотаск](../resources/todotask.md).</span><span class="sxs-lookup"><span data-stu-id="13d05-129">The following table shows the properties that are required when you create the [todoTask](../resources/todotask.md).</span></span>

|<span data-ttu-id="13d05-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="13d05-130">Property</span></span>|<span data-ttu-id="13d05-131">Тип</span><span class="sxs-lookup"><span data-stu-id="13d05-131">Type</span></span>|<span data-ttu-id="13d05-132">Описание</span><span class="sxs-lookup"><span data-stu-id="13d05-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13d05-133">id</span><span class="sxs-lookup"><span data-stu-id="13d05-133">id</span></span>|<span data-ttu-id="13d05-134">String</span><span class="sxs-lookup"><span data-stu-id="13d05-134">String</span></span>|<span data-ttu-id="13d05-135">Уникальный идентификатор задачи.</span><span class="sxs-lookup"><span data-stu-id="13d05-135">Unique identifier for the task.</span></span> <span data-ttu-id="13d05-136">По умолчанию это значение изменяется при перемещении элемента из одного списка в другой.</span><span class="sxs-lookup"><span data-stu-id="13d05-136">By default, this value changes when the item is moved from one list to another.</span></span>|
|<span data-ttu-id="13d05-137">body</span><span class="sxs-lookup"><span data-stu-id="13d05-137">body</span></span>|[<span data-ttu-id="13d05-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="13d05-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="13d05-139">Текст задачи, который обычно содержит сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="13d05-139">The task body that typically contains information about the task.</span></span>|
|<span data-ttu-id="13d05-140">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="13d05-140">completedDateTime</span></span>|[<span data-ttu-id="13d05-141">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="13d05-141">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="13d05-142">Дата в указанном часовом поясе, когда задача была завершена.</span><span class="sxs-lookup"><span data-stu-id="13d05-142">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="13d05-143">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="13d05-143">dueDateTime</span></span>|[<span data-ttu-id="13d05-144">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="13d05-144">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="13d05-145">Дата в указанном часовом поясе, когда задача должна быть завершена.</span><span class="sxs-lookup"><span data-stu-id="13d05-145">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="13d05-146">importance</span><span class="sxs-lookup"><span data-stu-id="13d05-146">importance</span></span>|<span data-ttu-id="13d05-147">importance</span><span class="sxs-lookup"><span data-stu-id="13d05-147">importance</span></span>|<span data-ttu-id="13d05-148">Важность задачи.</span><span class="sxs-lookup"><span data-stu-id="13d05-148">The importance of the task.</span></span> <span data-ttu-id="13d05-149">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="13d05-149">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="13d05-150">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="13d05-150">isReminderOn</span></span>|<span data-ttu-id="13d05-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="13d05-151">Boolean</span></span>|<span data-ttu-id="13d05-152">Присвоено значение true, если установлено напоминание пользователю о задаче.</span><span class="sxs-lookup"><span data-stu-id="13d05-152">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="13d05-153">recurrence</span><span class="sxs-lookup"><span data-stu-id="13d05-153">recurrence</span></span>|[<span data-ttu-id="13d05-154">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="13d05-154">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="13d05-155">Расписание повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="13d05-155">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="13d05-156">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="13d05-156">reminderDateTime</span></span>|[<span data-ttu-id="13d05-157">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="13d05-157">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="13d05-158">Дата и время появления напоминания о задаче.</span><span class="sxs-lookup"><span data-stu-id="13d05-158">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="13d05-159">status</span><span class="sxs-lookup"><span data-stu-id="13d05-159">status</span></span>|<span data-ttu-id="13d05-160">таскстатус</span><span class="sxs-lookup"><span data-stu-id="13d05-160">taskStatus</span></span>|<span data-ttu-id="13d05-161">Указывает состояние или ход выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="13d05-161">Indicates the state or progress of the task.</span></span> <span data-ttu-id="13d05-162">Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="13d05-162">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="13d05-163">title</span><span class="sxs-lookup"><span data-stu-id="13d05-163">title</span></span>|<span data-ttu-id="13d05-164">String</span><span class="sxs-lookup"><span data-stu-id="13d05-164">String</span></span>|<span data-ttu-id="13d05-165">Краткое описание задачи.</span><span class="sxs-lookup"><span data-stu-id="13d05-165">A brief description of the task.</span></span>|
|<span data-ttu-id="13d05-166">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13d05-166">createdDateTime</span></span>|<span data-ttu-id="13d05-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13d05-167">DateTimeOffset</span></span>|<span data-ttu-id="13d05-168">Дата и время создания задачи.</span><span class="sxs-lookup"><span data-stu-id="13d05-168">The date and time when the task was created.</span></span> <span data-ttu-id="13d05-169">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="13d05-169">By default, it is in UTC.</span></span> <span data-ttu-id="13d05-170">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="13d05-170">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="13d05-171">Значение свойства представлено в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="13d05-171">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="13d05-172">Например, полночь UTC 1 января 2020: ' 2020 – 01 – 01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="13d05-172">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="13d05-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13d05-173">lastModifiedDateTime</span></span>|<span data-ttu-id="13d05-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13d05-174">DateTimeOffset</span></span>|<span data-ttu-id="13d05-175">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="13d05-175">The date and time when the task was last modified.</span></span> <span data-ttu-id="13d05-176">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="13d05-176">By default, it is in UTC.</span></span> <span data-ttu-id="13d05-177">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="13d05-177">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="13d05-178">Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="13d05-178">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="13d05-179">Например, полночь UTC 1 января 2020: ' 2020 – 01 – 01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="13d05-179">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="13d05-180">бодиластмодифиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="13d05-180">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="13d05-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13d05-181">DateTimeOffset</span></span>|<span data-ttu-id="13d05-182">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="13d05-182">The date and time when the task was last modified.</span></span> <span data-ttu-id="13d05-183">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="13d05-183">By default, it is in UTC.</span></span> <span data-ttu-id="13d05-184">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="13d05-184">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="13d05-185">Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="13d05-185">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="13d05-186">Например, полночь UTC 1 января 2020: ' 2020 – 01 – 01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="13d05-186">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|



## <a name="response"></a><span data-ttu-id="13d05-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="13d05-187">Response</span></span>

<span data-ttu-id="13d05-188">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [тодотаск](../resources/todotask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13d05-188">If successful, this method returns a `201 Created` response code and a [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="13d05-189">Примеры</span><span class="sxs-lookup"><span data-stu-id="13d05-189">Examples</span></span>

### <a name="request"></a><span data-ttu-id="13d05-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="13d05-190">Request</span></span>
<span data-ttu-id="13d05-191">В следующем примере создается объект **тодотаск** в указанном списке задач и включается [линкедресаурце](../resources/linkedresource.md).</span><span class="sxs-lookup"><span data-stu-id="13d05-191">The following example creates a **todoTask** in the specified task list, and includes a [linkedResource](../resources/linkedresource.md).</span></span>

# <a name="http"></a>[<span data-ttu-id="13d05-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="13d05-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM"],
  "name": "create_todotask_from_tasks"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists/AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM/tasks
Content-Type: application/json
Content-length: 608

{
   "title":"A new task",
   "linkedResources":[
      {
         "webUrl":"http://microsoft.com",
         "applicationName":"Microsoft",
         "displayName":"Microsoft"
      }
   ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="13d05-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13d05-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-todotask-from-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="13d05-194">C#</span><span class="sxs-lookup"><span data-stu-id="13d05-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-todotask-from-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13d05-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13d05-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-todotask-from-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13d05-196">Java</span><span class="sxs-lookup"><span data-stu-id="13d05-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-todotask-from-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="13d05-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="13d05-197">Response</span></span>
<span data-ttu-id="13d05-198">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="13d05-198">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
   "@odata.etag":"W/\"xzyPKP0BiUGgld+lMKXwbQAAnBoTIw==\"",
   "importance":"low",
   "isReminderOn":false,
   "status":"notStarted",
   "title":"A new task",
   "createdDateTime":"2020-08-18T09:03:05.8339192Z",
   "lastModifiedDateTime":"2020-08-18T09:03:06.0827766Z",
   "id":"AlMKXwbQAAAJws6wcAAAA=",
   "body":{
      "content":"",
      "contentType":"text"
   },
   "linkedResources":[
      {
         "id":"f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
         "webUrl":"http://microsoft.com",
         "applicationName":"Microsoft",
         "displayName":"Microsoft"
      }
   ]
}
```



