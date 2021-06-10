---
title: 'message: replyAll'
description: Ответьте всем получателям сообщения в формате JSON или MIME.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a47223c925e9ac4c1e45769f3fe04f44c80c1c71
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869914"
---
# <a name="message-replyall"></a><span data-ttu-id="c914d-103">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="c914d-103">message: replyAll</span></span>

<span data-ttu-id="c914d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c914d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c914d-105">Ответьте всем получателям [сообщения в](../resources/message.md) формате JSON или MIME.</span><span class="sxs-lookup"><span data-stu-id="c914d-105">Reply to all recipients of a [message](../resources/message.md) using either JSON or MIME format.</span></span>

<span data-ttu-id="c914d-106">При использовании формата JSON:</span><span class="sxs-lookup"><span data-stu-id="c914d-106">When using JSON format:</span></span>
- <span data-ttu-id="c914d-107">Укажите комментарий или **свойство** тела `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="c914d-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="c914d-108">При указании обоих возвращается ошибка http 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="c914d-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="c914d-109">Если исходное сообщение указывает получателя в свойстве **replyTo,** в формате интернет-сообщений [(RFC 2822),](https://www.rfc-editor.org/info/rfc2822)отправьте ответ получателям в **replyTo,** а не получателю из **свойства.**</span><span class="sxs-lookup"><span data-stu-id="c914d-109">If the original message specifies a recipient in the **replyTo** property, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span>

<span data-ttu-id="c914d-110">При использовании формата MIME:</span><span class="sxs-lookup"><span data-stu-id="c914d-110">When using MIME format:</span></span>
- <span data-ttu-id="c914d-111">Укажите соответствующие [заголовки сообщений Интернета](https://tools.ietf.org/html/rfc2076) и [содержимое MIME](https://tools.ietf.org/html/rfc2045), а также закодируйте их в формате **Base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="c914d-111">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="c914d-112">Добавьте все вложения и свойства S/MIME в содержимое MIME.</span><span class="sxs-lookup"><span data-stu-id="c914d-112">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="c914d-113">Этот метод сохраняет сообщение в папке **Отправленные**.</span><span class="sxs-lookup"><span data-stu-id="c914d-113">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="c914d-114">Кроме того, [создайте черновик для](../api/message-createreplyall.md) ответа на сообщение и [отправьте его](../api/message-send.md) позже.</span><span class="sxs-lookup"><span data-stu-id="c914d-114">Alternatively, [create a draft to reply-all to a message](../api/message-createreplyall.md) and [send](../api/message-send.md) it later.</span></span>

## <a name="permissions"></a><span data-ttu-id="c914d-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c914d-115">Permissions</span></span>
<span data-ttu-id="c914d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c914d-p102">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c914d-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c914d-118">Permission type</span></span>      | <span data-ttu-id="c914d-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c914d-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c914d-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c914d-120">Delegated (work or school account)</span></span> | <span data-ttu-id="c914d-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c914d-121">Mail.Send</span></span>    |
|<span data-ttu-id="c914d-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c914d-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c914d-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c914d-123">Mail.Send</span></span>    |
|<span data-ttu-id="c914d-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c914d-124">Application</span></span> | <span data-ttu-id="c914d-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c914d-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="c914d-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c914d-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="c914d-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c914d-127">Request headers</span></span>
| <span data-ttu-id="c914d-128">Имя</span><span class="sxs-lookup"><span data-stu-id="c914d-128">Name</span></span>       | <span data-ttu-id="c914d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c914d-129">Type</span></span> | <span data-ttu-id="c914d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c914d-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c914d-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="c914d-131">Authorization</span></span>  | <span data-ttu-id="c914d-132">string</span><span class="sxs-lookup"><span data-stu-id="c914d-132">string</span></span>  | <span data-ttu-id="c914d-133">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="c914d-133">Bearer {token}.</span></span> <span data-ttu-id="c914d-134">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c914d-134">Required</span></span> |
| <span data-ttu-id="c914d-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c914d-135">Content-Type</span></span> | <span data-ttu-id="c914d-136">string</span><span class="sxs-lookup"><span data-stu-id="c914d-136">string</span></span>  | <span data-ttu-id="c914d-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c914d-p104">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="c914d-139">Используйте `application/json` для объекта JSON и `text/plain` для содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="c914d-139">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c914d-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c914d-140">Request body</span></span>
<span data-ttu-id="c914d-141">При использовании формата JSON укажи объект JSON в теле запроса со следующими параметрами.</span><span class="sxs-lookup"><span data-stu-id="c914d-141">When using JSON format, provide a JSON object in the request body with the following parameters.</span></span>

| <span data-ttu-id="c914d-142">Параметр</span><span class="sxs-lookup"><span data-stu-id="c914d-142">Parameter</span></span>    | <span data-ttu-id="c914d-143">Тип</span><span class="sxs-lookup"><span data-stu-id="c914d-143">Type</span></span>   |<span data-ttu-id="c914d-144">Описание</span><span class="sxs-lookup"><span data-stu-id="c914d-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c914d-145">comment</span><span class="sxs-lookup"><span data-stu-id="c914d-145">comment</span></span>|<span data-ttu-id="c914d-146">String</span><span class="sxs-lookup"><span data-stu-id="c914d-146">String</span></span>|<span data-ttu-id="c914d-p105">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="c914d-p105">A comment to include. Can be an empty string.</span></span>|

<span data-ttu-id="c914d-149">При указании тела в формате MIME укажите содержимое MIME с применимыми заглавными сообщениями в Интернете, все закодированные в **формате base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="c914d-149">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers, all encoded in **base64** format in the request body.</span></span> <span data-ttu-id="c914d-150">Этот метод загружает отправитель и всех получателей исходного сообщения в качестве получателей нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="c914d-150">This method loads the sender and all recipients of the original message as recipients of the new message.</span></span>

## <a name="response"></a><span data-ttu-id="c914d-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="c914d-151">Response</span></span>

<span data-ttu-id="c914d-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c914d-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="c914d-154">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает `400 Bad request` и следующее сообщение об ошибке: "Недопустимая строка Base 64 для содержимого MIME".</span><span class="sxs-lookup"><span data-stu-id="c914d-154">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="c914d-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="c914d-155">Examples</span></span>
### <a name="example-1-reply-all-in-json-format-to-a-message"></a><span data-ttu-id="c914d-156">Пример 1. Ответ на сообщение в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c914d-156">Example 1: Reply-all in JSON format to a message</span></span>
<span data-ttu-id="c914d-157">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c914d-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c914d-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="c914d-158">Request</span></span>
<span data-ttu-id="c914d-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c914d-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c914d-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="c914d-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/replyAll
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```
# <a name="c"></a>[<span data-ttu-id="c914d-161">C#</span><span class="sxs-lookup"><span data-stu-id="c914d-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c914d-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c914d-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c914d-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c914d-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c914d-164">Java</span><span class="sxs-lookup"><span data-stu-id="c914d-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="c914d-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="c914d-165">Response</span></span>
<span data-ttu-id="c914d-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c914d-166">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
### <a name="example-2-reply-all-in-mime-format-to-a-message"></a><span data-ttu-id="c914d-167">Пример 2. Ответ в формате MIME на сообщение</span><span class="sxs-lookup"><span data-stu-id="c914d-167">Example 2: Reply-all in MIME format to a message</span></span>
##### <a name="request"></a><span data-ttu-id="c914d-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="c914d-168">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_replyAll_mime_v1"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/replyAll
Content-type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np
```

##### <a name="response"></a><span data-ttu-id="c914d-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="c914d-169">Response</span></span>
<span data-ttu-id="c914d-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c914d-170">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="c914d-171">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="c914d-171">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

