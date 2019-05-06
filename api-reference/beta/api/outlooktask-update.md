---
title: Обновление outlooktask
description: Изменение свойств для записи в задаче Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fcd0c73e48cf98f52d0c87e3e48acb403d6558b2
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596527"
---
# <a name="update-outlooktask"></a><span data-ttu-id="bd107-103">Обновление outlooktask</span><span class="sxs-lookup"><span data-stu-id="bd107-103">Update outlooktask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd107-104">Изменение свойств для записи в задаче Outlook.</span><span class="sxs-lookup"><span data-stu-id="bd107-104">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="bd107-105">Свойство **комплетеддатетиме** может быть задано **полным** действием или явным образом с помощью операции patch.</span><span class="sxs-lookup"><span data-stu-id="bd107-105">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="bd107-106">Если вы используете патч для установки **комплетеддатетиме**, убедитесь, что вы также установили **состояние** `completed` .</span><span class="sxs-lookup"><span data-stu-id="bd107-106">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="bd107-107">По умолчанию эта операция (а также операции POST, GET и [Complete](../api/outlooktask-complete.md) ) Возвращает свойства, связанные с датами, в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="bd107-107">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="bd107-108">Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="bd107-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd107-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd107-109">Permissions</span></span>

<span data-ttu-id="bd107-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd107-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd107-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd107-112">Permission type</span></span>      | <span data-ttu-id="bd107-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd107-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd107-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd107-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bd107-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd107-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="bd107-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd107-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd107-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd107-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="bd107-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd107-118">Application</span></span> | <span data-ttu-id="bd107-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd107-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd107-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd107-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bd107-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd107-121">Request headers</span></span>

| <span data-ttu-id="bd107-122">Имя</span><span class="sxs-lookup"><span data-stu-id="bd107-122">Name</span></span>       | <span data-ttu-id="bd107-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bd107-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bd107-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd107-124">Authorization</span></span>  | <span data-ttu-id="bd107-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd107-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bd107-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="bd107-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="bd107-128">Задает часовой пояс для свойств времени в отклике в формате UTC, если заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="bd107-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="bd107-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="bd107-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd107-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd107-130">Request body</span></span>

