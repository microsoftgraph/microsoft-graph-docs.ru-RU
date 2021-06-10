---
title: 'message: createReply'
description: 'Создайте черновик для ответа на сообщение в формате JSON или MIME. '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1f9962a6432b130bfeb121bc273271cb3591e181
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868940"
---
# <a name="message-createreply"></a><span data-ttu-id="8a7f5-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="8a7f5-103">message: createReply</span></span>

<span data-ttu-id="8a7f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a7f5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a7f5-105">Создайте черновик для ответа отправителю сообщения в формате JSON или MIME. [](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="8a7f5-105">Create a draft to reply to the sender of a [message](../resources/message.md) in either JSON or MIME format.</span></span>

<span data-ttu-id="8a7f5-106">При использовании формата JSON:</span><span class="sxs-lookup"><span data-stu-id="8a7f5-106">When using JSON format:</span></span>
- <span data-ttu-id="8a7f5-107">Укажите комментарий или **свойство** тела `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="8a7f5-108">При указании обоих возвращается ошибка http 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="8a7f5-109">Если replyTo указывается в исходном сообщении в формате интернет-сообщений [(RFC 2822),](https://www.rfc-editor.org/info/rfc2822)необходимо отправить ответ получателям в **replyTo,** а не получателям из **.** </span><span class="sxs-lookup"><span data-stu-id="8a7f5-109">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span>
- <span data-ttu-id="8a7f5-110">Вы можете [обновить проект](../api/message-update.md) позже, чтобы добавить содержимое ответа в **тело или** изменить другие свойства сообщения.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-110">You can [update](../api/message-update.md) the draft later to add reply content to the **body** or change other message properties.</span></span>

<span data-ttu-id="8a7f5-111">При использовании формата MIME:</span><span class="sxs-lookup"><span data-stu-id="8a7f5-111">When using MIME format:</span></span>
- <span data-ttu-id="8a7f5-112">Укажите соответствующие [заголовки сообщений Интернета](https://tools.ietf.org/html/rfc2076) и [содержимое MIME](https://tools.ietf.org/html/rfc2045), а также закодируйте их в формате **Base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-112">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="8a7f5-113">Добавьте все вложения и свойства S/MIME в содержимое MIME.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-113">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="8a7f5-114">[Отправьте](../api/message-send.md) черновик сообщения в ходе последующей операции.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-114">[Send](../api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="8a7f5-115">Кроме того, [ответьте на сообщение в](../api/message-reply.md) одной операции.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-115">Alternatively, [reply to a message](../api/message-reply.md) in a single operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a7f5-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a7f5-116">Permissions</span></span>
<span data-ttu-id="8a7f5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a7f5-p102">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a7f5-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a7f5-119">Permission type</span></span>      | <span data-ttu-id="8a7f5-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a7f5-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a7f5-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a7f5-121">Delegated (work or school account)</span></span> | <span data-ttu-id="8a7f5-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a7f5-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8a7f5-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a7f5-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a7f5-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a7f5-124">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8a7f5-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a7f5-125">Application</span></span> | <span data-ttu-id="8a7f5-126">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a7f5-126">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a7f5-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a7f5-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```

## <a name="request-headers"></a><span data-ttu-id="8a7f5-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a7f5-128">Request headers</span></span>
| <span data-ttu-id="8a7f5-129">Имя</span><span class="sxs-lookup"><span data-stu-id="8a7f5-129">Name</span></span>       | <span data-ttu-id="8a7f5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8a7f5-130">Type</span></span> | <span data-ttu-id="8a7f5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8a7f5-131">Description</span></span>| 
|:---------------|:--------|:----------|
| <span data-ttu-id="8a7f5-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a7f5-132">Authorization</span></span>  | <span data-ttu-id="8a7f5-133">string</span><span class="sxs-lookup"><span data-stu-id="8a7f5-133">string</span></span>  | <span data-ttu-id="8a7f5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="8a7f5-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a7f5-136">Content-Type</span></span> | <span data-ttu-id="8a7f5-137">string</span><span class="sxs-lookup"><span data-stu-id="8a7f5-137">string</span></span>  | <span data-ttu-id="8a7f5-138">Характер данных в теле объекта.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-138">Nature of the data in the body of an entity.</span></span> <br/> <span data-ttu-id="8a7f5-139">Используйте `application/json` для объекта JSON и `text/plain` для содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-139">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a7f5-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a7f5-140">Request body</span></span>
<span data-ttu-id="8a7f5-141">Этот метод не требует тела запроса.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-141">This method does not require a request body.</span></span>

<span data-ttu-id="8a7f5-142">Однако для создания черновика ответа с помощью формата MIME предопрейте контент MIME применимыми заглавными сообщениями в Интернете, все закодированные в формате **base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-142">However, for creating a reply draft using MIME format, provide the MIME content with the applicable Internet message headers, all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="8a7f5-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a7f5-143">Response</span></span>

<span data-ttu-id="8a7f5-144">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-144">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="8a7f5-145">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает `400 Bad request` и следующее сообщение об ошибке: "Недопустимая строка Base 64 для содержимого MIME".</span><span class="sxs-lookup"><span data-stu-id="8a7f5-145">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="8a7f5-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="8a7f5-146">Examples</span></span>
### <a name="example-1-create-a-draft-message-in-json-format-to-reply-to-an-existing-message"></a><span data-ttu-id="8a7f5-147">Пример 1. Создание черновика сообщения в формате JSON для ответа на существующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-147">Example 1: Create a draft message in JSON format to reply to an existing message.</span></span>
<span data-ttu-id="8a7f5-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8a7f5-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a7f5-149">Request</span></span>
<span data-ttu-id="8a7f5-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8a7f5-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a7f5-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReply
```
# <a name="c"></a>[<span data-ttu-id="8a7f5-152">C#</span><span class="sxs-lookup"><span data-stu-id="8a7f5-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a7f5-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a7f5-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a7f5-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a7f5-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a7f5-155">Java</span><span class="sxs-lookup"><span data-stu-id="8a7f5-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8a7f5-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a7f5-156">Response</span></span>
<span data-ttu-id="8a7f5-p104">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

### <a name="example-2-create-a-draft-message-in-mime-format-to-reply-to-an-existing-message"></a><span data-ttu-id="8a7f5-159">Пример 2. Создание черновика сообщения в формате MIME для ответа на существующее сообщение</span><span class="sxs-lookup"><span data-stu-id="8a7f5-159">Example 2: Create a draft message in MIME format to reply to an existing message</span></span>
##### <a name="request"></a><span data-ttu-id="8a7f5-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a7f5-160">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_createReply_mime_v1"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/createReply
Content-type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM6IEludGVybmFsIFJlc3VtZSBTdWJtaXNzaW9uOiBT
YWxlcyBBc3NvY2lhdGUKVGhyZWFkLUluZGV4OiBjb2RlY29kZWNvZGVoZXJlaGVyZWhlcmUKRGF0
ZTogU3VuLCAyOCBGZWIgMjAyMSAwNzoxNTowMCA
```

##### <a name="response"></a><span data-ttu-id="8a7f5-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a7f5-161">Response</span></span>
<span data-ttu-id="8a7f5-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.message",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('0aaa0aa0-0000-0a00-a00a-0000009000a0')/messages/$entity",
    "@odata.etag": "W/\"AAAAAAAAAAAa00AAAa0aAaAa0a0AAAaAAAAaAa0a\"",
    "id": "AAMkADA1MTAAAAqldOAAA=",
    "createdDateTime": "2021-04-23T18:13:44Z",
    "lastModifiedDateTime": "2021-04-23T18:13:44Z",
    "changeKey": "AAAAAAAAAAAA00aaaa000aaA",
    "categories": [],
    "receivedDateTime": "2021-04-23T18:13:44Z",
    "sentDateTime": "2021-02-28T07:15:00Z",
    "hasAttachments": false,
    "internetMessageId": "<AAAAAAAAAA@AAAAAAA0001AA0000.codcod00.prod.outlook.com>",
    "subject": "Internal Resume Submission: Sales Associate",
    "bodyPreview": "Hi, Megan.I have an interest in the Sales Associate position. Please consider my resume, which you can access here...",
    "importance": "normal",
    "parentFolderId": "LKJDSKJHkjhfakKJHFKWKKJHKJdhkjHDK==",
    "conversationId": "SDSFSmFSDGI5LWZhYjc4fsdfsd=",
    "conversationIndex": "Adfsdfsdfsdfw==",
    "isDeliveryReceiptRequested": null,
    "isReadReceiptRequested": false,
    "isRead": true,
    "isDraft": true,
    "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkAGNhOWAvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "focused",
    "body": {
        "contentType": "text",
        "content": "Hi, Megan.I have an interest in the Sales Associate position. Please consider my resume, which you can access here... Regards,Alex"
    },
    "sender": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.com"
        }
    },
    "from": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.com"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.com"
            }
        }
    ],
    "ccRecipients": [],
    "bccRecipients": [],
    "replyTo": [],
    "flag": {
        "flagStatus": "notFlagged"
    }
}

```

<span data-ttu-id="8a7f5-163">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="8a7f5-163">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

