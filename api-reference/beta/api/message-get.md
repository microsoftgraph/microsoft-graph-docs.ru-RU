---
title: Вывод сообщения
description: Получение свойств и связей объекта Message.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 20a68ed4448c8762217ba0d37d368af63d58c8e9
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869467"
---
# <a name="get-message"></a><span data-ttu-id="49fd1-103">Вывод сообщения</span><span class="sxs-lookup"><span data-stu-id="49fd1-103">Get message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49fd1-104">Получение свойств и связей объекта [Message](../resources/message.md) .</span><span class="sxs-lookup"><span data-stu-id="49fd1-104">Retrieve the properties and relationships of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="49fd1-105">Например, вы можете получить сообщение и развернуть все экземпляры [упоминания](../resources/mention.md) в сообщении.</span><span class="sxs-lookup"><span data-stu-id="49fd1-105">For example, you can get a message and expand all the [mention](../resources/mention.md) instances in the message.</span></span>

<span data-ttu-id="49fd1-106">Вы можете использовать параметр `$value`, чтобы [получить MIME-содержимое сообщения](/graph/outlook-get-mime-message).</span><span class="sxs-lookup"><span data-stu-id="49fd1-106">You can use the `$value` parameter to [get the MIME content of a message](/graph/outlook-get-mime-message).</span></span>

<span data-ttu-id="49fd1-107">Существует два сценария, когда приложение может получить сообщение из папки почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="49fd1-107">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="49fd1-108">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="49fd1-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="49fd1-109">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="49fd1-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="49fd1-110">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="49fd1-110">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="49fd1-111">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="49fd1-111">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="49fd1-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49fd1-112">Permissions</span></span>
<span data-ttu-id="49fd1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49fd1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49fd1-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49fd1-115">Permission type</span></span>      | <span data-ttu-id="49fd1-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49fd1-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49fd1-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49fd1-117">Delegated (work or school account)</span></span> | <span data-ttu-id="49fd1-118">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="49fd1-118">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="49fd1-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49fd1-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49fd1-120">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="49fd1-120">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="49fd1-121">Для приложения</span><span class="sxs-lookup"><span data-stu-id="49fd1-121">Application</span></span> | <span data-ttu-id="49fd1-122">Mail.ReadBasic.All, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="49fd1-122">Mail.ReadBasic.All, Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="49fd1-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49fd1-123">HTTP request</span></span>

<span data-ttu-id="49fd1-124">Получение указанного сообщения:</span><span class="sxs-lookup"><span data-stu-id="49fd1-124">To get the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="49fd1-125">Получение содержимого MIME указанного сообщения:</span><span class="sxs-lookup"><span data-stu-id="49fd1-125">To get the MIME content of the specified message:</span></span>
<!-- { "blockType": "ignored" } --> 
```http 
GET /me/messages/{id}/$value 
GET /users/{id | userPrincipalName}/messages/{id}/$value 
GET /me/mailFolders/{id}/messages/{id}/$value 
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/$value 
```

<span data-ttu-id="49fd1-126">Чтобы получить сообщение и раскрыть все упоминания в сообщении, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="49fd1-126">To get a message and expand all mentions in the message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/messages/{id}?$expand=mentions
GET /me/mailFolders/{id}/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}?$expand=mentions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49fd1-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="49fd1-127">Optional query parameters</span></span>
<span data-ttu-id="49fd1-128">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="49fd1-128">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="49fd1-129">Используйте `$value` параметр для получения содержимого MIME сообщения.</span><span class="sxs-lookup"><span data-stu-id="49fd1-129">Use the `$value` parameter to get the MIME content of a message.</span></span>

<span data-ttu-id="49fd1-130">Используйте параметр `$expand` запроса в свойстве навигации **упоминания** , чтобы получить сообщение с подробными сведениями о каждом [упоминании](../resources/mention.md) в развернутом сообщении.</span><span class="sxs-lookup"><span data-stu-id="49fd1-130">Use the `$expand` query parameter on the **mentions** navigation property to get a message with the details of each [mention](../resources/mention.md) in the message expanded.</span></span>



