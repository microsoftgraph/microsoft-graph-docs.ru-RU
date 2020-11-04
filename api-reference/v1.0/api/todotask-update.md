---
title: Обновление Тодотаск
description: Обновление свойств объекта Тодотаск.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d64a024c3da7eeb944e21da53c99618918459b52
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905387"
---
# <a name="update-todotask"></a><span data-ttu-id="3d20b-103">Обновление Тодотаск</span><span class="sxs-lookup"><span data-stu-id="3d20b-103">Update todoTask</span></span>
<span data-ttu-id="3d20b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d20b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3d20b-105">Обновление свойств объекта [тодотаск](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="3d20b-105">Update the properties of a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d20b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d20b-106">Permissions</span></span>
<span data-ttu-id="3d20b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d20b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d20b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d20b-109">Permission type</span></span>|<span data-ttu-id="3d20b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d20b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d20b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d20b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3d20b-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d20b-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="3d20b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d20b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d20b-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d20b-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="3d20b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d20b-115">Application</span></span>|<span data-ttu-id="3d20b-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3d20b-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d20b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d20b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}/tasks/{taskId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="3d20b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d20b-118">Request headers</span></span>
|<span data-ttu-id="3d20b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3d20b-119">Name</span></span>|<span data-ttu-id="3d20b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3d20b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3d20b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d20b-121">Authorization</span></span>|<span data-ttu-id="3d20b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d20b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3d20b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3d20b-124">Content-Type</span></span>|<span data-ttu-id="3d20b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d20b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d20b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d20b-127">Request body</span></span>
<span data-ttu-id="3d20b-128">В тексте запроса добавьте представление объекта [тодотаск](../resources/todotask.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d20b-128">In the request body, supply a JSON representation of the [todoTask](../resources/todotask.md) object.</span></span>

<span data-ttu-id="3d20b-129">В следующей таблице приведены свойства, необходимые при создании [тодотаск](../resources/todotask.md).</span><span class="sxs-lookup"><span data-stu-id="3d20b-129">The following table shows the properties that are required when you create the [todoTask](../resources/todotask.md).</span></span>

|<span data-ttu-id="3d20b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d20b-130">Property</span></span>|<span data-ttu-id="3d20b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3d20b-131">Type</span></span>|<span data-ttu-id="3d20b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3d20b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d20b-133">id</span><span class="sxs-lookup"><span data-stu-id="3d20b-133">id</span></span>|<span data-ttu-id="3d20b-134">String</span><span class="sxs-lookup"><span data-stu-id="3d20b-134">String</span></span>|<span data-ttu-id="3d20b-135">Уникальный идентификатор задачи.</span><span class="sxs-lookup"><span data-stu-id="3d20b-135">The unique identifier of the task.</span></span> <span data-ttu-id="3d20b-136">Наследуется от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="3d20b-136">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="3d20b-137">body</span><span class="sxs-lookup"><span data-stu-id="3d20b-137">body</span></span>|[<span data-ttu-id="3d20b-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="3d20b-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="3d20b-139">Текст задачи, который обычно содержит сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="3d20b-139">The task body that typically contains information about the task.</span></span> <span data-ttu-id="3d20b-140">Обратите внимание, что поддерживается только тип HTML.</span><span class="sxs-lookup"><span data-stu-id="3d20b-140">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="3d20b-141">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d20b-141">completedDateTime</span></span>|[<span data-ttu-id="3d20b-142">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3d20b-142">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="3d20b-143">Дата в указанном часовом поясе, когда задача была завершена.</span><span class="sxs-lookup"><span data-stu-id="3d20b-143">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="3d20b-144">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="3d20b-144">dueDateTime</span></span>|[<span data-ttu-id="3d20b-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3d20b-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="3d20b-146">Дата в указанном часовом поясе, когда задача должна быть завершена.</span><span class="sxs-lookup"><span data-stu-id="3d20b-146">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="3d20b-147">importance</span><span class="sxs-lookup"><span data-stu-id="3d20b-147">importance</span></span>|<span data-ttu-id="3d20b-148">importance</span><span class="sxs-lookup"><span data-stu-id="3d20b-148">importance</span></span>|<span data-ttu-id="3d20b-149">Важность события.</span><span class="sxs-lookup"><span data-stu-id="3d20b-149">The importance of the event.</span></span> <span data-ttu-id="3d20b-150">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="3d20b-150">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="3d20b-151">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="3d20b-151">isReminderOn</span></span>|<span data-ttu-id="3d20b-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d20b-152">Boolean</span></span>|<span data-ttu-id="3d20b-153">Присвоено значение true, если установлено напоминание пользователю о задаче.</span><span class="sxs-lookup"><span data-stu-id="3d20b-153">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="3d20b-154">recurrence</span><span class="sxs-lookup"><span data-stu-id="3d20b-154">recurrence</span></span>|[<span data-ttu-id="3d20b-155">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="3d20b-155">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="3d20b-156">Расписание повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="3d20b-156">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="3d20b-157">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="3d20b-157">reminderDateTime</span></span>|[<span data-ttu-id="3d20b-158">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3d20b-158">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="3d20b-159">Дата и время появления напоминания о задаче.</span><span class="sxs-lookup"><span data-stu-id="3d20b-159">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="3d20b-160">status</span><span class="sxs-lookup"><span data-stu-id="3d20b-160">status</span></span>|<span data-ttu-id="3d20b-161">таскстатус</span><span class="sxs-lookup"><span data-stu-id="3d20b-161">taskStatus</span></span>|<span data-ttu-id="3d20b-162">Указывает состояние или ход выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="3d20b-162">Indicates state or progress of the task.</span></span> <span data-ttu-id="3d20b-163">Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="3d20b-163">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="3d20b-164">title</span><span class="sxs-lookup"><span data-stu-id="3d20b-164">title</span></span>|<span data-ttu-id="3d20b-165">String</span><span class="sxs-lookup"><span data-stu-id="3d20b-165">String</span></span>|<span data-ttu-id="3d20b-166">Краткое описание задачи.</span><span class="sxs-lookup"><span data-stu-id="3d20b-166">A brief description of the task.</span></span>|
|<span data-ttu-id="3d20b-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d20b-167">createdDateTime</span></span>|<span data-ttu-id="3d20b-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d20b-168">DateTimeOffset</span></span>|<span data-ttu-id="3d20b-169">Дата и время создания задачи.</span><span class="sxs-lookup"><span data-stu-id="3d20b-169">The date and time when the task was created.</span></span> <span data-ttu-id="3d20b-170">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="3d20b-170">By default, it is in UTC.</span></span> <span data-ttu-id="3d20b-171">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="3d20b-171">You can provide a custom time zone in the request header.</span></span>|
|<span data-ttu-id="3d20b-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d20b-172">lastModifiedDateTime</span></span>|<span data-ttu-id="3d20b-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d20b-173">DateTimeOffset</span></span>|<span data-ttu-id="3d20b-174">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="3d20b-174">The date and time when the task was last modified.</span></span> <span data-ttu-id="3d20b-175">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="3d20b-175">By default, it is in UTC.</span></span> <span data-ttu-id="3d20b-176">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="3d20b-176">You can provide a custom time zone in the request header.</span></span>|
|<span data-ttu-id="3d20b-177">бодиластмодифиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="3d20b-177">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="3d20b-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d20b-178">DateTimeOffset</span></span>|<span data-ttu-id="3d20b-179">Дата и время последнего изменения текста задачи.</span><span class="sxs-lookup"><span data-stu-id="3d20b-179">The date and time when the task body was last modified.</span></span> <span data-ttu-id="3d20b-180">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="3d20b-180">By default, it is in UTC.</span></span> <span data-ttu-id="3d20b-181">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="3d20b-181">You can provide a custom time zone in the request header.</span></span>|



## <a name="response"></a><span data-ttu-id="3d20b-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d20b-182">Response</span></span>

<span data-ttu-id="3d20b-183">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [тодотаск](../resources/todotask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3d20b-183">If successful, this method returns a `200 OK` response code and an updated [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3d20b-184">Примеры</span><span class="sxs-lookup"><span data-stu-id="3d20b-184">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3d20b-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d20b-185">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3d20b-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d20b-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_todotask",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
Content-Type: application/json
Content-length: 608

{
   "dueDateTime":{
      "dateTime":"2020-07-25T16:00:00",
      "timeZone":"Eastern Standard Time"
   }
}
```
# <a name="c"></a>[<span data-ttu-id="3d20b-187">C#</span><span class="sxs-lookup"><span data-stu-id="3d20b-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d20b-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d20b-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d20b-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d20b-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3d20b-190">Java</span><span class="sxs-lookup"><span data-stu-id="3d20b-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-todotask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3d20b-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d20b-191">Response</span></span>
<span data-ttu-id="3d20b-192">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3d20b-192">**Note:** The response object shown here might be shortened for readability.</span></span>
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



