---
title: 'message: createForward'
description: Создайте черновик для перенаадки существующего сообщения в формате JSON или MIME.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4f43bf932e207574d03a788e29cc884432e90919
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645558"
---
# <a name="message-createforward"></a><span data-ttu-id="2d9fa-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="2d9fa-103">message: createForward</span></span>

<span data-ttu-id="2d9fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d9fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d9fa-105">Создайте черновик для перенаадки существующего [сообщения](../resources/message.md)в формате JSON или MIME.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-105">Create a draft to forward an existing [message](../resources/message.md), in either JSON or MIME format.</span></span>

<span data-ttu-id="2d9fa-106">При использовании формата JSON можно:</span><span class="sxs-lookup"><span data-stu-id="2d9fa-106">When using JSON format, you can:</span></span> 
- <span data-ttu-id="2d9fa-107">Укажите комментарий или **свойство** тела `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="2d9fa-108">При указании обоих возвращается ошибка http 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="2d9fa-109">Укажите `toRecipients` параметр или **свойство toRecipients** `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-109">Specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="2d9fa-110">Указание обоих или указаний не возвращает ошибку http 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-110">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="2d9fa-111">[Обнови](../api/message-update.md) проект позже, чтобы добавить содержимое в **тело** или изменить другие свойства сообщения.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-111">[Update](../api/message-update.md) the draft later to add content to the **body** or change other message properties.</span></span>

