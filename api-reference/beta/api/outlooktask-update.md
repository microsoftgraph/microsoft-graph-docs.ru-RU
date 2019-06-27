---
title: Обновление outlooktask
description: Изменение свойств для записи в задаче Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4967be08228990dc8921780928db1c4c24c2be9b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266810"
---
# <a name="update-outlooktask"></a><span data-ttu-id="c7f70-103">Обновление outlooktask</span><span class="sxs-lookup"><span data-stu-id="c7f70-103">Update outlooktask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7f70-104">Изменение свойств для записи в задаче Outlook.</span><span class="sxs-lookup"><span data-stu-id="c7f70-104">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="c7f70-105">Свойство **комплетеддатетиме** может быть задано **полным** действием или явным образом с помощью операции patch.</span><span class="sxs-lookup"><span data-stu-id="c7f70-105">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="c7f70-106">Если вы используете патч для установки **комплетеддатетиме**, убедитесь, что вы также установили **состояние** `completed` .</span><span class="sxs-lookup"><span data-stu-id="c7f70-106">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="c7f70-107">По умолчанию эта операция (а также операции POST, GET и [Complete](../api/outlooktask-complete.md) ) Возвращает свойства, связанные с датами, в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c7f70-107">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="c7f70-108">Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="c7f70-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7f70-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7f70-109">Permissions</span></span>

<span data-ttu-id="c7f70-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7f70-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7f70-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7f70-112">Permission type</span></span>      | <span data-ttu-id="c7f70-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7f70-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7f70-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7f70-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c7f70-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7f70-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="c7f70-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7f70-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7f70-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7f70-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="c7f70-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7f70-118">Application</span></span> | <span data-ttu-id="c7f70-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7f70-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7f70-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7f70-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c7f70-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7f70-121">Request headers</span></span>

| <span data-ttu-id="c7f70-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c7f70-122">Name</span></span>       | <span data-ttu-id="c7f70-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c7f70-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c7f70-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7f70-124">Authorization</span></span>  | <span data-ttu-id="c7f70-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7f70-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7f70-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="c7f70-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="c7f70-128">Задает часовой пояс для свойств времени в отклике в формате UTC, если заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="c7f70-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="c7f70-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c7f70-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7f70-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c7f70-130">Request body</span></span>

