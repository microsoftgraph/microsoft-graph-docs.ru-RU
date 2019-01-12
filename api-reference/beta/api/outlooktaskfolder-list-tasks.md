---
title: Перечисление задач
description: Получите все задачи Outlook в указанной папке.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ec814616447db842f4eaaa230cd6634e98859198
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924519"
---
# <a name="list-tasks"></a><span data-ttu-id="7b297-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="7b297-103">List tasks</span></span>

> <span data-ttu-id="7b297-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b297-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b297-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b297-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b297-106">Получите все задачи Outlook в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="7b297-106">Get all the Outlook tasks in the specified folder.</span></span>

<span data-ttu-id="7b297-107">По умолчанию эта операция (и POST, ИСПРАВЛЕНИЙ и [выполнения](../api/outlooktask-complete.md) операции задачи) возвращает свойства, связанные с даты в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="7b297-107">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>  <span data-ttu-id="7b297-108">Можно использовать `Prefer: outlook.timezone` заголовка запроса, чтобы все свойства, связанный с данными в ответ, представленного в часовом поясе, отличного от UTC.</span><span class="sxs-lookup"><span data-stu-id="7b297-108">You can use a `Prefer: outlook.timezone` request header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="7b297-109">В разделе [Пример](outlooktask-get.md#example-2) для получения одну задачу.</span><span class="sxs-lookup"><span data-stu-id="7b297-109">See an [example](outlooktask-get.md#example-2) for getting a single task.</span></span> <span data-ttu-id="7b297-110">Можно применить заголовок аналогичным образом, чтобы получить несколько задач.</span><span class="sxs-lookup"><span data-stu-id="7b297-110">You can apply the header similarly to get multiple tasks.</span></span>

<span data-ttu-id="7b297-111">Если имеется несколько групп задач и вы хотите получить все задачи в группе определенной задачи, первый [Получение всех папок задач в этой группе задач](outlooktaskgroup-list-taskfolders.md)и затем получите задачи в каждой из этих папок задач.</span><span class="sxs-lookup"><span data-stu-id="7b297-111">If there is more than one task group, and you want to get all the tasks in a specific task group, first [get all the task folders in that task group](outlooktaskgroup-list-taskfolders.md), and then get the tasks in each of these task folders.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7b297-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b297-112">Permissions</span></span>
<span data-ttu-id="7b297-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b297-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b297-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b297-115">Permission type</span></span>      | <span data-ttu-id="7b297-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b297-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b297-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b297-117">Delegated (work or school account)</span></span> | <span data-ttu-id="7b297-118">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="7b297-118">Tasks.Read</span></span>    |
|<span data-ttu-id="7b297-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b297-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b297-120">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="7b297-120">Tasks.Read</span></span>    |
|<span data-ttu-id="7b297-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b297-121">Application</span></span> | <span data-ttu-id="7b297-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b297-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b297-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b297-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7b297-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7b297-124">Optional query parameters</span></span>
<span data-ttu-id="7b297-125">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7b297-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b297-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b297-126">Request headers</span></span>
| <span data-ttu-id="7b297-127">Имя</span><span class="sxs-lookup"><span data-stu-id="7b297-127">Name</span></span>      |<span data-ttu-id="7b297-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7b297-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7b297-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b297-129">Authorization</span></span>  | <span data-ttu-id="7b297-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b297-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7b297-132">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="7b297-132">Prefer: outlook.timezone</span></span> | <span data-ttu-id="7b297-133">Указывает часовой пояс для свойств времени в ответ, который может быть в формате UTC, если не указан этот заголовок.</span><span class="sxs-lookup"><span data-stu-id="7b297-133">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="7b297-134">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7b297-134">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b297-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b297-135">Request body</span></span>
<span data-ttu-id="7b297-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b297-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b297-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b297-137">Response</span></span>

<span data-ttu-id="7b297-138">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [outlookTask](../resources/outlooktask.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7b297-138">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7b297-139">Пример</span><span class="sxs-lookup"><span data-stu-id="7b297-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b297-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b297-140">Request</span></span>
<span data-ttu-id="7b297-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b297-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks
```
##### <a name="response"></a><span data-ttu-id="7b297-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b297-142">Response</span></span>
<span data-ttu-id="7b297-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7b297-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
