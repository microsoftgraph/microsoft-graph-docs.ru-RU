---
title: Создание объекта todoTask
description: Создание объекта задачи в указанном todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 457a855f7746ce2ce4924f03e6a7862be4bce41f
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850054"
---
# <a name="create-todotask"></a><span data-ttu-id="bf4ba-103">Создание объекта todoTask</span><span class="sxs-lookup"><span data-stu-id="bf4ba-103">Create todoTask</span></span>
<span data-ttu-id="bf4ba-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="bf4ba-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="bf4ba-105">Создание объекта задачи в указанном [todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="bf4ba-105">Create a new task object in a specified [todoTaskList](../resources/todotasklist.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bf4ba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf4ba-106">Permissions</span></span>
<span data-ttu-id="bf4ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf4ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf4ba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf4ba-109">Permission type</span></span>|<span data-ttu-id="bf4ba-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf4ba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf4ba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf4ba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bf4ba-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf4ba-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="bf4ba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf4ba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf4ba-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf4ba-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="bf4ba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf4ba-115">Application</span></span>|<span data-ttu-id="bf4ba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf4ba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf4ba-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="bf4ba-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf4ba-118">Request headers</span></span>
|<span data-ttu-id="bf4ba-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bf4ba-119">Name</span></span>|<span data-ttu-id="bf4ba-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bf4ba-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bf4ba-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf4ba-121">Authorization</span></span>|<span data-ttu-id="bf4ba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bf4ba-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf4ba-124">Content-Type</span></span>|<span data-ttu-id="bf4ba-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf4ba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf4ba-127">Request body</span></span>
<span data-ttu-id="bf4ba-128">Представьте в тексте запроса описание объекта [todoTask в формате JSON.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="bf4ba-128">In the request body, supply a JSON representation of the [todoTask](../resources/todotask.md) object.</span></span>

<span data-ttu-id="bf4ba-129">Ниже показаны свойства, которые необходимо указывать при создании [объекта todoTask.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="bf4ba-129">The following table shows the properties that are required when you create the [todoTask](../resources/todotask.md).</span></span>

|<span data-ttu-id="bf4ba-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf4ba-130">Property</span></span>|<span data-ttu-id="bf4ba-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bf4ba-131">Type</span></span>|<span data-ttu-id="bf4ba-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bf4ba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf4ba-133">id</span><span class="sxs-lookup"><span data-stu-id="bf4ba-133">id</span></span>|<span data-ttu-id="bf4ba-134">String</span><span class="sxs-lookup"><span data-stu-id="bf4ba-134">String</span></span>|<span data-ttu-id="bf4ba-135">Уникальный идентификатор задачи.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-135">Unique identifier for the task.</span></span> <span data-ttu-id="bf4ba-136">По умолчанию это значение изменяется при перемещении элемента из одного списка в другой.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-136">By default, this value changes when the item is moved from one list to another.</span></span>|
|<span data-ttu-id="bf4ba-137">body</span><span class="sxs-lookup"><span data-stu-id="bf4ba-137">body</span></span>|[<span data-ttu-id="bf4ba-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="bf4ba-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="bf4ba-139">Текст задачи, который обычно содержит сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-139">The task body that typically contains information about the task.</span></span>|
|<span data-ttu-id="bf4ba-140">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf4ba-140">completedDateTime</span></span>|[<span data-ttu-id="bf4ba-141">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bf4ba-141">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="bf4ba-142">Дата в указанном часовом поясе, когда задача была завершена.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-142">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="bf4ba-143">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="bf4ba-143">dueDateTime</span></span>|[<span data-ttu-id="bf4ba-144">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bf4ba-144">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="bf4ba-145">Дата в указанном часовом поясе, когда задача должна быть завершена.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-145">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="bf4ba-146">importance</span><span class="sxs-lookup"><span data-stu-id="bf4ba-146">importance</span></span>|<span data-ttu-id="bf4ba-147">importance</span><span class="sxs-lookup"><span data-stu-id="bf4ba-147">importance</span></span>|<span data-ttu-id="bf4ba-148">Важность задачи.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-148">The importance of the task.</span></span> <span data-ttu-id="bf4ba-149">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-149">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="bf4ba-150">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="bf4ba-150">isReminderOn</span></span>|<span data-ttu-id="bf4ba-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf4ba-151">Boolean</span></span>|<span data-ttu-id="bf4ba-152">Присвоено значение true, если установлено напоминание пользователю о задаче.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-152">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="bf4ba-153">recurrence</span><span class="sxs-lookup"><span data-stu-id="bf4ba-153">recurrence</span></span>|[<span data-ttu-id="bf4ba-154">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="bf4ba-154">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="bf4ba-155">Расписание повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-155">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="bf4ba-156">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="bf4ba-156">reminderDateTime</span></span>|[<span data-ttu-id="bf4ba-157">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bf4ba-157">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="bf4ba-158">Дата и время появления напоминания о задаче.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-158">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="bf4ba-159">status</span><span class="sxs-lookup"><span data-stu-id="bf4ba-159">status</span></span>|<span data-ttu-id="bf4ba-160">taskStatus</span><span class="sxs-lookup"><span data-stu-id="bf4ba-160">taskStatus</span></span>|<span data-ttu-id="bf4ba-161">Указывает состояние или ход выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-161">Indicates the state or progress of the task.</span></span> <span data-ttu-id="bf4ba-162">Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-162">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="bf4ba-163">title</span><span class="sxs-lookup"><span data-stu-id="bf4ba-163">title</span></span>|<span data-ttu-id="bf4ba-164">String</span><span class="sxs-lookup"><span data-stu-id="bf4ba-164">String</span></span>|<span data-ttu-id="bf4ba-165">Краткое описание задачи.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-165">A brief description of the task.</span></span>|
|<span data-ttu-id="bf4ba-166">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf4ba-166">createdDateTime</span></span>|<span data-ttu-id="bf4ba-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf4ba-167">DateTimeOffset</span></span>|<span data-ttu-id="bf4ba-168">Дата и время создания задачи.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-168">The date and time when the task was created.</span></span> <span data-ttu-id="bf4ba-169">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-169">By default, it is in UTC.</span></span> <span data-ttu-id="bf4ba-170">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-170">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="bf4ba-171">Значение свойства представлено в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-171">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="bf4ba-172">Например, значение полуночи 1 января 2020 г. в формате UTC выглядит так: "2020-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="bf4ba-172">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="bf4ba-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf4ba-173">lastModifiedDateTime</span></span>|<span data-ttu-id="bf4ba-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf4ba-174">DateTimeOffset</span></span>|<span data-ttu-id="bf4ba-175">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-175">The date and time when the task was last modified.</span></span> <span data-ttu-id="bf4ba-176">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-176">By default, it is in UTC.</span></span> <span data-ttu-id="bf4ba-177">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-177">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="bf4ba-178">Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bf4ba-178">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bf4ba-179">Например, значение полуночи 1 января 2020 г. в формате UTC выглядит так: "2020-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="bf4ba-179">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="bf4ba-180">bodyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf4ba-180">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="bf4ba-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf4ba-181">DateTimeOffset</span></span>|<span data-ttu-id="bf4ba-182">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-182">The date and time when the task was last modified.</span></span> <span data-ttu-id="bf4ba-183">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-183">By default, it is in UTC.</span></span> <span data-ttu-id="bf4ba-184">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-184">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="bf4ba-185">Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bf4ba-185">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bf4ba-186">Например, значение полуночи 1 января 2020 г. в формате UTC выглядит так: "2020-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="bf4ba-186">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|



## <a name="response"></a><span data-ttu-id="bf4ba-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf4ba-187">Response</span></span>

<span data-ttu-id="bf4ba-188">При успешном выполнении этот метод возвращает код `201 Created` ответа [и объект todoTask](../resources/todotask.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-188">If successful, this method returns a `201 Created` response code and a [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bf4ba-189">Примеры</span><span class="sxs-lookup"><span data-stu-id="bf4ba-189">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bf4ba-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf4ba-190">Request</span></span>
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
  "linkedResources": [{
            "webUrl": "http://microsoft.com",
            "applicationName": "Microsoft",
            "displayName": "Microsoft"
        }]
}
```


### <a name="response"></a><span data-ttu-id="bf4ba-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf4ba-191">Response</span></span>
<span data-ttu-id="bf4ba-192">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bf4ba-192">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.etag": "W/\"xzyPKP0BiUGgld+lMKXwbQAAnBoTIw==\"",
    "importance": "low",
    "isReminderOn": false,
    "status": "notStarted",
    "title": "A new task",
    "createdDateTime": "2020-08-18T09:03:05.8339192Z",
    "lastModifiedDateTime": "2020-08-18T09:03:06.0827766Z",
    "id": "AlMKXwbQAAAJws6wcAAAA=",
    "body": {
        "content": "",
        "contentType": "text"
    },
    "linkedResources": [{
      "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
            "webUrl": "http://microsoft.com",
            "applicationName": "Microsoft",
            "displayName": "Microsoft"
        }]
}
```

