---
title: Список сообщений
description: 'Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные"). '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3a29392318de78c1e1ff5bd4ad4b560bc9c460f4
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31518534"
---
# <a name="list-messages"></a><span data-ttu-id="56804-103">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="56804-103">List messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56804-104">Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные").</span><span class="sxs-lookup"><span data-stu-id="56804-104">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="56804-105">В частности, можно фильтровать сообщения и получать только те сообщения, которые содержат упоминание [](../resources/mention.md) пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="56804-105">In particular, you can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span>

<span data-ttu-id="56804-106">Обратите внимание, что по `GET /me/messages` умолчанию операция не возвращает свойство **упоминания** .</span><span class="sxs-lookup"><span data-stu-id="56804-106">Note that by default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="56804-107">Используйте параметр `$expand` запроса для [получения сведений о каждом упоминании в сообщении](../api/message-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="56804-107">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#request-2).</span></span>

<span data-ttu-id="56804-108">Существует два сценария, в которых приложение может получать сообщения в почтовой папке другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="56804-108">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="56804-109">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="56804-109">If the app has application permissions, or,</span></span>
* <span data-ttu-id="56804-110">Если у приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь предоставил доступ к почтовой папке этому пользователю или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="56804-110">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="56804-111">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="56804-111">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="56804-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56804-112">Permissions</span></span>
<span data-ttu-id="56804-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56804-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56804-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56804-115">Permission type</span></span>      | <span data-ttu-id="56804-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56804-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56804-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56804-117">Delegated (work or school account)</span></span> | <span data-ttu-id="56804-118">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56804-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="56804-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56804-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56804-120">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56804-120">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="56804-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56804-121">Application</span></span> | <span data-ttu-id="56804-122">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56804-122">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="56804-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56804-123">HTTP request</span></span>

<span data-ttu-id="56804-124">Для получения всех сообщений в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="56804-124">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="56804-125">Для получения сообщений из определенной папки в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="56804-125">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="56804-126">Для получения всех сообщений в почтовом ящике пользователя, содержащих **упоминание** пользователя:</span><span class="sxs-lookup"><span data-stu-id="56804-126">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56804-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="56804-127">Optional query parameters</span></span>
<span data-ttu-id="56804-128">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="56804-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="56804-129">Вы можете использовать параметр `$filter` запроса для свойства **ментионспревиев** , чтобы получить такие сообщения, которые упоминают пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="56804-129">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56804-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56804-130">Request headers</span></span>
| <span data-ttu-id="56804-131">Имя</span><span class="sxs-lookup"><span data-stu-id="56804-131">Name</span></span>       | <span data-ttu-id="56804-132">Тип</span><span class="sxs-lookup"><span data-stu-id="56804-132">Type</span></span> | <span data-ttu-id="56804-133">Описание</span><span class="sxs-lookup"><span data-stu-id="56804-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="56804-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="56804-134">Authorization</span></span>  | <span data-ttu-id="56804-135">string</span><span class="sxs-lookup"><span data-stu-id="56804-135">string</span></span>  | <span data-ttu-id="56804-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56804-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56804-138">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="56804-138">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="56804-139">string</span><span class="sxs-lookup"><span data-stu-id="56804-139">string</span></span> | <span data-ttu-id="56804-140">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="56804-140">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="56804-141">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="56804-141">Values can be "text" or "html".</span></span> <span data-ttu-id="56804-142">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="56804-142">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="56804-143">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="56804-143">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56804-144">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56804-144">Request body</span></span>
<span data-ttu-id="56804-145">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56804-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56804-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="56804-146">Response</span></span>

<span data-ttu-id="56804-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="56804-147">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="56804-148">Размер страницы по умолчанию для этого запроса предусматривает отображение 10 сообщений.</span><span class="sxs-lookup"><span data-stu-id="56804-148">The default page size for this request is 10 messages.</span></span> 

## <a name="example"></a><span data-ttu-id="56804-149">Пример</span><span class="sxs-lookup"><span data-stu-id="56804-149">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="56804-150">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="56804-150">Request 1</span></span>
<span data-ttu-id="56804-151">В первом примере возвращаются 10 самых популярных сообщений в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="56804-151">The first example gets the top 10 messages in the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages
```
##### <a name="response-1"></a><span data-ttu-id="56804-152">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="56804-152">Response 1</span></span>
<span data-ttu-id="56804-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="56804-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="56804-156">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="56804-156">Request 2</span></span>
<span data-ttu-id="56804-157">В следующем примере выполняется фильтрация всех сообщений в почтовом ящике вошедшего пользователя для тех, которые упоминают пользователя.</span><span class="sxs-lookup"><span data-stu-id="56804-157">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="56804-158">Он используется `$select` для возвращения подмножества свойств каждого сообщения в ответе.</span><span class="sxs-lookup"><span data-stu-id="56804-158">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="56804-159">В этом примере также используются URL-кодировка для пробелов в строке параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="56804-159">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
##### <a name="response-2"></a><span data-ttu-id="56804-160">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="56804-160">Response 2</span></span>
<span data-ttu-id="56804-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="56804-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-3"></a><span data-ttu-id="56804-164">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="56804-164">Request 3</span></span>
<span data-ttu-id="56804-165">В третьем примере показано, как использовать `Prefer: outlook.body-content-type="text"` заголовок для получения свойств **Body** и **uniqueBody** каждого сообщения в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="56804-165">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
##### <a name="response-3"></a><span data-ttu-id="56804-166">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="56804-166">Response 3</span></span>
<span data-ttu-id="56804-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56804-167">Here is an example of the response.</span></span> 

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
<!--
{
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-messages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
