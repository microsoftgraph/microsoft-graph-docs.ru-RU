---
title: Обновление outlooktask
description: Изменение свойств для записи в задаче Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c0d0736752e1f9127219ac3d7d9a64eb772ad81c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877666"
---
# <a name="update-outlooktask"></a><span data-ttu-id="a7e90-103">Обновление outlooktask</span><span class="sxs-lookup"><span data-stu-id="a7e90-103">Update outlooktask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7e90-104">Изменение свойств для записи в задаче Outlook.</span><span class="sxs-lookup"><span data-stu-id="a7e90-104">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="a7e90-105">Свойство **комплетеддатетиме** может быть задано **полным** действием или явным образом с помощью операции patch.</span><span class="sxs-lookup"><span data-stu-id="a7e90-105">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="a7e90-106">Если вы используете патч для установки **комплетеддатетиме**, убедитесь, что вы также установили **состояние** `completed` .</span><span class="sxs-lookup"><span data-stu-id="a7e90-106">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="a7e90-107">По умолчанию эта операция (а также операции POST, GET и [Complete](../api/outlooktask-complete.md) ) Возвращает свойства, связанные с датами, в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="a7e90-107">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="a7e90-108">Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="a7e90-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7e90-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7e90-109">Permissions</span></span>

<span data-ttu-id="a7e90-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7e90-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7e90-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7e90-112">Permission type</span></span>      | <span data-ttu-id="a7e90-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7e90-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7e90-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7e90-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a7e90-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7e90-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a7e90-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7e90-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7e90-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7e90-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a7e90-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7e90-118">Application</span></span> | <span data-ttu-id="a7e90-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7e90-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7e90-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7e90-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a7e90-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7e90-121">Request headers</span></span>

| <span data-ttu-id="a7e90-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a7e90-122">Name</span></span>       | <span data-ttu-id="a7e90-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a7e90-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a7e90-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7e90-124">Authorization</span></span>  | <span data-ttu-id="a7e90-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7e90-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a7e90-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="a7e90-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="a7e90-128">Задает часовой пояс для свойств времени в отклике в формате UTC, если заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="a7e90-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="a7e90-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="a7e90-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7e90-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a7e90-130">Request body</span></span>

