---
title: Отправка почты
description: Отправляйте сообщение, указанное в тексте запроса, в формате JSON или MIME.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: eb97568e946bf1b145391c7c875500b05a3b93a6
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868891"
---
# <a name="send-mail"></a><span data-ttu-id="11b60-103">Отправка почты</span><span class="sxs-lookup"><span data-stu-id="11b60-103">Send mail</span></span>

<span data-ttu-id="11b60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11b60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11b60-105">Отправляйте сообщение, указанное в тексте запроса, в формате JSON или MIME.</span><span class="sxs-lookup"><span data-stu-id="11b60-105">Send the message specified in the request body using either JSON or MIME format.</span></span>

<span data-ttu-id="11b60-106">При использовании формата JSON можно включить [](../resources/mention.md) [вложение](../resources/attachment.md) и использовать упоминание, чтобы вызвать другого пользователя в новом сообщении.</span><span class="sxs-lookup"><span data-stu-id="11b60-106">When using JSON format you can include an [attachment](../resources/attachment.md) and use a [mention](../resources/mention.md) to call out another user in the new message.</span></span>

<span data-ttu-id="11b60-107">При использовании формата MIME:</span><span class="sxs-lookup"><span data-stu-id="11b60-107">When using MIME format:</span></span>
- <span data-ttu-id="11b60-108">Укажите соответствующие [заголовки сообщений Интернета](https://tools.ietf.org/html/rfc2076) и [содержимое MIME](https://tools.ietf.org/html/rfc2045), а также закодируйте их в формате **Base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="11b60-108">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="11b60-109">Добавьте все вложения и свойства S/MIME в содержимое MIME.</span><span class="sxs-lookup"><span data-stu-id="11b60-109">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="11b60-110">Этот метод сохраняет сообщение в папке **Отправленные**.</span><span class="sxs-lookup"><span data-stu-id="11b60-110">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="11b60-111">Или [создайте черновик сообщения](../api/user-post-messages.md), чтобы отправить его позже.</span><span class="sxs-lookup"><span data-stu-id="11b60-111">Alternatively, [create a draft message](../api/user-post-messages.md) to send later.</span></span>

## <a name="permissions"></a><span data-ttu-id="11b60-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11b60-112">Permissions</span></span>
<span data-ttu-id="11b60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11b60-p101">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11b60-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11b60-115">Permission type</span></span>      | <span data-ttu-id="11b60-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11b60-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11b60-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11b60-117">Delegated (work or school account)</span></span> | <span data-ttu-id="11b60-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="11b60-118">Mail.Send</span></span>    |
|<span data-ttu-id="11b60-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11b60-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11b60-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="11b60-120">Mail.Send</span></span>    |
|<span data-ttu-id="11b60-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11b60-121">Application</span></span> | <span data-ttu-id="11b60-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="11b60-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="11b60-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11b60-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```

## <a name="request-headers"></a><span data-ttu-id="11b60-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11b60-124">Request headers</span></span>
| <span data-ttu-id="11b60-125">Имя</span><span class="sxs-lookup"><span data-stu-id="11b60-125">Name</span></span>       | <span data-ttu-id="11b60-126">Тип</span><span class="sxs-lookup"><span data-stu-id="11b60-126">Type</span></span> | <span data-ttu-id="11b60-127">Описание</span><span class="sxs-lookup"><span data-stu-id="11b60-127">Description</span></span>| 
|:---------------|:--------|:----------
| <span data-ttu-id="11b60-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="11b60-128">Authorization</span></span>  | <span data-ttu-id="11b60-129">string</span><span class="sxs-lookup"><span data-stu-id="11b60-129">string</span></span>  | <span data-ttu-id="11b60-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11b60-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="11b60-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11b60-132">Content-Type</span></span> | <span data-ttu-id="11b60-133">string</span><span class="sxs-lookup"><span data-stu-id="11b60-133">string</span></span>  | <span data-ttu-id="11b60-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11b60-p103">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="11b60-136">Используйте `application/json` для объекта JSON и `text/plain` для содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="11b60-136">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11b60-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11b60-137">Request body</span></span>
<span data-ttu-id="11b60-138">При использовании формата JSON укажите объект JSON со следующими параметрами.</span><span class="sxs-lookup"><span data-stu-id="11b60-138">When using JSON format, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="11b60-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="11b60-139">Parameter</span></span>    | <span data-ttu-id="11b60-140">Тип</span><span class="sxs-lookup"><span data-stu-id="11b60-140">Type</span></span>   |<span data-ttu-id="11b60-141">Описание</span><span class="sxs-lookup"><span data-stu-id="11b60-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11b60-142">Message</span><span class="sxs-lookup"><span data-stu-id="11b60-142">Message</span></span>|[<span data-ttu-id="11b60-143">Message</span><span class="sxs-lookup"><span data-stu-id="11b60-143">Message</span></span>](../resources/message.md)|<span data-ttu-id="11b60-p104">Отправляемое сообщение. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11b60-p104">The message to send. Required.</span></span>|
|<span data-ttu-id="11b60-146">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="11b60-146">SaveToSentItems</span></span>|<span data-ttu-id="11b60-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b60-147">Boolean</span></span>|<span data-ttu-id="11b60-p105">Указывает, нужно ли сохранять сообщение в папке "Отправленные". Указывайте этот параметр, если задано значение false (по умолчанию используется true).  Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="11b60-p105">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="11b60-151">Чтобы использовать **упоминание,** чтобы вызвать другого пользователя в новом сообщении:</span><span class="sxs-lookup"><span data-stu-id="11b60-151">To use **mention** to call out another user in the new message:</span></span>
- <span data-ttu-id="11b60-152">Включай в текст запроса обязательное свойство **toRecipients,** свойство **mentions** и любые полезные свойства сообщений.</span><span class="sxs-lookup"><span data-stu-id="11b60-152">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="11b60-153">Для каждого упоминания в **свойстве упоминаний** необходимо указать **упомянутое** свойство.</span><span class="sxs-lookup"><span data-stu-id="11b60-153">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="11b60-154">При указании текста в формате MIME укажите содержимое MIME в тексте запроса как **строку в кодировке Base 64**.</span><span class="sxs-lookup"><span data-stu-id="11b60-154">When specifying the body in MIME format, provide the MIME content as **a base64-encoded string** in the request body.</span></span> <span data-ttu-id="11b60-155">Не включай параметры.</span><span class="sxs-lookup"><span data-stu-id="11b60-155">Do not include parameters.</span></span>

## <a name="response"></a><span data-ttu-id="11b60-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="11b60-156">Response</span></span>

<span data-ttu-id="11b60-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="11b60-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="11b60-159">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает `400 Bad request` и следующее сообщение об ошибке: "Недопустимая строка Base 64 для содержимого MIME".</span><span class="sxs-lookup"><span data-stu-id="11b60-159">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="11b60-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="11b60-160">Examples</span></span>
### <a name="example-1-send-a-new-email-using-json-format"></a><span data-ttu-id="11b60-161">Пример 1. Отправка нового сообщения электронной почты в формате JSON</span><span class="sxs-lookup"><span data-stu-id="11b60-161">Example 1: Send a new email using JSON format</span></span>
<span data-ttu-id="11b60-162">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="11b60-162">Here is an example of how to call this API.</span></span>
#### <a name="request"></a><span data-ttu-id="11b60-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="11b60-163">Request</span></span>
<span data-ttu-id="11b60-164">Вот пример запроса на создание и отправку сообщения на лету.</span><span class="sxs-lookup"><span data-stu-id="11b60-164">Here is an example of the request to create and send a message on the fly.</span></span>

# <a name="http"></a>[<span data-ttu-id="11b60-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="11b60-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json
Content-length: 512

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "samanthab@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients": [
      {
        "emailAddress": {
          "address": "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  "saveToSentItems": "false"
}
```
# <a name="c"></a>[<span data-ttu-id="11b60-166">C#</span><span class="sxs-lookup"><span data-stu-id="11b60-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11b60-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11b60-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11b60-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11b60-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11b60-169">Java</span><span class="sxs-lookup"><span data-stu-id="11b60-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="11b60-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="11b60-170">Response</span></span>
<span data-ttu-id="11b60-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11b60-171">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-send-a-message-that-includes-an--mention"></a><span data-ttu-id="11b60-172">Пример 2. Отправка сообщения с упоминанием @</span><span class="sxs-lookup"><span data-stu-id="11b60-172">Example 2: Send a message that includes an @-mention</span></span>
#### <a name="request"></a><span data-ttu-id="11b60-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="11b60-173">Request</span></span>
<span data-ttu-id="11b60-174">В следующем примере показано сообщение подписанного пользователя в Samantha Booth.</span><span class="sxs-lookup"><span data-stu-id="11b60-174">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="11b60-175">В сообщении также содержится упоминание другого пользователя, Даны Swope.</span><span class="sxs-lookup"><span data-stu-id="11b60-175">The message also includes a mention of another user, Dana Swope.</span></span>

# <a name="http"></a>[<span data-ttu-id="11b60-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="11b60-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_mentions"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json
Content-length: 344

{
  "Message": {
    "subject": "Project kickoff",
    "toRecipients":[
      {
          "emailAddress":{
              "name":"Samantha Booth",
              "address":"samanthab@contoso.onmicrosoft.com"
          }
      }
    ],
    "mentions":[
      {
        "mentioned":{
          "name":"Dana Swope",
          "address":"danas@contoso.onmicrosoft.com"
         }
      }
    ]
  }
}
```

# <a name="c"></a>[<span data-ttu-id="11b60-177">C#</span><span class="sxs-lookup"><span data-stu-id="11b60-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11b60-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11b60-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11b60-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11b60-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11b60-180">Java</span><span class="sxs-lookup"><span data-stu-id="11b60-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-mentions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="11b60-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="11b60-181">Response</span></span>
<span data-ttu-id="11b60-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11b60-182">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-3-send-a-message-that-includes-custom-internet-message-headers"></a><span data-ttu-id="11b60-183">Пример 3. Отправка сообщения с пользовательскими загонами сообщений в Интернете</span><span class="sxs-lookup"><span data-stu-id="11b60-183">Example 3: Send a message that includes custom Internet message headers</span></span> 
#### <a name="request"></a><span data-ttu-id="11b60-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="11b60-184">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="11b60-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="11b60-185">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_headers"
}-->

```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json

{
  "message": {
    "subject": "9/9/2018: concert",
    "body": {
      "contentType": "HTML",
      "content": "The group represents Nevada."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "AlexW@contoso.OnMicrosoft.com"
        }
      }
    ],
    "internetMessageHeaders":[
      {
        "name":"x-custom-header-group-name",
        "value":"Nevada"
      },
      {
        "name":"x-custom-header-group-id",
        "value":"NV001"
      }
    ]
  }
}
```

# <a name="c"></a>[<span data-ttu-id="11b60-186">C#</span><span class="sxs-lookup"><span data-stu-id="11b60-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11b60-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11b60-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11b60-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11b60-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11b60-189">Java</span><span class="sxs-lookup"><span data-stu-id="11b60-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="11b60-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="11b60-190">Response</span></span>
<span data-ttu-id="11b60-191">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11b60-191">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-4-sends-a-message-with-a-file-attachment"></a><span data-ttu-id="11b60-192">Пример 4. Отправляет сообщение с вложением файла</span><span class="sxs-lookup"><span data-stu-id="11b60-192">Example 4: Sends a message with a file attachment</span></span>
#### <a name="request"></a><span data-ttu-id="11b60-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="11b60-193">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="11b60-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="11b60-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_attachment"
}-->

```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "meganb@contoso.onmicrosoft.com"
        }
      }
    ],
    "attachments": [
      {
        "@odata.type": "#microsoft.graph.fileAttachment",
        "name": "attachment.txt",
        "contentType": "text/plain",
        "contentBytes": "SGVsbG8gV29ybGQh"
      }
    ]
  }
}
```
# <a name="c"></a>[<span data-ttu-id="11b60-195">C#</span><span class="sxs-lookup"><span data-stu-id="11b60-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11b60-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11b60-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11b60-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11b60-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11b60-198">Java</span><span class="sxs-lookup"><span data-stu-id="11b60-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="11b60-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="11b60-199">Response</span></span>

<span data-ttu-id="11b60-200">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11b60-200">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```
### <a name="example-5-send-a-new-message-using-mime-format"></a><span data-ttu-id="11b60-201">Пример 5. Отправка нового сообщения в формате MIME</span><span class="sxs-lookup"><span data-stu-id="11b60-201">Example 5: Send a new message using MIME format</span></span>
#### <a name="request"></a><span data-ttu-id="11b60-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="11b60-202">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_send_mime_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM6IEludGVybmFsIFJlc3VtZSBTdWJtaXNzaW9uOiBT
YWxlcyBBc3NvY2lhdGUKVGhyZWFkLUluZGV4OiBjb2RlY29kZWNvZGVoZXJlaGVyZWhlcmUKRGF0
ZTogU3VuLCAyOCBGZWIgMjAyMSAwNzoxNTowMCArMDAwMApNZXNzYWdlLUlEOgoJPE1XSFBSMTMw
MU1CMjAwMDAwMDAwRDc2RDlDMjgyMjAwMDA5QUQ5QTlASFdIUFIxMzAxTUIwMDAwLmNvZGVudW0u
cHJvZC5vdXRsb29rLmNvbT4KQ29udGVudC1MYW5ndWFnZTogZW4tVVMKWC1NUy1IYXMtQXR0YWNo
OgpYLU1TLVRORUYtQ29ycmVsYXRvcjoKWC1NUy1Fe
```

#### <a name="response"></a><span data-ttu-id="11b60-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="11b60-203">Response</span></span>
<span data-ttu-id="11b60-204">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11b60-204">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="11b60-205">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="11b60-205">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 400 Bad Request
Content-type: application/json

{
    "error": {
        "code": "ErrorMimeContentInvalidBase64String",
        "message": "Invalid base64 string for MIME content."
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
