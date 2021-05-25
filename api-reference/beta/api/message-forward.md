---
title: 'message: forward'
description: Переад. сообщение в формате JSON или MIME
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1d652e9df5ce89c232d65b46bd8e1a60151bc704
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645649"
---
# <a name="message-forward"></a><span data-ttu-id="52886-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="52886-103">message: forward</span></span>

<span data-ttu-id="52886-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52886-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52886-105">Переад. сообщение в формате JSON или MIME.</span><span class="sxs-lookup"><span data-stu-id="52886-105">Forward a message using either JSON or MIME format.</span></span>

<span data-ttu-id="52886-106">При использовании формата JSON можно:</span><span class="sxs-lookup"><span data-stu-id="52886-106">When using JSON format, you can:</span></span>
- <span data-ttu-id="52886-107">Укажите комментарий или **свойство** тела `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="52886-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="52886-108">При указании обоих возвращается ошибка http 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="52886-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="52886-109">Укажите `toRecipients` параметр или **свойство toRecipients** `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="52886-109">Specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="52886-110">Указание обоих или указаний не возвращает ошибку http 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="52886-110">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

<span data-ttu-id="52886-111">При использовании формата MIME:</span><span class="sxs-lookup"><span data-stu-id="52886-111">When using MIME format:</span></span>
- <span data-ttu-id="52886-112">Предоформим соответствующие заголовки интернет-сообщений и [содержимое MIME](https://tools.ietf.org/html/rfc2045), все закодированные в [](https://tools.ietf.org/html/rfc2076) **формате base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="52886-112">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="52886-113">Добавьте все вложения и свойства S/MIME в содержимое MIME.</span><span class="sxs-lookup"><span data-stu-id="52886-113">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="52886-114">Этот метод сохраняет сообщение в папке **Отправленные** элементы.</span><span class="sxs-lookup"><span data-stu-id="52886-114">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="52886-115">Кроме того, [создайте черновик](../api/message-createforward.md)для отправки сообщения и [отправки](../api/message-send.md) его позже.</span><span class="sxs-lookup"><span data-stu-id="52886-115">Alternatively, [create a draft to forward a message](../api/message-createforward.md), and [send](../api/message-send.md) it later.</span></span>

## <a name="permissions"></a><span data-ttu-id="52886-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52886-116">Permissions</span></span>
<span data-ttu-id="52886-117">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="52886-117">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="52886-118">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52886-118">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52886-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52886-119">Permission type</span></span>      | <span data-ttu-id="52886-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52886-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52886-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52886-121">Delegated (work or school account)</span></span> | <span data-ttu-id="52886-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="52886-122">Mail.Send</span></span>    |
|<span data-ttu-id="52886-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52886-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52886-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="52886-124">Mail.Send</span></span>    |
|<span data-ttu-id="52886-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52886-125">Application</span></span> | <span data-ttu-id="52886-126">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="52886-126">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="52886-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52886-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="52886-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52886-128">Request headers</span></span>
| <span data-ttu-id="52886-129">Имя</span><span class="sxs-lookup"><span data-stu-id="52886-129">Name</span></span>       | <span data-ttu-id="52886-130">Тип</span><span class="sxs-lookup"><span data-stu-id="52886-130">Type</span></span> | <span data-ttu-id="52886-131">Описание</span><span class="sxs-lookup"><span data-stu-id="52886-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="52886-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="52886-132">Authorization</span></span>  | <span data-ttu-id="52886-133">string</span><span class="sxs-lookup"><span data-stu-id="52886-133">string</span></span>  | <span data-ttu-id="52886-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52886-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52886-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="52886-136">Content-Type</span></span> | <span data-ttu-id="52886-137">string</span><span class="sxs-lookup"><span data-stu-id="52886-137">string</span></span>  | <span data-ttu-id="52886-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52886-p105">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="52886-140">Используйте `application/json` для объекта JSON и `text/plain` контента MIME.</span><span class="sxs-lookup"><span data-stu-id="52886-140">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52886-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52886-141">Request body</span></span>
<span data-ttu-id="52886-142">При использовании формата JSON укажи объект JSON со следующими параметрами.</span><span class="sxs-lookup"><span data-stu-id="52886-142">When using JSON format, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="52886-143">Параметр</span><span class="sxs-lookup"><span data-stu-id="52886-143">Parameter</span></span>    | <span data-ttu-id="52886-144">Тип</span><span class="sxs-lookup"><span data-stu-id="52886-144">Type</span></span>   |<span data-ttu-id="52886-145">Описание</span><span class="sxs-lookup"><span data-stu-id="52886-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52886-146">comment</span><span class="sxs-lookup"><span data-stu-id="52886-146">comment</span></span>|<span data-ttu-id="52886-147">String</span><span class="sxs-lookup"><span data-stu-id="52886-147">String</span></span>|<span data-ttu-id="52886-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="52886-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="52886-150">toRecipients</span><span class="sxs-lookup"><span data-stu-id="52886-150">toRecipients</span></span>|<span data-ttu-id="52886-151">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="52886-151">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="52886-152">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="52886-152">The list of recipients.</span></span>|
|<span data-ttu-id="52886-153">message</span><span class="sxs-lookup"><span data-stu-id="52886-153">message</span></span>|[<span data-ttu-id="52886-154">message</span><span class="sxs-lookup"><span data-stu-id="52886-154">message</span></span>](../resources/message.md)|<span data-ttu-id="52886-155">Любые свойства, которые можно записать для обновления в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="52886-155">Any writeable properties to update in the reply message.</span></span>|

<span data-ttu-id="52886-156">При указании тела в формате MIME укажите содержимое MIME с применимыми заглавными интернет-сообщениями ("To", "CC", "BCC", "Subject"), все закодированные в **формате base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="52886-156">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="52886-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="52886-157">Response</span></span>

<span data-ttu-id="52886-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="52886-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="52886-160">Если в тексте запроса содержится неправильное содержимое MIME, этот метод возвращается и следующее сообщение об ошибке: "Недействительные строки `400 Bad request` base64 для контента MIME".</span><span class="sxs-lookup"><span data-stu-id="52886-160">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="52886-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="52886-161">Examples</span></span>
### <a name="example-1-forward-a-message-using-json-format"></a><span data-ttu-id="52886-162">Пример 1. Переоформить сообщение с помощью формата JSON</span><span class="sxs-lookup"><span data-stu-id="52886-162">Example 1: Forward a message using JSON format</span></span>
<span data-ttu-id="52886-163">В следующем примере свойство **isDeliveryReceiptRequested** задает значение true, добавляет комментарий и передает сообщение.</span><span class="sxs-lookup"><span data-stu-id="52886-163">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="52886-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="52886-164">Request</span></span>
<span data-ttu-id="52886-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52886-165">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52886-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="52886-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward
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
  "comment": "Dana, just want to make sure you get this." 
}
```
# <a name="c"></a>[<span data-ttu-id="52886-167">C#</span><span class="sxs-lookup"><span data-stu-id="52886-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52886-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52886-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52886-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52886-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52886-170">Java</span><span class="sxs-lookup"><span data-stu-id="52886-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="52886-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="52886-171">Response</span></span>
<span data-ttu-id="52886-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="52886-172">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-forward-a-message-using-mime-format"></a><span data-ttu-id="52886-173">Пример 2. Переадпрепровождение сообщения с помощью формата MIME</span><span class="sxs-lookup"><span data-stu-id="52886-173">Example 2: Forward a message using MIME format</span></span>

<!-- {
  "blockType": "request",
  "name": "message_forward_mime_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward
Content-Type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np...

```

##### <a name="response"></a><span data-ttu-id="52886-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="52886-174">Response</span></span>
<span data-ttu-id="52886-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="52886-175">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted

```

<span data-ttu-id="52886-176">Если в тексте запроса содержится недооформленное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="52886-176">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
