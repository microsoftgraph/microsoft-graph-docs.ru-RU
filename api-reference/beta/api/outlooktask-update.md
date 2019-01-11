---
title: Обновление outlooktask
description: Изменения для записи свойств задачи Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 13426446fec4e7d33ea0f7fe35cd28d12e4e61d0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874755"
---
# <a name="update-outlooktask"></a><span data-ttu-id="cedac-103">Обновление outlooktask</span><span class="sxs-lookup"><span data-stu-id="cedac-103">Update outlooktask</span></span>

> <span data-ttu-id="cedac-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cedac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cedac-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cedac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cedac-106">Изменения для записи свойств задачи Outlook.</span><span class="sxs-lookup"><span data-stu-id="cedac-106">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="cedac-107">Свойство **completedDateTime** можно задать с действия **завершения** , или явно операции обновления.</span><span class="sxs-lookup"><span data-stu-id="cedac-107">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="cedac-108">При использовании ИСПРАВЛЕНИЯ для значение **completedDateTime**, убедитесь, что вы установите **состояние** `completed` также.</span><span class="sxs-lookup"><span data-stu-id="cedac-108">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="cedac-109">По умолчанию эта операция (и POST, GET и [выполнения](../api/outlooktask-complete.md) операций задач) возвращает свойства, связанные с даты в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="cedac-109">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="cedac-110">Можно использовать `Prefer: outlook.timezone` заголовок, чтобы все свойства, связанный с данными в ответ, представленного в часовом поясе, отличного от UTC.</span><span class="sxs-lookup"><span data-stu-id="cedac-110">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="cedac-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cedac-111">Permissions</span></span>

<span data-ttu-id="cedac-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cedac-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cedac-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cedac-114">Permission type</span></span>      | <span data-ttu-id="cedac-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cedac-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cedac-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cedac-116">Delegated (work or school account)</span></span> | <span data-ttu-id="cedac-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cedac-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="cedac-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cedac-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cedac-119">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cedac-119">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="cedac-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cedac-120">Application</span></span> | <span data-ttu-id="cedac-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cedac-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cedac-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cedac-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cedac-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cedac-123">Request headers</span></span>

| <span data-ttu-id="cedac-124">Имя</span><span class="sxs-lookup"><span data-stu-id="cedac-124">Name</span></span>       | <span data-ttu-id="cedac-125">Описание</span><span class="sxs-lookup"><span data-stu-id="cedac-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cedac-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cedac-126">Authorization</span></span>  | <span data-ttu-id="cedac-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cedac-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cedac-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="cedac-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="cedac-130">Указывает часовой пояс для свойств времени в ответ, который может быть в формате UTC, если не указан этот заголовок.</span><span class="sxs-lookup"><span data-stu-id="cedac-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="cedac-131">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cedac-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cedac-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cedac-132">Request body</span></span>

