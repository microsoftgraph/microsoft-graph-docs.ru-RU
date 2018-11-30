---
title: Список сообщений
description: 'Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные"). '
ms.openlocfilehash: 6647b1c171bc415844d5154438469122161487eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080565"
---
# <a name="list-messages"></a><span data-ttu-id="a202e-103">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="a202e-103">List messages</span></span>

> <span data-ttu-id="a202e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a202e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a202e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a202e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a202e-106">Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные").</span><span class="sxs-lookup"><span data-stu-id="a202e-106">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="a202e-107">В частности можно отфильтровать сообщения и получить только те, которые включают [упомянуть](../resources/mention.md) о пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="a202e-107">In particular, you can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span>

<span data-ttu-id="a202e-108">Обратите внимание, что по умолчанию `GET /me/messages` операция не возвращает свойство **упоминания** .</span><span class="sxs-lookup"><span data-stu-id="a202e-108">Note that by default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="a202e-109">Использование `$expand` параметр, чтобы [Найти сведения о каждом упоминаются в сообщении](../api/message-get.md#request-2)запроса.</span><span class="sxs-lookup"><span data-stu-id="a202e-109">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#request-2).</span></span>

<span data-ttu-id="a202e-110">Существует два сценария, где приложения можно получить сообщения в почтовой папки другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a202e-110">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="a202e-111">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="a202e-111">If the app has application permissions, or,</span></span>
* <span data-ttu-id="a202e-112">Если приложение имеет соответствующий делегированных [разрешений](#permissions) от одного пользователя и другой пользователь доступ к папке почты с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="a202e-112">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="a202e-113">В разделе [сведения и примеры](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="a202e-113">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="a202e-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a202e-114">Permissions</span></span>
<span data-ttu-id="a202e-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a202e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a202e-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a202e-117">Permission type</span></span>      | <span data-ttu-id="a202e-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a202e-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a202e-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a202e-119">Delegated (work or school account)</span></span> | <span data-ttu-id="a202e-120">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a202e-120">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a202e-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a202e-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a202e-122">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a202e-122">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a202e-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a202e-123">Application</span></span> | <span data-ttu-id="a202e-124">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a202e-124">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a202e-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a202e-125">HTTP request</span></span>

<span data-ttu-id="a202e-126">Для получения всех сообщений в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="a202e-126">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="a202e-127">Для получения сообщений из определенной папки в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="a202e-127">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="a202e-128">Чтобы получить все сообщения в почтовом ящике пользователя, включающую **упомянуть** о пользователя:</span><span class="sxs-lookup"><span data-stu-id="a202e-128">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a202e-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a202e-129">Optional query parameters</span></span>
<span data-ttu-id="a202e-130">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a202e-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a202e-131">Можно использовать `$filter` параметр на **mentionsPreview** свойство, позволяющее получить сообщения, упомянуть пользователь выполнил вход запроса.</span><span class="sxs-lookup"><span data-stu-id="a202e-131">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a202e-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a202e-132">Request headers</span></span>
| <span data-ttu-id="a202e-133">Имя</span><span class="sxs-lookup"><span data-stu-id="a202e-133">Name</span></span>       | <span data-ttu-id="a202e-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a202e-134">Type</span></span> | <span data-ttu-id="a202e-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a202e-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a202e-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="a202e-136">Authorization</span></span>  | <span data-ttu-id="a202e-137">string</span><span class="sxs-lookup"><span data-stu-id="a202e-137">string</span></span>  | <span data-ttu-id="a202e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a202e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a202e-140">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="a202e-140">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="a202e-141">string</span><span class="sxs-lookup"><span data-stu-id="a202e-141">string</span></span> | <span data-ttu-id="a202e-142">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="a202e-142">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="a202e-143">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="a202e-143">Values can be "text" or "html".</span></span> <span data-ttu-id="a202e-144">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="a202e-144">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="a202e-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a202e-145">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a202e-146">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a202e-146">Request body</span></span>
<span data-ttu-id="a202e-147">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a202e-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a202e-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="a202e-148">Response</span></span>

<span data-ttu-id="a202e-149">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [сообщения](../resources/message.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a202e-149">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="a202e-150">Размер страницы по умолчанию для этого запроса предусматривает отображение 10 сообщений.</span><span class="sxs-lookup"><span data-stu-id="a202e-150">The default page size for this request is 10 messages.</span></span> 

## <a name="example"></a><span data-ttu-id="a202e-151">Пример</span><span class="sxs-lookup"><span data-stu-id="a202e-151">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="a202e-152">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="a202e-152">Request 1</span></span>
<span data-ttu-id="a202e-153">Первый пример возвращает верхней 10 сообщений в почтовый ящик пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="a202e-153">The first example gets the top 10 messages in the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages
```
##### <a name="response-1"></a><span data-ttu-id="a202e-154">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="a202e-154">Response 1</span></span>
<span data-ttu-id="a202e-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a202e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "2016-10-19T10:37:00Z",
      "sentDateTime": "2016-10-19T10:37:00Z",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```


##### <a name="request-2"></a><span data-ttu-id="a202e-158">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="a202e-158">Request 2</span></span>
<span data-ttu-id="a202e-159">Следующий пример фильтр все сообщения в почтовом ящике пользователь выполнил вход для тех, содержащие упоминание пользователя.</span><span class="sxs-lookup"><span data-stu-id="a202e-159">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="a202e-160">Он использует `$select` для возврата подмножество свойств каждого сообщения в ответе.</span><span class="sxs-lookup"><span data-stu-id="a202e-160">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="a202e-161">Пример также включает в себя URL-адрес, кодировка символов пространства в параметр строки запроса.</span><span class="sxs-lookup"><span data-stu-id="a202e-161">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
##### <a name="response-2"></a><span data-ttu-id="a202e-162">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="a202e-162">Response 2</span></span>
<span data-ttu-id="a202e-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a202e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 987

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages(subject,sender,receivedDateTime,mentionsPreview)",
  "value":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
      "id":"AQMkADJmMTUAAAgVZAAAA",
      "receivedDateTime":"2016-07-21T07:40:21Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    },
    {
      "@odata.id":"https://graph.microsoft.com/beta/Users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/Messages('AQMkADJmMTUAAAjwVAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAEGj\"",
      "id":"AQMkADJmMTUAAAjwVAAAA",
      "receivedDateTime":"2016-07-21T07:40:20Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    }
  ]
}
```

##### <a name="request-3"></a><span data-ttu-id="a202e-166">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="a202e-166">Request 3</span></span>
<span data-ttu-id="a202e-167">Третий пример показано, как использовать `Prefer: outlook.body-content-type="text"` заголовка для получения свойства **body** и **uniqueBody** каждого сообщения в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="a202e-167">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
##### <a name="response-3"></a><span data-ttu-id="a202e-168">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="a202e-168">Response 3</span></span>
<span data-ttu-id="a202e-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a202e-169">Here is an example of the response.</span></span> 

<!--
Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.
-->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2704

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)",
    "value":[
        {
            "@odata.type":"#microsoft.graph.eventMessageRequest",
            "@odata.etag":"W/\"CwAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj5\"",
            "id":"AAMkAGIAAAoZCfIAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
            "id":"AAMkAGIAAAoZCfHAAA=",
            "subject":"Welcome to our group!",
            "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nTh",
            "body":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nThanks!\r\n\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\nThanks!\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAAAAjr\"",
            "id":"AQMkAGIAAAIJTQAAAA==",
            "subject":"Welcome aboard!",
            "bodyPreview":"Welcome to the Support group!",
            "body":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
