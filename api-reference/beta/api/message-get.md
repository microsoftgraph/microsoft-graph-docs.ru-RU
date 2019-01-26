---
title: Получение message
description: Извлечение свойств и связи объекта message.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6699a11d11349b50c6ef53ffd17e3b490c4123e2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572523"
---
# <a name="get-message"></a><span data-ttu-id="f43fa-103">Получение message</span><span class="sxs-lookup"><span data-stu-id="f43fa-103">Get message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f43fa-104">Извлечение свойств и связи объекта [message](../resources/message.md) .</span><span class="sxs-lookup"><span data-stu-id="f43fa-104">Retrieve the properties and relationships of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="f43fa-105">К примеру можно получить сообщение и разверните все экземпляры [упомянуть](../resources/mention.md) в сообщении.</span><span class="sxs-lookup"><span data-stu-id="f43fa-105">For example, you can get a message and expand all the [mention](../resources/mention.md) instances in the message.</span></span>

<span data-ttu-id="f43fa-106">Существует два сценария, где приложения можно получить сообщение в почтовой папки другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="f43fa-106">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="f43fa-107">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="f43fa-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="f43fa-108">Если приложение имеет соответствующий делегированных [разрешений](#permissions) от одного пользователя и другой пользователь доступ к папке почты с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="f43fa-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="f43fa-109">В разделе [сведения и примеры](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="f43fa-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="f43fa-110">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="f43fa-110">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="f43fa-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f43fa-111">Permissions</span></span>
<span data-ttu-id="f43fa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f43fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f43fa-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f43fa-114">Permission type</span></span>      | <span data-ttu-id="f43fa-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f43fa-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f43fa-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f43fa-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f43fa-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f43fa-117">Mail.Read</span></span>    |
|<span data-ttu-id="f43fa-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f43fa-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f43fa-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f43fa-119">Mail.Read</span></span>    |
|<span data-ttu-id="f43fa-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f43fa-120">Application</span></span> | <span data-ttu-id="f43fa-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f43fa-121">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f43fa-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f43fa-122">HTTP request</span></span>

<span data-ttu-id="f43fa-123">Для получения указанного сообщения:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="f43fa-123">To get the specified message: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="f43fa-124">Чтобы получить сообщение и разверните все упоминания в сообщении:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="f43fa-124">To get a message and expand all mentions in the message: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/messages/{id}?$expand=mentions
GET /me/mailFolders/{id}/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}?$expand=mentions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f43fa-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f43fa-125">Optional query parameters</span></span>
<span data-ttu-id="f43fa-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f43fa-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f43fa-127">Можно использовать `$expand` были развернуты параметр запроса на **упоминания** свойство навигации для получения сообщений подробные сведения о каждом [упомянуть](../resources/mention.md) в сообщении.</span><span class="sxs-lookup"><span data-stu-id="f43fa-127">You can use the `$expand` query parameter on the **mentions** navigation property to get a message with the details of each [mention](../resources/mention.md) in the message expanded.</span></span>



## <a name="request-headers"></a><span data-ttu-id="f43fa-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f43fa-128">Request headers</span></span>
| <span data-ttu-id="f43fa-129">Имя</span><span class="sxs-lookup"><span data-stu-id="f43fa-129">Name</span></span>       | <span data-ttu-id="f43fa-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f43fa-130">Type</span></span> | <span data-ttu-id="f43fa-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f43fa-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f43fa-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="f43fa-132">Authorization</span></span>  | <span data-ttu-id="f43fa-133">string</span><span class="sxs-lookup"><span data-stu-id="f43fa-133">string</span></span>  | <span data-ttu-id="f43fa-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f43fa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f43fa-136">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="f43fa-136">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="f43fa-137">string</span><span class="sxs-lookup"><span data-stu-id="f43fa-137">string</span></span> | <span data-ttu-id="f43fa-138">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="f43fa-138">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="f43fa-139">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="f43fa-139">Values can be "text" or "html".</span></span> <span data-ttu-id="f43fa-140">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="f43fa-140">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="f43fa-141">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="f43fa-141">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="f43fa-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f43fa-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f43fa-143">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f43fa-143">Request body</span></span>
<span data-ttu-id="f43fa-144">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f43fa-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f43fa-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="f43fa-145">Response</span></span>