<span data-ttu-id="c7f70-p106">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c7f70-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c7f70-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7f70-134">Property</span></span> | <span data-ttu-id="c7f70-135">Тип</span><span class="sxs-lookup"><span data-stu-id="c7f70-135">Type</span></span> | <span data-ttu-id="c7f70-136">Описание</span><span class="sxs-lookup"><span data-stu-id="c7f70-136">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c7f70-137">assignedTo</span><span class="sxs-lookup"><span data-stu-id="c7f70-137">assignedTo</span></span>|<span data-ttu-id="c7f70-138">String</span><span class="sxs-lookup"><span data-stu-id="c7f70-138">String</span></span>|<span data-ttu-id="c7f70-139">Имя пользователя, которому назначена задача.</span><span class="sxs-lookup"><span data-stu-id="c7f70-139">The name of the person who has been assigned the task.</span></span>|
|<span data-ttu-id="c7f70-140">body</span><span class="sxs-lookup"><span data-stu-id="c7f70-140">body</span></span>|[<span data-ttu-id="c7f70-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="c7f70-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="c7f70-142">Текст задачи, который обычно содержит сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="c7f70-142">The task body that typically contains information about the task.</span></span> <span data-ttu-id="c7f70-143">Обратите внимание, что поддерживается только тип HTML.</span><span class="sxs-lookup"><span data-stu-id="c7f70-143">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="c7f70-144">categories</span><span class="sxs-lookup"><span data-stu-id="c7f70-144">categories</span></span>|<span data-ttu-id="c7f70-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c7f70-145">String collection</span></span>|<span data-ttu-id="c7f70-146">Категории, связанные с задачей.</span><span class="sxs-lookup"><span data-stu-id="c7f70-146">The categories associated with the task.</span></span>|
|<span data-ttu-id="c7f70-147">changeKey</span><span class="sxs-lookup"><span data-stu-id="c7f70-147">changeKey</span></span>|<span data-ttu-id="c7f70-148">Строка</span><span class="sxs-lookup"><span data-stu-id="c7f70-148">String</span></span>|<span data-ttu-id="c7f70-149">Версия задачи.</span><span class="sxs-lookup"><span data-stu-id="c7f70-149">The version of the task.</span></span>|
|<span data-ttu-id="c7f70-150">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7f70-150">completedDateTime</span></span>|[<span data-ttu-id="c7f70-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c7f70-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="c7f70-152">Дата в указанном часовом поясе, когда задача была завершена.</span><span class="sxs-lookup"><span data-stu-id="c7f70-152">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="c7f70-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7f70-153">createdDateTime</span></span>|<span data-ttu-id="c7f70-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7f70-154">DateTimeOffset</span></span>|<span data-ttu-id="c7f70-155">Дата и время создания задачи.</span><span class="sxs-lookup"><span data-stu-id="c7f70-155">The date and time when the task was created.</span></span> <span data-ttu-id="c7f70-156">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="c7f70-156">By default, it is in UTC.</span></span> <span data-ttu-id="c7f70-157">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="c7f70-157">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="c7f70-158">Значение свойства представлено в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="c7f70-158">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="c7f70-159">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c7f70-159">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="c7f70-160">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="c7f70-160">dueDateTime</span></span>|[<span data-ttu-id="c7f70-161">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c7f70-161">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="c7f70-162">Дата в указанном часовом поясе, когда задача должна быть завершена.</span><span class="sxs-lookup"><span data-stu-id="c7f70-162">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="c7f70-163">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="c7f70-163">hasAttachments</span></span>|<span data-ttu-id="c7f70-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7f70-164">Boolean</span></span>|<span data-ttu-id="c7f70-165">Присвоено значение true, если у задачи есть вложения.</span><span class="sxs-lookup"><span data-stu-id="c7f70-165">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="c7f70-166">importance</span><span class="sxs-lookup"><span data-stu-id="c7f70-166">importance</span></span>|<span data-ttu-id="c7f70-167">строка</span><span class="sxs-lookup"><span data-stu-id="c7f70-167">string</span></span>|<span data-ttu-id="c7f70-168">Важность события.</span><span class="sxs-lookup"><span data-stu-id="c7f70-168">The importance of the event.</span></span> <span data-ttu-id="c7f70-169">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="c7f70-169">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="c7f70-170">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="c7f70-170">isReminderOn</span></span>|<span data-ttu-id="c7f70-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7f70-171">Boolean</span></span>|<span data-ttu-id="c7f70-172">Присвоено значение true, если установлено напоминание пользователю о задаче.</span><span class="sxs-lookup"><span data-stu-id="c7f70-172">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="c7f70-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7f70-173">lastModifiedDateTime</span></span>|<span data-ttu-id="c7f70-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7f70-174">DateTimeOffset</span></span>|<span data-ttu-id="c7f70-175">Дата и время последнего изменения задачи.</span><span class="sxs-lookup"><span data-stu-id="c7f70-175">The date and time when the task was last modified.</span></span> <span data-ttu-id="c7f70-176">По умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="c7f70-176">By default, it is in UTC.</span></span> <span data-ttu-id="c7f70-177">Можно указать пользовательский часовой пояс в заголовке запроса.</span><span class="sxs-lookup"><span data-stu-id="c7f70-177">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="c7f70-178">Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c7f70-178">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c7f70-179">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c7f70-179">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="c7f70-180">owner</span><span class="sxs-lookup"><span data-stu-id="c7f70-180">owner</span></span>|<span data-ttu-id="c7f70-181">String</span><span class="sxs-lookup"><span data-stu-id="c7f70-181">String</span></span>|<span data-ttu-id="c7f70-182">Имя пользователя, создавшего задачу.</span><span class="sxs-lookup"><span data-stu-id="c7f70-182">The name of the person who created the task.</span></span>|
|<span data-ttu-id="c7f70-183">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="c7f70-183">parentFolderId</span></span>|<span data-ttu-id="c7f70-184">Строка</span><span class="sxs-lookup"><span data-stu-id="c7f70-184">String</span></span>|<span data-ttu-id="c7f70-185">Уникальный идентификатор родительской папки задачи.</span><span class="sxs-lookup"><span data-stu-id="c7f70-185">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="c7f70-186">recurrence</span><span class="sxs-lookup"><span data-stu-id="c7f70-186">recurrence</span></span>|[<span data-ttu-id="c7f70-187">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="c7f70-187">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="c7f70-188">Расписание повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="c7f70-188">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="c7f70-189">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="c7f70-189">reminderDateTime</span></span>|[<span data-ttu-id="c7f70-190">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c7f70-190">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="c7f70-191">Дата и время появления напоминания о задаче.</span><span class="sxs-lookup"><span data-stu-id="c7f70-191">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="c7f70-192">sensitivity</span><span class="sxs-lookup"><span data-stu-id="c7f70-192">sensitivity</span></span>|<span data-ttu-id="c7f70-193">string</span><span class="sxs-lookup"><span data-stu-id="c7f70-193">string</span></span>|<span data-ttu-id="c7f70-194">Указывает уровень конфиденциальности для задачи.</span><span class="sxs-lookup"><span data-stu-id="c7f70-194">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="c7f70-195">Возможные значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="c7f70-195">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="c7f70-196">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c7f70-196">startDateTime</span></span>|[<span data-ttu-id="c7f70-197">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c7f70-197">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="c7f70-198">Дата в указанном часовом поясе, когда задача должна быть начата.</span><span class="sxs-lookup"><span data-stu-id="c7f70-198">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="c7f70-199">status</span><span class="sxs-lookup"><span data-stu-id="c7f70-199">status</span></span>|<span data-ttu-id="c7f70-200">string</span><span class="sxs-lookup"><span data-stu-id="c7f70-200">string</span></span>|<span data-ttu-id="c7f70-201">Указывает состояние или ход выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="c7f70-201">Indicates the state or progress of the task.</span></span> <span data-ttu-id="c7f70-202">Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="c7f70-202">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="c7f70-203">subject</span><span class="sxs-lookup"><span data-stu-id="c7f70-203">subject</span></span>|<span data-ttu-id="c7f70-204">String</span><span class="sxs-lookup"><span data-stu-id="c7f70-204">String</span></span>|<span data-ttu-id="c7f70-205">Краткое описание или название задачи.</span><span class="sxs-lookup"><span data-stu-id="c7f70-205">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="c7f70-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7f70-206">Response</span></span>

<span data-ttu-id="c7f70-207">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [outlookTask](../resources/outlooktask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7f70-207">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7f70-208">Пример</span><span class="sxs-lookup"><span data-stu-id="c7f70-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7f70-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7f70-209">Request</span></span>

<span data-ttu-id="c7f70-210">В примере ниже показано, как изменить свойство **дуедатетиме** и использовать `Prefer: outlook.timezone` заголовок, чтобы указать свойства, связанные с датами, в ответе на зимнее стандартное время (EST).</span><span class="sxs-lookup"><span data-stu-id="c7f70-210">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>
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

### <a name="response"></a><span data-ttu-id="c7f70-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7f70-211">Response</span></span>

<span data-ttu-id="c7f70-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7f70-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c7f70-215">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c7f70-215">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c7f70-216">C#</span><span class="sxs-lookup"><span data-stu-id="c7f70-216">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_outlooktask-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7f70-217">Javascript</span><span class="sxs-lookup"><span data-stu-id="c7f70-217">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_outlooktask-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c7f70-218">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c7f70-218">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_outlooktask-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
