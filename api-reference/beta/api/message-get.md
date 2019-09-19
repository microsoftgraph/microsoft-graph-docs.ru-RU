---
title: Вывод сообщения
description: Получение свойств и связей объекта Message.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0746cddf987c6fed21fb27c2e0fffb09b596c520
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036174"
---
# <a name="get-message"></a><span data-ttu-id="f6773-103">Вывод сообщения</span><span class="sxs-lookup"><span data-stu-id="f6773-103">Get message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6773-104">Получение свойств и связей объекта [Message](../resources/message.md) .</span><span class="sxs-lookup"><span data-stu-id="f6773-104">Retrieve the properties and relationships of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="f6773-105">Например, вы можете получить сообщение и развернуть все экземпляры [упоминания](../resources/mention.md) в сообщении.</span><span class="sxs-lookup"><span data-stu-id="f6773-105">For example, you can get a message and expand all the [mention](../resources/mention.md) instances in the message.</span></span>

<span data-ttu-id="f6773-106">Вы можете использовать `$value` параметр для [получения содержимого MIME сообщения](/graph/outlook-get-mime-message).</span><span class="sxs-lookup"><span data-stu-id="f6773-106">You can use the `$value` parameter to [get the MIME content of a message](/graph/outlook-get-mime-message).</span></span>

<span data-ttu-id="f6773-107">Существует два сценария, когда приложение может получить сообщение из папки почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="f6773-107">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="f6773-108">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="f6773-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="f6773-109">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="f6773-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="f6773-110">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="f6773-110">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="f6773-111">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="f6773-111">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="f6773-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6773-112">Permissions</span></span>
<span data-ttu-id="f6773-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6773-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6773-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6773-115">Permission type</span></span>      | <span data-ttu-id="f6773-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6773-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6773-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6773-117">Delegated (work or school account)</span></span> | <span data-ttu-id="f6773-118">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="f6773-118">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="f6773-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6773-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6773-120">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="f6773-120">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="f6773-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6773-121">Application</span></span> | <span data-ttu-id="f6773-122">Mail. ReadBasic. ALL, mail. Read</span><span class="sxs-lookup"><span data-stu-id="f6773-122">Mail.ReadBasic.All, Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6773-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6773-123">HTTP request</span></span>

<span data-ttu-id="f6773-124">Получение указанного сообщения:</span><span class="sxs-lookup"><span data-stu-id="f6773-124">To get the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="f6773-125">Получение содержимого MIME указанного сообщения:</span><span class="sxs-lookup"><span data-stu-id="f6773-125">To get the MIME content of the specified message:</span></span>
<!-- { "blockType": "ignored" } --> 
```http 
GET /me/messages/{id}/$value 
GET /users/{id | userPrincipalName}/messages/{id}/$value 
GET /me/mailFolders/{id}/messages/{id}/$value 
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/$value 
```

<span data-ttu-id="f6773-126">Чтобы получить сообщение и раскрыть все упоминания в сообщении, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="f6773-126">To get a message and expand all mentions in the message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/messages/{id}?$expand=mentions
GET /me/mailFolders/{id}/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}?$expand=mentions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6773-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6773-127">Optional query parameters</span></span>
<span data-ttu-id="f6773-128">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f6773-128">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="f6773-129">Используйте `$value` параметр для получения содержимого MIME сообщения.</span><span class="sxs-lookup"><span data-stu-id="f6773-129">Use the `$value` parameter to get the MIME content of a message.</span></span>

<span data-ttu-id="f6773-130">Используйте параметр `$expand` запроса в свойстве навигации **упоминания** , чтобы получить сообщение с подробными сведениями о каждом [упоминании](../resources/mention.md) в развернутом сообщении.</span><span class="sxs-lookup"><span data-stu-id="f6773-130">Use the `$expand` query parameter on the **mentions** navigation property to get a message with the details of each [mention](../resources/mention.md) in the message expanded.</span></span>



## <a name="request-headers"></a><span data-ttu-id="f6773-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6773-131">Request headers</span></span>
| <span data-ttu-id="f6773-132">Имя</span><span class="sxs-lookup"><span data-stu-id="f6773-132">Name</span></span>       | <span data-ttu-id="f6773-133">Тип</span><span class="sxs-lookup"><span data-stu-id="f6773-133">Type</span></span> | <span data-ttu-id="f6773-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f6773-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f6773-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6773-135">Authorization</span></span>  | <span data-ttu-id="f6773-136">string</span><span class="sxs-lookup"><span data-stu-id="f6773-136">string</span></span>  | <span data-ttu-id="f6773-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6773-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f6773-139">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="f6773-139">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="f6773-140">string</span><span class="sxs-lookup"><span data-stu-id="f6773-140">string</span></span> | <span data-ttu-id="f6773-141">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="f6773-141">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="f6773-142">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="f6773-142">Values can be "text" or "html".</span></span> <span data-ttu-id="f6773-143">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="f6773-143">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="f6773-144">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="f6773-144">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="f6773-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f6773-145">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6773-146">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6773-146">Request body</span></span>
<span data-ttu-id="f6773-147">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6773-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6773-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6773-148">Response</span></span>

