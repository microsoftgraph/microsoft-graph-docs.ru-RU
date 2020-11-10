---
title: Перечисление задач
description: Получение всех задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 42e062a41b0c8e4fd5dd46a0e4b605300e22b66b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979459"
---
# <a name="list-tasks-deprecated"></a><span data-ttu-id="67830-103">Перечисление задач (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="67830-103">List tasks (deprecated)</span></span>

<span data-ttu-id="67830-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67830-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="67830-105">Получение всех задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="67830-105">Get all the Outlook tasks in the user's mailbox.</span></span>

<span data-ttu-id="67830-106">По умолчанию эта операция (а также операции POST, PATCH и [Complete](../api/outlooktask-complete.md) ) Возвращает свойства, связанные с датами, в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="67830-106">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>
<span data-ttu-id="67830-107">Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="67830-107">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="67830-108">[Пример](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) получения одной задачи.</span><span class="sxs-lookup"><span data-stu-id="67830-108">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="67830-109">Заголовок можно применить точно так же, как и для получения нескольких задач.</span><span class="sxs-lookup"><span data-stu-id="67830-109">You can apply the header similarly to get multiple tasks.</span></span>

## <a name="permissions"></a><span data-ttu-id="67830-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67830-110">Permissions</span></span>
<span data-ttu-id="67830-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67830-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67830-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67830-113">Permission type</span></span>      | <span data-ttu-id="67830-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67830-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67830-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67830-115">Delegated (work or school account)</span></span> | <span data-ttu-id="67830-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="67830-116">Tasks.Read</span></span>    |
|<span data-ttu-id="67830-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67830-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67830-118">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="67830-118">Tasks.Read</span></span>    |
|<span data-ttu-id="67830-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67830-119">Application</span></span> | <span data-ttu-id="67830-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67830-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67830-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67830-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks
GET /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="67830-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="67830-122">Optional query parameters</span></span>
<span data-ttu-id="67830-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="67830-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67830-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67830-124">Request headers</span></span>
| <span data-ttu-id="67830-125">Имя</span><span class="sxs-lookup"><span data-stu-id="67830-125">Name</span></span>      |<span data-ttu-id="67830-126">Описание</span><span class="sxs-lookup"><span data-stu-id="67830-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="67830-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67830-127">Authorization</span></span>  | <span data-ttu-id="67830-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67830-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="67830-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="67830-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="67830-131">Задает часовой пояс для свойств времени в отклике в формате UTC, если заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="67830-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="67830-132">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="67830-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67830-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67830-133">Request body</span></span>
<span data-ttu-id="67830-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="67830-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67830-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="67830-135">Response</span></span>

<span data-ttu-id="67830-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [outlookTask](../resources/outlooktask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="67830-136">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67830-137">Пример</span><span class="sxs-lookup"><span data-stu-id="67830-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67830-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="67830-138">Request</span></span>
<span data-ttu-id="67830-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67830-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67830-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="67830-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlookuser_get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/tasks
```
# <a name="c"></a>[<span data-ttu-id="67830-141">C#</span><span class="sxs-lookup"><span data-stu-id="67830-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlookuser-get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67830-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67830-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlookuser-get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67830-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67830-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlookuser-get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67830-144">Java</span><span class="sxs-lookup"><span data-stu-id="67830-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/outlookuser-get-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="67830-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="67830-145">Response</span></span>
<span data-ttu-id="67830-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="67830-146">Here is an example of the response.</span></span> <span data-ttu-id="67830-147">По умолчанию свойства даты и времени в ответе возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="67830-147">By default, the date-time properties in the response are in UTC.</span></span>

<span data-ttu-id="67830-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67830-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 465

{
  "value": [
   {
      "id": "AAMkADA1MTrfAAA=",
      "createdDateTime": "2016-04-22T05:44:01.2012012Z",
      "lastModifiedDateTime": "2016-04-22T05:44:02.9980882Z",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMxw==",
      "categories": [ ],
      "assignedTo": null,
      "body": {
        "contentType": "text",
        "content": ""
      },
      "completedDateTime": null,
      "dueDateTime": {
        "dateTime": "2016-04-25T07:00:00.0000000",
        "timeZone": "UTC"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
        "dateTime": "2016-04-23T07:00:00.0000000",
        "timeZone": "UTC"
      },
      "status": "notStarted",
      "subject": "Shop for dinner"
    },
    {
      "id": "AAMkADA1MTrgAAA=",
      "createdDateTime": "2016-04-22T06:03:35.9279794Z",
      "lastModifiedDateTime": "2016-04-22T06:03:35.9436052Z",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMyQ==",
      "categories": [ ],
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
      "hasAttachments":false,
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List Tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
