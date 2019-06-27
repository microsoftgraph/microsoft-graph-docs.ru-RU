---
title: Перечисление задач
description: Получение всех задач Outlook в указанной папке.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9e9a484492929a6f939eed8cde9ec6c3040b8695
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265746"
---
# <a name="list-tasks"></a><span data-ttu-id="65078-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="65078-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65078-104">Получение всех задач Outlook в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="65078-104">Get all the Outlook tasks in the specified folder.</span></span>

<span data-ttu-id="65078-105">По умолчанию эта операция (а также операции POST, PATCH и [Complete](../api/outlooktask-complete.md) ) Возвращает свойства, связанные с датами, в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="65078-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>  <span data-ttu-id="65078-106">С помощью заголовка `Prefer: outlook.timezone` запроса можно получить все свойства, связанные с датами, в ответе, представленном в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="65078-106">You can use a `Prefer: outlook.timezone` request header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="65078-107">[Пример](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) получения одной задачи.</span><span class="sxs-lookup"><span data-stu-id="65078-107">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="65078-108">Заголовок можно применить точно так же, как и для получения нескольких задач.</span><span class="sxs-lookup"><span data-stu-id="65078-108">You can apply the header similarly to get multiple tasks.</span></span>

<span data-ttu-id="65078-109">Если имеется несколько групп задач, и вы хотите получить все задачи в определенной группе задач, сначала [получите все папки задач в этой группе задач](outlooktaskgroup-list-taskfolders.md), а затем получите задачи в каждой из этих папок задач.</span><span class="sxs-lookup"><span data-stu-id="65078-109">If there is more than one task group, and you want to get all the tasks in a specific task group, first [get all the task folders in that task group](outlooktaskgroup-list-taskfolders.md), and then get the tasks in each of these task folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="65078-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65078-110">Permissions</span></span>
<span data-ttu-id="65078-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65078-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65078-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65078-113">Permission type</span></span>      | <span data-ttu-id="65078-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65078-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65078-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65078-115">Delegated (work or school account)</span></span> | <span data-ttu-id="65078-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="65078-116">Tasks.Read</span></span>    |
|<span data-ttu-id="65078-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65078-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65078-118">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="65078-118">Tasks.Read</span></span>    |
|<span data-ttu-id="65078-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65078-119">Application</span></span> | <span data-ttu-id="65078-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65078-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="65078-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65078-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}/tasks
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="65078-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="65078-122">Optional query parameters</span></span>
<span data-ttu-id="65078-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="65078-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65078-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65078-124">Request headers</span></span>
| <span data-ttu-id="65078-125">Имя</span><span class="sxs-lookup"><span data-stu-id="65078-125">Name</span></span>      |<span data-ttu-id="65078-126">Описание</span><span class="sxs-lookup"><span data-stu-id="65078-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="65078-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65078-127">Authorization</span></span>  | <span data-ttu-id="65078-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65078-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="65078-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="65078-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="65078-131">Задает часовой пояс для свойств времени в отклике в формате UTC, если заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="65078-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="65078-132">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="65078-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65078-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="65078-133">Request body</span></span>
<span data-ttu-id="65078-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="65078-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65078-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="65078-135">Response</span></span>

<span data-ttu-id="65078-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [outlookTask](../resources/outlooktask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="65078-136">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65078-137">Пример</span><span class="sxs-lookup"><span data-stu-id="65078-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65078-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="65078-138">Request</span></span>
<span data-ttu-id="65078-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65078-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks
```
##### <a name="response"></a><span data-ttu-id="65078-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="65078-140">Response</span></span>
<span data-ttu-id="65078-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65078-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="65078-144">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="65078-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="65078-145">C#</span><span class="sxs-lookup"><span data-stu-id="65078-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_tasks-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65078-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="65078-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_tasks-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="65078-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="65078-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_tasks-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-list-tasks.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlooktaskfolder-list-tasks.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktaskfolder-list-tasks.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
