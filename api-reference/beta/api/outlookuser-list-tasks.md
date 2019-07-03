---
title: Перечисление задач
description: Получение всех задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 5d08e9e8ade8a3537d27ec33a61006456668ddae
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447140"
---
# <a name="list-tasks"></a><span data-ttu-id="8af27-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="8af27-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8af27-104">Получение всех задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="8af27-104">Get all the Outlook tasks in the user's mailbox.</span></span>

<span data-ttu-id="8af27-105">По умолчанию эта операция (а также операции POST, PATCH и [Complete](../api/outlooktask-complete.md) ) Возвращает свойства, связанные с датами, в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="8af27-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>
<span data-ttu-id="8af27-106">Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="8af27-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="8af27-107">[Пример](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) получения одной задачи.</span><span class="sxs-lookup"><span data-stu-id="8af27-107">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="8af27-108">Заголовок можно применить точно так же, как и для получения нескольких задач.</span><span class="sxs-lookup"><span data-stu-id="8af27-108">You can apply the header similarly to get multiple tasks.</span></span>

## <a name="permissions"></a><span data-ttu-id="8af27-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8af27-109">Permissions</span></span>
<span data-ttu-id="8af27-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8af27-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8af27-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8af27-112">Permission type</span></span>      | <span data-ttu-id="8af27-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8af27-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8af27-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8af27-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8af27-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="8af27-115">Tasks.Read</span></span>    |
|<span data-ttu-id="8af27-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8af27-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8af27-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="8af27-117">Tasks.Read</span></span>    |
|<span data-ttu-id="8af27-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8af27-118">Application</span></span> | <span data-ttu-id="8af27-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8af27-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8af27-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8af27-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks
GET /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8af27-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8af27-121">Optional query parameters</span></span>
<span data-ttu-id="8af27-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8af27-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8af27-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8af27-123">Request headers</span></span>
| <span data-ttu-id="8af27-124">Имя</span><span class="sxs-lookup"><span data-stu-id="8af27-124">Name</span></span>      |<span data-ttu-id="8af27-125">Описание</span><span class="sxs-lookup"><span data-stu-id="8af27-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8af27-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8af27-126">Authorization</span></span>  | <span data-ttu-id="8af27-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8af27-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8af27-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="8af27-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="8af27-130">Задает часовой пояс для свойств времени в отклике в формате UTC, если заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="8af27-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="8af27-131">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8af27-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8af27-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8af27-132">Request body</span></span>
<span data-ttu-id="8af27-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8af27-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8af27-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8af27-134">Response</span></span>

<span data-ttu-id="8af27-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [outlookTask](../resources/outlooktask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8af27-135">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8af27-136">Пример</span><span class="sxs-lookup"><span data-stu-id="8af27-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8af27-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="8af27-137">Request</span></span>
<span data-ttu-id="8af27-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8af27-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8af27-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="8af27-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/tasks
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8af27-140">C#</span><span class="sxs-lookup"><span data-stu-id="8af27-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8af27-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="8af27-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8af27-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8af27-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8af27-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8af27-143">Response</span></span>
<span data-ttu-id="8af27-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8af27-144">Here is an example of the response.</span></span> <span data-ttu-id="8af27-145">По умолчанию свойства даты и времени в ответе возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="8af27-145">By default, the date-time properties in the response are in UTC.</span></span>

<span data-ttu-id="8af27-p106">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8af27-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
