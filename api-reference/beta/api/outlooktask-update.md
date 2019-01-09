---
title: Обновление outlooktask
description: Изменения для записи свойств задачи Outlook.
author: angelgolfer-ms
ms.openlocfilehash: 0cd4907c4ab1cb517ab2611cc4dc30431e496440
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771732"
---
# <a name="update-outlooktask"></a><span data-ttu-id="29ba1-103">Обновление outlooktask</span><span class="sxs-lookup"><span data-stu-id="29ba1-103">Update outlooktask</span></span>

> <span data-ttu-id="29ba1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="29ba1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29ba1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29ba1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="29ba1-106">Изменения для записи свойств задачи Outlook.</span><span class="sxs-lookup"><span data-stu-id="29ba1-106">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="29ba1-107">Свойство **completedDateTime** можно задать с действия **завершения** , или явно операции обновления.</span><span class="sxs-lookup"><span data-stu-id="29ba1-107">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="29ba1-108">При использовании ИСПРАВЛЕНИЯ для значение **completedDateTime**, убедитесь, что вы установите **состояние** `completed` также.</span><span class="sxs-lookup"><span data-stu-id="29ba1-108">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="29ba1-109">По умолчанию эта операция (и POST, GET и [выполнения](../api/outlooktask-complete.md) операций задач) возвращает свойства, связанные с даты в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="29ba1-109">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="29ba1-110">Можно использовать `Prefer: outlook.timezone` заголовок, чтобы все свойства, связанный с данными в ответ, представленного в часовом поясе, отличного от UTC.</span><span class="sxs-lookup"><span data-stu-id="29ba1-110">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="29ba1-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29ba1-111">Permissions</span></span>

<span data-ttu-id="29ba1-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29ba1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29ba1-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29ba1-114">Permission type</span></span>      | <span data-ttu-id="29ba1-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29ba1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29ba1-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29ba1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="29ba1-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29ba1-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="29ba1-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29ba1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29ba1-119">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29ba1-119">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="29ba1-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29ba1-120">Application</span></span> | <span data-ttu-id="29ba1-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29ba1-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29ba1-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29ba1-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="29ba1-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29ba1-123">Request headers</span></span>

| <span data-ttu-id="29ba1-124">Имя</span><span class="sxs-lookup"><span data-stu-id="29ba1-124">Name</span></span>       | <span data-ttu-id="29ba1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="29ba1-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="29ba1-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29ba1-126">Authorization</span></span>  | <span data-ttu-id="29ba1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29ba1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29ba1-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="29ba1-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="29ba1-130">Указывает часовой пояс для свойств времени в ответ, который может быть в формате UTC, если не указан этот заголовок.</span><span class="sxs-lookup"><span data-stu-id="29ba1-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="29ba1-131">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="29ba1-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29ba1-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="29ba1-132">Request body</span></span>

