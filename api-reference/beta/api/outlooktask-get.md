---
title: Получение outlookTask
description: Получение свойств и связей задачи Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8db32df8b0e92451c98e4d6bde6a2c503bb17c67
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055493"
---
# <a name="get-outlooktask-deprecated"></a><span data-ttu-id="5b89c-103">Get outlookTask (deprecated)</span><span class="sxs-lookup"><span data-stu-id="5b89c-103">Get outlookTask (deprecated)</span></span>

<span data-ttu-id="5b89c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b89c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="5b89c-105">Получение свойств и связей задачи Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="5b89c-105">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="5b89c-106">По умолчанию эта операция (и POST, [](../api/outlooktask-complete.md) PATCH и полные операции задач) возвращает свойства, связанные с датами в UTC.</span><span class="sxs-lookup"><span data-stu-id="5b89c-106">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="5b89c-107">Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="5b89c-107">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b89c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b89c-108">Permissions</span></span>

<span data-ttu-id="5b89c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b89c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b89c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b89c-111">Permission type</span></span>                        | <span data-ttu-id="5b89c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b89c-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="5b89c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b89c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b89c-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5b89c-114">Tasks.Read</span></span>                          |
| <span data-ttu-id="5b89c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b89c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b89c-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5b89c-116">Tasks.Read</span></span>                          |
| <span data-ttu-id="5b89c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b89c-117">Application</span></span>                            | <span data-ttu-id="5b89c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b89c-118">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="5b89c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b89c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b89c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5b89c-120">Optional query parameters</span></span>

<span data-ttu-id="5b89c-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5b89c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b89c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b89c-122">Request headers</span></span>

| <span data-ttu-id="5b89c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="5b89c-123">Name</span></span>                     | <span data-ttu-id="5b89c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5b89c-124">Description</span></span>                                       |
|:-------------------------|:--------------------------------------------------|
| <span data-ttu-id="5b89c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b89c-125">Authorization</span></span>            | <span data-ttu-id="5b89c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b89c-p103">Bearer {token}. Required.</span></span>                         |
| <span data-ttu-id="5b89c-128">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="5b89c-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="5b89c-129">Указывает часовой пояс для свойств времени в ответе, который будет в UTC, если этот заглавный не указан.</span><span class="sxs-lookup"><span data-stu-id="5b89c-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="5b89c-130">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="5b89c-130">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b89c-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b89c-131">Request body</span></span>

<span data-ttu-id="5b89c-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b89c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b89c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b89c-133">Response</span></span>

<span data-ttu-id="5b89c-134">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект OutlookTask](../resources/outlooktask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5b89c-134">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b89c-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="5b89c-135">Examples</span></span>

### <a name="example-1-get-an-outlook-task"></a><span data-ttu-id="5b89c-136">Пример 1. Получить Outlook задачу</span><span class="sxs-lookup"><span data-stu-id="5b89c-136">Example 1: Get an Outlook task</span></span>

#### <a name="request"></a><span data-ttu-id="5b89c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b89c-137">Request</span></span>

<span data-ttu-id="5b89c-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b89c-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5b89c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b89c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktask_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MTrgAAA=
```
# <a name="c"></a>[<span data-ttu-id="5b89c-140">C#</span><span class="sxs-lookup"><span data-stu-id="5b89c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktask-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b89c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b89c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktask-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b89c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b89c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktask-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5b89c-143">Java</span><span class="sxs-lookup"><span data-stu-id="5b89c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlooktask-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="5b89c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b89c-144">Response</span></span>

<span data-ttu-id="5b89c-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b89c-145">Here is an example of the response.</span></span> <span data-ttu-id="5b89c-146">По умолчанию свойства даты и времени в ответе возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="5b89c-146">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="5b89c-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5b89c-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time"></a><span data-ttu-id="5b89c-148">Пример 2. Outlook задачу со свойствами даты в тихоокеанском стандартном времени</span><span class="sxs-lookup"><span data-stu-id="5b89c-148">Example 2: Get Outlook task with date-time properties in Pacific Standard Time</span></span>

#### <a name="request"></a><span data-ttu-id="5b89c-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b89c-149">Request</span></span>

<span data-ttu-id="5b89c-150">В этом примере заголовка указывает, что API должен возвращать свойства даты в ответе `Prefer: outlook.timezone` в тихоокеанском стандартном времени.</span><span class="sxs-lookup"><span data-stu-id="5b89c-150">This example uses the `Prefer: outlook.timezone` header to specify that the API should return date-time properties in the response in Pacific Standard Time.</span></span>


# <a name="http"></a>[<span data-ttu-id="5b89c-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b89c-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktask_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MHgwAAA=
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="5b89c-152">C#</span><span class="sxs-lookup"><span data-stu-id="5b89c-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktask-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b89c-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b89c-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktask-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b89c-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b89c-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktask-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5b89c-155">Java</span><span class="sxs-lookup"><span data-stu-id="5b89c-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlooktask-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5b89c-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b89c-156">Response</span></span>

<span data-ttu-id="5b89c-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b89c-157">Here is an example of the response.</span></span> <span data-ttu-id="5b89c-158">Свойства времени даты в ответе возвращаются в указанное тихоокеанское стандартное время.</span><span class="sxs-lookup"><span data-stu-id="5b89c-158">The date-time properties in the response are returned in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="5b89c-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5b89c-159">**Note:** The response object shown here might be shortened for readability.</span></span>

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
