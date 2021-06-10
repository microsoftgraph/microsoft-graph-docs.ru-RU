---
title: 'message: replyAll'
description: Ответьте всем получателям сообщения в формате JSON или MIME.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a20827d2ea6c58339f5c1563c2d61354fa6c52d1
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870495"
---
# <a name="message-replyall"></a><span data-ttu-id="e740c-103">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="e740c-103">message: replyAll</span></span>

<span data-ttu-id="e740c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e740c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e740c-105">Ответьте всем получателям [сообщения в](../resources/message.md) формате JSON или MIME.</span><span class="sxs-lookup"><span data-stu-id="e740c-105">Reply to all recipients of a [message](../resources/message.md) using either JSON or MIME format.</span></span>

<span data-ttu-id="e740c-106">При использовании формата JSON:</span><span class="sxs-lookup"><span data-stu-id="e740c-106">When using JSON format:</span></span>
- <span data-ttu-id="e740c-107">Укажите комментарий или **свойство** тела `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="e740c-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="e740c-108">При указании обоих возвращается ошибка http 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="e740c-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="e740c-109">Если исходное сообщение указывает получателя в свойстве **replyTo,** в формате интернет-сообщений [(RFC 2822),](https://www.rfc-editor.org/info/rfc2822)отправьте ответ получателям в **replyTo,** а не получателю из **свойства.**</span><span class="sxs-lookup"><span data-stu-id="e740c-109">If the original message specifies a recipient in the **replyTo** property, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span>

<span data-ttu-id="e740c-110">При использовании формата MIME:</span><span class="sxs-lookup"><span data-stu-id="e740c-110">When using MIME format:</span></span>
- <span data-ttu-id="e740c-111">Укажите соответствующие [заголовки сообщений Интернета](https://tools.ietf.org/html/rfc2076) и [содержимое MIME](https://tools.ietf.org/html/rfc2045), а также закодируйте их в формате **Base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="e740c-111">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="e740c-112">Добавьте все вложения и свойства S/MIME в содержимое MIME.</span><span class="sxs-lookup"><span data-stu-id="e740c-112">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="e740c-113">Этот метод сохраняет сообщение в папке **Отправленные**.</span><span class="sxs-lookup"><span data-stu-id="e740c-113">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="e740c-114">Кроме того, [создайте черновик](../api/message-createreplyall.md)для ответа на сообщение и [отправьте его](../api/message-send.md) позже.</span><span class="sxs-lookup"><span data-stu-id="e740c-114">Alternatively, [create a draft to reply-all to a message](../api/message-createreplyall.md), and [send](../api/message-send.md) it later.</span></span>

## <a name="permissions"></a><span data-ttu-id="e740c-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e740c-115">Permissions</span></span>
<span data-ttu-id="e740c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e740c-p102">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e740c-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e740c-118">Permission type</span></span>      | <span data-ttu-id="e740c-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e740c-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e740c-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e740c-120">Delegated (work or school account)</span></span> | <span data-ttu-id="e740c-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e740c-121">Mail.Send</span></span>    |
|<span data-ttu-id="e740c-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e740c-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e740c-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e740c-123">Mail.Send</span></span>    |
|<span data-ttu-id="e740c-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e740c-124">Application</span></span> | <span data-ttu-id="e740c-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e740c-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="e740c-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e740c-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="e740c-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e740c-127">Request headers</span></span>
| <span data-ttu-id="e740c-128">Имя</span><span class="sxs-lookup"><span data-stu-id="e740c-128">Name</span></span>       | <span data-ttu-id="e740c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e740c-129">Type</span></span> | <span data-ttu-id="e740c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e740c-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e740c-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="e740c-131">Authorization</span></span>  | <span data-ttu-id="e740c-132">string</span><span class="sxs-lookup"><span data-stu-id="e740c-132">string</span></span>  | <span data-ttu-id="e740c-133">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="e740c-133">Bearer {token}.</span></span> <span data-ttu-id="e740c-134">Обязательный</span><span class="sxs-lookup"><span data-stu-id="e740c-134">Required</span></span>|
| <span data-ttu-id="e740c-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e740c-135">Content-Type</span></span> | <span data-ttu-id="e740c-136">string</span><span class="sxs-lookup"><span data-stu-id="e740c-136">string</span></span>  | <span data-ttu-id="e740c-137">Характер данных в теле объекта.</span><span class="sxs-lookup"><span data-stu-id="e740c-137">Nature of the data in the body of an entity.</span></span> <span data-ttu-id="e740c-138">Обязательный</span><span class="sxs-lookup"><span data-stu-id="e740c-138">Required</span></span> <br/> <span data-ttu-id="e740c-139">Использование `application/json` объекта JSON и `text/plain` контента MIME</span><span class="sxs-lookup"><span data-stu-id="e740c-139">Use `application/json` for a JSON object and `text/plain` for MIME content</span></span> |

## <a name="request-body"></a><span data-ttu-id="e740c-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e740c-140">Request body</span></span>
<span data-ttu-id="e740c-141">При использовании формата JSON укажите объект JSON со следующими параметрами.</span><span class="sxs-lookup"><span data-stu-id="e740c-141">When using JSON format, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e740c-142">Параметр</span><span class="sxs-lookup"><span data-stu-id="e740c-142">Parameter</span></span>    | <span data-ttu-id="e740c-143">Тип</span><span class="sxs-lookup"><span data-stu-id="e740c-143">Type</span></span>   |<span data-ttu-id="e740c-144">Описание</span><span class="sxs-lookup"><span data-stu-id="e740c-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e740c-145">comment</span><span class="sxs-lookup"><span data-stu-id="e740c-145">comment</span></span>|<span data-ttu-id="e740c-146">String</span><span class="sxs-lookup"><span data-stu-id="e740c-146">String</span></span>|<span data-ttu-id="e740c-p105">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="e740c-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="e740c-149">message</span><span class="sxs-lookup"><span data-stu-id="e740c-149">message</span></span>|[<span data-ttu-id="e740c-150">message</span><span class="sxs-lookup"><span data-stu-id="e740c-150">message</span></span>](../resources/message.md)|<span data-ttu-id="e740c-151">Любые свойства, которые можно записать для обновления в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="e740c-151">Any writeable properties to update in the reply message.</span></span>|

<span data-ttu-id="e740c-152">При указании тела в формате MIME укажите содержимое MIME с применимыми заглавными сообщениями в Интернете, все закодированные в **формате base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="e740c-152">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers, all encoded in **base64** format in the request body.</span></span> <span data-ttu-id="e740c-153">Этот метод загружает отправитель и всех получателей исходного сообщения в качестве получателей нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="e740c-153">This method loads the sender and all recipients of the original message as recipients of the new message.</span></span>

## <a name="response"></a><span data-ttu-id="e740c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="e740c-154">Response</span></span>

<span data-ttu-id="e740c-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e740c-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="e740c-157">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает `400 Bad request` и следующее сообщение об ошибке: "Недопустимая строка Base 64 для содержимого MIME".</span><span class="sxs-lookup"><span data-stu-id="e740c-157">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="e740c-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="e740c-158">Examples</span></span>
### <a name="example-1-reply-all-to-a-message-in-json-format"></a><span data-ttu-id="e740c-159">Пример 1. Ответ на сообщение в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e740c-159">Example 1: Reply-all to a message in JSON format</span></span>
<span data-ttu-id="e740c-160">В следующем примере содержится комментарий и добавляется вложение в сообщение для всех ответов.</span><span class="sxs-lookup"><span data-stu-id="e740c-160">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="e740c-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="e740c-161">Request</span></span>
<span data-ttu-id="e740c-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e740c-162">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e740c-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="e740c-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll
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
    "comment": "Please take a look at the attached guidelines before you decide on the name." 
}
```
# <a name="c"></a>[<span data-ttu-id="e740c-164">C#</span><span class="sxs-lookup"><span data-stu-id="e740c-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e740c-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e740c-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e740c-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e740c-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e740c-167">Java</span><span class="sxs-lookup"><span data-stu-id="e740c-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e740c-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="e740c-168">Response</span></span>
<span data-ttu-id="e740c-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e740c-169">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reply-all-to-a-message-in-mime-format"></a><span data-ttu-id="e740c-170">Пример 2. Ответ на сообщение в формате MIME</span><span class="sxs-lookup"><span data-stu-id="e740c-170">Example 2: Reply-all to a message in MIME format</span></span>
##### <a name="request"></a><span data-ttu-id="e740c-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="e740c-171">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_replyAll_mime_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/replyAll
Content-Type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM...

```

##### <a name="response"></a><span data-ttu-id="e740c-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="e740c-172">Response</span></span>
<span data-ttu-id="e740c-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e740c-173">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="e740c-174">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e740c-174">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