<span data-ttu-id="cedac-p107">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="cedac-p107">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cedac-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="cedac-136">Property</span></span> | <span data-ttu-id="cedac-137">Тип</span><span class="sxs-lookup"><span data-stu-id="cedac-137">Type</span></span> | <span data-ttu-id="cedac-138">Описание</span><span class="sxs-lookup"><span data-stu-id="cedac-138">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cedac-139">assignedTo</span><span class="sxs-lookup"><span data-stu-id="cedac-139">assignedTo</span></span>|<span data-ttu-id="cedac-140">Строка</span><span class="sxs-lookup"><span data-stu-id="cedac-140">String</span></span>|<span data-ttu-id="cedac-141">Имя пользователя, которому назначена задача.</span><span class="sxs-lookup"><span data-stu-id="cedac-141">The name of the person who has been assigned the task.</span></span>|
|<span data-ttu-id="cedac-142">body</span><span class="sxs-lookup"><span data-stu-id="cedac-142">body</span></span>|[<span data-ttu-id="cedac-143">itemBody</span><span class="sxs-lookup"><span data-stu-id="cedac-143">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="cedac-144">Основная задача, который обычно содержит сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="cedac-144">The task body that typically contains information about the task.</span></span> <span data-ttu-id="cedac-145">Обратите внимание на то, что поддерживается только тип HTML-код.</span><span class="sxs-lookup"><span data-stu-id="cedac-145">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="cedac-146">categories</span><span class="sxs-lookup"><span data-stu-id="cedac-146">categories</span></span>|<span data-ttu-id="cedac-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cedac-147">String collection</span></span>|<span data-ttu-id="cedac-148">Категории, связанные с задачей.</span><span class="sxs-lookup"><span data-stu-id="cedac-148">The categories associated with the task.</span></span>|
|<span data-ttu-id="cedac-149">changeKey</span><span class="sxs-lookup"><span data-stu-id="cedac-149">changeKey</span></span>|<span data-ttu-id="cedac-150">Строка</span><span class="sxs-lookup"><span data-stu-id="cedac-150">String</span></span>|<span data-ttu-id="cedac-151">Версия задачи.</span><span class="sxs-lookup"><span data-stu-id="cedac-151">The version of the task.</span></span>|
|<span data-ttu-id="cedac-152">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="cedac-152">completedDateTime</span></span>|[<span data-ttu-id="cedac-153">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="cedac-153">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="cedac-154">Дата в указанный часовой пояс, окончания задачи.</span><span class="sxs-lookup"><span data-stu-id="cedac-154">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="cedac-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cedac-155">createdDateTime</span></span>|<span data-ttu-id="cedac-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cedac-156">DateTimeOffset</span></span>|<span data-ttu-id="cedac-157">Дата и время создания задачи.</span><span class="sxs-lookup"><span data-stu-id="cedac-157">The date and time when the task was created.</span></span> <span data-ttu-id="cedac-158">По умолчанию он не в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="cedac-158">By default, it is in UTC.</span></span> <span data-ttu-id="cedac-159">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="cedac-159">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="cedac-160">Значение свойства используется формат ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="cedac-160">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="cedac-161">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cedac-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="cedac-162">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="cedac-162">dueDateTime</span></span>|[<span data-ttu-id="cedac-163">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="cedac-163">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="cedac-164">Дата в указанный часовой пояс, которую требуется завершения задачи.</span><span class="sxs-lookup"><span data-stu-id="cedac-164">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="cedac-165">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="cedac-165">hasAttachments</span></span>|<span data-ttu-id="cedac-166">Логический</span><span class="sxs-lookup"><span data-stu-id="cedac-166">Boolean</span></span>|<span data-ttu-id="cedac-167">Значение true, если у задачи вложения.</span><span class="sxs-lookup"><span data-stu-id="cedac-167">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="cedac-168">importance</span><span class="sxs-lookup"><span data-stu-id="cedac-168">importance</span></span>|<span data-ttu-id="cedac-169">string</span><span class="sxs-lookup"><span data-stu-id="cedac-169">string</span></span>|<span data-ttu-id="cedac-170">Важность события.</span><span class="sxs-lookup"><span data-stu-id="cedac-170">The importance of the event.</span></span> <span data-ttu-id="cedac-171">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="cedac-171">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="cedac-172">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="cedac-172">isReminderOn</span></span>|<span data-ttu-id="cedac-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="cedac-173">Boolean</span></span>|<span data-ttu-id="cedac-174">Значение true, если оповещение установлено значение Напоминать пользователю задачи.</span><span class="sxs-lookup"><span data-stu-id="cedac-174">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="cedac-175">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cedac-175">lastModifiedDateTime</span></span>|<span data-ttu-id="cedac-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cedac-176">DateTimeOffset</span></span>|<span data-ttu-id="cedac-177">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="cedac-177">The date and time when the task was last modified.</span></span> <span data-ttu-id="cedac-178">По умолчанию он не в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="cedac-178">By default, it is in UTC.</span></span> <span data-ttu-id="cedac-179">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="cedac-179">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="cedac-180">Значение свойства в формате ISO 8601 и всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="cedac-180">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cedac-181">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cedac-181">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="cedac-182">owner</span><span class="sxs-lookup"><span data-stu-id="cedac-182">owner</span></span>|<span data-ttu-id="cedac-183">Строка</span><span class="sxs-lookup"><span data-stu-id="cedac-183">String</span></span>|<span data-ttu-id="cedac-184">Имя человека, создавшего задачу.</span><span class="sxs-lookup"><span data-stu-id="cedac-184">The name of the person who created the task.</span></span>|
|<span data-ttu-id="cedac-185">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="cedac-185">parentFolderId</span></span>|<span data-ttu-id="cedac-186">Строка</span><span class="sxs-lookup"><span data-stu-id="cedac-186">String</span></span>|<span data-ttu-id="cedac-187">Уникальный идентификатор родительской папки задач.</span><span class="sxs-lookup"><span data-stu-id="cedac-187">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="cedac-188">recurrence</span><span class="sxs-lookup"><span data-stu-id="cedac-188">recurrence</span></span>|[<span data-ttu-id="cedac-189">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="cedac-189">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="cedac-190">Шаблон повторения для задачи.</span><span class="sxs-lookup"><span data-stu-id="cedac-190">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="cedac-191">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="cedac-191">reminderDateTime</span></span>|[<span data-ttu-id="cedac-192">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="cedac-192">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="cedac-193">Дата и время оповещения напоминание задачи, будет выполнена.</span><span class="sxs-lookup"><span data-stu-id="cedac-193">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="cedac-194">sensitivity</span><span class="sxs-lookup"><span data-stu-id="cedac-194">sensitivity</span></span>|<span data-ttu-id="cedac-195">string</span><span class="sxs-lookup"><span data-stu-id="cedac-195">string</span></span>|<span data-ttu-id="cedac-196">Указывает уровень конфиденциальности для задачи.</span><span class="sxs-lookup"><span data-stu-id="cedac-196">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="cedac-197">Возможные значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="cedac-197">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="cedac-198">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cedac-198">startDateTime</span></span>|[<span data-ttu-id="cedac-199">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="cedac-199">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="cedac-200">Дата в указанном часовом поясе после начала задачи.</span><span class="sxs-lookup"><span data-stu-id="cedac-200">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="cedac-201">status</span><span class="sxs-lookup"><span data-stu-id="cedac-201">status</span></span>|<span data-ttu-id="cedac-202">string</span><span class="sxs-lookup"><span data-stu-id="cedac-202">string</span></span>|<span data-ttu-id="cedac-203">Указывает состояние или хода выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="cedac-203">Indicates the state or progress of the task.</span></span> <span data-ttu-id="cedac-204">Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="cedac-204">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="cedac-205">subject</span><span class="sxs-lookup"><span data-stu-id="cedac-205">subject</span></span>|<span data-ttu-id="cedac-206">Строка</span><span class="sxs-lookup"><span data-stu-id="cedac-206">String</span></span>|<span data-ttu-id="cedac-207">Краткое описание или название задачи.</span><span class="sxs-lookup"><span data-stu-id="cedac-207">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="cedac-208">Ответ</span><span class="sxs-lookup"><span data-stu-id="cedac-208">Response</span></span>

<span data-ttu-id="cedac-209">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [outlookTask](../resources/outlooktask.md) объект в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cedac-209">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cedac-210">Пример</span><span class="sxs-lookup"><span data-stu-id="cedac-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="cedac-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="cedac-211">Request</span></span>

<span data-ttu-id="cedac-212">В следующем примере изменяется свойство **dueDateTime** и использует `Prefer: outlook.timezone` заголовка для указания выражения свойств с датами в ответ в Восточное время (ПРИБЛ).</span><span class="sxs-lookup"><span data-stu-id="cedac-212">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlooktask"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTHgwAAA=')

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

### <a name="response"></a><span data-ttu-id="cedac-213">Ответ</span><span class="sxs-lookup"><span data-stu-id="cedac-213">Response</span></span>

<span data-ttu-id="cedac-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cedac-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
