---
title: Отправка почты
description: Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1258b7808b15348b38fceaf084626a6d89629cc3
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774460"
---
# <a name="send-mail"></a><span data-ttu-id="d1632-104">Отправка почты</span><span class="sxs-lookup"><span data-stu-id="d1632-104">Send mail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1632-p102">Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d1632-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="d1632-107">В одном вызове метода **sendMail** можно выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="d1632-107">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="d1632-108">Включение [вложения](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="d1632-108">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="d1632-109">Используйте [упоминание](../resources/mention.md) , чтобы вызвонить другому пользователю в новом сообщении.</span><span class="sxs-lookup"><span data-stu-id="d1632-109">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="d1632-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1632-110">Permissions</span></span>
<span data-ttu-id="d1632-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1632-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d1632-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1632-113">Permission type</span></span>      | <span data-ttu-id="d1632-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1632-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1632-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1632-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d1632-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d1632-116">Mail.Send</span></span>    |
|<span data-ttu-id="d1632-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1632-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1632-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d1632-118">Mail.Send</span></span>    |
|<span data-ttu-id="d1632-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1632-119">Application</span></span> | <span data-ttu-id="d1632-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d1632-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1632-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1632-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="d1632-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1632-122">Request headers</span></span>
| <span data-ttu-id="d1632-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1632-123">Header</span></span>       | <span data-ttu-id="d1632-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d1632-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d1632-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1632-125">Authorization</span></span>  | <span data-ttu-id="d1632-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1632-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d1632-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1632-128">Content-Type</span></span>  | <span data-ttu-id="d1632-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d1632-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d1632-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1632-130">Request body</span></span>
<span data-ttu-id="d1632-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d1632-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d1632-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="d1632-132">Parameter</span></span>    | <span data-ttu-id="d1632-133">Тип</span><span class="sxs-lookup"><span data-stu-id="d1632-133">Type</span></span>   |<span data-ttu-id="d1632-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d1632-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1632-135">Message</span><span class="sxs-lookup"><span data-stu-id="d1632-135">Message</span></span>|[<span data-ttu-id="d1632-136">Message</span><span class="sxs-lookup"><span data-stu-id="d1632-136">Message</span></span>](../resources/message.md)|<span data-ttu-id="d1632-p105">Отправляемое сообщение. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1632-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="d1632-139">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="d1632-139">SaveToSentItems</span></span>|<span data-ttu-id="d1632-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1632-140">Boolean</span></span>|<span data-ttu-id="d1632-p106">Указывает, нужно ли сохранять сообщение в папке "Отправленные". Указывайте этот параметр, если задано значение false (по умолчанию используется true).  Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d1632-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="d1632-144">Если вы хотите использовать **упоминание** , чтобы вызвонить другому пользователю в новом сообщении:</span><span class="sxs-lookup"><span data-stu-id="d1632-144">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="d1632-145">Включите в текст запроса обязательное свойство **toRecipients** , свойства **упоминаютх** и все доступные для записи свойства сообщения.</span><span class="sxs-lookup"><span data-stu-id="d1632-145">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="d1632-146">Для каждого упоминания в свойстве **упоминания** необходимо указать **указанное свойство.**</span><span class="sxs-lookup"><span data-stu-id="d1632-146">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="d1632-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1632-147">Response</span></span>

<span data-ttu-id="d1632-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d1632-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1632-150">Пример</span><span class="sxs-lookup"><span data-stu-id="d1632-150">Example</span></span>
<span data-ttu-id="d1632-151">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d1632-151">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="d1632-152">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="d1632-152">Request 1</span></span>
<span data-ttu-id="d1632-153">Ниже приведен пример запроса на динамическое создание и отправку сообщения.</span><span class="sxs-lookup"><span data-stu-id="d1632-153">Here is an example of the request to create and send a message on the fly.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d1632-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1632-154">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d1632-155">C#</span><span class="sxs-lookup"><span data-stu-id="d1632-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1632-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1632-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d1632-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1632-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="d1632-158">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="d1632-158">Response 1</span></span>
<span data-ttu-id="d1632-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d1632-159">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="d1632-160">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="d1632-160">Request 2</span></span>
<span data-ttu-id="d1632-161">В следующем примере показано сообщение от пользователя, выполнившего вход, в Samantha стенд.</span><span class="sxs-lookup"><span data-stu-id="d1632-161">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="d1632-162">Сообщение также содержит упоминание другого пользователя, дана свопе.</span><span class="sxs-lookup"><span data-stu-id="d1632-162">The message also includes a mention of another user, Dana Swope.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d1632-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1632-163">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d1632-164">C#</span><span class="sxs-lookup"><span data-stu-id="d1632-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1632-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1632-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d1632-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1632-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="d1632-167">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="d1632-167">Response 2</span></span>
<span data-ttu-id="d1632-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1632-168">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="d1632-169">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="d1632-169">Request 3</span></span>
<span data-ttu-id="d1632-170">В следующем примере создается сообщение с использованием настраиваемых заголовков сообщений Интернета и выполняется его отправка.</span><span class="sxs-lookup"><span data-stu-id="d1632-170">The next example creates a message with custom Internet message headers and sends the message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d1632-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1632-171">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d1632-172">C#</span><span class="sxs-lookup"><span data-stu-id="d1632-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1632-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1632-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d1632-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1632-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-3"></a><span data-ttu-id="d1632-175">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="d1632-175">Response 3</span></span>
<span data-ttu-id="d1632-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1632-176">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-4"></a><span data-ttu-id="d1632-177">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="d1632-177">Request 4</span></span>

<span data-ttu-id="d1632-178">В следующем примере создается сообщение с вложением файла и отправляется сообщение.</span><span class="sxs-lookup"><span data-stu-id="d1632-178">The next example creates a message with a file attachment and sends the message.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d1632-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1632-179">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d1632-180">C#</span><span class="sxs-lookup"><span data-stu-id="d1632-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1632-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1632-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d1632-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1632-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-4"></a><span data-ttu-id="d1632-183">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="d1632-183">Response 4</span></span>

<span data-ttu-id="d1632-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1632-184">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
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
