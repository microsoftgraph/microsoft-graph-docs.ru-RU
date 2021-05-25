---
title: 'message: createReplyAll'
description: Создание черновика для ответа всем получателям сообщения в формате JSON или MIME
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9eac6d007e77d6e4e840299d8ac50530dd3172b3
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645579"
---
# <a name="message-createreplyall"></a><span data-ttu-id="2e55a-103">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="2e55a-103">message: createReplyAll</span></span>

<span data-ttu-id="2e55a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e55a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e55a-105">Создайте черновик для ответа отправителю и [](../resources/message.md) всем получателям сообщения в формате JSON или MIME.</span><span class="sxs-lookup"><span data-stu-id="2e55a-105">Create a draft to reply to the sender and all recipients of a [message](../resources/message.md) in either JSON or MIME format.</span></span>

<span data-ttu-id="2e55a-106">При использовании формата JSON:</span><span class="sxs-lookup"><span data-stu-id="2e55a-106">When using JSON format:</span></span>
- <span data-ttu-id="2e55a-107">Укажите комментарий или **свойство** тела `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="2e55a-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="2e55a-108">При указании обоих возвращается ошибка http 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="2e55a-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="2e55a-109">Если исходное сообщение указывает получателя в свойстве **replyTo,** в формате интернет-сообщений  [(RFC 2822),](https://www.rfc-editor.org/info/rfc2822)необходимо отправить ответ получателям в **свойствах replyTo** и **toRecipients,** а не получателям в свойствах from and **toRecipients.**</span><span class="sxs-lookup"><span data-stu-id="2e55a-109">If the original message specifies a recipient in the **replyTo** property, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the **replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 
- <span data-ttu-id="2e55a-110">Вы можете [обновить](../api/message-update.md) черновик сообщения позже.</span><span class="sxs-lookup"><span data-stu-id="2e55a-110">You can [update](../api/message-update.md) the draft message later.</span></span>

<span data-ttu-id="2e55a-111">При использовании формата MIME:</span><span class="sxs-lookup"><span data-stu-id="2e55a-111">When using MIME format:</span></span>
- <span data-ttu-id="2e55a-112">Предоформим соответствующие заголовки интернет-сообщений и [содержимое MIME](https://tools.ietf.org/html/rfc2045), все закодированные в [](https://tools.ietf.org/html/rfc2076) **формате base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="2e55a-112">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="2e55a-113">Добавьте все вложения и свойства S/MIME в содержимое MIME.</span><span class="sxs-lookup"><span data-stu-id="2e55a-113">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="2e55a-114">[Отправка](../api/message-send.md) черновика сообщения в последующей операции.</span><span class="sxs-lookup"><span data-stu-id="2e55a-114">[Send](../api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="2e55a-115">Кроме того, [ответьте всем на сообщение](../api/message-replyall.md) в одном действии.</span><span class="sxs-lookup"><span data-stu-id="2e55a-115">Alternatively, [reply-all to a message](../api/message-replyall.md) in a single action.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e55a-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e55a-116">Permissions</span></span>
<span data-ttu-id="2e55a-117">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="2e55a-117">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="2e55a-118">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e55a-118">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e55a-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e55a-119">Permission type</span></span>      | <span data-ttu-id="2e55a-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e55a-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e55a-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e55a-121">Delegated (work or school account)</span></span> | <span data-ttu-id="2e55a-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e55a-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2e55a-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e55a-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e55a-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e55a-124">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2e55a-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e55a-125">Application</span></span> | <span data-ttu-id="2e55a-126">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e55a-126">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e55a-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e55a-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="2e55a-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e55a-128">Request headers</span></span>
| <span data-ttu-id="2e55a-129">Имя</span><span class="sxs-lookup"><span data-stu-id="2e55a-129">Name</span></span>       | <span data-ttu-id="2e55a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2e55a-130">Type</span></span> | <span data-ttu-id="2e55a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2e55a-131">Description</span></span>| 
|:---------------|:--------|:----------|
| <span data-ttu-id="2e55a-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e55a-132">Authorization</span></span>  | <span data-ttu-id="2e55a-133">string</span><span class="sxs-lookup"><span data-stu-id="2e55a-133">string</span></span>  | <span data-ttu-id="2e55a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e55a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2e55a-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2e55a-136">Content-Type</span></span> | <span data-ttu-id="2e55a-137">string</span><span class="sxs-lookup"><span data-stu-id="2e55a-137">string</span></span>  | <span data-ttu-id="2e55a-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e55a-p104">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="2e55a-140">Используйте `application/json` для объекта JSON и `text/plain` контента MIME.</span><span class="sxs-lookup"><span data-stu-id="2e55a-140">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e55a-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e55a-141">Request body</span></span>
<span data-ttu-id="2e55a-142">При использовании формата JSON укажи объект JSON со следующими параметрами.</span><span class="sxs-lookup"><span data-stu-id="2e55a-142">When using JSON format, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2e55a-143">Параметр</span><span class="sxs-lookup"><span data-stu-id="2e55a-143">Parameter</span></span>    | <span data-ttu-id="2e55a-144">Тип</span><span class="sxs-lookup"><span data-stu-id="2e55a-144">Type</span></span>   |<span data-ttu-id="2e55a-145">Описание</span><span class="sxs-lookup"><span data-stu-id="2e55a-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e55a-146">comment</span><span class="sxs-lookup"><span data-stu-id="2e55a-146">comment</span></span>|<span data-ttu-id="2e55a-147">String</span><span class="sxs-lookup"><span data-stu-id="2e55a-147">String</span></span>|<span data-ttu-id="2e55a-p105">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="2e55a-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="2e55a-150">message</span><span class="sxs-lookup"><span data-stu-id="2e55a-150">message</span></span>|[<span data-ttu-id="2e55a-151">message</span><span class="sxs-lookup"><span data-stu-id="2e55a-151">message</span></span>](../resources/message.md)|<span data-ttu-id="2e55a-152">Любые свойства для записи, которые необходимо обновить в сообщении для всех ответов.</span><span class="sxs-lookup"><span data-stu-id="2e55a-152">Any writeable properties to update in the reply-all message.</span></span>|

<span data-ttu-id="2e55a-153">При указании тела в формате MIME укажите содержимое MIME с применимыми заглавными сообщениями в Интернете, все закодированные в **формате base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="2e55a-153">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers, all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="2e55a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e55a-154">Response</span></span>

<span data-ttu-id="2e55a-155">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2e55a-155">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="2e55a-156">Если в тексте запроса содержится неправильное содержимое MIME, этот метод возвращается и следующее сообщение об ошибке: "Недействительные строки `400 Bad request` base64 для контента MIME".</span><span class="sxs-lookup"><span data-stu-id="2e55a-156">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="2e55a-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="2e55a-157">Examples</span></span>
### <a name="example-1-create-a-draft-in-json-format-to-reply-all-to-an-existing-message"></a><span data-ttu-id="2e55a-158">Пример 1. Создание черновика в формате JSON для ответа всех на существующее сообщение</span><span class="sxs-lookup"><span data-stu-id="2e55a-158">Example 1: Create a draft in JSON format to reply-all to an existing message</span></span>
<span data-ttu-id="2e55a-159">В следующем примере создается черновик для ответа всех и добавляется вложение и комментарий в одном **вызове createReplyAll.**</span><span class="sxs-lookup"><span data-stu-id="2e55a-159">The following example creates a draft to reply all, and adds an attachment and comment all in one **createReplyAll** call.</span></span>
##### <a name="request"></a><span data-ttu-id="2e55a-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e55a-160">Request</span></span>
<span data-ttu-id="2e55a-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e55a-161">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e55a-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e55a-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/createReplyAll
Content-Type: application/json

{
    "message":{
      "attachments": [ 
        { 
          "@odata.type": "#microsoft.graph.fileAttachment", 
          "name": "guidelines.txt", 
          "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk=" 
        } 
      ]
    },
    "comment": "if the project gets approved, please take a look at the attached guidelines before you decide on the name." 
}
```
# <a name="c"></a>[<span data-ttu-id="2e55a-163">C#</span><span class="sxs-lookup"><span data-stu-id="2e55a-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreplyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e55a-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e55a-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreplyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e55a-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e55a-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreplyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e55a-166">Java</span><span class="sxs-lookup"><span data-stu-id="2e55a-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreplyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2e55a-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e55a-167">Response</span></span>
<span data-ttu-id="2e55a-p106">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2e55a-p106">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKpAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DP\"",
  "id": "AAMkADA1MTAAAH5JKpAAA=",
  "subject": "RE: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body dir=\"ltr\">\r\nif the project gets approved, please take a look at the attached guidelines before you decide on the name.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:36:32 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group\r\n<div>Samantha, Randi, would you name the group please?\r\n<b>From:</b> Samantha Booth<br>\r\n<b>Sent:</b> Friday, March 4, 2016 12:23:35 AM<br>\r\n<b>To:</b> Admin<br>\r\n<b>Subject:</b> Re: Let's start a group</font>\r\n</body>\r\n</html>"
  },
  "sender": {
    "emailAddress": {
      "name": "Admin",
      "address": "admin@contoso.onmicrosoft.com"
    }
  },
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com"
      }
    },
    {
      "emailAddress": {
        "name": "Randi Welch",
        "address": "randiw@contoso.onmicrosoft.com"
      }
    }
  ]
}
```

### <a name="example-2-create-a-draft-using-mime-format-to-reply-all-to-an-existing-message"></a><span data-ttu-id="2e55a-170">Пример 2. Создание проекта с использованием формата MIME для ответа на существующее сообщение</span><span class="sxs-lookup"><span data-stu-id="2e55a-170">Example 2: Create a draft using MIME format to reply-all to an existing message</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreplyall_mime_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/createReplyAll
Content-Type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np...
```
##### <a name="response"></a><span data-ttu-id="2e55a-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e55a-171">Response</span></span>
<span data-ttu-id="2e55a-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2e55a-172">Here is an example of the response.</span></span>

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

<span data-ttu-id="2e55a-173">Если в тексте запроса содержится недооформленное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="2e55a-173">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


