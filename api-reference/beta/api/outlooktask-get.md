---
title: Получение outlookTask
description: Получите свойства и связи задачи Outlook в почтовом ящике пользователя.
localization_priority: Normal
ms.openlocfilehash: f93bc46a1bbe3f7a6c145458606174b6e3a13f1c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822227"
---
# <a name="get-outlooktask"></a><span data-ttu-id="f6098-103">Получение outlookTask</span><span class="sxs-lookup"><span data-stu-id="f6098-103">Get outlookTask</span></span>

> <span data-ttu-id="f6098-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f6098-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6098-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6098-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f6098-106">Получите свойства и связи задачи Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="f6098-106">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="f6098-107">По умолчанию эта операция (и POST, ИСПРАВЛЕНИЙ и [выполнения](../api/outlooktask-complete.md) операции задачи) возвращает свойства, связанные с даты в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="f6098-107">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="f6098-108">Можно использовать `Prefer: outlook.timezone` заголовок, чтобы все свойства, связанный с данными в ответ, представленного в часовом поясе, отличного от UTC.</span><span class="sxs-lookup"><span data-stu-id="f6098-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6098-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6098-109">Permissions</span></span>

<span data-ttu-id="f6098-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6098-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6098-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6098-112">Permission type</span></span>      | <span data-ttu-id="f6098-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6098-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6098-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6098-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f6098-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f6098-115">Tasks.Read</span></span>    |
|<span data-ttu-id="f6098-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6098-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6098-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f6098-117">Tasks.Read</span></span>    |
|<span data-ttu-id="f6098-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6098-118">Application</span></span> | <span data-ttu-id="f6098-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6098-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6098-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6098-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6098-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6098-121">Optional query parameters</span></span>

<span data-ttu-id="f6098-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f6098-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6098-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6098-123">Request headers</span></span>

| <span data-ttu-id="f6098-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f6098-124">Name</span></span>      |<span data-ttu-id="f6098-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f6098-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f6098-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6098-126">Authorization</span></span>  | <span data-ttu-id="f6098-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6098-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f6098-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f6098-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="f6098-130">Указывает часовой пояс для свойств времени в ответ, который может быть в формате UTC, если не указан этот заголовок.</span><span class="sxs-lookup"><span data-stu-id="f6098-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="f6098-131">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f6098-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6098-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6098-132">Request body</span></span>

<span data-ttu-id="f6098-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6098-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6098-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6098-134">Response</span></span>

<span data-ttu-id="f6098-135">Успешно завершена, этот метод возвращает `200 OK` объект [outlookTask](../resources/outlooktask.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f6098-135">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="f6098-136">Пример 1</span><span class="sxs-lookup"><span data-stu-id="f6098-136">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="f6098-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6098-137">Request</span></span>

<span data-ttu-id="f6098-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6098-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTrgAAA=')
```

### <a name="response"></a><span data-ttu-id="f6098-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6098-139">Response</span></span>

<span data-ttu-id="f6098-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f6098-140">Here is an example of the response.</span></span> <span data-ttu-id="f6098-141">По умолчанию свойства даты и времени в ответе возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="f6098-141">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="f6098-142">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="f6098-142">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f6098-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6098-143">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 376

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
```

## <a name="example-2"></a><span data-ttu-id="f6098-144">Пример 2</span><span class="sxs-lookup"><span data-stu-id="f6098-144">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="f6098-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6098-145">Request</span></span>

<span data-ttu-id="f6098-146">В этом примере используется `Prefer: outlook.timezone` заголовка для указания отображение свойства даты и времени в ответ в Тихоокеанское время.</span><span class="sxs-lookup"><span data-stu-id="f6098-146">This example uses the `Prefer: outlook.timezone` header to specify displaying date-time properties in the response in Pacific Standard Time.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MHgwAAA=')
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="f6098-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6098-147">Response</span></span>

<span data-ttu-id="f6098-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6098-148">Here is an example of the response.</span></span> <span data-ttu-id="f6098-149">В указанном Тихоокеанское время отображения свойств даты и времени в ответе.</span><span class="sxs-lookup"><span data-stu-id="f6098-149">The date-time properties in the response are displayed in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="f6098-150">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="f6098-150">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f6098-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6098-151">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 576

{
  "id": "AAMkADA1MHgwAAA=",
  "createdDateTime": "2016-04-22T15:19:18.9526004-07:00",
  "lastModifiedDateTime": "2016-04-22T15:19:19.015101-07:00",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXA==",
  "categories": [ ],
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
  "hasAttachments":false,
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
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
