---
title: Получение outlookTask
description: Получение свойств и связей задачи Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 50bc54603005d226f6c05c03f4ccee772ec1d8fb
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849718"
---
# <a name="get-outlooktask"></a><span data-ttu-id="07768-103">Получение outlookTask</span><span class="sxs-lookup"><span data-stu-id="07768-103">Get outlookTask</span></span>

<span data-ttu-id="07768-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07768-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="07768-105">Получение свойств и связей задачи Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="07768-105">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="07768-106">По умолчанию эта операция (post, PATCH и выполненные [операции](../api/outlooktask-complete.md) задач) возвращает связанные с датами свойства в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="07768-106">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="07768-107">Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="07768-107">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="07768-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07768-108">Permissions</span></span>

<span data-ttu-id="07768-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07768-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07768-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07768-111">Permission type</span></span>                        | <span data-ttu-id="07768-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07768-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="07768-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07768-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="07768-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="07768-114">Tasks.Read</span></span>                          |
| <span data-ttu-id="07768-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07768-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07768-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="07768-116">Tasks.Read</span></span>                          |
| <span data-ttu-id="07768-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07768-117">Application</span></span>                            | <span data-ttu-id="07768-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07768-118">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="07768-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07768-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07768-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="07768-120">Optional query parameters</span></span>

<span data-ttu-id="07768-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="07768-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07768-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07768-122">Request headers</span></span>

| <span data-ttu-id="07768-123">Имя</span><span class="sxs-lookup"><span data-stu-id="07768-123">Name</span></span>                     | <span data-ttu-id="07768-124">Описание</span><span class="sxs-lookup"><span data-stu-id="07768-124">Description</span></span>                                       |
|:-------------------------|:--------------------------------------------------|
| <span data-ttu-id="07768-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07768-125">Authorization</span></span>            | <span data-ttu-id="07768-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07768-p103">Bearer {token}. Required.</span></span>                         |
| <span data-ttu-id="07768-128">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="07768-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="07768-129">Задает часовой пояс для свойств времени в ответе, который будет быть указан в формате UTC, если этот заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="07768-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="07768-130">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="07768-130">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07768-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07768-131">Request body</span></span>

<span data-ttu-id="07768-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07768-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07768-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="07768-133">Response</span></span>

<span data-ttu-id="07768-134">При успешном выполнении этот метод возвращает `200 OK` код ответа [и объект outlookTask](../resources/outlooktask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="07768-134">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="07768-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="07768-135">Examples</span></span>

### <a name="example-1-get-an-outlook-task"></a><span data-ttu-id="07768-136">Пример 1. Получение задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="07768-136">Example 1: Get an Outlook task</span></span>

#### <a name="request"></a><span data-ttu-id="07768-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="07768-137">Request</span></span>

<span data-ttu-id="07768-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07768-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="07768-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="07768-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MTrgAAA=
```
# <a name="c"></a>[<span data-ttu-id="07768-140">C#</span><span class="sxs-lookup"><span data-stu-id="07768-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07768-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07768-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07768-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07768-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="07768-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="07768-143">Response</span></span>

<span data-ttu-id="07768-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="07768-144">Here is an example of the response.</span></span> <span data-ttu-id="07768-145">По умолчанию свойства даты и времени в ответе возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="07768-145">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="07768-146">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="07768-146">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="07768-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07768-147">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkADA1MTrgAAA=",
  "createdDateTime": "2016-04-22T06:03:35.9279794Z",
  "lastModifiedDateTime": "2016-04-22T06:03:35.9436052Z",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMyQ==",
  "categories": [],
  "assignedTo": null,
  "body": {
    "contentType": "text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-04-27T04:00:00.0000000",
    "timeZone": "UTC"
  },
  "hasAttachments": false,
  "importance": "normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTBEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "normal",
  "startDateTime": {
    "dateTime": "2016-04-26T04:00:00.0000000",
    "timeZone": "UTC"
  },
  "status": "notStarted",
  "subject": "Shop for dinner"
}
```

### <a name="example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time"></a><span data-ttu-id="07768-148">Пример 2. Получение задачи Outlook со свойствами даты и времени по тихоокеанскоу времени</span><span class="sxs-lookup"><span data-stu-id="07768-148">Example 2: Get Outlook task with date-time properties in Pacific Standard Time</span></span>

#### <a name="request"></a><span data-ttu-id="07768-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="07768-149">Request</span></span>

<span data-ttu-id="07768-150">В этом примере `Prefer: outlook.timezone` используется заголовок, чтобы API возвращал свойства даты и времени в ответе по тихоокеанскому времени.</span><span class="sxs-lookup"><span data-stu-id="07768-150">This example uses the `Prefer: outlook.timezone` header to specify that the API should return date-time properties in the response in Pacific Standard Time.</span></span>


# <a name="http"></a>[<span data-ttu-id="07768-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="07768-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MHgwAAA=
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="07768-152">C#</span><span class="sxs-lookup"><span data-stu-id="07768-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07768-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07768-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07768-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07768-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="07768-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="07768-155">Response</span></span>

<span data-ttu-id="07768-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="07768-156">Here is an example of the response.</span></span> <span data-ttu-id="07768-157">Свойства даты и времени в ответе возвращаются в указанном тихоокеанское время.</span><span class="sxs-lookup"><span data-stu-id="07768-157">The date-time properties in the response are returned in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="07768-158">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="07768-158">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="07768-159">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07768-159">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkADA1MHgwAAA=",
  "createdDateTime": "2016-04-22T15:19:18.9526004-07:00",
  "lastModifiedDateTime": "2016-04-22T15:19:19.015101-07:00",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXA==",
  "categories": [],
  "assignedTo": "Dana Swope",
  "body": {
    "contentType": "text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-05-04T021:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "hasAttachments": false,
  "importance": "normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "normal",
  "startDateTime": {
    "dateTime": "2016-05-02T21:00:00.0000000",
    "timeZone": "Pacific Standard Time"
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
  "description": "Get outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