<span data-ttu-id="bd107-p106">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="bd107-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bd107-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd107-134">Property</span></span> | <span data-ttu-id="bd107-135">Тип</span><span class="sxs-lookup"><span data-stu-id="bd107-135">Type</span></span> | <span data-ttu-id="bd107-136">Описание</span><span class="sxs-lookup"><span data-stu-id="bd107-136">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bd107-137">assignedTo</span><span class="sxs-lookup"><span data-stu-id="bd107-137">assignedTo</span></span>|<span data-ttu-id="bd107-138">String</span><span class="sxs-lookup"><span data-stu-id="bd107-138">String</span></span>|<span data-ttu-id="bd107-139">Имя пользователя, которому назначена задача.</span><span class="sxs-lookup"><span data-stu-id="bd107-139">The name of the person who has been assigned the task.</span></span>|
|<span data-ttu-id="bd107-140">body</span><span class="sxs-lookup"><span data-stu-id="bd107-140">body</span></span>|[<span data-ttu-id="bd107-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="bd107-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="bd107-142">Текст задачи, который обычно содержит сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="bd107-142">The task body that typically contains information about the task.</span></span> <span data-ttu-id="bd107-143">Обратите внимание, что поддерживается только тип HTML.</span><span class="sxs-lookup"><span data-stu-id="bd107-143">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="bd107-144">categories</span><span class="sxs-lookup"><span data-stu-id="bd107-144">categories</span></span>|<span data-ttu-id="bd107-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bd107-145">String collection</span></span>|<span data-ttu-id="bd107-146">Категории, связанные с задачей.</span><span class="sxs-lookup"><span data-stu-id="bd107-146">The categories associated with the task.</span></span>|
|<span data-ttu-id="bd107-147">changeKey</span><span class="sxs-lookup"><span data-stu-id="bd107-147">changeKey</span></span>|<span data-ttu-id="bd107-148">Строка</span><span class="sxs-lookup"><span data-stu-id="bd107-148">String</span></span>|<span data-ttu-id="bd107-149">Версия задачи.</span><span class="sxs-lookup"><span data-stu-id="bd107-149">The version of the task.</span></span>|
|<span data-ttu-id="bd107-150">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd107-150">completedDateTime</span></span>|[<span data-ttu-id="bd107-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bd107-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="bd107-152">Дата в указанном часовом поясе, когда задача была завершена.</span><span class="sxs-lookup"><span data-stu-id="bd107-152">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="bd107-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd107-153">createdDateTime</span></span>|<span data-ttu-id="bd107-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd107-154">DateTimeOffset</span></span>|<span data-ttu-id="bd107-155">Дата и время создания задачи.</span><span class="sxs-lookup"><span data-stu-id="bd107-155">The date and time when the task was created.</span></span> <span data-ttu-id="bd107-156">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="bd107-156">By default, it is in UTC.</span></span> <span data-ttu-id="bd107-157">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="bd107-157">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="bd107-158">Значение свойства представлено в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="bd107-158">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="bd107-159">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="bd107-159">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="bd107-160">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="bd107-160">dueDateTime</span></span>|[<span data-ttu-id="bd107-161">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bd107-161">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="bd107-162">Дата в указанном часовом поясе, когда задача должна быть завершена.</span><span class="sxs-lookup"><span data-stu-id="bd107-162">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="bd107-163">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="bd107-163">hasAttachments</span></span>|<span data-ttu-id="bd107-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd107-164">Boolean</span></span>|<span data-ttu-id="bd107-165">Присвоено значение true, если у задачи есть вложения.</span><span class="sxs-lookup"><span data-stu-id="bd107-165">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="bd107-166">importance</span><span class="sxs-lookup"><span data-stu-id="bd107-166">importance</span></span>|<span data-ttu-id="bd107-167">строка</span><span class="sxs-lookup"><span data-stu-id="bd107-167">string</span></span>|<span data-ttu-id="bd107-168">Важность события.</span><span class="sxs-lookup"><span data-stu-id="bd107-168">The importance of the event.</span></span> <span data-ttu-id="bd107-169">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="bd107-169">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="bd107-170">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="bd107-170">isReminderOn</span></span>|<span data-ttu-id="bd107-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd107-171">Boolean</span></span>|<span data-ttu-id="bd107-172">Присвоено значение true, если установлено напоминание пользователю о задаче.</span><span class="sxs-lookup"><span data-stu-id="bd107-172">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="bd107-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd107-173">lastModifiedDateTime</span></span>|<span data-ttu-id="bd107-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd107-174">DateTimeOffset</span></span>|<span data-ttu-id="bd107-175">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="bd107-175">The date and time when the task was last modified.</span></span> <span data-ttu-id="bd107-176">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="bd107-176">By default, it is in UTC.</span></span> <span data-ttu-id="bd107-177">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="bd107-177">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="bd107-178">Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bd107-178">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bd107-179">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="bd107-179">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="bd107-180">owner</span><span class="sxs-lookup"><span data-stu-id="bd107-180">owner</span></span>|<span data-ttu-id="bd107-181">String</span><span class="sxs-lookup"><span data-stu-id="bd107-181">String</span></span>|<span data-ttu-id="bd107-182">Имя пользователя, создавшего задачу.</span><span class="sxs-lookup"><span data-stu-id="bd107-182">The name of the person who created the task.</span></span>|
|<span data-ttu-id="bd107-183">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="bd107-183">parentFolderId</span></span>|<span data-ttu-id="bd107-184">Строка</span><span class="sxs-lookup"><span data-stu-id="bd107-184">String</span></span>|<span data-ttu-id="bd107-185">Уникальный идентификатор родительской папки задачи.</span><span class="sxs-lookup"><span data-stu-id="bd107-185">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="bd107-186">recurrence</span><span class="sxs-lookup"><span data-stu-id="bd107-186">recurrence</span></span>|[<span data-ttu-id="bd107-187">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="bd107-187">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="bd107-188">Расписание повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="bd107-188">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="bd107-189">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="bd107-189">reminderDateTime</span></span>|[<span data-ttu-id="bd107-190">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bd107-190">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="bd107-191">Дата и время появления напоминания о задаче.</span><span class="sxs-lookup"><span data-stu-id="bd107-191">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="bd107-192">sensitivity</span><span class="sxs-lookup"><span data-stu-id="bd107-192">sensitivity</span></span>|<span data-ttu-id="bd107-193">string</span><span class="sxs-lookup"><span data-stu-id="bd107-193">string</span></span>|<span data-ttu-id="bd107-194">Указывает уровень конфиденциальности для задачи.</span><span class="sxs-lookup"><span data-stu-id="bd107-194">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="bd107-195">Возможные значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="bd107-195">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="bd107-196">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bd107-196">startDateTime</span></span>|[<span data-ttu-id="bd107-197">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bd107-197">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="bd107-198">Дата в указанном часовом поясе, когда задача должна быть начата.</span><span class="sxs-lookup"><span data-stu-id="bd107-198">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="bd107-199">status</span><span class="sxs-lookup"><span data-stu-id="bd107-199">status</span></span>|<span data-ttu-id="bd107-200">string</span><span class="sxs-lookup"><span data-stu-id="bd107-200">string</span></span>|<span data-ttu-id="bd107-201">Указывает состояние или ход выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="bd107-201">Indicates the state or progress of the task.</span></span> <span data-ttu-id="bd107-202">Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="bd107-202">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="bd107-203">subject</span><span class="sxs-lookup"><span data-stu-id="bd107-203">subject</span></span>|<span data-ttu-id="bd107-204">String</span><span class="sxs-lookup"><span data-stu-id="bd107-204">String</span></span>|<span data-ttu-id="bd107-205">Краткое описание или название задачи.</span><span class="sxs-lookup"><span data-stu-id="bd107-205">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="bd107-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd107-206">Response</span></span>

<span data-ttu-id="bd107-207">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [outlookTask](../resources/outlooktask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd107-207">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd107-208">Пример</span><span class="sxs-lookup"><span data-stu-id="bd107-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd107-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd107-209">Request</span></span>

<span data-ttu-id="bd107-210">В примере ниже показано, как изменить свойство **дуедатетиме** и использовать `Prefer: outlook.timezone` заголовок, чтобы указать свойства, связанные с датами, в ответе на зимнее стандартное время (EST).</span><span class="sxs-lookup"><span data-stu-id="bd107-210">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlooktask"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MTHgwAAA=
Prefer: outlook.timezone="Eastern Standard Time"
Content-type: application/json
Content-length: 76

{
  "dueDateTime":  {
      "dateTime": "2016-05-06T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```

### <a name="response"></a><span data-ttu-id="bd107-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd107-211">Response</span></span>

<span data-ttu-id="bd107-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd107-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 376

{
    "id": "AAMkADA1MTHgwAAA=",
    "createdDateTime": "2016-04-22T18:19:18.9526004-04:00",
    "lastModifiedDateTime": "2016-04-22T18:38:20.5541528-04:00",
    "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXg==",
    "categories": [
    ],
    "assignedTo": null,
    "body": {
        "contentType": "text",
        "content": ""
    },
    "completedDateTime": null,
    "dueDateTime": {
        "dateTime": "2016-05-06T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
    },
    "hasAttachments":false,
    "importance": "normal",
    "isReminderOn": false,
    "owner": "Administrator",
    "parentFolderId": "AQMkADA1MTIBEgAAAA==",
    "recurrence": null,
    "reminderDateTime": null,
    "sensitivity": "normal",
    "startDateTime": {
        "dateTime": "2016-05-03T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
    },
    "status": "notStarted",
    "subject": "Shop for children's weekend"

}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bd107-215">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="bd107-215">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bd107-216">Языках</span><span class="sxs-lookup"><span data-stu-id="bd107-216">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_outlooktask-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd107-217">Язык</span><span class="sxs-lookup"><span data-stu-id="bd107-217">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_outlooktask-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