<span data-ttu-id="f6773-149">В случае успеха этот метод возвращает код отклика `200 OK` и объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6773-149">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f6773-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="f6773-150">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="f6773-151">Пример 1</span><span class="sxs-lookup"><span data-stu-id="f6773-151">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="f6773-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6773-152">Request</span></span>
<span data-ttu-id="f6773-153">В первом примере показано получение указанного сообщения.</span><span class="sxs-lookup"><span data-stu-id="f6773-153">The first example gets the specified message.</span></span> <span data-ttu-id="f6773-154">Он не задает заголовок, указывающий нужный формат возвращаемого текста.</span><span class="sxs-lookup"><span data-stu-id="f6773-154">It does not specify any header to indicate the desired format of the body to be returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f6773-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6773-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6773-156">C#</span><span class="sxs-lookup"><span data-stu-id="f6773-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6773-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6773-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6773-158">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f6773-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f6773-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6773-159">Response</span></span>
<span data-ttu-id="f6773-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6773-160">Here is an example of the response.</span></span> <span data-ttu-id="f6773-161">Свойства **Body** и **uniqueBody** возвращаются в формате HTML по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6773-161">The **body** and **uniqueBody** properties are returned in the default HTML format.</span></span>
<span data-ttu-id="f6773-162">Note: объект Response, показанный здесь, усекается для краткости.</span><span class="sxs-lookup"><span data-stu-id="f6773-162">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="f6773-163">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6773-163">All of the properties will be returned from an actual call.</span></span>
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


### <a name="example-2"></a><span data-ttu-id="f6773-164">Пример 2</span><span class="sxs-lookup"><span data-stu-id="f6773-164">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="f6773-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6773-165">Request</span></span>
<span data-ttu-id="f6773-166">В следующем примере вошедшего пользователя является дана свопе.</span><span class="sxs-lookup"><span data-stu-id="f6773-166">In the next example, the signed-in user is Dana Swope.</span></span> <span data-ttu-id="f6773-167">В этом примере показано, как получить сведения обо всех упоминаниях в заданном сообщении в почтовом ящике пользователя дана.</span><span class="sxs-lookup"><span data-stu-id="f6773-167">The example shows getting the details of all the mentions in the specified message in Dana's mailbox.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f6773-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6773-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADJmMTUAAAgVZAAAA"],
  "name": "get_mentions_in_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AQMkADJmMTUAAAgVZAAAA/?$expand=mentions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6773-169">C#</span><span class="sxs-lookup"><span data-stu-id="f6773-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mentions-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6773-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6773-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mentions-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6773-171">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f6773-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mentions-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f6773-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6773-172">Response</span></span>
<span data-ttu-id="f6773-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6773-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-3"></a><span data-ttu-id="f6773-176">Пример 3</span><span class="sxs-lookup"><span data-stu-id="f6773-176">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="f6773-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6773-177">Request</span></span>

<span data-ttu-id="f6773-178">В третьем примере показано, как использовать `Prefer: outlook.body-content-type="text"` заголовок для получения **основного текста** и **uniqueBody** указанного сообщения в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="f6773-178">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f6773-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6773-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6773-180">C#</span><span class="sxs-lookup"><span data-stu-id="f6773-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6773-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6773-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6773-182">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f6773-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f6773-183">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6773-183">Response</span></span>

<span data-ttu-id="f6773-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6773-184">Here is an example of the response.</span></span> <span data-ttu-id="f6773-185">Note: ответ содержит `Preference-Applied: outlook.body-content-type` заголовок для подтверждения заголовка `Prefer: outlook.body-content-type` запроса.</span><span class="sxs-lookup"><span data-stu-id="f6773-185">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"

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
### <a name="example-4"></a><span data-ttu-id="f6773-186">Пример 4</span><span class="sxs-lookup"><span data-stu-id="f6773-186">Example 4</span></span>
#### <a name="request"></a><span data-ttu-id="f6773-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6773-187">Request</span></span>

<span data-ttu-id="f6773-188">В четвертом примере показано, как получить заголовки сообщений Интернета для определенного сообщения.</span><span class="sxs-lookup"><span data-stu-id="f6773-188">The fourth example shows how to get the Internet message headers of a specific message.</span></span>  


# <a name="httptabhttp"></a>[<span data-ttu-id="f6773-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6773-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEz"],
  "name": "get_message_internet_headers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGVmMDEz/?$select=internetMessageHeaders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6773-190">C#</span><span class="sxs-lookup"><span data-stu-id="f6773-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-internet-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6773-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6773-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-internet-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6773-192">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f6773-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-internet-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f6773-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6773-193">Response</span></span>

<span data-ttu-id="f6773-194">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6773-194">Here is an example of the response.</span></span> <span data-ttu-id="f6773-195">Note: количество заголовков сообщений в Интернете в объекте Response было сокращено для краткости.</span><span class="sxs-lookup"><span data-stu-id="f6773-195">Note: The number of Internet message headers in the response object has been reduced for brevity.</span></span>

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
      "value":"binary"
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

## <a name="see-also"></a><span data-ttu-id="f6773-196">См. также</span><span class="sxs-lookup"><span data-stu-id="f6773-196">See also</span></span>

- [<span data-ttu-id="f6773-197">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="f6773-197">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f6773-198">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="f6773-198">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f6773-199">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="f6773-199">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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
    "Error: get_message_internet_headers/internetMessageHeaders/member/value:\r\n       Expected type String but actual was Binary. Property: value, actual value: 'binary'"
  ]
}
-->