<span data-ttu-id="2d9fa-112">При использовании формата MIME:</span><span class="sxs-lookup"><span data-stu-id="2d9fa-112">When using MIME format:</span></span>
- <span data-ttu-id="2d9fa-113">Предоформим соответствующие заголовки интернет-сообщений и [содержимое MIME](https://tools.ietf.org/html/rfc2045), все закодированные в [](https://tools.ietf.org/html/rfc2076) **формате base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-113">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="2d9fa-114">Добавьте все вложения и свойства S/MIME в содержимое MIME.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-114">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="2d9fa-115">[Отправка](../api/message-send.md) черновика сообщения в последующей операции.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-115">[Send](../api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="2d9fa-116">Кроме того, [переадрисуем сообщение](../api/message-forward.md) в одной операции.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-116">Alternatively, [forward a message](../api/message-forward.md) in a single operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d9fa-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d9fa-117">Permissions</span></span>
<span data-ttu-id="2d9fa-118">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-118">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="2d9fa-119">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d9fa-119">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d9fa-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d9fa-120">Permission type</span></span>      | <span data-ttu-id="2d9fa-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d9fa-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d9fa-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d9fa-122">Delegated (work or school account)</span></span> | <span data-ttu-id="2d9fa-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d9fa-123">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2d9fa-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d9fa-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d9fa-125">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d9fa-125">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2d9fa-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d9fa-126">Application</span></span> | <span data-ttu-id="2d9fa-127">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d9fa-127">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d9fa-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d9fa-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="2d9fa-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d9fa-129">Request headers</span></span>
| <span data-ttu-id="2d9fa-130">Имя</span><span class="sxs-lookup"><span data-stu-id="2d9fa-130">Name</span></span>       | <span data-ttu-id="2d9fa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2d9fa-131">Type</span></span> | <span data-ttu-id="2d9fa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2d9fa-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2d9fa-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d9fa-133">Authorization</span></span>  | <span data-ttu-id="2d9fa-134">string</span><span class="sxs-lookup"><span data-stu-id="2d9fa-134">string</span></span>  | <span data-ttu-id="2d9fa-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="2d9fa-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d9fa-137">Content-Type</span></span> | <span data-ttu-id="2d9fa-138">string</span><span class="sxs-lookup"><span data-stu-id="2d9fa-138">string</span></span>  | <span data-ttu-id="2d9fa-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-p105">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="2d9fa-141">Используйте `application/json` для объекта JSON и `text/plain` контента MIME.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-141">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d9fa-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d9fa-142">Request body</span></span>
<span data-ttu-id="2d9fa-143">Чтобы отправить объект JSON, укажи следующие параметры.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-143">To send a JSON object provide the following parameters.</span></span>

| <span data-ttu-id="2d9fa-144">Параметр</span><span class="sxs-lookup"><span data-stu-id="2d9fa-144">Parameter</span></span>    | <span data-ttu-id="2d9fa-145">Тип</span><span class="sxs-lookup"><span data-stu-id="2d9fa-145">Type</span></span>   |<span data-ttu-id="2d9fa-146">Описание</span><span class="sxs-lookup"><span data-stu-id="2d9fa-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d9fa-147">comment</span><span class="sxs-lookup"><span data-stu-id="2d9fa-147">comment</span></span>|<span data-ttu-id="2d9fa-148">String</span><span class="sxs-lookup"><span data-stu-id="2d9fa-148">String</span></span>|<span data-ttu-id="2d9fa-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="2d9fa-151">toRecipients</span><span class="sxs-lookup"><span data-stu-id="2d9fa-151">toRecipients</span></span>|<span data-ttu-id="2d9fa-152">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="2d9fa-152">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="2d9fa-153">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-153">The list of recipients.</span></span>|
|<span data-ttu-id="2d9fa-154">message</span><span class="sxs-lookup"><span data-stu-id="2d9fa-154">message</span></span>|[<span data-ttu-id="2d9fa-155">message</span><span class="sxs-lookup"><span data-stu-id="2d9fa-155">message</span></span>](../resources/message.md)|<span data-ttu-id="2d9fa-156">Любые свойства, которые можно записать для обновления в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-156">Any writeable properties to update in the reply message.</span></span>|

<span data-ttu-id="2d9fa-157">При указании тела в формате MIME укажите содержимое MIME с применимыми заглавными интернет-сообщениями ("To", "CC", "BCC", "Subject"), все закодированные в **формате base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-157">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="2d9fa-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d9fa-158">Response</span></span>

<span data-ttu-id="2d9fa-159">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-159">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="2d9fa-160">Если в тексте запроса содержится неправильное содержимое MIME, этот метод возвращается и следующее сообщение об ошибке: "Недействительные строки `400 Bad request` base64 для контента MIME".</span><span class="sxs-lookup"><span data-stu-id="2d9fa-160">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="2d9fa-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="2d9fa-161">Examples</span></span>

### <a name="example-1-create-a-draft-message-in-json-format-to-forward-an-existing-message"></a><span data-ttu-id="2d9fa-162">Пример 1. Создание черновика сообщения в формате JSON для переададки существующего сообщения</span><span class="sxs-lookup"><span data-stu-id="2d9fa-162">Example 1: Create a draft message in JSON format to forward an existing message</span></span>
<span data-ttu-id="2d9fa-163">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-163">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2d9fa-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d9fa-164">Request</span></span>
<span data-ttu-id="2d9fa-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-165">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2d9fa-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d9fa-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/createForward
Content-Type: application/json

{
  "message":{  
    "isDeliveryReceiptRequested": true,
    "toRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ]
  },
  "comment": "Dana, just want to make sure you get this; you'll need this if the project gets approved." 
}
```
# <a name="c"></a>[<span data-ttu-id="2d9fa-167">C#</span><span class="sxs-lookup"><span data-stu-id="2d9fa-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createforward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d9fa-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d9fa-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createforward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d9fa-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d9fa-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createforward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d9fa-170">Java</span><span class="sxs-lookup"><span data-stu-id="2d9fa-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createforward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2d9fa-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d9fa-171">Response</span></span>
<span data-ttu-id="2d9fa-p107">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-p107">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 272

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKqAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DQ\"",
  "id": "AAMkADA1MTAAAH5JKqAAA=",
  "subject": "FW: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body>\r\nDana, just want to make sure you get this; you'll need this if the project gets approved.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:47:54 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group</body>\r\n</html>\r\n"
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
        "name": "Dana Swope",
        "address": "danas@contoso.onmicrosoft.com"
      }
    }
  ]
}
```


### <a name="example-2-create-a-draft-message-in-mime-format-to-forward-an-existing-message"></a><span data-ttu-id="2d9fa-174">Пример 2. Создание черновика сообщения в формате MIME для переададки существующего сообщения</span><span class="sxs-lookup"><span data-stu-id="2d9fa-174">Example 2: Create a draft message in MIME format to forward an existing message</span></span>

##### <a name="request"></a><span data-ttu-id="2d9fa-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d9fa-175">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createForward_mime_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/createForward
Content-Type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM6IEludGVybmFsIFJlc3VtZSBTdWJtaXNzaW9uOiBT
YWxlcyBBc3NvY2lhdGUKVGhyZWFkLUluZGV4OiBjb2RlY29kZWNvZGVoZXJlaGVyZWhlcmUKRGF0
ZTogU3VuLCAyOCBGZWIgMjAyMSAwNzoxNTowMCArMDAwMApNZXNzYWdlLUlEOgoJPE1XSFBSMTMw
MU1CMjAwMDAwMDAwRDc2RDlDMjgyMjAwMDA5QUQ5QTlASFdIUFIxMzAxTUIwMDAwLmNvZGVudW0u
cHJvZC5vdXRsb29rLmNvbT4KQ29udGVudC1MYW5ndWFnZTogZW4tVVMKWC1NUy1IYXMtQXR0YWNo
OgpYLU1TLVRORUYtQ29ycmVsYXRvcjoKWC1NUy1FeGNoYW5n
```
##### <a name="response"></a><span data-ttu-id="2d9fa-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d9fa-176">Response</span></span>
<span data-ttu-id="2d9fa-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-177">Here is an example of the response.</span></span>

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

<span data-ttu-id="2d9fa-178">Если в тексте запроса содержится недооформленное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="2d9fa-178">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
