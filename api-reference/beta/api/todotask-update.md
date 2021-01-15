---
title: Обновление todoTask
description: Обновление свойств объекта todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ffc7d5c90d2ec88638e35456ff74a2c48e3f1dc4
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873936"
---
# <a name="update-todotask"></a><span data-ttu-id="23535-103">Обновление todoTask</span><span class="sxs-lookup"><span data-stu-id="23535-103">Update todoTask</span></span>
<span data-ttu-id="23535-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="23535-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="23535-105">Обновление свойств объекта [todoTask.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="23535-105">Update the properties of a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="23535-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23535-106">Permissions</span></span>
<span data-ttu-id="23535-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23535-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23535-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23535-109">Permission type</span></span>|<span data-ttu-id="23535-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23535-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23535-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23535-111">Delegated (work or school account)</span></span>|<span data-ttu-id="23535-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23535-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="23535-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23535-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23535-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23535-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="23535-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23535-115">Application</span></span>|<span data-ttu-id="23535-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="23535-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="23535-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23535-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}/tasks/{taskId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="23535-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23535-118">Request headers</span></span>
|<span data-ttu-id="23535-119">Имя</span><span class="sxs-lookup"><span data-stu-id="23535-119">Name</span></span>|<span data-ttu-id="23535-120">Описание</span><span class="sxs-lookup"><span data-stu-id="23535-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="23535-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23535-121">Authorization</span></span>|<span data-ttu-id="23535-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23535-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="23535-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23535-124">Content-Type</span></span>|<span data-ttu-id="23535-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23535-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23535-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="23535-127">Request body</span></span>
<span data-ttu-id="23535-128">В теле запроса укажу представление объекта [todoTask](../resources/todotask.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="23535-128">In the request body, supply a JSON representation of the [todoTask](../resources/todotask.md) object.</span></span>

<span data-ttu-id="23535-129">В следующей таблице показаны свойства, необходимые при создании [объекта todoTask.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="23535-129">The following table shows the properties that are required when you create the [todoTask](../resources/todotask.md).</span></span>

|<span data-ttu-id="23535-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="23535-130">Property</span></span>|<span data-ttu-id="23535-131">Тип</span><span class="sxs-lookup"><span data-stu-id="23535-131">Type</span></span>|<span data-ttu-id="23535-132">Описание</span><span class="sxs-lookup"><span data-stu-id="23535-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23535-133">id</span><span class="sxs-lookup"><span data-stu-id="23535-133">id</span></span>|<span data-ttu-id="23535-134">String</span><span class="sxs-lookup"><span data-stu-id="23535-134">String</span></span>|<span data-ttu-id="23535-135">Уникальный идентификатор задачи.</span><span class="sxs-lookup"><span data-stu-id="23535-135">The unique identifier of the task.</span></span> <span data-ttu-id="23535-136">Наследуется [от объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="23535-136">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="23535-137">body</span><span class="sxs-lookup"><span data-stu-id="23535-137">body</span></span>|[<span data-ttu-id="23535-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="23535-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="23535-139">Текст задачи, который обычно содержит сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="23535-139">The task body that typically contains information about the task.</span></span> <span data-ttu-id="23535-140">Обратите внимание, что поддерживается только тип HTML.</span><span class="sxs-lookup"><span data-stu-id="23535-140">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="23535-141">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="23535-141">completedDateTime</span></span>|[<span data-ttu-id="23535-142">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="23535-142">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="23535-143">Дата в указанном часовом поясе, когда задача была завершена.</span><span class="sxs-lookup"><span data-stu-id="23535-143">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="23535-144">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="23535-144">dueDateTime</span></span>|[<span data-ttu-id="23535-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="23535-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="23535-146">Дата в указанном часовом поясе, когда задача должна быть завершена.</span><span class="sxs-lookup"><span data-stu-id="23535-146">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="23535-147">importance</span><span class="sxs-lookup"><span data-stu-id="23535-147">importance</span></span>|<span data-ttu-id="23535-148">importance</span><span class="sxs-lookup"><span data-stu-id="23535-148">importance</span></span>|<span data-ttu-id="23535-149">Важность события.</span><span class="sxs-lookup"><span data-stu-id="23535-149">The importance of the event.</span></span> <span data-ttu-id="23535-150">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="23535-150">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="23535-151">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="23535-151">isReminderOn</span></span>|<span data-ttu-id="23535-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="23535-152">Boolean</span></span>|<span data-ttu-id="23535-153">Присвоено значение true, если установлено напоминание пользователю о задаче.</span><span class="sxs-lookup"><span data-stu-id="23535-153">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="23535-154">recurrence</span><span class="sxs-lookup"><span data-stu-id="23535-154">recurrence</span></span>|[<span data-ttu-id="23535-155">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="23535-155">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="23535-156">Расписание повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="23535-156">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="23535-157">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="23535-157">reminderDateTime</span></span>|[<span data-ttu-id="23535-158">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="23535-158">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="23535-159">Дата и время появления напоминания о задаче.</span><span class="sxs-lookup"><span data-stu-id="23535-159">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="23535-160">status</span><span class="sxs-lookup"><span data-stu-id="23535-160">status</span></span>|<span data-ttu-id="23535-161">taskStatus</span><span class="sxs-lookup"><span data-stu-id="23535-161">taskStatus</span></span>|<span data-ttu-id="23535-162">Указывает состояние или ход выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="23535-162">Indicates state or progress of the task.</span></span> <span data-ttu-id="23535-163">Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="23535-163">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="23535-164">title</span><span class="sxs-lookup"><span data-stu-id="23535-164">title</span></span>|<span data-ttu-id="23535-165">String</span><span class="sxs-lookup"><span data-stu-id="23535-165">String</span></span>|<span data-ttu-id="23535-166">Краткое описание задачи.</span><span class="sxs-lookup"><span data-stu-id="23535-166">A brief description of the task.</span></span>|
|<span data-ttu-id="23535-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23535-167">createdDateTime</span></span>|<span data-ttu-id="23535-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23535-168">DateTimeOffset</span></span>|<span data-ttu-id="23535-169">Дата и время создания задачи.</span><span class="sxs-lookup"><span data-stu-id="23535-169">The date and time when the task was created.</span></span> <span data-ttu-id="23535-170">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="23535-170">By default, it is in UTC.</span></span> <span data-ttu-id="23535-171">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="23535-171">You can provide a custom time zone in the request header.</span></span>|
|<span data-ttu-id="23535-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23535-172">lastModifiedDateTime</span></span>|<span data-ttu-id="23535-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23535-173">DateTimeOffset</span></span>|<span data-ttu-id="23535-174">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="23535-174">The date and time when the task was last modified.</span></span> <span data-ttu-id="23535-175">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="23535-175">By default, it is in UTC.</span></span> <span data-ttu-id="23535-176">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="23535-176">You can provide a custom time zone in the request header.</span></span>|
|<span data-ttu-id="23535-177">bodyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23535-177">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="23535-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23535-178">DateTimeOffset</span></span>|<span data-ttu-id="23535-179">Дата и время последнего изменения тела задачи.</span><span class="sxs-lookup"><span data-stu-id="23535-179">The date and time when the task body was last modified.</span></span> <span data-ttu-id="23535-180">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="23535-180">By default, it is in UTC.</span></span> <span data-ttu-id="23535-181">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="23535-181">You can provide a custom time zone in the request header.</span></span>|



## <a name="response"></a><span data-ttu-id="23535-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="23535-182">Response</span></span>

<span data-ttu-id="23535-183">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [todoTask](../resources/todotask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23535-183">If successful, this method returns a `200 OK` response code and an updated [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="23535-184">Примеры</span><span class="sxs-lookup"><span data-stu-id="23535-184">Examples</span></span>

### <a name="request"></a><span data-ttu-id="23535-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="23535-185">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="23535-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="23535-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_todotask",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
Content-Type: application/json
Content-length: 608

{
   "dueDateTime":{
      "dateTime":"2020-07-25T16:00:00",
      "timeZone":"Eastern Standard Time"
   }
}
```
# <a name="javascript"></a>[<span data-ttu-id="23535-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23535-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="23535-188">C#</span><span class="sxs-lookup"><span data-stu-id="23535-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23535-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23535-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23535-190">Java</span><span class="sxs-lookup"><span data-stu-id="23535-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-todotask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="23535-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="23535-191">Response</span></span>
<span data-ttu-id="23535-192">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="23535-192">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
   "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tasks/$entity",
    "@odata.etag": "W/\"s8/ERWT3WEeFpBGD0bDgAA+TWq9g==\"",
    "importance": "low",
    "isReminderOn": false,
    "status": "notStarted",
    "title": "Shop for dinner",
    "createdDateTime": "2020-07-22T10:39:03.7937971Z",
    "lastModifiedDateTime": "2020-07-22T12:02:10.8835421Z",
    "id": "721a35e2-35e2-721a-e235-1a72e2351a72",
    "body": {
        "content": "",
        "contentType": "text"
    },
    "dueDateTime": {
        "dateTime": "2020-08-25T04:00:00.0000000",
        "timeZone": "UTC"
    }
}
   
```