<span data-ttu-id="a7e90-p106">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a7e90-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a7e90-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7e90-134">Property</span></span> | <span data-ttu-id="a7e90-135">Тип</span><span class="sxs-lookup"><span data-stu-id="a7e90-135">Type</span></span> | <span data-ttu-id="a7e90-136">Описание</span><span class="sxs-lookup"><span data-stu-id="a7e90-136">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a7e90-137">body</span><span class="sxs-lookup"><span data-stu-id="a7e90-137">body</span></span>|[<span data-ttu-id="a7e90-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="a7e90-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="a7e90-139">Текст задачи, который обычно содержит сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="a7e90-139">The task body that typically contains information about the task.</span></span> <span data-ttu-id="a7e90-140">Обратите внимание, что поддерживается только тип HTML.</span><span class="sxs-lookup"><span data-stu-id="a7e90-140">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="a7e90-141">categories</span><span class="sxs-lookup"><span data-stu-id="a7e90-141">categories</span></span>|<span data-ttu-id="a7e90-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a7e90-142">String collection</span></span>|<span data-ttu-id="a7e90-143">Категории, связанные с задачей.</span><span class="sxs-lookup"><span data-stu-id="a7e90-143">The categories associated with the task.</span></span>|
|<span data-ttu-id="a7e90-144">changeKey</span><span class="sxs-lookup"><span data-stu-id="a7e90-144">changeKey</span></span>|<span data-ttu-id="a7e90-145">String</span><span class="sxs-lookup"><span data-stu-id="a7e90-145">String</span></span>|<span data-ttu-id="a7e90-146">Версия задачи.</span><span class="sxs-lookup"><span data-stu-id="a7e90-146">The version of the task.</span></span>|
|<span data-ttu-id="a7e90-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7e90-147">completedDateTime</span></span>|[<span data-ttu-id="a7e90-148">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a7e90-148">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="a7e90-149">Дата в указанном часовом поясе, когда задача была завершена.</span><span class="sxs-lookup"><span data-stu-id="a7e90-149">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="a7e90-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7e90-150">createdDateTime</span></span>|<span data-ttu-id="a7e90-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7e90-151">DateTimeOffset</span></span>|<span data-ttu-id="a7e90-152">Дата и время создания задачи.</span><span class="sxs-lookup"><span data-stu-id="a7e90-152">The date and time when the task was created.</span></span> <span data-ttu-id="a7e90-153">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="a7e90-153">By default, it is in UTC.</span></span> <span data-ttu-id="a7e90-154">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="a7e90-154">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="a7e90-155">Значение свойства представлено в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="a7e90-155">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="a7e90-156">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a7e90-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a7e90-157">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="a7e90-157">dueDateTime</span></span>|[<span data-ttu-id="a7e90-158">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a7e90-158">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="a7e90-159">Дата в указанном часовом поясе, когда задача должна быть завершена.</span><span class="sxs-lookup"><span data-stu-id="a7e90-159">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="a7e90-160">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="a7e90-160">hasAttachments</span></span>|<span data-ttu-id="a7e90-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7e90-161">Boolean</span></span>|<span data-ttu-id="a7e90-162">Присвоено значение true, если у задачи есть вложения.</span><span class="sxs-lookup"><span data-stu-id="a7e90-162">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="a7e90-163">importance</span><span class="sxs-lookup"><span data-stu-id="a7e90-163">importance</span></span>|<span data-ttu-id="a7e90-164">строка</span><span class="sxs-lookup"><span data-stu-id="a7e90-164">string</span></span>|<span data-ttu-id="a7e90-165">Важность события.</span><span class="sxs-lookup"><span data-stu-id="a7e90-165">The importance of the event.</span></span> <span data-ttu-id="a7e90-166">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="a7e90-166">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="a7e90-167">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="a7e90-167">isReminderOn</span></span>|<span data-ttu-id="a7e90-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7e90-168">Boolean</span></span>|<span data-ttu-id="a7e90-169">Присвоено значение true, если установлено напоминание пользователю о задаче.</span><span class="sxs-lookup"><span data-stu-id="a7e90-169">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="a7e90-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7e90-170">lastModifiedDateTime</span></span>|<span data-ttu-id="a7e90-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7e90-171">DateTimeOffset</span></span>|<span data-ttu-id="a7e90-172">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="a7e90-172">The date and time when the task was last modified.</span></span> <span data-ttu-id="a7e90-173">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="a7e90-173">By default, it is in UTC.</span></span> <span data-ttu-id="a7e90-174">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="a7e90-174">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="a7e90-175">Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a7e90-175">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a7e90-176">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a7e90-176">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a7e90-177">owner</span><span class="sxs-lookup"><span data-stu-id="a7e90-177">owner</span></span>|<span data-ttu-id="a7e90-178">String</span><span class="sxs-lookup"><span data-stu-id="a7e90-178">String</span></span>|<span data-ttu-id="a7e90-179">Имя пользователя, создавшего задачу.</span><span class="sxs-lookup"><span data-stu-id="a7e90-179">The name of the person who created the task.</span></span>|
|<span data-ttu-id="a7e90-180">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="a7e90-180">parentFolderId</span></span>|<span data-ttu-id="a7e90-181">Строка</span><span class="sxs-lookup"><span data-stu-id="a7e90-181">String</span></span>|<span data-ttu-id="a7e90-182">Уникальный идентификатор родительской папки задачи.</span><span class="sxs-lookup"><span data-stu-id="a7e90-182">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="a7e90-183">recurrence</span><span class="sxs-lookup"><span data-stu-id="a7e90-183">recurrence</span></span>|[<span data-ttu-id="a7e90-184">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="a7e90-184">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="a7e90-185">Расписание повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="a7e90-185">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="a7e90-186">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="a7e90-186">reminderDateTime</span></span>|[<span data-ttu-id="a7e90-187">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a7e90-187">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="a7e90-188">Дата и время появления напоминания о задаче.</span><span class="sxs-lookup"><span data-stu-id="a7e90-188">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="a7e90-189">sensitivity</span><span class="sxs-lookup"><span data-stu-id="a7e90-189">sensitivity</span></span>|<span data-ttu-id="a7e90-190">string</span><span class="sxs-lookup"><span data-stu-id="a7e90-190">string</span></span>|<span data-ttu-id="a7e90-191">Указывает уровень конфиденциальности для задачи.</span><span class="sxs-lookup"><span data-stu-id="a7e90-191">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="a7e90-192">Возможные значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="a7e90-192">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="a7e90-193">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a7e90-193">startDateTime</span></span>|[<span data-ttu-id="a7e90-194">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a7e90-194">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="a7e90-195">Дата в указанном часовом поясе, когда задача должна быть начата.</span><span class="sxs-lookup"><span data-stu-id="a7e90-195">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="a7e90-196">status</span><span class="sxs-lookup"><span data-stu-id="a7e90-196">status</span></span>|<span data-ttu-id="a7e90-197">string</span><span class="sxs-lookup"><span data-stu-id="a7e90-197">string</span></span>|<span data-ttu-id="a7e90-198">Указывает состояние или ход выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="a7e90-198">Indicates the state or progress of the task.</span></span> <span data-ttu-id="a7e90-199">Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="a7e90-199">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="a7e90-200">subject</span><span class="sxs-lookup"><span data-stu-id="a7e90-200">subject</span></span>|<span data-ttu-id="a7e90-201">String</span><span class="sxs-lookup"><span data-stu-id="a7e90-201">String</span></span>|<span data-ttu-id="a7e90-202">Краткое описание или название задачи.</span><span class="sxs-lookup"><span data-stu-id="a7e90-202">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="a7e90-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7e90-203">Response</span></span>

<span data-ttu-id="a7e90-204">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [outlookTask](../resources/outlooktask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7e90-204">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7e90-205">Пример</span><span class="sxs-lookup"><span data-stu-id="a7e90-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7e90-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7e90-206">Request</span></span>

<span data-ttu-id="a7e90-207">В примере ниже показано, как изменить свойство **дуедатетиме** и использовать `Prefer: outlook.timezone` заголовок, чтобы указать свойства, связанные с датами, в ответе на зимнее стандартное время (EST).</span><span class="sxs-lookup"><span data-stu-id="a7e90-207">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a7e90-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7e90-208">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a7e90-209">C#</span><span class="sxs-lookup"><span data-stu-id="a7e90-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7e90-210">Javascript</span><span class="sxs-lookup"><span data-stu-id="a7e90-210">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a7e90-211">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a7e90-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a7e90-212">Java</span><span class="sxs-lookup"><span data-stu-id="a7e90-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlooktask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a7e90-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7e90-213">Response</span></span>

<span data-ttu-id="a7e90-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7e90-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