## <a name="request-headers"></a><span data-ttu-id="49fd1-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49fd1-131">Request headers</span></span>
| <span data-ttu-id="49fd1-132">Имя</span><span class="sxs-lookup"><span data-stu-id="49fd1-132">Name</span></span>       | <span data-ttu-id="49fd1-133">Тип</span><span class="sxs-lookup"><span data-stu-id="49fd1-133">Type</span></span> | <span data-ttu-id="49fd1-134">Описание</span><span class="sxs-lookup"><span data-stu-id="49fd1-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="49fd1-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="49fd1-135">Authorization</span></span>  | <span data-ttu-id="49fd1-136">string</span><span class="sxs-lookup"><span data-stu-id="49fd1-136">string</span></span>  | <span data-ttu-id="49fd1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49fd1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49fd1-139">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="49fd1-139">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="49fd1-140">string</span><span class="sxs-lookup"><span data-stu-id="49fd1-140">string</span></span> | <span data-ttu-id="49fd1-141">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="49fd1-141">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="49fd1-142">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="49fd1-142">Values can be "text" or "html".</span></span> <span data-ttu-id="49fd1-143">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="49fd1-143">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="49fd1-144">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="49fd1-144">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="49fd1-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="49fd1-145">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49fd1-146">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="49fd1-146">Request body</span></span>
<span data-ttu-id="49fd1-147">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49fd1-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49fd1-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="49fd1-148">Response</span></span>

<span data-ttu-id="49fd1-149">В случае успеха этот метод возвращает код отклика `200 OK` и объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49fd1-149">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="49fd1-150">Указание `$value` параметра возвращает содержимое сообщения в формате MIME, а не в ресурсе **Message** .</span><span class="sxs-lookup"><span data-stu-id="49fd1-150">Specifying the `$value` parameter returns the message content in MIME format, and not a **message** resource.</span></span>

## <a name="examples"></a><span data-ttu-id="49fd1-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="49fd1-151">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="49fd1-152">Пример 1</span><span class="sxs-lookup"><span data-stu-id="49fd1-152">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="49fd1-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="49fd1-153">Request</span></span>
<span data-ttu-id="49fd1-154">В первом примере показано получение указанного сообщения.</span><span class="sxs-lookup"><span data-stu-id="49fd1-154">The first example gets the specified message.</span></span> <span data-ttu-id="49fd1-155">Он не задает заголовок, указывающий нужный формат возвращаемого текста.</span><span class="sxs-lookup"><span data-stu-id="49fd1-155">It does not specify any header to indicate the desired format of the body to be returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="49fd1-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="49fd1-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49fd1-157">C#</span><span class="sxs-lookup"><span data-stu-id="49fd1-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49fd1-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49fd1-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49fd1-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49fd1-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="49fd1-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="49fd1-160">Response</span></span>
<span data-ttu-id="49fd1-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49fd1-161">Here is an example of the response.</span></span> <span data-ttu-id="49fd1-162">Свойства **Body** и **uniqueBody** возвращаются в формате HTML по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="49fd1-162">The **body** and **uniqueBody** properties are returned in the default HTML format.</span></span>
<span data-ttu-id="49fd1-163">Note: объект Response, показанный здесь, усекается для краткости.</span><span class="sxs-lookup"><span data-stu-id="49fd1-163">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="49fd1-164">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49fd1-164">All of the properties will be returned from an actual call.</span></span>
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