<span data-ttu-id="f43fa-146">В случае успеха этот метод возвращает код отклика `200 OK` и объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f43fa-146">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f43fa-147">Пример</span><span class="sxs-lookup"><span data-stu-id="f43fa-147">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="f43fa-148">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="f43fa-148">Request 1</span></span>
<span data-ttu-id="f43fa-149">Первый пример получает указанное сообщение.</span><span class="sxs-lookup"><span data-stu-id="f43fa-149">The first example gets the specified message.</span></span> <span data-ttu-id="f43fa-150">Не указывается любой заголовок для указания нужный формат текста которого требуется получить.</span><span class="sxs-lookup"><span data-stu-id="f43fa-150">It does not specify any header to indicate the desired format of the body to be returned.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGI1AAAoZCfHAAA=')
```
##### <a name="response-1"></a><span data-ttu-id="f43fa-151">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="f43fa-151">Response 1</span></span>
<span data-ttu-id="f43fa-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f43fa-152">Here is an example of the response.</span></span> <span data-ttu-id="f43fa-153">Свойства **body** и **uniqueBody** возвращаются в формате HTML по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f43fa-153">The **body** and **uniqueBody** properties are returned in the default HTML format.</span></span>
<span data-ttu-id="f43fa-154">Примечание: Для краткости усекается объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="f43fa-154">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="f43fa-155">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f43fa-155">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 523

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
    "id":"AAMkAGI1AAAoZCfHAAA=",
    "subject":"Welcome to our group!",
    "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head></head><body><p>Welcome to our group, Dana! Hope you will enjoy working with us </p></body></html>\r\n"
    },
    "uniqueBody":{
        "contentType":"html",
        "content":"<html>\r\n<head></head><body><p>Welcome to our group, Dana! Hope you will enjoy working with us </p></body></html>\r\n"
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="f43fa-156">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="f43fa-156">Request 2</span></span>
<span data-ttu-id="f43fa-157">В следующем примере пользователь выполнил вход — Swope Дану.</span><span class="sxs-lookup"><span data-stu-id="f43fa-157">In the next example, the signed-in user is Dana Swope.</span></span> <span data-ttu-id="f43fa-158">В примере показано получение сведения обо всех упоминания в указанное сообщение в почтовый ящик пользователя Дану.</span><span class="sxs-lookup"><span data-stu-id="f43fa-158">The example shows getting the details of all the mentions in the specified message in Dana's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADJmMTUAAAgVZAAAA"],
  "name": "get_mentions_in_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/('AQMkADJmMTUAAAgVZAAAA')?$expand=mentions
```
##### <a name="response-2"></a><span data-ttu-id="f43fa-159">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="f43fa-159">Response 2</span></span>
<span data-ttu-id="f43fa-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f43fa-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2248

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages/$entity",
  "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
  "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
  "id":"AQMkADJmMTUAAAgVZAAAA",
  "subject":"Start planning soon",
  "body":{
    "contentType":"HTML",
    "content":"<html><head></head><body><p><a href=\"mailto:danas@contoso.onmicrosoft.com\">@Dana Swope</a>,<a href=\"mailto:randiw@contoso.onmicrosoft.com\">@Randi Welch</a>, forgot to mention, I will be away&nbsp;this weekend. I can start on Monday though.</p></body></html>"
  },
  "bodyPreview":"@Dana Swope<mailto:danas@contoso.onmicrosoft.com>, @Randi Welch, forgot to mention, I will be away this weekend. I can start on Monday though.",
  "sender":{
    "emailAddress":{
      "name":"Samantha Booth",
      "address":"samanthab@contoso.onmicrosoft.com"
    }
  },
  "from":{
    "emailAddress":{
      "name":"Samantha Booth",
      "address":"samanthab@contoso.onmicrosoft.com"
    }
  },
  "toRecipients":[
    {
      "emailAddress":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      }
    },
    {
      "emailAddress":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      }
    }
  ],
  "ccRecipients":[
  ],
  "bccRecipients":[
  ],
  "mentionsPreview":{
    "isMentioned":true
  },
  "mentions@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages('AQMkADJmMTUAAAgVZAAAA')/mentions",
  "mentions":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')/mentions('138f4c0a-1130-4776-b780-bf79d73abb3f')",
      "id":"138f4c0a-1130-4776-b780-bf79d73abb3f",
      "mentioned":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-21T07:40:20.152Z",
      "serverCreatedDateTime":"2016-07-21T07:40:20.152Z",
      "deepLink":null,
      "application":null
    },
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')/mentions('7b94df1a-0086-482a-b0da-e62fae12f983')",
      "id":"7b94df1a-0086-482a-b0da-e62fae12f983",
      "mentioned":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-21T07:40:20.158Z",
      "serverCreatedDateTime":"2016-07-21T07:40:20.158Z",
      "deepLink":null,
      "application":null
    }
  ]
}
```


##### <a name="request-3"></a><span data-ttu-id="f43fa-163">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="f43fa-163">Request 3</span></span>

<span data-ttu-id="f43fa-164">Третий пример показано, как использовать `Prefer: outlook.body-content-type="text"` заголовка для получения **uniqueBody** указанного сообщения и **основной текст** в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="f43fa-164">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGI1AAAoZCfHAAA=')?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```

