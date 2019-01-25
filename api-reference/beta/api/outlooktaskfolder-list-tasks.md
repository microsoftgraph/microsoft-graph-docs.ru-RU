---
title: Перечисление задач
description: Получите все задачи Outlook в указанной папке.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 892409d6622ffd7b6e0243f7bcdb8807f2ee1305
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509345"
---
# <a name="list-tasks"></a><span data-ttu-id="7b1d3-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="7b1d3-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b1d3-104">Получите все задачи Outlook в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="7b1d3-104">Get all the Outlook tasks in the specified folder.</span></span>

<span data-ttu-id="7b1d3-105">По умолчанию эта операция (и POST, ИСПРАВЛЕНИЙ и [выполнения](../api/outlooktask-complete.md) операции задачи) возвращает свойства, связанные с даты в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="7b1d3-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>  <span data-ttu-id="7b1d3-106">Можно использовать `Prefer: outlook.timezone` заголовка запроса, чтобы все свойства, связанный с данными в ответ, представленного в часовом поясе, отличного от UTC.</span><span class="sxs-lookup"><span data-stu-id="7b1d3-106">You can use a `Prefer: outlook.timezone` request header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="7b1d3-107">В разделе [Пример](outlooktask-get.md#example-2) для получения одну задачу.</span><span class="sxs-lookup"><span data-stu-id="7b1d3-107">See an [example](outlooktask-get.md#example-2) for getting a single task.</span></span> <span data-ttu-id="7b1d3-108">Можно применить заголовок аналогичным образом, чтобы получить несколько задач.</span><span class="sxs-lookup"><span data-stu-id="7b1d3-108">You can apply the header similarly to get multiple tasks.</span></span>

<span data-ttu-id="7b1d3-109">Если имеется несколько групп задач и вы хотите получить все задачи в группе определенной задачи, первый [Получение всех папок задач в этой группе задач](outlooktaskgroup-list-taskfolders.md)и затем получите задачи в каждой из этих папок задач.</span><span class="sxs-lookup"><span data-stu-id="7b1d3-109">If there is more than one task group, and you want to get all the tasks in a specific task group, first [get all the task folders in that task group](outlooktaskgroup-list-taskfolders.md), and then get the tasks in each of these task folders.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7b1d3-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b1d3-110">Permissions</span></span>
<span data-ttu-id="7b1d3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b1d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b1d3-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b1d3-113">Permission type</span></span>      | <span data-ttu-id="7b1d3-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b1d3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b1d3-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b1d3-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7b1d3-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="7b1d3-116">Tasks.Read</span></span>    |
|<span data-ttu-id="7b1d3-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b1d3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b1d3-118">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="7b1d3-118">Tasks.Read</span></span>    |
|<span data-ttu-id="7b1d3-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b1d3-119">Application</span></span> | <span data-ttu-id="7b1d3-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b1d3-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b1d3-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b1d3-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7b1d3-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7b1d3-122">Optional query parameters</span></span>
<span data-ttu-id="7b1d3-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7b1d3-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b1d3-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b1d3-124">Request headers</span></span>
| <span data-ttu-id="7b1d3-125">Имя</span><span class="sxs-lookup"><span data-stu-id="7b1d3-125">Name</span></span>      |<span data-ttu-id="7b1d3-126">Описание</span><span class="sxs-lookup"><span data-stu-id="7b1d3-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7b1d3-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b1d3-127">Authorization</span></span>  | <span data-ttu-id="7b1d3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b1d3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7b1d3-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="7b1d3-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="7b1d3-131">Указывает часовой пояс для свойств времени в ответ, который может быть в формате UTC, если не указан этот заголовок.</span><span class="sxs-lookup"><span data-stu-id="7b1d3-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="7b1d3-132">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7b1d3-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b1d3-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b1d3-133">Request body</span></span>
<span data-ttu-id="7b1d3-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b1d3-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b1d3-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b1d3-135">Response</span></span>

<span data-ttu-id="7b1d3-136">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [outlookTask](../resources/outlooktask.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7b1d3-136">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7b1d3-137">Пример</span><span class="sxs-lookup"><span data-stu-id="7b1d3-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b1d3-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b1d3-138">Request</span></span>
<span data-ttu-id="7b1d3-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b1d3-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks
```
##### <a name="response"></a><span data-ttu-id="7b1d3-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b1d3-140">Response</span></span>
<span data-ttu-id="7b1d3-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7b1d3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-list-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