<span data-ttu-id="29ba1-p107">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="29ba1-p107">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="29ba1-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="29ba1-136">Property</span></span> | <span data-ttu-id="29ba1-137">Тип</span><span class="sxs-lookup"><span data-stu-id="29ba1-137">Type</span></span> | <span data-ttu-id="29ba1-138">Описание</span><span class="sxs-lookup"><span data-stu-id="29ba1-138">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="29ba1-139">assignedTo</span><span class="sxs-lookup"><span data-stu-id="29ba1-139">assignedTo</span></span>|<span data-ttu-id="29ba1-140">String</span><span class="sxs-lookup"><span data-stu-id="29ba1-140">String</span></span>|<span data-ttu-id="29ba1-141">Имя пользователя, которому назначена задача.</span><span class="sxs-lookup"><span data-stu-id="29ba1-141">The name of the person who has been assigned the task.</span></span>|
|<span data-ttu-id="29ba1-142">body</span><span class="sxs-lookup"><span data-stu-id="29ba1-142">body</span></span>|[<span data-ttu-id="29ba1-143">itemBody</span><span class="sxs-lookup"><span data-stu-id="29ba1-143">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="29ba1-144">Основная задача, который обычно содержит сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="29ba1-144">The task body that typically contains information about the task.</span></span> <span data-ttu-id="29ba1-145">Обратите внимание на то, что поддерживается только тип HTML-код.</span><span class="sxs-lookup"><span data-stu-id="29ba1-145">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="29ba1-146">categories</span><span class="sxs-lookup"><span data-stu-id="29ba1-146">categories</span></span>|<span data-ttu-id="29ba1-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="29ba1-147">String collection</span></span>|<span data-ttu-id="29ba1-148">Категории, связанные с задачей.</span><span class="sxs-lookup"><span data-stu-id="29ba1-148">The categories associated with the task.</span></span>|
|<span data-ttu-id="29ba1-149">changeKey</span><span class="sxs-lookup"><span data-stu-id="29ba1-149">changeKey</span></span>|<span data-ttu-id="29ba1-150">String</span><span class="sxs-lookup"><span data-stu-id="29ba1-150">String</span></span>|<span data-ttu-id="29ba1-151">Версия задачи.</span><span class="sxs-lookup"><span data-stu-id="29ba1-151">The version of the task.</span></span>|
|<span data-ttu-id="29ba1-152">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="29ba1-152">completedDateTime</span></span>|[<span data-ttu-id="29ba1-153">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="29ba1-153">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="29ba1-154">Дата в указанный часовой пояс, окончания задачи.</span><span class="sxs-lookup"><span data-stu-id="29ba1-154">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="29ba1-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29ba1-155">createdDateTime</span></span>|<span data-ttu-id="29ba1-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29ba1-156">DateTimeOffset</span></span>|<span data-ttu-id="29ba1-157">Дата и время создания задачи.</span><span class="sxs-lookup"><span data-stu-id="29ba1-157">The date and time when the task was created.</span></span> <span data-ttu-id="29ba1-158">По умолчанию он не в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="29ba1-158">By default, it is in UTC.</span></span> <span data-ttu-id="29ba1-159">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="29ba1-159">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="29ba1-160">Значение свойства используется формат ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="29ba1-160">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="29ba1-161">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="29ba1-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="29ba1-162">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="29ba1-162">dueDateTime</span></span>|[<span data-ttu-id="29ba1-163">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="29ba1-163">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="29ba1-164">Дата в указанный часовой пояс, которую требуется завершения задачи.</span><span class="sxs-lookup"><span data-stu-id="29ba1-164">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="29ba1-165">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="29ba1-165">hasAttachments</span></span>|<span data-ttu-id="29ba1-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="29ba1-166">Boolean</span></span>|<span data-ttu-id="29ba1-167">Значение true, если у задачи вложения.</span><span class="sxs-lookup"><span data-stu-id="29ba1-167">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="29ba1-168">importance</span><span class="sxs-lookup"><span data-stu-id="29ba1-168">importance</span></span>|<span data-ttu-id="29ba1-169">string</span><span class="sxs-lookup"><span data-stu-id="29ba1-169">string</span></span>|<span data-ttu-id="29ba1-170">Важность события.</span><span class="sxs-lookup"><span data-stu-id="29ba1-170">The importance of the event.</span></span> <span data-ttu-id="29ba1-171">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="29ba1-171">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="29ba1-172">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="29ba1-172">isReminderOn</span></span>|<span data-ttu-id="29ba1-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="29ba1-173">Boolean</span></span>|<span data-ttu-id="29ba1-174">Значение true, если оповещение установлено значение Напоминать пользователю задачи.</span><span class="sxs-lookup"><span data-stu-id="29ba1-174">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="29ba1-175">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29ba1-175">lastModifiedDateTime</span></span>|<span data-ttu-id="29ba1-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29ba1-176">DateTimeOffset</span></span>|<span data-ttu-id="29ba1-177">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="29ba1-177">The date and time when the task was last modified.</span></span> <span data-ttu-id="29ba1-178">По умолчанию он не в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="29ba1-178">By default, it is in UTC.</span></span> <span data-ttu-id="29ba1-179">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="29ba1-179">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="29ba1-180">Значение свойства в формате ISO 8601 и всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="29ba1-180">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29ba1-181">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="29ba1-181">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="29ba1-182">owner</span><span class="sxs-lookup"><span data-stu-id="29ba1-182">owner</span></span>|<span data-ttu-id="29ba1-183">String</span><span class="sxs-lookup"><span data-stu-id="29ba1-183">String</span></span>|<span data-ttu-id="29ba1-184">Имя человека, создавшего задачу.</span><span class="sxs-lookup"><span data-stu-id="29ba1-184">The name of the person who created the task.</span></span>|
|<span data-ttu-id="29ba1-185">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="29ba1-185">parentFolderId</span></span>|<span data-ttu-id="29ba1-186">String</span><span class="sxs-lookup"><span data-stu-id="29ba1-186">String</span></span>|<span data-ttu-id="29ba1-187">Уникальный идентификатор родительской папки задач.</span><span class="sxs-lookup"><span data-stu-id="29ba1-187">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="29ba1-188">recurrence</span><span class="sxs-lookup"><span data-stu-id="29ba1-188">recurrence</span></span>|[<span data-ttu-id="29ba1-189">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="29ba1-189">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="29ba1-190">Шаблон повторения для задачи.</span><span class="sxs-lookup"><span data-stu-id="29ba1-190">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="29ba1-191">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="29ba1-191">reminderDateTime</span></span>|[<span data-ttu-id="29ba1-192">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="29ba1-192">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="29ba1-193">Дата и время оповещения напоминание задачи, будет выполнена.</span><span class="sxs-lookup"><span data-stu-id="29ba1-193">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="29ba1-194">sensitivity</span><span class="sxs-lookup"><span data-stu-id="29ba1-194">sensitivity</span></span>|<span data-ttu-id="29ba1-195">string</span><span class="sxs-lookup"><span data-stu-id="29ba1-195">string</span></span>|<span data-ttu-id="29ba1-196">Указывает уровень конфиденциальности для задачи.</span><span class="sxs-lookup"><span data-stu-id="29ba1-196">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="29ba1-197">Возможные значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="29ba1-197">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="29ba1-198">startDateTime</span><span class="sxs-lookup"><span data-stu-id="29ba1-198">startDateTime</span></span>|[<span data-ttu-id="29ba1-199">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="29ba1-199">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="29ba1-200">Дата в указанном часовом поясе после начала задачи.</span><span class="sxs-lookup"><span data-stu-id="29ba1-200">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="29ba1-201">status</span><span class="sxs-lookup"><span data-stu-id="29ba1-201">status</span></span>|<span data-ttu-id="29ba1-202">string</span><span class="sxs-lookup"><span data-stu-id="29ba1-202">string</span></span>|<span data-ttu-id="29ba1-203">Указывает состояние или хода выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="29ba1-203">Indicates the state or progress of the task.</span></span> <span data-ttu-id="29ba1-204">Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="29ba1-204">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="29ba1-205">subject</span><span class="sxs-lookup"><span data-stu-id="29ba1-205">subject</span></span>|<span data-ttu-id="29ba1-206">String</span><span class="sxs-lookup"><span data-stu-id="29ba1-206">String</span></span>|<span data-ttu-id="29ba1-207">Краткое описание или название задачи.</span><span class="sxs-lookup"><span data-stu-id="29ba1-207">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="29ba1-208">Ответ</span><span class="sxs-lookup"><span data-stu-id="29ba1-208">Response</span></span>

<span data-ttu-id="29ba1-209">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [outlookTask](../resources/outlooktask.md) объект в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="29ba1-209">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29ba1-210">Пример</span><span class="sxs-lookup"><span data-stu-id="29ba1-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="29ba1-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="29ba1-211">Request</span></span>

<span data-ttu-id="29ba1-212">В следующем примере изменяется свойство **dueDateTime** и использует `Prefer: outlook.timezone` заголовка для указания выражения свойств с датами в ответ в Восточное время (ПРИБЛ).</span><span class="sxs-lookup"><span data-stu-id="29ba1-212">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>
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

### <a name="response"></a><span data-ttu-id="29ba1-213">Ответ</span><span class="sxs-lookup"><span data-stu-id="29ba1-213">Response</span></span>

<span data-ttu-id="29ba1-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="29ba1-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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