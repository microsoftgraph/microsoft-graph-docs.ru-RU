---
title: Перечисление задач
description: Получение всех задач Outlook в указанной папке.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3e04d42e851fcd6dc37f8251a9c40698de471fab
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458006"
---
# <a name="list-tasks-deprecated"></a><span data-ttu-id="03ca7-103">Список задач (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="03ca7-103">List tasks (deprecated)</span></span>

<span data-ttu-id="03ca7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03ca7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="03ca7-105">Получение всех задач Outlook в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="03ca7-105">Get all the Outlook tasks in the specified folder.</span></span>

<span data-ttu-id="03ca7-106">По умолчанию эта операция (а также операции POST, PATCH и [Complete](../api/outlooktask-complete.md) ) Возвращает свойства, связанные с датами, в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="03ca7-106">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>  <span data-ttu-id="03ca7-107">С помощью `Prefer: outlook.timezone` заголовка запроса можно получить все свойства, связанные с датами, в ответе, представленном в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="03ca7-107">You can use a `Prefer: outlook.timezone` request header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="03ca7-108">[Пример](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) получения одной задачи.</span><span class="sxs-lookup"><span data-stu-id="03ca7-108">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="03ca7-109">Заголовок можно применить точно так же, как и для получения нескольких задач.</span><span class="sxs-lookup"><span data-stu-id="03ca7-109">You can apply the header similarly to get multiple tasks.</span></span>

<span data-ttu-id="03ca7-110">Если имеется несколько групп задач, и вы хотите получить все задачи в определенной группе задач, сначала [получите все папки задач в этой группе задач](outlooktaskgroup-list-taskfolders.md), а затем получите задачи в каждой из этих папок задач.</span><span class="sxs-lookup"><span data-stu-id="03ca7-110">If there is more than one task group, and you want to get all the tasks in a specific task group, first [get all the task folders in that task group](outlooktaskgroup-list-taskfolders.md), and then get the tasks in each of these task folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="03ca7-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03ca7-111">Permissions</span></span>
<span data-ttu-id="03ca7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03ca7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03ca7-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03ca7-114">Permission type</span></span>      | <span data-ttu-id="03ca7-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03ca7-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03ca7-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03ca7-116">Delegated (work or school account)</span></span> | <span data-ttu-id="03ca7-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="03ca7-117">Tasks.Read</span></span>    |
|<span data-ttu-id="03ca7-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03ca7-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03ca7-119">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="03ca7-119">Tasks.Read</span></span>    |
|<span data-ttu-id="03ca7-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03ca7-120">Application</span></span> | <span data-ttu-id="03ca7-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03ca7-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03ca7-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03ca7-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}/tasks
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="03ca7-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="03ca7-123">Optional query parameters</span></span>
<span data-ttu-id="03ca7-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="03ca7-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03ca7-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03ca7-125">Request headers</span></span>
| <span data-ttu-id="03ca7-126">Имя</span><span class="sxs-lookup"><span data-stu-id="03ca7-126">Name</span></span>      |<span data-ttu-id="03ca7-127">Описание</span><span class="sxs-lookup"><span data-stu-id="03ca7-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="03ca7-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03ca7-128">Authorization</span></span>  | <span data-ttu-id="03ca7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03ca7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03ca7-131">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="03ca7-131">Prefer: outlook.timezone</span></span> | <span data-ttu-id="03ca7-132">Задает часовой пояс для свойств времени в отклике в формате UTC, если заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="03ca7-132">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="03ca7-133">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="03ca7-133">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03ca7-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03ca7-134">Request body</span></span>
<span data-ttu-id="03ca7-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03ca7-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03ca7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="03ca7-136">Response</span></span>

<span data-ttu-id="03ca7-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [outlookTask](../resources/outlooktask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03ca7-137">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="03ca7-138">Пример</span><span class="sxs-lookup"><span data-stu-id="03ca7-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03ca7-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="03ca7-139">Request</span></span>
<span data-ttu-id="03ca7-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03ca7-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="03ca7-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="03ca7-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlooktaskfolder_get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks
```
# <a name="c"></a>[<span data-ttu-id="03ca7-142">C#</span><span class="sxs-lookup"><span data-stu-id="03ca7-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlooktaskfolder-get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03ca7-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03ca7-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlooktaskfolder-get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03ca7-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03ca7-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlooktaskfolder-get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="03ca7-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="03ca7-145">Response</span></span>
<span data-ttu-id="03ca7-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03ca7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
