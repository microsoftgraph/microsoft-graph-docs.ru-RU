---
title: Обновление outlooktask
description: Изменение свойств для записи в задаче Outlook.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cc311b0e95e33dd189908d7bbec8fa9d57fd0282
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413596"
---
# <a name="update-outlooktask"></a><span data-ttu-id="da5ab-103">Обновление outlooktask</span><span class="sxs-lookup"><span data-stu-id="da5ab-103">Update outlooktask</span></span>

<span data-ttu-id="da5ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da5ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da5ab-105">Изменение свойств для записи в задаче Outlook.</span><span class="sxs-lookup"><span data-stu-id="da5ab-105">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="da5ab-106">Свойство **комплетеддатетиме** может быть задано **полным** действием или явным образом с помощью операции patch.</span><span class="sxs-lookup"><span data-stu-id="da5ab-106">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="da5ab-107">Если вы используете патч для установки **комплетеддатетиме**, убедитесь, что вы также установили **состояние** `completed` .</span><span class="sxs-lookup"><span data-stu-id="da5ab-107">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="da5ab-108">По умолчанию эта операция (а также операции POST, GET и [Complete](../api/outlooktask-complete.md) ) Возвращает свойства, связанные с датами, в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="da5ab-108">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="da5ab-109">Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="da5ab-109">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="da5ab-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da5ab-110">Permissions</span></span>

<span data-ttu-id="da5ab-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da5ab-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da5ab-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da5ab-113">Permission type</span></span>      | <span data-ttu-id="da5ab-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da5ab-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da5ab-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da5ab-115">Delegated (work or school account)</span></span> | <span data-ttu-id="da5ab-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da5ab-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="da5ab-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da5ab-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da5ab-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da5ab-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="da5ab-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da5ab-119">Application</span></span> | <span data-ttu-id="da5ab-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da5ab-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da5ab-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da5ab-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="da5ab-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da5ab-122">Request headers</span></span>

| <span data-ttu-id="da5ab-123">Имя</span><span class="sxs-lookup"><span data-stu-id="da5ab-123">Name</span></span>       | <span data-ttu-id="da5ab-124">Описание</span><span class="sxs-lookup"><span data-stu-id="da5ab-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="da5ab-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da5ab-125">Authorization</span></span>  | <span data-ttu-id="da5ab-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da5ab-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="da5ab-128">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="da5ab-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="da5ab-129">Задает часовой пояс для свойств времени в отклике в формате UTC, если заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="da5ab-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="da5ab-130">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="da5ab-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da5ab-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="da5ab-131">Request body</span></span>

