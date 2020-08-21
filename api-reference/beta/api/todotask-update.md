---
title: Обновление объекта todoTask
description: Обновление свойств объекта todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d692bfefb35beffbdc3fb9969836ae947c68fa0f
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850063"
---
# <a name="update-todotask"></a><span data-ttu-id="0b3d1-103">Обновление объекта todoTask</span><span class="sxs-lookup"><span data-stu-id="0b3d1-103">Update todoTask</span></span>
<span data-ttu-id="0b3d1-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="0b3d1-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="0b3d1-105">Обновление свойств объекта [todoTask.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="0b3d1-105">Update the properties of a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b3d1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b3d1-106">Permissions</span></span>
<span data-ttu-id="0b3d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b3d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b3d1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b3d1-109">Permission type</span></span>|<span data-ttu-id="0b3d1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b3d1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b3d1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b3d1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b3d1-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b3d1-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="0b3d1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b3d1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b3d1-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b3d1-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="0b3d1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b3d1-115">Application</span></span>|<span data-ttu-id="0b3d1-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0b3d1-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b3d1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b3d1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}/tasks/{taskId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="0b3d1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b3d1-118">Request headers</span></span>
|<span data-ttu-id="0b3d1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0b3d1-119">Name</span></span>|<span data-ttu-id="0b3d1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0b3d1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0b3d1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b3d1-121">Authorization</span></span>|<span data-ttu-id="0b3d1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0b3d1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b3d1-124">Content-Type</span></span>|<span data-ttu-id="0b3d1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b3d1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b3d1-127">Request body</span></span>
<span data-ttu-id="0b3d1-128">Представьте в тексте запроса описание объекта [todoTask в формате JSON.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="0b3d1-128">In the request body, supply a JSON representation of the [todoTask](../resources/todotask.md) object.</span></span>

<span data-ttu-id="0b3d1-129">Ниже показаны свойства, которые необходимо указывать при создании [объекта todoTask.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="0b3d1-129">The following table shows the properties that are required when you create the [todoTask](../resources/todotask.md).</span></span>

|<span data-ttu-id="0b3d1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b3d1-130">Property</span></span>|<span data-ttu-id="0b3d1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0b3d1-131">Type</span></span>|<span data-ttu-id="0b3d1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0b3d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b3d1-133">id</span><span class="sxs-lookup"><span data-stu-id="0b3d1-133">id</span></span>|<span data-ttu-id="0b3d1-134">String</span><span class="sxs-lookup"><span data-stu-id="0b3d1-134">String</span></span>|<span data-ttu-id="0b3d1-135">Уникальный идентификатор задачи.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-135">The unique identifier of the task.</span></span> <span data-ttu-id="0b3d1-136">Наследуется от [сущности](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="0b3d1-136">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="0b3d1-137">body</span><span class="sxs-lookup"><span data-stu-id="0b3d1-137">body</span></span>|[<span data-ttu-id="0b3d1-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="0b3d1-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="0b3d1-139">Текст задачи, который обычно содержит сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-139">The task body that typically contains information about the task.</span></span> <span data-ttu-id="0b3d1-140">Обратите внимание, что поддерживается только тип HTML.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-140">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="0b3d1-141">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b3d1-141">completedDateTime</span></span>|[<span data-ttu-id="0b3d1-142">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0b3d1-142">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="0b3d1-143">Дата в указанном часовом поясе, когда задача была завершена.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-143">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="0b3d1-144">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="0b3d1-144">dueDateTime</span></span>|[<span data-ttu-id="0b3d1-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0b3d1-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="0b3d1-146">Дата в указанном часовом поясе, когда задача должна быть завершена.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-146">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="0b3d1-147">importance</span><span class="sxs-lookup"><span data-stu-id="0b3d1-147">importance</span></span>|<span data-ttu-id="0b3d1-148">importance</span><span class="sxs-lookup"><span data-stu-id="0b3d1-148">importance</span></span>|<span data-ttu-id="0b3d1-149">Важность события.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-149">The importance of the event.</span></span> <span data-ttu-id="0b3d1-150">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-150">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="0b3d1-151">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="0b3d1-151">isReminderOn</span></span>|<span data-ttu-id="0b3d1-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b3d1-152">Boolean</span></span>|<span data-ttu-id="0b3d1-153">Присвоено значение true, если установлено напоминание пользователю о задаче.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-153">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="0b3d1-154">recurrence</span><span class="sxs-lookup"><span data-stu-id="0b3d1-154">recurrence</span></span>|[<span data-ttu-id="0b3d1-155">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="0b3d1-155">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="0b3d1-156">Расписание повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-156">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="0b3d1-157">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="0b3d1-157">reminderDateTime</span></span>|[<span data-ttu-id="0b3d1-158">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0b3d1-158">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="0b3d1-159">Дата и время появления напоминания о задаче.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-159">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="0b3d1-160">status</span><span class="sxs-lookup"><span data-stu-id="0b3d1-160">status</span></span>|<span data-ttu-id="0b3d1-161">taskStatus</span><span class="sxs-lookup"><span data-stu-id="0b3d1-161">taskStatus</span></span>|<span data-ttu-id="0b3d1-162">Указывает состояние или ход выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-162">Indicates state or progress of the task.</span></span> <span data-ttu-id="0b3d1-163">Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-163">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="0b3d1-164">title</span><span class="sxs-lookup"><span data-stu-id="0b3d1-164">title</span></span>|<span data-ttu-id="0b3d1-165">String</span><span class="sxs-lookup"><span data-stu-id="0b3d1-165">String</span></span>|<span data-ttu-id="0b3d1-166">Краткое описание задачи.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-166">A brief description of the task.</span></span>|
|<span data-ttu-id="0b3d1-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b3d1-167">createdDateTime</span></span>|<span data-ttu-id="0b3d1-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b3d1-168">DateTimeOffset</span></span>|<span data-ttu-id="0b3d1-169">Дата и время создания задачи.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-169">The date and time when the task was created.</span></span> <span data-ttu-id="0b3d1-170">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-170">By default, it is in UTC.</span></span> <span data-ttu-id="0b3d1-171">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-171">You can provide a custom time zone in the request header.</span></span>|
|<span data-ttu-id="0b3d1-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b3d1-172">lastModifiedDateTime</span></span>|<span data-ttu-id="0b3d1-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b3d1-173">DateTimeOffset</span></span>|<span data-ttu-id="0b3d1-174">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-174">The date and time when the task was last modified.</span></span> <span data-ttu-id="0b3d1-175">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-175">By default, it is in UTC.</span></span> <span data-ttu-id="0b3d1-176">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-176">You can provide a custom time zone in the request header.</span></span>|
|<span data-ttu-id="0b3d1-177">bodyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b3d1-177">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="0b3d1-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b3d1-178">DateTimeOffset</span></span>|<span data-ttu-id="0b3d1-179">Дата и время последнего изменения текста задачи.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-179">The date and time when the task body was last modified.</span></span> <span data-ttu-id="0b3d1-180">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-180">By default, it is in UTC.</span></span> <span data-ttu-id="0b3d1-181">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-181">You can provide a custom time zone in the request header.</span></span>|



## <a name="response"></a><span data-ttu-id="0b3d1-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b3d1-182">Response</span></span>

<span data-ttu-id="0b3d1-183">При успешном выполнении этот метод возвращает код `200 OK` ответа и обновленный [объект todoTask](../resources/todotask.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-183">If successful, this method returns a `200 OK` response code and an updated [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b3d1-184">Примеры</span><span class="sxs-lookup"><span data-stu-id="0b3d1-184">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0b3d1-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b3d1-185">Request</span></span>
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
    "dueDateTime":
    {
        "dateTime":"2020-07-25T16:00:00",
        "timeZone":"Eastern Standard Time"
    }
}
```


### <a name="response"></a><span data-ttu-id="0b3d1-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b3d1-186">Response</span></span>
<span data-ttu-id="0b3d1-187">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0b3d1-187">**Note:** The response object shown here might be shortened for readability.</span></span>
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

