---
title: 'message: reply'
description: Ответ отправилю сообщения в формате JSON или MIME.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e5a9cab87389f41c795268a1d7964a7d8e987269
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870502"
---
# <a name="message-reply"></a><span data-ttu-id="d773b-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="d773b-103">message: reply</span></span>

<span data-ttu-id="d773b-104">Пространство имен: microsoft.graph.</span><span class="sxs-lookup"><span data-stu-id="d773b-104">Namespace: microsoft.graph.</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d773b-105">Ответ отправилю сообщения [в](../resources/message.md) формате JSON или MIME.</span><span class="sxs-lookup"><span data-stu-id="d773b-105">Reply to the sender of a [message](../resources/message.md) using either JSON or MIME format.</span></span>

<span data-ttu-id="d773b-106">При использовании формата JSON:</span><span class="sxs-lookup"><span data-stu-id="d773b-106">When using JSON format:</span></span>
- <span data-ttu-id="d773b-107">Укажите комментарий или **свойство** тела `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="d773b-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="d773b-108">При указании обоих возвращается ошибка http 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="d773b-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="d773b-109">Если исходное сообщение указывает получателя в свойстве **replyTo,** в формате интернет-сообщений [(RFC 2822),](https://www.rfc-editor.org/info/rfc2822)отправьте ответ получателям в **replyTo,** а не получателю из **свойства.**</span><span class="sxs-lookup"><span data-stu-id="d773b-109">If the original message specifies a recipient in the **replyTo** property, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span>

<span data-ttu-id="d773b-110">При использовании формата MIME:</span><span class="sxs-lookup"><span data-stu-id="d773b-110">When using MIME format:</span></span>
- <span data-ttu-id="d773b-111">Укажите соответствующие [заголовки сообщений Интернета](https://tools.ietf.org/html/rfc2076) и [содержимое MIME](https://tools.ietf.org/html/rfc2045), а также закодируйте их в формате **Base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="d773b-111">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="d773b-112">Добавьте все вложения и свойства S/MIME в содержимое MIME.</span><span class="sxs-lookup"><span data-stu-id="d773b-112">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="d773b-113">Этот метод сохраняет сообщение в папке **Отправленные**.</span><span class="sxs-lookup"><span data-stu-id="d773b-113">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="d773b-114">Кроме того, [создайте черновик](../api/message-createreply.md)для ответа на сообщение и [отправьте его](../api/message-send.md) позже.</span><span class="sxs-lookup"><span data-stu-id="d773b-114">Alternatively, [create a draft to reply to a message](../api/message-createreply.md), and [send](../api/message-send.md) it later.</span></span>

## <a name="permissions"></a><span data-ttu-id="d773b-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d773b-115">Permissions</span></span>
<span data-ttu-id="d773b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d773b-p102">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d773b-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d773b-118">Permission type</span></span>      | <span data-ttu-id="d773b-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d773b-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d773b-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d773b-120">Delegated (work or school account)</span></span> | <span data-ttu-id="d773b-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d773b-121">Mail.Send</span></span>    |
|<span data-ttu-id="d773b-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d773b-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d773b-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d773b-123">Mail.Send</span></span>    |
|<span data-ttu-id="d773b-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d773b-124">Application</span></span> | <span data-ttu-id="d773b-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d773b-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="d773b-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d773b-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```

## <a name="request-headers"></a><span data-ttu-id="d773b-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d773b-127">Request headers</span></span>
| <span data-ttu-id="d773b-128">Имя</span><span class="sxs-lookup"><span data-stu-id="d773b-128">Name</span></span>       | <span data-ttu-id="d773b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d773b-129">Type</span></span> | <span data-ttu-id="d773b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d773b-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d773b-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="d773b-131">Authorization</span></span>  | <span data-ttu-id="d773b-132">string</span><span class="sxs-lookup"><span data-stu-id="d773b-132">string</span></span>  | <span data-ttu-id="d773b-133">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="d773b-133">Bearer {token}.</span></span> <span data-ttu-id="d773b-134">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d773b-134">Required</span></span> |
| <span data-ttu-id="d773b-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d773b-135">Content-Type</span></span> | <span data-ttu-id="d773b-136">string</span><span class="sxs-lookup"><span data-stu-id="d773b-136">string</span></span>  | <span data-ttu-id="d773b-137">Характер данных в теле объекта.</span><span class="sxs-lookup"><span data-stu-id="d773b-137">Nature of the data in the body of an entity.</span></span> <span data-ttu-id="d773b-138">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d773b-138">Required</span></span> <br/> <span data-ttu-id="d773b-139">Использование `application/json` объекта JSON и `text/plain` контента MIME</span><span class="sxs-lookup"><span data-stu-id="d773b-139">Use `application/json` for a JSON object and `text/plain` for MIME content</span></span> |

