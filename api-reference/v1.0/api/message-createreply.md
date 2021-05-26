---
title: 'message: createReply'
description: 'Создайте черновик для ответа на сообщение в формате JSON или MIME. '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 023b04f37f0320ca3a74801f9d2e92d19553a10c
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645600"
---
# <a name="message-createreply"></a><span data-ttu-id="8250b-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="8250b-103">message: createReply</span></span>

<span data-ttu-id="8250b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8250b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8250b-105">Создайте черновик для ответа отправителю сообщения в формате JSON или MIME. [](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="8250b-105">Create a draft to reply to the sender of a [message](../resources/message.md) in either JSON or MIME format.</span></span>

<span data-ttu-id="8250b-106">При использовании формата JSON:</span><span class="sxs-lookup"><span data-stu-id="8250b-106">When using JSON format:</span></span>
- <span data-ttu-id="8250b-107">Укажите комментарий или **свойство** тела `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="8250b-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="8250b-108">При указании обоих возвращается ошибка http 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="8250b-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="8250b-109">Если replyTo указывается в исходном сообщении в формате интернет-сообщений [(RFC 2822),](https://www.rfc-editor.org/info/rfc2822)необходимо отправить ответ получателям в **replyTo,** а не получателям из **.** </span><span class="sxs-lookup"><span data-stu-id="8250b-109">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span>
- <span data-ttu-id="8250b-110">Вы можете [обновить проект](../api/message-update.md) позже, чтобы добавить содержимое ответа в **тело или** изменить другие свойства сообщения.</span><span class="sxs-lookup"><span data-stu-id="8250b-110">You can [update](../api/message-update.md) the draft later to add reply content to the **body** or change other message properties.</span></span>

<span data-ttu-id="8250b-111">При использовании формата MIME:</span><span class="sxs-lookup"><span data-stu-id="8250b-111">When using MIME format:</span></span>
- <span data-ttu-id="8250b-112">Предоформим соответствующие заголовки интернет-сообщений и [содержимое MIME](https://tools.ietf.org/html/rfc2045), все закодированные в [](https://tools.ietf.org/html/rfc2076) **формате base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="8250b-112">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="8250b-113">Добавьте все вложения и свойства S/MIME в содержимое MIME.</span><span class="sxs-lookup"><span data-stu-id="8250b-113">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="8250b-114">[Отправка](../api/message-send.md) черновика сообщения в последующей операции.</span><span class="sxs-lookup"><span data-stu-id="8250b-114">[Send](../api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="8250b-115">Кроме того, [ответьте на сообщение в](../api/message-reply.md) одной операции.</span><span class="sxs-lookup"><span data-stu-id="8250b-115">Alternatively, [reply to a message](../api/message-reply.md) in a single operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="8250b-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8250b-116">Permissions</span></span>
<span data-ttu-id="8250b-117">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="8250b-117">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="8250b-118">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8250b-118">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8250b-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8250b-119">Permission type</span></span>      | <span data-ttu-id="8250b-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8250b-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8250b-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8250b-121">Delegated (work or school account)</span></span> | <span data-ttu-id="8250b-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8250b-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8250b-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8250b-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8250b-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8250b-124">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8250b-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8250b-125">Application</span></span> | <span data-ttu-id="8250b-126">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8250b-126">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8250b-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8250b-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```

## <a name="request-headers"></a><span data-ttu-id="8250b-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8250b-128">Request headers</span></span>
| <span data-ttu-id="8250b-129">Имя</span><span class="sxs-lookup"><span data-stu-id="8250b-129">Name</span></span>       | <span data-ttu-id="8250b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8250b-130">Type</span></span> | <span data-ttu-id="8250b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8250b-131">Description</span></span>| 
|:---------------|:--------|:----------|
| <span data-ttu-id="8250b-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="8250b-132">Authorization</span></span>  | <span data-ttu-id="8250b-133">string</span><span class="sxs-lookup"><span data-stu-id="8250b-133">string</span></span>  | <span data-ttu-id="8250b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8250b-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="8250b-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8250b-136">Content-Type</span></span> | <span data-ttu-id="8250b-137">string</span><span class="sxs-lookup"><span data-stu-id="8250b-137">string</span></span>  | <span data-ttu-id="8250b-138">Характер данных в теле объекта.</span><span class="sxs-lookup"><span data-stu-id="8250b-138">Nature of the data in the body of an entity.</span></span> <br/> <span data-ttu-id="8250b-139">Используйте `application/json` для объекта JSON и `text/plain` контента MIME.</span><span class="sxs-lookup"><span data-stu-id="8250b-139">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8250b-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8250b-140">Request body</span></span>
<span data-ttu-id="8250b-141">Этот метод не требует тела запроса.</span><span class="sxs-lookup"><span data-stu-id="8250b-141">This method does not require a request body.</span></span>

<span data-ttu-id="8250b-142">Однако для создания черновика ответа с помощью формата MIME предопрейте контент MIME применимыми заглавными сообщениями в Интернете, все закодированные в формате **base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="8250b-142">However, for creating a reply draft using MIME format, provide the MIME content with the applicable Internet message headers, all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="8250b-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="8250b-143">Response</span></span>

<span data-ttu-id="8250b-144">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8250b-144">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="8250b-145">Если в тексте запроса содержится неправильное содержимое MIME, этот метод возвращается и следующее сообщение об ошибке: "Недействительные строки `400 Bad request` base64 для контента MIME".</span><span class="sxs-lookup"><span data-stu-id="8250b-145">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="8250b-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="8250b-146">Examples</span></span>
### <a name="example-1-create-a-draft-message-in-json-format-to-reply-to-an-existing-message"></a><span data-ttu-id="8250b-147">Пример 1. Создание черновика сообщения в формате JSON для ответа на существующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="8250b-147">Example 1: Create a draft message in JSON format to reply to an existing message.</span></span>
<span data-ttu-id="8250b-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8250b-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8250b-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="8250b-149">Request</span></span>
<span data-ttu-id="8250b-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8250b-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8250b-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="8250b-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReply
```
# <a name="c"></a>[<span data-ttu-id="8250b-152">C#</span><span class="sxs-lookup"><span data-stu-id="8250b-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8250b-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8250b-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8250b-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8250b-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8250b-155">Java</span><span class="sxs-lookup"><span data-stu-id="8250b-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8250b-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="8250b-156">Response</span></span>
<span data-ttu-id="8250b-p104">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8250b-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-create-a-draft-message-in-mime-format-to-reply-to-an-existing-message"></a><span data-ttu-id="8250b-159">Пример 2. Создание черновика сообщения в формате MIME для ответа на существующее сообщение</span><span class="sxs-lookup"><span data-stu-id="8250b-159">Example 2: Create a draft message in MIME format to reply to an existing message</span></span>
##### <a name="request"></a><span data-ttu-id="8250b-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="8250b-160">Request</span></span>
<!-- {
  "blockType": "request",
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

##### <a name="response"></a><span data-ttu-id="8250b-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="8250b-161">Response</span></span>
<span data-ttu-id="8250b-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8250b-162">Here is an example of the response.</span></span>
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

<span data-ttu-id="8250b-163">Если в тексте запроса содержится недооформленное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="8250b-163">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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

