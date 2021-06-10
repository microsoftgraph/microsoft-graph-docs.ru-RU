---
title: 'message: forward'
description: Переад. сообщение в формате JSON или MIME.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3e0004bae41d7b700ae3a337bce27b214ba209cb
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870404"
---
# <a name="message-forward"></a><span data-ttu-id="d1a41-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="d1a41-103">message: forward</span></span>

<span data-ttu-id="d1a41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1a41-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d1a41-105">Переад. сообщение в формате JSON или MIME.</span><span class="sxs-lookup"><span data-stu-id="d1a41-105">Forward a message using either JSON or MIME format.</span></span>

<span data-ttu-id="d1a41-106">При использовании формата JSON можно:</span><span class="sxs-lookup"><span data-stu-id="d1a41-106">When using JSON format, you can:</span></span>
- <span data-ttu-id="d1a41-107">Укажите комментарий или **свойство** тела `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="d1a41-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="d1a41-108">При указании обоих возвращается ошибка http 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="d1a41-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="d1a41-109">Укажите `toRecipients` параметр или **свойство toRecipients** `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="d1a41-109">Specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="d1a41-110">Указание обоих или указаний не возвращает ошибку http 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="d1a41-110">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

<span data-ttu-id="d1a41-111">При использовании формата MIME:</span><span class="sxs-lookup"><span data-stu-id="d1a41-111">When using MIME format:</span></span>
- <span data-ttu-id="d1a41-112">Укажите соответствующие [заголовки сообщений Интернета](https://tools.ietf.org/html/rfc2076) и [содержимое MIME](https://tools.ietf.org/html/rfc2045), а также закодируйте их в формате **Base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="d1a41-112">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="d1a41-113">Добавьте все вложения и свойства S/MIME в содержимое MIME.</span><span class="sxs-lookup"><span data-stu-id="d1a41-113">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="d1a41-114">Этот метод сохраняет сообщение в папке **Отправленные**.</span><span class="sxs-lookup"><span data-stu-id="d1a41-114">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="d1a41-115">Кроме того, [создайте черновик](../api/message-createforward.md)для отправки сообщения и [отправки](../api/message-send.md) его позже.</span><span class="sxs-lookup"><span data-stu-id="d1a41-115">Alternatively, [create a draft to forward a message](../api/message-createforward.md), and [send](../api/message-send.md) it later.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1a41-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1a41-116">Permissions</span></span>
<span data-ttu-id="d1a41-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1a41-p103">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1a41-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1a41-119">Permission type</span></span>      | <span data-ttu-id="d1a41-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1a41-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1a41-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1a41-121">Delegated (work or school account)</span></span> | <span data-ttu-id="d1a41-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d1a41-122">Mail.Send</span></span>    |
|<span data-ttu-id="d1a41-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1a41-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1a41-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d1a41-124">Mail.Send</span></span>    |
|<span data-ttu-id="d1a41-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1a41-125">Application</span></span> | <span data-ttu-id="d1a41-126">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d1a41-126">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1a41-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1a41-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="d1a41-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1a41-128">Request headers</span></span>
| <span data-ttu-id="d1a41-129">Имя</span><span class="sxs-lookup"><span data-stu-id="d1a41-129">Name</span></span>       | <span data-ttu-id="d1a41-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d1a41-130">Type</span></span> | <span data-ttu-id="d1a41-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d1a41-131">Description</span></span>| 
|:---------------|:--------|:----------|
| <span data-ttu-id="d1a41-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1a41-132">Authorization</span></span>  | <span data-ttu-id="d1a41-133">string</span><span class="sxs-lookup"><span data-stu-id="d1a41-133">string</span></span>  | <span data-ttu-id="d1a41-134">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="d1a41-134">Bearer {token}.</span></span> <span data-ttu-id="d1a41-135">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d1a41-135">Required</span></span> |
| <span data-ttu-id="d1a41-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1a41-136">Content-Type</span></span> | <span data-ttu-id="d1a41-137">string</span><span class="sxs-lookup"><span data-stu-id="d1a41-137">string</span></span>  | <span data-ttu-id="d1a41-138">Характер данных в теле объекта.</span><span class="sxs-lookup"><span data-stu-id="d1a41-138">Nature of the data in the body of an entity.</span></span>  <span data-ttu-id="d1a41-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1a41-139">Required.</span></span> <br/> <span data-ttu-id="d1a41-140">Используйте `application/json` для объекта JSON и `text/plain` для содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="d1a41-140">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1a41-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1a41-141">Request body</span></span>
<span data-ttu-id="d1a41-142">При использовании формата JSON укажи объект JSON в теле запроса со следующими параметрами.</span><span class="sxs-lookup"><span data-stu-id="d1a41-142">When using JSON format, provide a JSON object in the request body with the following parameters.</span></span>

| <span data-ttu-id="d1a41-143">Параметр</span><span class="sxs-lookup"><span data-stu-id="d1a41-143">Parameter</span></span>    | <span data-ttu-id="d1a41-144">Тип</span><span class="sxs-lookup"><span data-stu-id="d1a41-144">Type</span></span>   |<span data-ttu-id="d1a41-145">Описание</span><span class="sxs-lookup"><span data-stu-id="d1a41-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1a41-146">comment</span><span class="sxs-lookup"><span data-stu-id="d1a41-146">comment</span></span>|<span data-ttu-id="d1a41-147">String</span><span class="sxs-lookup"><span data-stu-id="d1a41-147">String</span></span>|<span data-ttu-id="d1a41-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="d1a41-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="d1a41-150">toRecipients</span><span class="sxs-lookup"><span data-stu-id="d1a41-150">toRecipients</span></span>|<span data-ttu-id="d1a41-151">Коллекция объектов [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="d1a41-151">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="d1a41-152">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="d1a41-152">The list of recipients.</span></span>|

<span data-ttu-id="d1a41-153">При указании текста в формате MIME укажите содержимое MIME с применимыми заголовками сообщений Интернета ("Кому", "Копия", "Скрытая копия", "Тема"), все закодированные сообщения в формате **Base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="d1a41-153">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="d1a41-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1a41-154">Response</span></span>

<span data-ttu-id="d1a41-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d1a41-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="d1a41-157">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает `400 Bad request` и следующее сообщение об ошибке: "Недопустимая строка Base 64 для содержимого MIME".</span><span class="sxs-lookup"><span data-stu-id="d1a41-157">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="d1a41-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="d1a41-158">Examples</span></span>
### <a name="example-1-forward-a-message-using-json-format"></a><span data-ttu-id="d1a41-159">Пример 1. Переоформить сообщение с помощью формата JSON</span><span class="sxs-lookup"><span data-stu-id="d1a41-159">Example 1: Forward a message using JSON format</span></span>
<span data-ttu-id="d1a41-160">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d1a41-160">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d1a41-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1a41-161">Request</span></span>
<span data-ttu-id="d1a41-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1a41-162">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1a41-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1a41-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="d1a41-164">C#</span><span class="sxs-lookup"><span data-stu-id="d1a41-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1a41-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1a41-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1a41-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1a41-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1a41-167">Java</span><span class="sxs-lookup"><span data-stu-id="d1a41-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d1a41-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1a41-168">Response</span></span>
<span data-ttu-id="d1a41-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1a41-169">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

### <a name="example-2-forward-a-message-using-mime-content"></a><span data-ttu-id="d1a41-170">Пример 2. Переопрепровождение сообщения с помощью контента MIME</span><span class="sxs-lookup"><span data-stu-id="d1a41-170">Example 2: Forward a message using MIME content</span></span>
##### <a name="request"></a><span data-ttu-id="d1a41-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1a41-171">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_forward_mime_v1"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/forward
Content-type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np
```

##### <a name="response"></a><span data-ttu-id="d1a41-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1a41-172">Response</span></span>
<span data-ttu-id="d1a41-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1a41-173">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="d1a41-174">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="d1a41-174">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