## <a name="request-body"></a><span data-ttu-id="d773b-140">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d773b-140">Request body</span></span>
<span data-ttu-id="d773b-141">При использовании формата JSON включаем объект JSON со следующими параметрами.</span><span class="sxs-lookup"><span data-stu-id="d773b-141">When using JSON format, include a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d773b-142">Параметр</span><span class="sxs-lookup"><span data-stu-id="d773b-142">Parameter</span></span>    | <span data-ttu-id="d773b-143">Тип</span><span class="sxs-lookup"><span data-stu-id="d773b-143">Type</span></span>   |<span data-ttu-id="d773b-144">Описание</span><span class="sxs-lookup"><span data-stu-id="d773b-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d773b-145">comment</span><span class="sxs-lookup"><span data-stu-id="d773b-145">comment</span></span>|<span data-ttu-id="d773b-146">String</span><span class="sxs-lookup"><span data-stu-id="d773b-146">String</span></span>|<span data-ttu-id="d773b-p105">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="d773b-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="d773b-149">message</span><span class="sxs-lookup"><span data-stu-id="d773b-149">message</span></span>|[<span data-ttu-id="d773b-150">message</span><span class="sxs-lookup"><span data-stu-id="d773b-150">message</span></span>](../resources/message.md) | <span data-ttu-id="d773b-151">Любые свойства, которые можно записать для обновления в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="d773b-151">Any writeable properties to update in the reply message.</span></span>|

<span data-ttu-id="d773b-152">При указании тела в формате MIME укажите содержимое MIME с применимыми заглавными сообщениями в Интернете, все закодированные в **формате base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="d773b-152">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers, all encoded in **base64** format in the request body.</span></span> <span data-ttu-id="d773b-153">Этот метод использует отправитель исходного сообщения в качестве получателя.</span><span class="sxs-lookup"><span data-stu-id="d773b-153">This method uses the sender of the original message as recipient.</span></span>

## <a name="response"></a><span data-ttu-id="d773b-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="d773b-154">Response</span></span>

<span data-ttu-id="d773b-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d773b-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="d773b-157">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает `400 Bad request` и следующее сообщение об ошибке: "Недопустимая строка Base 64 для содержимого MIME".</span><span class="sxs-lookup"><span data-stu-id="d773b-157">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="d773b-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="d773b-158">Examples</span></span>
### <a name="example-1-reply-to-a-message-in-json-format"></a><span data-ttu-id="d773b-159">Пример 1. Ответ на сообщение в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d773b-159">Example 1: Reply to a message in JSON format</span></span>
<span data-ttu-id="d773b-160">В следующем примере содержится комментарий и добавляется получатель в ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="d773b-160">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="d773b-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="d773b-161">Request</span></span>
<span data-ttu-id="d773b-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d773b-162">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d773b-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="d773b-163">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "message_reply_beta",
  "sampleKeys": ["AAMkADA1MTAAAAqldOAAA="]
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: application/json

{
  "message":{  
    "toRecipients":[
      {
        "emailAddress": {
          "address":"samanthab@contoso.onmicrosoft.com",
          "name":"Samantha Booth"
        }
      },
      {
        "emailAddress":{
          "address":"randiw@contoso.onmicrosoft.com",
          "name":"Randi Welch"
        }
      }
     ]
  },
  "comment": "Samantha, Randi, would you name the group please?" 
}

```

# <a name="c"></a>[<span data-ttu-id="d773b-164">C#</span><span class="sxs-lookup"><span data-stu-id="d773b-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d773b-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d773b-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d773b-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d773b-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d773b-167">Java</span><span class="sxs-lookup"><span data-stu-id="d773b-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-reply-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d773b-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="d773b-168">Response</span></span>
<span data-ttu-id="d773b-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d773b-169">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reply-to-a-message-in-mime-format"></a><span data-ttu-id="d773b-170">Пример 2. Ответ на сообщение в формате MIME</span><span class="sxs-lookup"><span data-stu-id="d773b-170">Example 2: Reply to a message in MIME format</span></span>
##### <a name="request"></a><span data-ttu-id="d773b-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="d773b-171">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_reply_mime_beta"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: text/plain

UmVjZWl2ZWQ6IGZyb20gY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSBieSAKY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSB3aXRoIE1pY3Jvc29mdCAKU01UUCBTZXJ2ZXIgKHZlcnNpb249VExTMV8yLCAKY2lwaGVyPVRMU19FQ0RIRV9SU0FfV0lUSF9BRVNfMjU2X0NCQ19TSEEzODRfUDI1NikgaW

```

##### <a name="response"></a><span data-ttu-id="d773b-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="d773b-172">Response</span></span>
<span data-ttu-id="d773b-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d773b-173">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="d773b-174">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="d773b-174">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
