---
title: Отправка почты
description: Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2ac87c9e2ea9bd0778db7d96dfa79a0280c42ce3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451639"
---
# <a name="send-mail"></a><span data-ttu-id="561cd-104">Отправка почты</span><span class="sxs-lookup"><span data-stu-id="561cd-104">Send mail</span></span>

<span data-ttu-id="561cd-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="561cd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="561cd-106">Отправка сообщения, указанного в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="561cd-106">Send the message specified in the request body.</span></span> <span data-ttu-id="561cd-107">Сообщение сохраняется в папке "Отправленные" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="561cd-107">The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="561cd-108">В одном вызове метода **sendMail** можно выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="561cd-108">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="561cd-109">Включение [вложения](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="561cd-109">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="561cd-110">Используйте [упоминание](../resources/mention.md) , чтобы вызвонить другому пользователю в новом сообщении.</span><span class="sxs-lookup"><span data-stu-id="561cd-110">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="561cd-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="561cd-111">Permissions</span></span>
<span data-ttu-id="561cd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="561cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="561cd-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="561cd-114">Permission type</span></span>      | <span data-ttu-id="561cd-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="561cd-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="561cd-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="561cd-116">Delegated (work or school account)</span></span> | <span data-ttu-id="561cd-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="561cd-117">Mail.Send</span></span>    |
|<span data-ttu-id="561cd-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="561cd-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="561cd-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="561cd-119">Mail.Send</span></span>    |
|<span data-ttu-id="561cd-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="561cd-120">Application</span></span> | <span data-ttu-id="561cd-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="561cd-121">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="561cd-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="561cd-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="561cd-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="561cd-123">Request headers</span></span>
| <span data-ttu-id="561cd-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="561cd-124">Header</span></span>       | <span data-ttu-id="561cd-125">Значение</span><span class="sxs-lookup"><span data-stu-id="561cd-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="561cd-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="561cd-126">Authorization</span></span>  | <span data-ttu-id="561cd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="561cd-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="561cd-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="561cd-129">Content-Type</span></span>  | <span data-ttu-id="561cd-130">application/json</span><span class="sxs-lookup"><span data-stu-id="561cd-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="561cd-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="561cd-131">Request body</span></span>
<span data-ttu-id="561cd-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="561cd-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="561cd-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="561cd-133">Parameter</span></span>    | <span data-ttu-id="561cd-134">Тип</span><span class="sxs-lookup"><span data-stu-id="561cd-134">Type</span></span>   |<span data-ttu-id="561cd-135">Описание</span><span class="sxs-lookup"><span data-stu-id="561cd-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="561cd-136">Message</span><span class="sxs-lookup"><span data-stu-id="561cd-136">Message</span></span>|[<span data-ttu-id="561cd-137">Message</span><span class="sxs-lookup"><span data-stu-id="561cd-137">Message</span></span>](../resources/message.md)|<span data-ttu-id="561cd-p105">Отправляемое сообщение. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="561cd-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="561cd-140">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="561cd-140">SaveToSentItems</span></span>|<span data-ttu-id="561cd-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="561cd-141">Boolean</span></span>|<span data-ttu-id="561cd-p106">Указывает, нужно ли сохранять сообщение в папке "Отправленные". Указывайте этот параметр, если задано значение false (по умолчанию используется true).  Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="561cd-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="561cd-145">Если вы хотите использовать **упоминание** , чтобы вызвонить другому пользователю в новом сообщении:</span><span class="sxs-lookup"><span data-stu-id="561cd-145">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="561cd-146">Включите в текст запроса обязательное свойство **toRecipients** , свойства **упоминаютх** и все доступные для записи свойства сообщения.</span><span class="sxs-lookup"><span data-stu-id="561cd-146">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="561cd-147">Для каждого упоминания в свойстве **упоминания** необходимо указать **указанное свойство.**</span><span class="sxs-lookup"><span data-stu-id="561cd-147">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="561cd-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="561cd-148">Response</span></span>

<span data-ttu-id="561cd-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="561cd-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="561cd-151">Пример</span><span class="sxs-lookup"><span data-stu-id="561cd-151">Example</span></span>
<span data-ttu-id="561cd-152">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="561cd-152">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="561cd-153">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="561cd-153">Request 1</span></span>
<span data-ttu-id="561cd-154">Ниже приведен пример запроса на динамическое создание и отправку сообщения.</span><span class="sxs-lookup"><span data-stu-id="561cd-154">Here is an example of the request to create and send a message on the fly.</span></span>

# <a name="http"></a>[<span data-ttu-id="561cd-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="561cd-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="561cd-156">C#</span><span class="sxs-lookup"><span data-stu-id="561cd-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="561cd-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="561cd-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="561cd-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="561cd-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="561cd-159">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="561cd-159">Response 1</span></span>
<span data-ttu-id="561cd-160">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="561cd-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="561cd-161">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="561cd-161">Request 2</span></span>
<span data-ttu-id="561cd-162">В следующем примере показано сообщение от пользователя, выполнившего вход, в Samantha стенд.</span><span class="sxs-lookup"><span data-stu-id="561cd-162">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="561cd-163">Сообщение также содержит упоминание другого пользователя, дана свопе.</span><span class="sxs-lookup"><span data-stu-id="561cd-163">The message also includes a mention of another user, Dana Swope.</span></span>

# <a name="http"></a>[<span data-ttu-id="561cd-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="561cd-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="561cd-165">C#</span><span class="sxs-lookup"><span data-stu-id="561cd-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="561cd-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="561cd-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="561cd-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="561cd-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="561cd-168">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="561cd-168">Response 2</span></span>
<span data-ttu-id="561cd-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="561cd-169">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="561cd-170">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="561cd-170">Request 3</span></span>
<span data-ttu-id="561cd-171">В следующем примере создается сообщение с использованием настраиваемых заголовков сообщений Интернета и выполняется его отправка.</span><span class="sxs-lookup"><span data-stu-id="561cd-171">The next example creates a message with custom Internet message headers and sends the message.</span></span>

# <a name="http"></a>[<span data-ttu-id="561cd-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="561cd-172">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="561cd-173">C#</span><span class="sxs-lookup"><span data-stu-id="561cd-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="561cd-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="561cd-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="561cd-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="561cd-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-3"></a><span data-ttu-id="561cd-176">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="561cd-176">Response 3</span></span>
<span data-ttu-id="561cd-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="561cd-177">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-4"></a><span data-ttu-id="561cd-178">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="561cd-178">Request 4</span></span>

<span data-ttu-id="561cd-179">В следующем примере создается сообщение с вложением файла и отправляется сообщение.</span><span class="sxs-lookup"><span data-stu-id="561cd-179">The next example creates a message with a file attachment and sends the message.</span></span>


# <a name="http"></a>[<span data-ttu-id="561cd-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="561cd-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="561cd-181">C#</span><span class="sxs-lookup"><span data-stu-id="561cd-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="561cd-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="561cd-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="561cd-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="561cd-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-4"></a><span data-ttu-id="561cd-184">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="561cd-184">Response 4</span></span>

<span data-ttu-id="561cd-185">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="561cd-185">Here is an example of the response.</span></span>
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
