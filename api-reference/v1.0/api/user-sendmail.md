---
title: Отправка почты
description: Отправляйте сообщение, указанное в тексте запроса, в формате JSON или MIME.
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 460e09371869fec98b24bd81dc5ab44cc8b199b8
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870390"
---
# <a name="send-mail"></a><span data-ttu-id="49dfc-103">Отправка почты</span><span class="sxs-lookup"><span data-stu-id="49dfc-103">Send mail</span></span>

<span data-ttu-id="49dfc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49dfc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49dfc-105">Отправляйте сообщение, указанное в тексте запроса, в формате JSON или MIME.</span><span class="sxs-lookup"><span data-stu-id="49dfc-105">Send the message specified in the request body using either JSON or MIME format.</span></span>

<span data-ttu-id="49dfc-106">При использовании формата JSON вы можете включить [вложенный файл](../resources/fileattachment.md) при вызове действия **sendMail**.</span><span class="sxs-lookup"><span data-stu-id="49dfc-106">When using JSON format you can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

<span data-ttu-id="49dfc-107">При использовании формата MIME:</span><span class="sxs-lookup"><span data-stu-id="49dfc-107">When using MIME format:</span></span>
- <span data-ttu-id="49dfc-108">Укажите соответствующие [заголовки сообщений Интернета](https://tools.ietf.org/html/rfc2076) и [содержимое MIME](https://tools.ietf.org/html/rfc2045), а также закодируйте их в формате **Base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="49dfc-108">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="49dfc-109">Добавьте все вложения и свойства S/MIME в содержимое MIME.</span><span class="sxs-lookup"><span data-stu-id="49dfc-109">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="49dfc-110">Этот метод сохраняет сообщение в папке **Отправленные**.</span><span class="sxs-lookup"><span data-stu-id="49dfc-110">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="49dfc-111">Или [создайте черновик сообщения](../api/user-post-messages.md), чтобы отправить его позже.</span><span class="sxs-lookup"><span data-stu-id="49dfc-111">Alternatively, [create a draft message](../api/user-post-messages.md) to send later.</span></span>

## <a name="permissions"></a><span data-ttu-id="49dfc-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49dfc-112">Permissions</span></span>
<span data-ttu-id="49dfc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49dfc-p101">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49dfc-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49dfc-115">Permission type</span></span>      | <span data-ttu-id="49dfc-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49dfc-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49dfc-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49dfc-117">Delegated (work or school account)</span></span> | <span data-ttu-id="49dfc-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="49dfc-118">Mail.Send</span></span>    |
|<span data-ttu-id="49dfc-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49dfc-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49dfc-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="49dfc-120">Mail.Send</span></span>    |
|<span data-ttu-id="49dfc-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49dfc-121">Application</span></span> | <span data-ttu-id="49dfc-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="49dfc-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="49dfc-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49dfc-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```

## <a name="request-headers"></a><span data-ttu-id="49dfc-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49dfc-124">Request headers</span></span>
| <span data-ttu-id="49dfc-125">Имя</span><span class="sxs-lookup"><span data-stu-id="49dfc-125">Name</span></span>       | <span data-ttu-id="49dfc-126">Тип</span><span class="sxs-lookup"><span data-stu-id="49dfc-126">Type</span></span> | <span data-ttu-id="49dfc-127">Описание</span><span class="sxs-lookup"><span data-stu-id="49dfc-127">Description</span></span>| 
|:---------------|:--------|:----------
| <span data-ttu-id="49dfc-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="49dfc-128">Authorization</span></span>  | <span data-ttu-id="49dfc-129">string</span><span class="sxs-lookup"><span data-stu-id="49dfc-129">string</span></span>  | <span data-ttu-id="49dfc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49dfc-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="49dfc-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49dfc-132">Content-Type</span></span> | <span data-ttu-id="49dfc-133">string</span><span class="sxs-lookup"><span data-stu-id="49dfc-133">string</span></span>  | <span data-ttu-id="49dfc-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49dfc-p103">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="49dfc-136">Используйте `application/json` для объекта JSON и `text/plain` для содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="49dfc-136">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49dfc-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49dfc-137">Request body</span></span>
<span data-ttu-id="49dfc-138">При использовании формата JSON укажите объект JSON со следующими параметрами.</span><span class="sxs-lookup"><span data-stu-id="49dfc-138">When using JSON format, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="49dfc-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="49dfc-139">Parameter</span></span>    | <span data-ttu-id="49dfc-140">Тип</span><span class="sxs-lookup"><span data-stu-id="49dfc-140">Type</span></span>   |<span data-ttu-id="49dfc-141">Описание</span><span class="sxs-lookup"><span data-stu-id="49dfc-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49dfc-142">message</span><span class="sxs-lookup"><span data-stu-id="49dfc-142">message</span></span>|[<span data-ttu-id="49dfc-143">Message</span><span class="sxs-lookup"><span data-stu-id="49dfc-143">Message</span></span>](../resources/message.md)|<span data-ttu-id="49dfc-p104">Отправляемое сообщение. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49dfc-p104">The message to send. Required.</span></span>|
|<span data-ttu-id="49dfc-146">saveToSentItems</span><span class="sxs-lookup"><span data-stu-id="49dfc-146">saveToSentItems</span></span>|<span data-ttu-id="49dfc-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="49dfc-147">Boolean</span></span>|<span data-ttu-id="49dfc-p105">Указывает, нужно ли сохранять сообщение в папке "Отправленные". Указывайте этот параметр, если задано значение false (по умолчанию используется true).  Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="49dfc-p105">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

<span data-ttu-id="49dfc-151">При указании текста в формате MIME укажите содержимое MIME в тексте запроса как **строку в кодировке Base 64**.</span><span class="sxs-lookup"><span data-stu-id="49dfc-151">When specifying the body in MIME format, provide the MIME content as **a base64-encoded string** in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="49dfc-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="49dfc-152">Response</span></span>

<span data-ttu-id="49dfc-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="49dfc-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="49dfc-155">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает `400 Bad request` и следующее сообщение об ошибке: "Недопустимая строка Base 64 для содержимого MIME".</span><span class="sxs-lookup"><span data-stu-id="49dfc-155">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="49dfc-156">Примеры</span><span class="sxs-lookup"><span data-stu-id="49dfc-156">Examples</span></span>
### <a name="example-1-send-a-new-email-using-json-format"></a><span data-ttu-id="49dfc-157">Пример 1. Отправка нового сообщения электронной почты в формате JSON</span><span class="sxs-lookup"><span data-stu-id="49dfc-157">Example 1: Send a new email using JSON format</span></span>
<span data-ttu-id="49dfc-158">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="49dfc-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="49dfc-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="49dfc-159">Request</span></span>
<span data-ttu-id="49dfc-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49dfc-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49dfc-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="49dfc-161">HTTP</span></span>](#tab/http)

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
# <a name="c"></a>[<span data-ttu-id="49dfc-162">C#</span><span class="sxs-lookup"><span data-stu-id="49dfc-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49dfc-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49dfc-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49dfc-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49dfc-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49dfc-165">Java</span><span class="sxs-lookup"><span data-stu-id="49dfc-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="49dfc-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="49dfc-166">Response</span></span>
<span data-ttu-id="49dfc-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49dfc-167">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-create-a-message-with-custom-internet-message-headers-and-send-the-message"></a><span data-ttu-id="49dfc-168">Пример 2: Создание сообщение с использованием настраиваемых заголовков сообщений Интернета и выполнение его отправки</span><span class="sxs-lookup"><span data-stu-id="49dfc-168">Example 2: Create a message with custom Internet message headers and send the message</span></span>
#### <a name="request"></a><span data-ttu-id="49dfc-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="49dfc-169">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="49dfc-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="49dfc-170">HTTP</span></span>](#tab/http)

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
# <a name="c"></a>[<span data-ttu-id="49dfc-171">C#</span><span class="sxs-lookup"><span data-stu-id="49dfc-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49dfc-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49dfc-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49dfc-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49dfc-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49dfc-174">Java</span><span class="sxs-lookup"><span data-stu-id="49dfc-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="49dfc-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="49dfc-175">Response</span></span>
<span data-ttu-id="49dfc-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49dfc-176">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-3--create-a-message-with-a-file-attachment-and-send-the-message"></a><span data-ttu-id="49dfc-177">Пример 3. Создание сообщения с вложением файла и отправка сообщения</span><span class="sxs-lookup"><span data-stu-id="49dfc-177">Example 3:  Create a message with a file attachment and send the message</span></span>
#### <a name="request"></a><span data-ttu-id="49dfc-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="49dfc-178">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="49dfc-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="49dfc-179">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="49dfc-180">C#</span><span class="sxs-lookup"><span data-stu-id="49dfc-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49dfc-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49dfc-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49dfc-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49dfc-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49dfc-183">Java</span><span class="sxs-lookup"><span data-stu-id="49dfc-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="49dfc-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="49dfc-184">Response</span></span>
<span data-ttu-id="49dfc-185">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49dfc-185">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-4-send-a-new-message-using-mime-format"></a><span data-ttu-id="49dfc-186">Пример 4. Отправка нового сообщения в формате MIME</span><span class="sxs-lookup"><span data-stu-id="49dfc-186">Example 4: Send a new message using MIME format</span></span>
#### <a name="request"></a><span data-ttu-id="49dfc-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="49dfc-187">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_send_mime_beta"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/sendMail
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

#### <a name="response"></a><span data-ttu-id="49dfc-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="49dfc-188">Response</span></span>
<span data-ttu-id="49dfc-189">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49dfc-189">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="49dfc-190">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="49dfc-190">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
