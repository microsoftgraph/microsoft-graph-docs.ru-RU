---
title: Отправка почты
description: Отправьте сообщение, указанное в тексте запроса, в формате JSON или MIME.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5ee3bc0682f6611a06cb5e24e66b2c665a0be123
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645642"
---
# <a name="send-mail"></a><span data-ttu-id="56906-103">Отправка почты</span><span class="sxs-lookup"><span data-stu-id="56906-103">Send mail</span></span>

<span data-ttu-id="56906-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56906-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56906-105">Отправьте сообщение, указанное в тексте запроса, в формате JSON или MIME.</span><span class="sxs-lookup"><span data-stu-id="56906-105">Send the message specified in the request body using either JSON or MIME format.</span></span>

<span data-ttu-id="56906-106">При использовании формата JSON можно включить [](../resources/mention.md) [вложение](../resources/attachment.md) и использовать упоминание, чтобы вызвать другого пользователя в новом сообщении.</span><span class="sxs-lookup"><span data-stu-id="56906-106">When using JSON format you can include an [attachment](../resources/attachment.md) and use a [mention](../resources/mention.md) to call out another user in the new message.</span></span>

<span data-ttu-id="56906-107">При использовании формата MIME:</span><span class="sxs-lookup"><span data-stu-id="56906-107">When using MIME format:</span></span>
- <span data-ttu-id="56906-108">Предоформим соответствующие заголовки интернет-сообщений и [содержимое MIME](https://tools.ietf.org/html/rfc2045), все закодированные в [](https://tools.ietf.org/html/rfc2076) **формате base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="56906-108">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="56906-109">Добавьте все вложения и свойства S/MIME в содержимое MIME.</span><span class="sxs-lookup"><span data-stu-id="56906-109">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="56906-110">Этот метод сохраняет сообщение в папке **Отправленные** элементы.</span><span class="sxs-lookup"><span data-stu-id="56906-110">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="56906-111">Кроме того, [создайте черновик сообщения для](../api/user-post-messages.md) отправки позже.</span><span class="sxs-lookup"><span data-stu-id="56906-111">Alternatively, [create a draft message](../api/user-post-messages.md) to send later.</span></span>

## <a name="permissions"></a><span data-ttu-id="56906-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56906-112">Permissions</span></span>
<span data-ttu-id="56906-113">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="56906-113">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="56906-114">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56906-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56906-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56906-115">Permission type</span></span>      | <span data-ttu-id="56906-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56906-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56906-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56906-117">Delegated (work or school account)</span></span> | <span data-ttu-id="56906-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="56906-118">Mail.Send</span></span>    |
|<span data-ttu-id="56906-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56906-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56906-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="56906-120">Mail.Send</span></span>    |
|<span data-ttu-id="56906-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56906-121">Application</span></span> | <span data-ttu-id="56906-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="56906-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="56906-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56906-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```

## <a name="request-headers"></a><span data-ttu-id="56906-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56906-124">Request headers</span></span>
| <span data-ttu-id="56906-125">Имя</span><span class="sxs-lookup"><span data-stu-id="56906-125">Name</span></span>       | <span data-ttu-id="56906-126">Тип</span><span class="sxs-lookup"><span data-stu-id="56906-126">Type</span></span> | <span data-ttu-id="56906-127">Описание</span><span class="sxs-lookup"><span data-stu-id="56906-127">Description</span></span>| 
|:---------------|:--------|:----------
| <span data-ttu-id="56906-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="56906-128">Authorization</span></span>  | <span data-ttu-id="56906-129">string</span><span class="sxs-lookup"><span data-stu-id="56906-129">string</span></span>  | <span data-ttu-id="56906-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56906-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="56906-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56906-132">Content-Type</span></span> | <span data-ttu-id="56906-133">string</span><span class="sxs-lookup"><span data-stu-id="56906-133">string</span></span>  | <span data-ttu-id="56906-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56906-p103">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="56906-136">Используйте `application/json` для объекта JSON и `text/plain` контента MIME.</span><span class="sxs-lookup"><span data-stu-id="56906-136">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56906-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56906-137">Request body</span></span>
<span data-ttu-id="56906-138">При использовании формата JSON укажи объект JSON со следующими параметрами.</span><span class="sxs-lookup"><span data-stu-id="56906-138">When using JSON format, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="56906-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="56906-139">Parameter</span></span>    | <span data-ttu-id="56906-140">Тип</span><span class="sxs-lookup"><span data-stu-id="56906-140">Type</span></span>   |<span data-ttu-id="56906-141">Описание</span><span class="sxs-lookup"><span data-stu-id="56906-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56906-142">Message</span><span class="sxs-lookup"><span data-stu-id="56906-142">Message</span></span>|[<span data-ttu-id="56906-143">Message</span><span class="sxs-lookup"><span data-stu-id="56906-143">Message</span></span>](../resources/message.md)|<span data-ttu-id="56906-p104">Отправляемое сообщение. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56906-p104">The message to send. Required.</span></span>|
|<span data-ttu-id="56906-146">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="56906-146">SaveToSentItems</span></span>|<span data-ttu-id="56906-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="56906-147">Boolean</span></span>|<span data-ttu-id="56906-p105">Указывает, нужно ли сохранять сообщение в папке "Отправленные". Указывайте этот параметр, если задано значение false (по умолчанию используется true).  Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="56906-p105">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="56906-151">Чтобы использовать **упоминание,** чтобы вызвать другого пользователя в новом сообщении:</span><span class="sxs-lookup"><span data-stu-id="56906-151">To use **mention** to call out another user in the new message:</span></span>
- <span data-ttu-id="56906-152">Включай в текст запроса обязательное свойство **toRecipients,** свойство **mentions** и любые полезные свойства сообщений.</span><span class="sxs-lookup"><span data-stu-id="56906-152">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="56906-153">Для каждого упоминания в **свойстве упоминаний** необходимо указать **упомянутое** свойство.</span><span class="sxs-lookup"><span data-stu-id="56906-153">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="56906-154">При указании тела в формате MIME укажите содержимое MIME в виде строки с кодом **base64** в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="56906-154">When specifying the body in MIME format, provide the MIME content as **a base64-encoded string** in the request body.</span></span> <span data-ttu-id="56906-155">Не включай параметры.</span><span class="sxs-lookup"><span data-stu-id="56906-155">Do not include parameters.</span></span>

## <a name="response"></a><span data-ttu-id="56906-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="56906-156">Response</span></span>

<span data-ttu-id="56906-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="56906-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="56906-159">Если в тексте запроса содержится неправильное содержимое MIME, этот метод возвращается и следующее сообщение об ошибке: "Недействительные строки `400 Bad request` base64 для контента MIME".</span><span class="sxs-lookup"><span data-stu-id="56906-159">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="56906-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="56906-160">Examples</span></span>
### <a name="example-1-send-a-new-email-using-json-format"></a><span data-ttu-id="56906-161">Пример 1. Отправка новой электронной почты с помощью формата JSON</span><span class="sxs-lookup"><span data-stu-id="56906-161">Example 1: Send a new email using JSON format</span></span>
<span data-ttu-id="56906-162">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="56906-162">Here is an example of how to call this API.</span></span>
#### <a name="request"></a><span data-ttu-id="56906-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="56906-163">Request</span></span>
<span data-ttu-id="56906-164">Вот пример запроса на создание и отправку сообщения на лету.</span><span class="sxs-lookup"><span data-stu-id="56906-164">Here is an example of the request to create and send a message on the fly.</span></span>

# <a name="http"></a>[<span data-ttu-id="56906-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="56906-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="56906-166">C#</span><span class="sxs-lookup"><span data-stu-id="56906-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56906-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56906-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56906-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56906-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56906-169">Java</span><span class="sxs-lookup"><span data-stu-id="56906-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="56906-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="56906-170">Response</span></span>
<span data-ttu-id="56906-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56906-171">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-send-a-message-that-includes-an--mention"></a><span data-ttu-id="56906-172">Пример 2. Отправка сообщения с упоминанием @</span><span class="sxs-lookup"><span data-stu-id="56906-172">Example 2: Send a message that includes an @-mention</span></span>
#### <a name="request"></a><span data-ttu-id="56906-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="56906-173">Request</span></span>
<span data-ttu-id="56906-174">В следующем примере показано сообщение подписанного пользователя в Samantha Booth.</span><span class="sxs-lookup"><span data-stu-id="56906-174">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="56906-175">В сообщении также содержится упоминание другого пользователя, Даны Swope.</span><span class="sxs-lookup"><span data-stu-id="56906-175">The message also includes a mention of another user, Dana Swope.</span></span>

# <a name="http"></a>[<span data-ttu-id="56906-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="56906-176">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="56906-177">C#</span><span class="sxs-lookup"><span data-stu-id="56906-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56906-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56906-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56906-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56906-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56906-180">Java</span><span class="sxs-lookup"><span data-stu-id="56906-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-mentions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="56906-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="56906-181">Response</span></span>
<span data-ttu-id="56906-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56906-182">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-3-send-a-message-that-includes-custom-internet-message-headers"></a><span data-ttu-id="56906-183">Пример 3. Отправка сообщения с пользовательскими загонами сообщений в Интернете</span><span class="sxs-lookup"><span data-stu-id="56906-183">Example 3: Send a message that includes custom Internet message headers</span></span> 
#### <a name="request"></a><span data-ttu-id="56906-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="56906-184">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="56906-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="56906-185">HTTP</span></span>](#tab/http)

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

# <a name="c"></a>[<span data-ttu-id="56906-186">C#</span><span class="sxs-lookup"><span data-stu-id="56906-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56906-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56906-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56906-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56906-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56906-189">Java</span><span class="sxs-lookup"><span data-stu-id="56906-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="56906-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="56906-190">Response</span></span>
<span data-ttu-id="56906-191">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56906-191">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-4-sends-a-message-with-a-file-attachment"></a><span data-ttu-id="56906-192">Пример 4. Отправляет сообщение с вложением файла</span><span class="sxs-lookup"><span data-stu-id="56906-192">Example 4: Sends a message with a file attachment</span></span>
#### <a name="request"></a><span data-ttu-id="56906-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="56906-193">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="56906-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="56906-194">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="56906-195">C#</span><span class="sxs-lookup"><span data-stu-id="56906-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56906-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56906-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56906-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56906-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56906-198">Java</span><span class="sxs-lookup"><span data-stu-id="56906-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="56906-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="56906-199">Response</span></span>

<span data-ttu-id="56906-200">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56906-200">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```
### <a name="example-5-send-a-new-message-using-mime-format"></a><span data-ttu-id="56906-201">Пример 5. Отправка нового сообщения в формате MIME</span><span class="sxs-lookup"><span data-stu-id="56906-201">Example 5: Send a new message using MIME format</span></span>
#### <a name="request"></a><span data-ttu-id="56906-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="56906-202">Request</span></span>

<!-- {
  "blockType": "request",
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
#### <a name="response"></a><span data-ttu-id="56906-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="56906-203">Response</span></span>
<span data-ttu-id="56906-204">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56906-204">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="56906-205">Если в тексте запроса содержится недооформленное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="56906-205">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