### <a name="example-2"></a><span data-ttu-id="49fd1-165">Пример 2</span><span class="sxs-lookup"><span data-stu-id="49fd1-165">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="49fd1-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="49fd1-166">Request</span></span>
<span data-ttu-id="49fd1-167">В следующем примере вошедшего пользователя является дана свопе.</span><span class="sxs-lookup"><span data-stu-id="49fd1-167">In the next example, the signed-in user is Dana Swope.</span></span> <span data-ttu-id="49fd1-168">В этом примере показано, как получить сведения обо всех упоминаниях в заданном сообщении в почтовом ящике пользователя дана.</span><span class="sxs-lookup"><span data-stu-id="49fd1-168">The example shows getting the details of all the mentions in the specified message in Dana's mailbox.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="49fd1-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="49fd1-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADJmMTUAAAgVZAAAA"],
  "name": "get_mentions_in_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AQMkADJmMTUAAAgVZAAAA/?$expand=mentions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49fd1-170">C#</span><span class="sxs-lookup"><span data-stu-id="49fd1-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mentions-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49fd1-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49fd1-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mentions-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49fd1-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49fd1-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mentions-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="49fd1-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="49fd1-173">Response</span></span>
<span data-ttu-id="49fd1-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49fd1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-3"></a><span data-ttu-id="49fd1-177">Пример 3</span><span class="sxs-lookup"><span data-stu-id="49fd1-177">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="49fd1-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="49fd1-178">Request</span></span>

<span data-ttu-id="49fd1-179">В третьем примере показано, как использовать заголовок `Prefer: outlook.body-content-type="text"`, чтобы получить свойства **body** и **uniqueBody** указанного сообщения в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="49fd1-179">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="49fd1-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="49fd1-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49fd1-181">C#</span><span class="sxs-lookup"><span data-stu-id="49fd1-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49fd1-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49fd1-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49fd1-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49fd1-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="49fd1-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="49fd1-184">Response</span></span>

<span data-ttu-id="49fd1-185">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49fd1-185">Here is an example of the response.</span></span> <span data-ttu-id="49fd1-186">Примечание. Отклик включает заголовок `Preference-Applied: outlook.body-content-type`, подтверждающий заголовок запроса `Prefer: outlook.body-content-type`.</span><span class="sxs-lookup"><span data-stu-id="49fd1-186">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
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
### <a name="example-4"></a><span data-ttu-id="49fd1-187">Пример 4</span><span class="sxs-lookup"><span data-stu-id="49fd1-187">Example 4</span></span>
#### <a name="request"></a><span data-ttu-id="49fd1-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="49fd1-188">Request</span></span>

<span data-ttu-id="49fd1-189">В четвертом примере показано, как получить заголовки сообщений Интернета для определенного сообщения.</span><span class="sxs-lookup"><span data-stu-id="49fd1-189">The fourth example shows how to get the Internet message headers of a specific message.</span></span>  


# <a name="httptabhttp"></a>[<span data-ttu-id="49fd1-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="49fd1-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEz"],
  "name": "get_message_internet_headers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGVmMDEz/?$select=internetMessageHeaders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49fd1-191">C#</span><span class="sxs-lookup"><span data-stu-id="49fd1-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-internet-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49fd1-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49fd1-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-internet-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49fd1-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49fd1-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-internet-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="49fd1-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="49fd1-194">Response</span></span>

<span data-ttu-id="49fd1-195">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49fd1-195">Here is an example of the response.</span></span> <span data-ttu-id="49fd1-196">Note: количество заголовков сообщений в Интернете в объекте Response было сокращено для краткости.</span><span class="sxs-lookup"><span data-stu-id="49fd1-196">Note: The number of Internet message headers in the response object has been reduced for brevity.</span></span>

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


