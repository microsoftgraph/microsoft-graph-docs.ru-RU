---
title: Вывод сообщения
description: Извлечение свойств и связей объекта сообщения.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a727179016a5352a55d0923dfcd5ac5834f73d84
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050159"
---
# <a name="get-message"></a><span data-ttu-id="44761-103">Вывод сообщения</span><span class="sxs-lookup"><span data-stu-id="44761-103">Get message</span></span>

<span data-ttu-id="44761-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44761-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44761-105">Извлечение свойств и связей объекта [сообщения.](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="44761-105">Retrieve the properties and relationships of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="44761-106">Например, вы можете получить сообщение и расширить все [экземпляры](../resources/mention.md) упоминания в сообщении.</span><span class="sxs-lookup"><span data-stu-id="44761-106">For instance, you can get a message and expand all the [mention](../resources/mention.md) instances in the message.</span></span> <span data-ttu-id="44761-107">См. [пример](#example-2-get-all-mentions-in-a-specific-message) ниже.</span><span class="sxs-lookup"><span data-stu-id="44761-107">See an [example](#example-2-get-all-mentions-in-a-specific-message) below.</span></span>

<span data-ttu-id="44761-108">Вы можете использовать параметр `$value`, чтобы [получить MIME-содержимое сообщения](/graph/outlook-get-mime-message).</span><span class="sxs-lookup"><span data-stu-id="44761-108">You can use the `$value` parameter to [get the MIME content of a message](/graph/outlook-get-mime-message).</span></span> <span data-ttu-id="44761-109">Также см. [пример](#example-5-get-mime-content) ниже.</span><span class="sxs-lookup"><span data-stu-id="44761-109">See also an [example](#example-5-get-mime-content) below.</span></span>

<span data-ttu-id="44761-110">Существует два сценария, когда приложение может получить сообщение из папки почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="44761-110">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="44761-111">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="44761-111">If the app has application permissions, or,</span></span>
* <span data-ttu-id="44761-112">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="44761-112">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="44761-113">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="44761-113">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="44761-114">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="44761-114">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="44761-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44761-115">Permissions</span></span>
<span data-ttu-id="44761-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44761-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44761-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44761-118">Permission type</span></span>      | <span data-ttu-id="44761-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44761-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44761-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44761-120">Delegated (work or school account)</span></span> | <span data-ttu-id="44761-121">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="44761-121">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="44761-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44761-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44761-123">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="44761-123">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="44761-124">Для приложения</span><span class="sxs-lookup"><span data-stu-id="44761-124">Application</span></span> | <span data-ttu-id="44761-125">Mail.ReadBasic.All, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="44761-125">Mail.ReadBasic.All, Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="44761-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44761-126">HTTP request</span></span>

<span data-ttu-id="44761-127">Для получения указанного сообщения:</span><span class="sxs-lookup"><span data-stu-id="44761-127">To get the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="44761-128">Для получения MIME-содержимого указанного сообщения:</span><span class="sxs-lookup"><span data-stu-id="44761-128">To get the MIME content of the specified message:</span></span>
<!-- { "blockType": "ignored" } --> 
```http 
GET /me/messages/{id}/$value 
GET /users/{id | userPrincipalName}/messages/{id}/$value 
GET /me/mailFolders/{id}/messages/{id}/$value 
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/$value 
```

<span data-ttu-id="44761-129">Чтобы получить сообщение и расширить все упоминания в сообщении:</span><span class="sxs-lookup"><span data-stu-id="44761-129">To get a message and expand all mentions in the message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/messages/{id}?$expand=mentions
GET /me/mailFolders/{id}/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}?$expand=mentions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44761-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="44761-130">Optional query parameters</span></span>
<span data-ttu-id="44761-131">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="44761-131">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="44761-132">Используйте параметр `$value`, чтобы получить MIME-содержимое сообщения.</span><span class="sxs-lookup"><span data-stu-id="44761-132">Use the `$value` parameter to get the MIME content of a message.</span></span>

<span data-ttu-id="44761-133">Используйте параметр запроса в свойстве навигации упоминаний, чтобы получить сообщение с подробными сведениями о каждом упоминаемом в `$expand` расширенном сообщении.  [](../resources/mention.md)</span><span class="sxs-lookup"><span data-stu-id="44761-133">Use the `$expand` query parameter on the **mentions** navigation property to get a message with the details of each [mention](../resources/mention.md) in the message expanded.</span></span>



## <a name="request-headers"></a><span data-ttu-id="44761-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44761-134">Request headers</span></span>
| <span data-ttu-id="44761-135">Имя</span><span class="sxs-lookup"><span data-stu-id="44761-135">Name</span></span>       | <span data-ttu-id="44761-136">Тип</span><span class="sxs-lookup"><span data-stu-id="44761-136">Type</span></span> | <span data-ttu-id="44761-137">Описание</span><span class="sxs-lookup"><span data-stu-id="44761-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="44761-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="44761-138">Authorization</span></span>  | <span data-ttu-id="44761-139">string</span><span class="sxs-lookup"><span data-stu-id="44761-139">string</span></span>  | <span data-ttu-id="44761-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44761-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="44761-142">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="44761-142">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="44761-143">string</span><span class="sxs-lookup"><span data-stu-id="44761-143">string</span></span> | <span data-ttu-id="44761-144">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="44761-144">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="44761-145">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="44761-145">Values can be "text" or "html".</span></span> <span data-ttu-id="44761-146">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="44761-146">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="44761-147">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="44761-147">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="44761-148">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="44761-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44761-149">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44761-149">Request body</span></span>
<span data-ttu-id="44761-150">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44761-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44761-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="44761-151">Response</span></span>

<span data-ttu-id="44761-152">В случае успеха этот метод возвращает код отклика `200 OK` и объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44761-152">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="44761-153">При указании параметра `$value` возвращается содержимое сообщения в формате MIME, а не ресурс **message**.</span><span class="sxs-lookup"><span data-stu-id="44761-153">Specifying the `$value` parameter returns the message content in MIME format, and not a **message** resource.</span></span>

## <a name="examples"></a><span data-ttu-id="44761-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="44761-154">Examples</span></span>
### <a name="example-1-get-a-specific-message"></a><span data-ttu-id="44761-155">Пример 1. Получение определенного сообщения</span><span class="sxs-lookup"><span data-stu-id="44761-155">Example 1: Get a specific message</span></span>
#### <a name="request"></a><span data-ttu-id="44761-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="44761-156">Request</span></span>
<span data-ttu-id="44761-157">В первом примере получается указанное сообщение.</span><span class="sxs-lookup"><span data-stu-id="44761-157">The first example gets the specified message.</span></span> <span data-ttu-id="44761-158">Он не указывает какой-либо заголовок, чтобы указать нужный формат тела, который будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="44761-158">It does not specify any header to indicate the desired format of the body to be returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="44761-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="44761-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=
```
# <a name="c"></a>[<span data-ttu-id="44761-160">C#</span><span class="sxs-lookup"><span data-stu-id="44761-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44761-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44761-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44761-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44761-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44761-163">Java</span><span class="sxs-lookup"><span data-stu-id="44761-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="44761-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="44761-164">Response</span></span>
<span data-ttu-id="44761-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44761-165">Here is an example of the response.</span></span> <span data-ttu-id="44761-166">Свойства **body** и **uniqueBody** возвращаются в формате HTML по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="44761-166">The **body** and **uniqueBody** properties are returned in the default HTML format.</span></span>
<span data-ttu-id="44761-167">Примечание. Показанный здесь объект ответа усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="44761-167">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="44761-168">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44761-168">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_message",
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


### <a name="example-2-get-all-mentions-in-a-specific-message"></a><span data-ttu-id="44761-169">Пример 2. Получить все упоминания в определенном сообщении</span><span class="sxs-lookup"><span data-stu-id="44761-169">Example 2: Get all mentions in a specific message</span></span>
#### <a name="request"></a><span data-ttu-id="44761-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="44761-170">Request</span></span>
<span data-ttu-id="44761-171">В следующем примере пользователь, вписав его, — Дана Swope.</span><span class="sxs-lookup"><span data-stu-id="44761-171">In the next example, the signed-in user is Dana Swope.</span></span> <span data-ttu-id="44761-172">В примере показано получение сведений о всех упоминаниях в указанном сообщении в почтовом ящике Даны.</span><span class="sxs-lookup"><span data-stu-id="44761-172">The example shows getting the details of all the mentions in the specified message in Dana's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="44761-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="44761-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADJmMTUAAAgVZAAAA"],
  "name": "get_mentions_in_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AQMkADJmMTUAAAgVZAAAA/?$expand=mentions
```
# <a name="c"></a>[<span data-ttu-id="44761-174">C#</span><span class="sxs-lookup"><span data-stu-id="44761-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mentions-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44761-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44761-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mentions-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44761-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44761-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mentions-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44761-177">Java</span><span class="sxs-lookup"><span data-stu-id="44761-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mentions-in-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="44761-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="44761-178">Response</span></span>
<span data-ttu-id="44761-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44761-179">Here is an example of the response.</span></span> <span data-ttu-id="44761-180">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="44761-180">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_mentions_in_message",
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

### <a name="example-3-get-message-body-in-text-format"></a><span data-ttu-id="44761-181">Пример 3. Получение текста сообщения в текстовом формате</span><span class="sxs-lookup"><span data-stu-id="44761-181">Example 3: Get message body in text format</span></span>
#### <a name="request"></a><span data-ttu-id="44761-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="44761-182">Request</span></span>

<span data-ttu-id="44761-183">В третьем примере показано, как использовать заголовок `Prefer: outlook.body-content-type="text"`, чтобы получить свойства **body** и **uniqueBody** указанного сообщения в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="44761-183">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>


# <a name="http"></a>[<span data-ttu-id="44761-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="44761-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="44761-185">C#</span><span class="sxs-lookup"><span data-stu-id="44761-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44761-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44761-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44761-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44761-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44761-188">Java</span><span class="sxs-lookup"><span data-stu-id="44761-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44761-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="44761-189">Response</span></span>

<span data-ttu-id="44761-190">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44761-190">Here is an example of the response.</span></span> <span data-ttu-id="44761-191">Примечание. Отклик включает заголовок `Preference-Applied: outlook.body-content-type`, подтверждающий заголовок запроса `Prefer: outlook.body-content-type`.</span><span class="sxs-lookup"><span data-stu-id="44761-191">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_message_in_text",
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
### <a name="example-4-get-internet-message-headers"></a><span data-ttu-id="44761-192">Пример 4. Получить заглавные главы сообщений в Интернете</span><span class="sxs-lookup"><span data-stu-id="44761-192">Example 4: Get Internet message headers</span></span>
#### <a name="request"></a><span data-ttu-id="44761-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="44761-193">Request</span></span>

<span data-ttu-id="44761-194">В четвертом примере показано, как получить в Интернете заглавные главы определенного сообщения.</span><span class="sxs-lookup"><span data-stu-id="44761-194">The fourth example shows how to get the Internet message headers of a specific message.</span></span>  


# <a name="http"></a>[<span data-ttu-id="44761-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="44761-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEz"],
  "name": "get_message_internet_headers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGVmMDEz/?$select=internetMessageHeaders
```
# <a name="c"></a>[<span data-ttu-id="44761-196">C#</span><span class="sxs-lookup"><span data-stu-id="44761-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-internet-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44761-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44761-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-internet-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44761-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44761-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-internet-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44761-199">Java</span><span class="sxs-lookup"><span data-stu-id="44761-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-internet-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44761-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="44761-200">Response</span></span>

<span data-ttu-id="44761-201">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44761-201">Here is an example of the response.</span></span> <span data-ttu-id="44761-202">Примечание. Количество заглавных сообщений Интернета в объекте ответа сократилось для краткости.</span><span class="sxs-lookup"><span data-stu-id="44761-202">Note: The number of Internet message headers in the response object has been reduced for brevity.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_message_internet_headers",
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


### <a name="example-5-get-mime-content"></a><span data-ttu-id="44761-203">Пример 5. Получить контент MIME</span><span class="sxs-lookup"><span data-stu-id="44761-203">Example 5: Get MIME content</span></span>
#### <a name="request"></a><span data-ttu-id="44761-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="44761-204">Request</span></span>
<span data-ttu-id="44761-205">В пятом примере получается содержимое MIME сообщения в почтовом ящике пользователя, вписав его.</span><span class="sxs-lookup"><span data-stu-id="44761-205">The fifth example gets the MIME content of a message in the signed-in user's mailbox.</span></span>


# <a name="http"></a>[<span data-ttu-id="44761-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="44761-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_message_in_mime",
  "sampleKeys": ["4aade2547798441eab5188a7a2436bc1"]
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/4aade2547798441eab5188a7a2436bc1/$value
```
# <a name="c"></a>[<span data-ttu-id="44761-207">C#</span><span class="sxs-lookup"><span data-stu-id="44761-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-mime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44761-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44761-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-mime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44761-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44761-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-mime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44761-210">Java</span><span class="sxs-lookup"><span data-stu-id="44761-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-mime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44761-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="44761-211">Response</span></span>
<span data-ttu-id="44761-212">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="44761-212">The following is the response.</span></span> <span data-ttu-id="44761-213">Содержимое MIME начинается с заголовка `MIME-Version`.</span><span class="sxs-lookup"><span data-stu-id="44761-213">The MIME content begins with the `MIME-Version` header.</span></span> 
<!-- {
  "blockType": "response",
  "name": "get_message_in_mime",
  "truncated": true,
  "@odata.type": "string"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

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


## <a name="see-also"></a><span data-ttu-id="44761-214">См. также</span><span class="sxs-lookup"><span data-stu-id="44761-214">See also</span></span>

- [<span data-ttu-id="44761-215">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="44761-215">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="44761-216">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="44761-216">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="44761-217">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="44761-217">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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


