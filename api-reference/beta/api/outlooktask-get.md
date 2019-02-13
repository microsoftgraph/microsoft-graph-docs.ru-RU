---
title: Получение outlookTask
description: Получение свойств и связей задачи Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f140734b6e5fa3e6488b71dbe183a9e3d82fc795
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967293"
---
# <a name="get-outlooktask"></a><span data-ttu-id="e1fab-103">Получение outlookTask</span><span class="sxs-lookup"><span data-stu-id="e1fab-103">Get outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1fab-104">Получение свойств и связей задачи Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="e1fab-104">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="e1fab-105">По умолчанию эта операция (и POST, ИСПРАВЛЕНИЙ и [выполнения](../api/outlooktask-complete.md) операции задачи) возвращает свойства, связанные с даты в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="e1fab-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="e1fab-106">Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="e1fab-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1fab-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1fab-107">Permissions</span></span>

<span data-ttu-id="e1fab-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1fab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1fab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1fab-110">Permission type</span></span>                        | <span data-ttu-id="e1fab-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1fab-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="e1fab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1fab-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1fab-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e1fab-113">Tasks.Read</span></span>                          |
| <span data-ttu-id="e1fab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1fab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1fab-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e1fab-115">Tasks.Read</span></span>                          |
| <span data-ttu-id="e1fab-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1fab-116">Application</span></span>                            | <span data-ttu-id="e1fab-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1fab-117">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="e1fab-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1fab-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1fab-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e1fab-119">Optional query parameters</span></span>

<span data-ttu-id="e1fab-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e1fab-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1fab-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1fab-121">Request headers</span></span>

| <span data-ttu-id="e1fab-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e1fab-122">Name</span></span>                     | <span data-ttu-id="e1fab-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e1fab-123">Description</span></span>                                       |
|:-------------------------|:--------------------------------------------------|
| <span data-ttu-id="e1fab-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1fab-124">Authorization</span></span>            | <span data-ttu-id="e1fab-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1fab-p103">Bearer {token}. Required.</span></span>                         |
| <span data-ttu-id="e1fab-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="e1fab-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="e1fab-128">Указывает часовой пояс для свойств времени в ответ, который может быть в формате UTC, если не указан этот заголовок.</span><span class="sxs-lookup"><span data-stu-id="e1fab-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="e1fab-129">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="e1fab-129">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1fab-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1fab-130">Request body</span></span>

<span data-ttu-id="e1fab-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1fab-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1fab-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1fab-132">Response</span></span>

<span data-ttu-id="e1fab-133">Успешно завершена, этот метод возвращает `200 OK` объект [outlookTask](../resources/outlooktask.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e1fab-133">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1fab-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="e1fab-134">Examples</span></span>

### <a name="example-1-get-an-outlook-task"></a><span data-ttu-id="e1fab-135">В примере 1: Получение задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="e1fab-135">Example 1: Get an Outlook task</span></span>

#### <a name="request"></a><span data-ttu-id="e1fab-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1fab-136">Request</span></span>

<span data-ttu-id="e1fab-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1fab-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTrgAAA=')
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="e1fab-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1fab-138">Response</span></span>

<span data-ttu-id="e1fab-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e1fab-139">Here is an example of the response.</span></span> <span data-ttu-id="e1fab-140">По умолчанию свойства даты и времени в ответе возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="e1fab-140">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="e1fab-141">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="e1fab-141">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e1fab-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1fab-142">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time"></a><span data-ttu-id="e1fab-143">Пример 2: Получение задачи Outlook с помощью свойства даты и времени в Тихоокеанское время</span><span class="sxs-lookup"><span data-stu-id="e1fab-143">Example 2: Get Outlook task with date-time properties in Pacific Standard Time</span></span>

#### <a name="request"></a><span data-ttu-id="e1fab-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1fab-144">Request</span></span>

<span data-ttu-id="e1fab-145">В этом примере используется `Prefer: outlook.timezone` заголовок, чтобы указать, что API должен возвращать свойства даты и времени в ответ в Тихоокеанское время.</span><span class="sxs-lookup"><span data-stu-id="e1fab-145">This example uses the `Prefer: outlook.timezone` header to specify that the API should return date-time properties in the response in Pacific Standard Time.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MHgwAAA=')
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="e1fab-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1fab-146">Response</span></span>

<span data-ttu-id="e1fab-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1fab-147">Here is an example of the response.</span></span> <span data-ttu-id="e1fab-148">Свойства даты и времени в ответе возвращаются в указанном Тихоокеанское время.</span><span class="sxs-lookup"><span data-stu-id="e1fab-148">The date-time properties in the response are returned in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="e1fab-149">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="e1fab-149">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e1fab-150">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1fab-150">All of the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/outlooktask-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