### <a name="example-5"></a><span data-ttu-id="49fd1-197">Пример 5</span><span class="sxs-lookup"><span data-stu-id="49fd1-197">Example 5</span></span>
#### <a name="request"></a><span data-ttu-id="49fd1-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="49fd1-198">Request</span></span>
<span data-ttu-id="49fd1-199">В пятом примере показано получение содержимого MIME сообщения в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="49fd1-199">The fifth example gets the MIME content of a message in the signed-in user's mailbox.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/4aade2547798441eab5188a7a2436bc1/$value
```

#### <a name="response"></a><span data-ttu-id="49fd1-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="49fd1-200">Response</span></span>
<span data-ttu-id="49fd1-201">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="49fd1-201">The following is the response.</span></span> <span data-ttu-id="49fd1-202">Содержимое MIME начинается с заголовка `MIME-Version`.</span><span class="sxs-lookup"><span data-stu-id="49fd1-202">The MIME content begins with the `MIME-Version` header.</span></span> 
<!-- {
  "blockType": "ignored"
} -->
```http
HTTP/1.1 200 OK

Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0 via Mailbox 
Transport; Mon, 4 Sep 2017 03:00:08 -0700 
Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0; Mon, 4 Sep 
2017 03:00:07 -0700 
Received: from contoso.com 
(fe80::5bf:5059:4ca0:5017) by contoso.com 
(fe80::5bf:5059:4ca0:5017%12) with mapi id 15.01.1374.000; Mon, 4 Sep 2017 
03:00:01 -0700 
From: Administrator <admin@contoso.com> 
To: Administrator <admin@contoso.com> 
Subject: This email has attachment. 
Thread-Topic: This email has attachment. 
Thread-Index: AQHTJWSHSywMzSz8o0OJud48nG50GQ== 
Date: Mon, 4 Sep 2017 10:00:00 +0000 
Message-ID: 
                <4aade2547798441eab5188a7a2436bc1@contoso.com> 
Accept-Language: en-US 
Content-Language: en-US 
X-MS-Exchange-Organization-AuthAs: Internal 
X-MS-Exchange-Organization-AuthMechanism: 04 
X-MS-Exchange-Organization-AuthSource: 
                contoso.com 
X-MS-Has-Attach: yes 
X-MS-Exchange-Organization-Network-Message-Id: 
                0ffdb402-ec03-42c8-5d32-08d4f37bb517 
X-MS-Exchange-Organization-SCL: -1 
X-MS-TNEF-Correlator: 
X-MS-Exchange-Organization-RecordReviewCfmType: 0 
x-ms-publictraffictype: Emai

```http
MIME-Version: 1.0 
Content-Type: multipart/mixed; 
                boundary="_004_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: multipart/alternative; 
                boundary="_000_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/plain; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
The attachment is an email. 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/html; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
<html> 
<head> 
<meta http-equiv=3D"Content-Type" content=3D"text/html; charset=3Diso-8859-= 
1"> 
<style type=3D"text/css" style=3D"display:none;"><!-- P {margin-top:0;margi= 
n-bottom:0;} --></style> 
</head> 
<body dir=3D"ltr"> 
<div id=3D"divtagdefaultwrapper" style=3D"font-size:12pt;color:#000000;font= 
-family:Calibri,Helvetica,sans-serif;" dir=3D"ltr"> 
<p>The attachment is an email.</p> 
</div> 
</body> 
</html> 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_-- 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: application/octet-stream; name="Attachment email.eml" 
Content-Description: Attachment email.eml 
Content-Disposition: attachment; filename="Attachment email.eml"; size=408; 
                creation-date="Mon, 04 Sep 2017 09:59:43 GMT"; 
                modification-date="Mon, 04 Sep 2017 09:59:43 GMT" 
Content-Transfer-Encoding: base64 
 
RnJvbToJQWRtaW5pc3RyYXRvciA8YWRtaW5AdGVuYW50LUVYSEItMTQ3MS5jb20+DQpTZW50OglN 
b25kYXksIFNlcHRlbWJlciA0LCAyMDE3IDM6MjYgUE0NClRvOglTcml2YXJkaGFuIEhlYmJhcg0K 
U3ViamVjdDoJQXR0YWNobWVudCBlbWFpbA0KDQpJIHdpbGwgYXR0YWNoIHRoaXMgZW1haWwgdG8g 
YW5vdGhlciBtYWlsLg0K 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_-- 
```


## <a name="see-also"></a><span data-ttu-id="49fd1-203">См. также</span><span class="sxs-lookup"><span data-stu-id="49fd1-203">See also</span></span>

- [<span data-ttu-id="49fd1-204">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="49fd1-204">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="49fd1-205">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="49fd1-205">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="49fd1-206">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="49fd1-206">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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
