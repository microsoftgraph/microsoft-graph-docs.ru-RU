---
title: Отправка почты
description: Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cfb9fcd33a87b2112616241757a44f515f968df6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137216"
---
# <a name="send-mail"></a><span data-ttu-id="432b7-104">Отправка почты</span><span class="sxs-lookup"><span data-stu-id="432b7-104">Send mail</span></span>

<span data-ttu-id="432b7-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="432b7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="432b7-p102">Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="432b7-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="432b7-108">Вы можете включить [вложенный файл](../resources/fileattachment.md) при вызове действия **sendMail**.</span><span class="sxs-lookup"><span data-stu-id="432b7-108">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="432b7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="432b7-109">Permissions</span></span>
<span data-ttu-id="432b7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="432b7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="432b7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="432b7-112">Permission type</span></span>      | <span data-ttu-id="432b7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="432b7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="432b7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="432b7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="432b7-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="432b7-115">Mail.Send</span></span>    |
|<span data-ttu-id="432b7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="432b7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="432b7-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="432b7-117">Mail.Send</span></span>    |
|<span data-ttu-id="432b7-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="432b7-118">Application</span></span> | <span data-ttu-id="432b7-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="432b7-119">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="432b7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="432b7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="432b7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="432b7-121">Request headers</span></span>
| <span data-ttu-id="432b7-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="432b7-122">Header</span></span>       | <span data-ttu-id="432b7-123">Значение</span><span class="sxs-lookup"><span data-stu-id="432b7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="432b7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="432b7-124">Authorization</span></span>  | <span data-ttu-id="432b7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="432b7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="432b7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="432b7-127">Content-Type</span></span>  | <span data-ttu-id="432b7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="432b7-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="432b7-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="432b7-129">Request body</span></span>
<span data-ttu-id="432b7-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="432b7-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="432b7-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="432b7-131">Parameter</span></span>    | <span data-ttu-id="432b7-132">Тип</span><span class="sxs-lookup"><span data-stu-id="432b7-132">Type</span></span>   |<span data-ttu-id="432b7-133">Описание</span><span class="sxs-lookup"><span data-stu-id="432b7-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="432b7-134">message</span><span class="sxs-lookup"><span data-stu-id="432b7-134">message</span></span>|[<span data-ttu-id="432b7-135">Message</span><span class="sxs-lookup"><span data-stu-id="432b7-135">Message</span></span>](../resources/message.md)|<span data-ttu-id="432b7-p105">Отправляемое сообщение. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="432b7-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="432b7-138">saveToSentItems</span><span class="sxs-lookup"><span data-stu-id="432b7-138">saveToSentItems</span></span>|<span data-ttu-id="432b7-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="432b7-139">Boolean</span></span>|<span data-ttu-id="432b7-p106">Указывает, нужно ли сохранять сообщение в папке "Отправленные". Указывайте этот параметр, если задано значение false (по умолчанию используется true).  Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="432b7-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="432b7-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="432b7-143">Response</span></span>

<span data-ttu-id="432b7-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="432b7-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="432b7-146">Пример</span><span class="sxs-lookup"><span data-stu-id="432b7-146">Example</span></span>
<span data-ttu-id="432b7-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="432b7-147">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="432b7-148">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="432b7-148">Request 1</span></span>
<span data-ttu-id="432b7-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="432b7-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="432b7-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="432b7-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
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
          "address": "fannyd@contoso.onmicrosoft.com"
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
# <a name="c"></a>[<span data-ttu-id="432b7-151">C#</span><span class="sxs-lookup"><span data-stu-id="432b7-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="432b7-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="432b7-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="432b7-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="432b7-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="432b7-154">Java</span><span class="sxs-lookup"><span data-stu-id="432b7-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="432b7-155">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="432b7-155">Response 1</span></span>
<span data-ttu-id="432b7-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="432b7-156">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-2"></a><span data-ttu-id="432b7-157">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="432b7-157">Request 2</span></span>
<span data-ttu-id="432b7-158">В следующем примере создается сообщение с использованием настраиваемых заголовков сообщений Интернета и выполняется его отправка.</span><span class="sxs-lookup"><span data-stu-id="432b7-158">The next example creates a message with custom Internet message headers and sends the message.</span></span>

# <a name="http"></a>[<span data-ttu-id="432b7-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="432b7-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_headers"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
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
# <a name="c"></a>[<span data-ttu-id="432b7-160">C#</span><span class="sxs-lookup"><span data-stu-id="432b7-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="432b7-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="432b7-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="432b7-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="432b7-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="432b7-163">Java</span><span class="sxs-lookup"><span data-stu-id="432b7-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="432b7-164">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="432b7-164">Response 2</span></span>
<span data-ttu-id="432b7-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="432b7-165">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="432b7-166">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="432b7-166">Request 3</span></span>

<span data-ttu-id="432b7-167">В следующем примере создается сообщение с вложением файла и отправляется сообщение.</span><span class="sxs-lookup"><span data-stu-id="432b7-167">The next example creates a message with a file attachment and sends the message.</span></span>


# <a name="http"></a>[<span data-ttu-id="432b7-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="432b7-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_attachment"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/sendMail
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
# <a name="c"></a>[<span data-ttu-id="432b7-169">C#</span><span class="sxs-lookup"><span data-stu-id="432b7-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="432b7-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="432b7-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="432b7-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="432b7-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="432b7-172">Java</span><span class="sxs-lookup"><span data-stu-id="432b7-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-3"></a><span data-ttu-id="432b7-173">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="432b7-173">Response 3</span></span>

<span data-ttu-id="432b7-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="432b7-174">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