<span data-ttu-id="da5ab-p106">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="da5ab-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="da5ab-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="da5ab-135">Property</span></span> | <span data-ttu-id="da5ab-136">Тип</span><span class="sxs-lookup"><span data-stu-id="da5ab-136">Type</span></span> | <span data-ttu-id="da5ab-137">Описание</span><span class="sxs-lookup"><span data-stu-id="da5ab-137">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="da5ab-138">body</span><span class="sxs-lookup"><span data-stu-id="da5ab-138">body</span></span>|[<span data-ttu-id="da5ab-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="da5ab-139">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="da5ab-140">Текст задачи, который обычно содержит сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="da5ab-140">The task body that typically contains information about the task.</span></span> <span data-ttu-id="da5ab-141">Обратите внимание, что поддерживается только тип HTML.</span><span class="sxs-lookup"><span data-stu-id="da5ab-141">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="da5ab-142">categories</span><span class="sxs-lookup"><span data-stu-id="da5ab-142">categories</span></span>|<span data-ttu-id="da5ab-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="da5ab-143">String collection</span></span>|<span data-ttu-id="da5ab-144">Категории, связанные с задачей.</span><span class="sxs-lookup"><span data-stu-id="da5ab-144">The categories associated with the task.</span></span>|
|<span data-ttu-id="da5ab-145">changeKey</span><span class="sxs-lookup"><span data-stu-id="da5ab-145">changeKey</span></span>|<span data-ttu-id="da5ab-146">String</span><span class="sxs-lookup"><span data-stu-id="da5ab-146">String</span></span>|<span data-ttu-id="da5ab-147">Версия задачи.</span><span class="sxs-lookup"><span data-stu-id="da5ab-147">The version of the task.</span></span>|
|<span data-ttu-id="da5ab-148">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="da5ab-148">completedDateTime</span></span>|[<span data-ttu-id="da5ab-149">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="da5ab-149">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="da5ab-150">Дата в указанном часовом поясе, когда задача была завершена.</span><span class="sxs-lookup"><span data-stu-id="da5ab-150">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="da5ab-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da5ab-151">createdDateTime</span></span>|<span data-ttu-id="da5ab-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da5ab-152">DateTimeOffset</span></span>|<span data-ttu-id="da5ab-153">Дата и время создания задачи.</span><span class="sxs-lookup"><span data-stu-id="da5ab-153">The date and time when the task was created.</span></span> <span data-ttu-id="da5ab-154">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="da5ab-154">By default, it is in UTC.</span></span> <span data-ttu-id="da5ab-155">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="da5ab-155">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="da5ab-156">Значение свойства представлено в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="da5ab-156">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="da5ab-157">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="da5ab-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="da5ab-158">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="da5ab-158">dueDateTime</span></span>|[<span data-ttu-id="da5ab-159">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="da5ab-159">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="da5ab-160">Дата в указанном часовом поясе, когда задача должна быть завершена.</span><span class="sxs-lookup"><span data-stu-id="da5ab-160">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="da5ab-161">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="da5ab-161">hasAttachments</span></span>|<span data-ttu-id="da5ab-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="da5ab-162">Boolean</span></span>|<span data-ttu-id="da5ab-163">Присвоено значение true, если у задачи есть вложения.</span><span class="sxs-lookup"><span data-stu-id="da5ab-163">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="da5ab-164">importance</span><span class="sxs-lookup"><span data-stu-id="da5ab-164">importance</span></span>|<span data-ttu-id="da5ab-165">строка</span><span class="sxs-lookup"><span data-stu-id="da5ab-165">string</span></span>|<span data-ttu-id="da5ab-166">Важность события.</span><span class="sxs-lookup"><span data-stu-id="da5ab-166">The importance of the event.</span></span> <span data-ttu-id="da5ab-167">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="da5ab-167">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="da5ab-168">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="da5ab-168">isReminderOn</span></span>|<span data-ttu-id="da5ab-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="da5ab-169">Boolean</span></span>|<span data-ttu-id="da5ab-170">Присвоено значение true, если установлено напоминание пользователю о задаче.</span><span class="sxs-lookup"><span data-stu-id="da5ab-170">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="da5ab-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da5ab-171">lastModifiedDateTime</span></span>|<span data-ttu-id="da5ab-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da5ab-172">DateTimeOffset</span></span>|<span data-ttu-id="da5ab-173">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="da5ab-173">The date and time when the task was last modified.</span></span> <span data-ttu-id="da5ab-174">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="da5ab-174">By default, it is in UTC.</span></span> <span data-ttu-id="da5ab-175">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="da5ab-175">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="da5ab-176">Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="da5ab-176">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="da5ab-177">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="da5ab-177">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="da5ab-178">owner</span><span class="sxs-lookup"><span data-stu-id="da5ab-178">owner</span></span>|<span data-ttu-id="da5ab-179">String</span><span class="sxs-lookup"><span data-stu-id="da5ab-179">String</span></span>|<span data-ttu-id="da5ab-180">Имя пользователя, создавшего задачу.</span><span class="sxs-lookup"><span data-stu-id="da5ab-180">The name of the person who created the task.</span></span>|
|<span data-ttu-id="da5ab-181">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="da5ab-181">parentFolderId</span></span>|<span data-ttu-id="da5ab-182">Строка</span><span class="sxs-lookup"><span data-stu-id="da5ab-182">String</span></span>|<span data-ttu-id="da5ab-183">Уникальный идентификатор родительской папки задачи.</span><span class="sxs-lookup"><span data-stu-id="da5ab-183">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="da5ab-184">recurrence</span><span class="sxs-lookup"><span data-stu-id="da5ab-184">recurrence</span></span>|[<span data-ttu-id="da5ab-185">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="da5ab-185">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="da5ab-186">Расписание повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="da5ab-186">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="da5ab-187">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="da5ab-187">reminderDateTime</span></span>|[<span data-ttu-id="da5ab-188">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="da5ab-188">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="da5ab-189">Дата и время появления напоминания о задаче.</span><span class="sxs-lookup"><span data-stu-id="da5ab-189">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="da5ab-190">sensitivity</span><span class="sxs-lookup"><span data-stu-id="da5ab-190">sensitivity</span></span>|<span data-ttu-id="da5ab-191">string</span><span class="sxs-lookup"><span data-stu-id="da5ab-191">string</span></span>|<span data-ttu-id="da5ab-192">Указывает уровень конфиденциальности для задачи.</span><span class="sxs-lookup"><span data-stu-id="da5ab-192">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="da5ab-193">Возможные значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="da5ab-193">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="da5ab-194">startDateTime</span><span class="sxs-lookup"><span data-stu-id="da5ab-194">startDateTime</span></span>|[<span data-ttu-id="da5ab-195">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="da5ab-195">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="da5ab-196">Дата в указанном часовом поясе, когда задача должна быть начата.</span><span class="sxs-lookup"><span data-stu-id="da5ab-196">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="da5ab-197">status</span><span class="sxs-lookup"><span data-stu-id="da5ab-197">status</span></span>|<span data-ttu-id="da5ab-198">string</span><span class="sxs-lookup"><span data-stu-id="da5ab-198">string</span></span>|<span data-ttu-id="da5ab-199">Указывает состояние или ход выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="da5ab-199">Indicates the state or progress of the task.</span></span> <span data-ttu-id="da5ab-200">Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="da5ab-200">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="da5ab-201">subject</span><span class="sxs-lookup"><span data-stu-id="da5ab-201">subject</span></span>|<span data-ttu-id="da5ab-202">String</span><span class="sxs-lookup"><span data-stu-id="da5ab-202">String</span></span>|<span data-ttu-id="da5ab-203">Краткое описание или название задачи.</span><span class="sxs-lookup"><span data-stu-id="da5ab-203">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="da5ab-204">Ответ</span><span class="sxs-lookup"><span data-stu-id="da5ab-204">Response</span></span>

<span data-ttu-id="da5ab-205">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [outlookTask](../resources/outlooktask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da5ab-205">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da5ab-206">Пример</span><span class="sxs-lookup"><span data-stu-id="da5ab-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="da5ab-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="da5ab-207">Request</span></span>

<span data-ttu-id="da5ab-208">В примере ниже показано, как изменить свойство **дуедатетиме** и использовать `Prefer: outlook.timezone` заголовок, чтобы указать свойства, связанные с датами, в ответе на зимнее стандартное время (EST).</span><span class="sxs-lookup"><span data-stu-id="da5ab-208">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>

# <a name="http"></a>[<span data-ttu-id="da5ab-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="da5ab-209">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="da5ab-210">C#</span><span class="sxs-lookup"><span data-stu-id="da5ab-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da5ab-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da5ab-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da5ab-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da5ab-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="da5ab-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="da5ab-213">Response</span></span>

<span data-ttu-id="da5ab-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da5ab-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
