---
title: 'message: createReplyAll'
description: Создайте черновик для ответа отправителю и всем получателям указанного сообщения в формате JSON или MIME.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2d1b3970995db5e3d678e0e1b6daeef6a72ee40b
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870418"
---
# <a name="message-createreplyall"></a><span data-ttu-id="45606-103">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="45606-103">message: createReplyAll</span></span>

<span data-ttu-id="45606-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45606-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="45606-105">Создайте черновик для ответа отправителю и [](../resources/message.md) всем получателям сообщения в формате JSON или MIME.</span><span class="sxs-lookup"><span data-stu-id="45606-105">Create a draft to reply to the sender and all recipients of a [message](../resources/message.md) in either JSON or MIME format.</span></span> 

<span data-ttu-id="45606-106">При использовании формата JSON:</span><span class="sxs-lookup"><span data-stu-id="45606-106">When using JSON format:</span></span>
- <span data-ttu-id="45606-107">Укажите комментарий или **свойство** тела `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="45606-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="45606-108">При указании обоих возвращается ошибка http 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="45606-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="45606-109">Если исходное сообщение указывает получателя в свойстве **replyTo,** в формате интернет-сообщений  [(RFC 2822),](https://www.rfc-editor.org/info/rfc2822)необходимо отправить ответ получателям в **свойствах replyTo** и **toRecipients,** а не получателям в свойствах from and **toRecipients.**</span><span class="sxs-lookup"><span data-stu-id="45606-109">If the original message specifies a recipient in the **replyTo** property, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the **replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 
- <span data-ttu-id="45606-110">Вы можете [обновить проект](../api/message-update.md) позже, чтобы добавить содержимое ответа в **тело или** изменить другие свойства сообщения.</span><span class="sxs-lookup"><span data-stu-id="45606-110">You can [update](../api/message-update.md) the draft later to add reply content to the **body** or change other message properties.</span></span>

<span data-ttu-id="45606-111">При использовании формата MIME:</span><span class="sxs-lookup"><span data-stu-id="45606-111">When using MIME format:</span></span>
- <span data-ttu-id="45606-112">Укажите соответствующие [заголовки сообщений Интернета](https://tools.ietf.org/html/rfc2076) и [содержимое MIME](https://tools.ietf.org/html/rfc2045), а также закодируйте их в формате **Base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="45606-112">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="45606-113">Добавьте все вложения и свойства S/MIME в содержимое MIME.</span><span class="sxs-lookup"><span data-stu-id="45606-113">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="45606-114">[Отправьте](../api/message-send.md) черновик сообщения в ходе последующей операции.</span><span class="sxs-lookup"><span data-stu-id="45606-114">[Send](../api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="45606-115">Кроме того, [ответьте всем на сообщение](../api/message-replyall.md) в одном действии.</span><span class="sxs-lookup"><span data-stu-id="45606-115">Alternatively, [reply-all to a message](../api/message-replyall.md) in a single action.</span></span>

## <a name="permissions"></a><span data-ttu-id="45606-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45606-116">Permissions</span></span>
<span data-ttu-id="45606-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45606-p102">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45606-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45606-119">Permission type</span></span>      | <span data-ttu-id="45606-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45606-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45606-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45606-121">Delegated (work or school account)</span></span> | <span data-ttu-id="45606-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45606-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="45606-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45606-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45606-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45606-124">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="45606-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45606-125">Application</span></span> | <span data-ttu-id="45606-126">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45606-126">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="45606-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45606-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```

## <a name="request-headers"></a><span data-ttu-id="45606-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45606-128">Request headers</span></span>
| <span data-ttu-id="45606-129">Имя</span><span class="sxs-lookup"><span data-stu-id="45606-129">Name</span></span>       | <span data-ttu-id="45606-130">Тип</span><span class="sxs-lookup"><span data-stu-id="45606-130">Type</span></span> | <span data-ttu-id="45606-131">Описание</span><span class="sxs-lookup"><span data-stu-id="45606-131">Description</span></span>| 
|:---------------|:--------|:----------|
| <span data-ttu-id="45606-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="45606-132">Authorization</span></span>  | <span data-ttu-id="45606-133">string</span><span class="sxs-lookup"><span data-stu-id="45606-133">string</span></span>  | <span data-ttu-id="45606-134">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="45606-134">Bearer {token}.</span></span> <span data-ttu-id="45606-135">Обязательный</span><span class="sxs-lookup"><span data-stu-id="45606-135">Required</span></span> |
| <span data-ttu-id="45606-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="45606-136">Content-Type</span></span> | <span data-ttu-id="45606-137">string</span><span class="sxs-lookup"><span data-stu-id="45606-137">string</span></span>  | <span data-ttu-id="45606-138">Характер данных в теле объекта.</span><span class="sxs-lookup"><span data-stu-id="45606-138">Nature of the data in the body of an entity.</span></span> <br/> <span data-ttu-id="45606-139">Используйте `application/json` для объекта JSON и `text/plain` для содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="45606-139">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45606-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45606-140">Request body</span></span>
<span data-ttu-id="45606-141">Этот метод не требует тела запроса.</span><span class="sxs-lookup"><span data-stu-id="45606-141">This method does not require a request body.</span></span> 

<span data-ttu-id="45606-142">Однако для создания проекта replyAll с помощью формата MIME уделяйте контенту MIME применимые заглавные сообщения в Интернете, все закодированные в формате **base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="45606-142">However, for creating a replyAll draft using MIME format, provide the MIME content with the applicable Internet message headers, all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="45606-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="45606-143">Response</span></span>

<span data-ttu-id="45606-144">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45606-144">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="45606-145">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает `400 Bad request` и следующее сообщение об ошибке: "Недопустимая строка Base 64 для содержимого MIME".</span><span class="sxs-lookup"><span data-stu-id="45606-145">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="45606-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="45606-146">Examples</span></span>
### <a name="example-1-create-a-message-draft-in-json-format-to-reply-all-to-an-existing-message"></a><span data-ttu-id="45606-147">Пример 1. Создание черновика сообщения в формате JSON, чтобы ответить всем на существующее сообщение</span><span class="sxs-lookup"><span data-stu-id="45606-147">Example 1: Create a message draft in JSON format to reply-all to an existing message</span></span>
<span data-ttu-id="45606-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="45606-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="45606-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="45606-149">Request</span></span>
<span data-ttu-id="45606-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45606-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45606-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="45606-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReplyAll
```
# <a name="c"></a>[<span data-ttu-id="45606-152">C#</span><span class="sxs-lookup"><span data-stu-id="45606-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreplyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45606-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45606-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreplyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45606-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45606-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreplyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45606-155">Java</span><span class="sxs-lookup"><span data-stu-id="45606-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreplyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="45606-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="45606-156">Response</span></span>
<span data-ttu-id="45606-p104">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="45606-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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
### <a name="example-2-create-a-message-draft-in-mime-format-to-reply-all-to-an-existing-message"></a><span data-ttu-id="45606-159">Пример 2. Создание черновика сообщения в формате MIME, чтобы ответить всем на существующее сообщение</span><span class="sxs-lookup"><span data-stu-id="45606-159">Example 2: Create a message draft in MIME format to reply-all to an existing message</span></span>
##### <a name="request"></a><span data-ttu-id="45606-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="45606-160">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_createreplyAll_mime_v1"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAH5JaLAAA=/createReplyAll
Content-type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np
```

##### <a name="response"></a><span data-ttu-id="45606-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="45606-161">Response</span></span>
<span data-ttu-id="45606-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="45606-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.message",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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

<span data-ttu-id="45606-163">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="45606-163">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