##### <a name="response-3"></a><span data-ttu-id="f43fa-165">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="f43fa-165">Response 3</span></span>

<span data-ttu-id="f43fa-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f43fa-166">Here is an example of the response.</span></span> <span data-ttu-id="f43fa-167">Примечание: Ответ включает `Preference-Applied: outlook.body-content-type` заголовок, чтобы подтвердить `Prefer: outlook.body-content-type` заголовка запроса.</span><span class="sxs-lookup"><span data-stu-id="f43fa-167">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 1550

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)/$entity",
    "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
    "id":"AAMkAGI1AAAoZCfHAAA=",
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
}
```

##### <a name="request-4"></a><span data-ttu-id="f43fa-168">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="f43fa-168">Request 4</span></span>

<span data-ttu-id="f43fa-169">Четвертый примере показано, как получить заголовки сообщений Интернета для конкретного сообщения.</span><span class="sxs-lookup"><span data-stu-id="f43fa-169">The fourth example shows how to get the Internet message headers of a specific message.</span></span>  

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEz"],
  "name": "get_message_internet_headers"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGVmMDEz')?$select=internetMessageHeaders
```

##### <a name="response-4"></a><span data-ttu-id="f43fa-170">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="f43fa-170">Response 4</span></span>

<span data-ttu-id="f43fa-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f43fa-171">Here is an example of the response.</span></span> <span data-ttu-id="f43fa-172">Примечание: Число заголовков сообщений Интернета в объекте ответа были ограничены, для краткости.</span><span class="sxs-lookup"><span data-stu-id="f43fa-172">Note: The number of Internet message headers in the response object has been reduced for brevity.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('48d31887-5fad-4d73-a9f5-3c356e68a038')/messages(internetMessageHeaders)/$entity",
  "@odata.type":"#microsoft.graph.eventMessageRequest",
  "@odata.etag":"W/\"CwAAABYAAAAiIsqMbYjsT5e/T7KzowPTAAAa/qUB\"",
  "id":"AAMkAGVmMDEz",
  "internetMessageHeaders":[
    {
      "name":"Content-Type",
      "value":"application/ms-tnef"
    },
    {
      "name":"Content-Transfer-Encoding",
      "value":"String"
    },
    {
      "name":"Subject",
      "value":"Cloud and Mobile Working Group"
    },
    {
      "name":"x-custom-header-group-name",
      "value":"Washington"
    },
    {
      "name":"x-custom-header-group-id",
      "value":"WA001"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="f43fa-173">См. также</span><span class="sxs-lookup"><span data-stu-id="f43fa-173">See also</span></span>

- [<span data-ttu-id="f43fa-174">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="f43fa-174">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f43fa-175">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="f43fa-175">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f43fa-176">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="f43fa-176">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
