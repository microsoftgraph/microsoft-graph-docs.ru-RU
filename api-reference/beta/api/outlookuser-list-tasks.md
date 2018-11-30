---
title: Перечисление задач
description: Получите все задачи Outlook в почтовом ящике пользователя.
ms.openlocfilehash: df295b40b0813813733b61c2a09b53903cce0d79
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077031"
---
# <a name="list-tasks"></a><span data-ttu-id="01a40-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="01a40-103">List tasks</span></span>

> <span data-ttu-id="01a40-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01a40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01a40-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01a40-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01a40-106">Получите все задачи Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="01a40-106">Get all the Outlook tasks in the user's mailbox.</span></span>

<span data-ttu-id="01a40-107">По умолчанию эта операция (и POST, ИСПРАВЛЕНИЙ и [выполнения](../api/outlooktask-complete.md) операции задачи) возвращает свойства, связанные с даты в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="01a40-107">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="01a40-108">Можно использовать `Prefer: outlook.timezone` заголовок, чтобы все свойства, связанный с данными в ответ, представленного в часовом поясе, отличного от UTC.</span><span class="sxs-lookup"><span data-stu-id="01a40-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="01a40-109">В разделе [Пример](outlooktask-get.md#example-2) для получения одну задачу.</span><span class="sxs-lookup"><span data-stu-id="01a40-109">See an [example](outlooktask-get.md#example-2) for getting a single task.</span></span> <span data-ttu-id="01a40-110">Можно применить заголовок аналогичным образом, чтобы получить несколько задач.</span><span class="sxs-lookup"><span data-stu-id="01a40-110">You can apply the header similarly to get multiple tasks.</span></span> 

## <a name="permissions"></a><span data-ttu-id="01a40-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01a40-111">Permissions</span></span>
<span data-ttu-id="01a40-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01a40-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01a40-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01a40-114">Permission type</span></span>      | <span data-ttu-id="01a40-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01a40-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01a40-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01a40-116">Delegated (work or school account)</span></span> | <span data-ttu-id="01a40-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="01a40-117">Tasks.Read</span></span>    |
|<span data-ttu-id="01a40-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01a40-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01a40-119">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="01a40-119">Tasks.Read</span></span>    |
|<span data-ttu-id="01a40-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01a40-120">Application</span></span> | <span data-ttu-id="01a40-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01a40-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01a40-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01a40-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01a40-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="01a40-123">Optional query parameters</span></span>
<span data-ttu-id="01a40-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="01a40-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01a40-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01a40-125">Request headers</span></span>
| <span data-ttu-id="01a40-126">Имя</span><span class="sxs-lookup"><span data-stu-id="01a40-126">Name</span></span>      |<span data-ttu-id="01a40-127">Описание</span><span class="sxs-lookup"><span data-stu-id="01a40-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="01a40-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01a40-128">Authorization</span></span>  | <span data-ttu-id="01a40-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01a40-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01a40-131">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="01a40-131">Prefer: outlook.timezone</span></span> | <span data-ttu-id="01a40-132">Указывает часовой пояс для свойств времени в ответ, который может быть в формате UTC, если не указан этот заголовок.</span><span class="sxs-lookup"><span data-stu-id="01a40-132">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="01a40-133">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="01a40-133">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01a40-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01a40-134">Request body</span></span>
<span data-ttu-id="01a40-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01a40-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01a40-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="01a40-136">Response</span></span>

<span data-ttu-id="01a40-137">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [outlookTask](../resources/outlooktask.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="01a40-137">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01a40-138">Пример</span><span class="sxs-lookup"><span data-stu-id="01a40-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01a40-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="01a40-139">Request</span></span>
<span data-ttu-id="01a40-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01a40-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/tasks
```
##### <a name="response"></a><span data-ttu-id="01a40-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="01a40-141">Response</span></span>
<span data-ttu-id="01a40-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="01a40-142">Here is an example of the response.</span></span> <span data-ttu-id="01a40-143">По умолчанию свойства даты и времени в ответе возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="01a40-143">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="01a40-p107">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01a40-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List Tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->