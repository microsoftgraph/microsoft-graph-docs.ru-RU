---
title: 'message: forward'
description: 'Переадментировать сообщение, добавить комментарий или изменить любые обновляемые свойства  '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fb90daf582c1697dbab8f8d50e68885c91af28d3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130352"
---
# <a name="message-forward"></a><span data-ttu-id="6debb-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="6debb-103">message: forward</span></span>

<span data-ttu-id="6debb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6debb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6debb-105">Переадментировать сообщение, добавить комментарий или изменить любые обновляемые свойства</span><span class="sxs-lookup"><span data-stu-id="6debb-105">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="6debb-106">все в одном **переад вызовах.**</span><span class="sxs-lookup"><span data-stu-id="6debb-106">all in one **forward** call.</span></span> <span data-ttu-id="6debb-107">Сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="6debb-107">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="6debb-108">Кроме того, сначала [](../api/message-createforward.md) можно создать черновик переадментного сообщения, включив комментарий или обновив свойства сообщения, а затем [отправить](../api/message-send.md) черновик сообщения.</span><span class="sxs-lookup"><span data-stu-id="6debb-108">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="6debb-109">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="6debb-109">**Note**</span></span>

- <span data-ttu-id="6debb-110">Можно указать комментарий или свойство **body** `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="6debb-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="6debb-111">Если указать оба этих запроса, будет возвращена ошибка "HTTP 400 Bad Request".</span><span class="sxs-lookup"><span data-stu-id="6debb-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="6debb-112">Необходимо указать либо параметр, либо свойство `toRecipients` **toRecipients** `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="6debb-112">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="6debb-113">Если указать и то, и другое, не будет возвращена ошибка HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="6debb-113">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="6debb-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6debb-114">Permissions</span></span>
<span data-ttu-id="6debb-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6debb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6debb-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6debb-117">Permission type</span></span>      | <span data-ttu-id="6debb-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6debb-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6debb-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6debb-119">Delegated (work or school account)</span></span> | <span data-ttu-id="6debb-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="6debb-120">Mail.Send</span></span>    |
|<span data-ttu-id="6debb-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6debb-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6debb-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="6debb-122">Mail.Send</span></span>    |
|<span data-ttu-id="6debb-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6debb-123">Application</span></span> | <span data-ttu-id="6debb-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="6debb-124">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="6debb-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6debb-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="6debb-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6debb-126">Request headers</span></span>
| <span data-ttu-id="6debb-127">Имя</span><span class="sxs-lookup"><span data-stu-id="6debb-127">Name</span></span>       | <span data-ttu-id="6debb-128">Тип</span><span class="sxs-lookup"><span data-stu-id="6debb-128">Type</span></span> | <span data-ttu-id="6debb-129">Описание</span><span class="sxs-lookup"><span data-stu-id="6debb-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6debb-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6debb-130">Authorization</span></span>  | <span data-ttu-id="6debb-131">string</span><span class="sxs-lookup"><span data-stu-id="6debb-131">string</span></span>  | <span data-ttu-id="6debb-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6debb-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6debb-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6debb-134">Content-Type</span></span> | <span data-ttu-id="6debb-135">string</span><span class="sxs-lookup"><span data-stu-id="6debb-135">string</span></span>  | <span data-ttu-id="6debb-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6debb-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6debb-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6debb-138">Request body</span></span>
<span data-ttu-id="6debb-139">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6debb-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6debb-140">Параметр</span><span class="sxs-lookup"><span data-stu-id="6debb-140">Parameter</span></span>    | <span data-ttu-id="6debb-141">Тип</span><span class="sxs-lookup"><span data-stu-id="6debb-141">Type</span></span>   |<span data-ttu-id="6debb-142">Описание</span><span class="sxs-lookup"><span data-stu-id="6debb-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6debb-143">comment</span><span class="sxs-lookup"><span data-stu-id="6debb-143">comment</span></span>|<span data-ttu-id="6debb-144">String</span><span class="sxs-lookup"><span data-stu-id="6debb-144">String</span></span>|<span data-ttu-id="6debb-p107">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="6debb-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="6debb-147">toRecipients</span><span class="sxs-lookup"><span data-stu-id="6debb-147">toRecipients</span></span>|<span data-ttu-id="6debb-148">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="6debb-148">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="6debb-149">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="6debb-149">The list of recipients.</span></span>|
|<span data-ttu-id="6debb-150">message</span><span class="sxs-lookup"><span data-stu-id="6debb-150">message</span></span>|[<span data-ttu-id="6debb-151">message</span><span class="sxs-lookup"><span data-stu-id="6debb-151">message</span></span>](../resources/message.md)|<span data-ttu-id="6debb-152">Любые записаемые свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="6debb-152">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="6debb-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="6debb-153">Response</span></span>

<span data-ttu-id="6debb-p108">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6debb-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6debb-156">Пример</span><span class="sxs-lookup"><span data-stu-id="6debb-156">Example</span></span>
<span data-ttu-id="6debb-157">В следующем примере **свойству isDeliveryReceiptRequested** задается значение true, добавляется комментарий и переадрежается сообщение.</span><span class="sxs-lookup"><span data-stu-id="6debb-157">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="6debb-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="6debb-158">Request</span></span>
<span data-ttu-id="6debb-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6debb-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6debb-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="6debb-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6debb-161">C#</span><span class="sxs-lookup"><span data-stu-id="6debb-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6debb-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6debb-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6debb-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6debb-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6debb-164">Java</span><span class="sxs-lookup"><span data-stu-id="6debb-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6debb-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="6debb-165">Response</span></span>
<span data-ttu-id="6debb-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6debb-166">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
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


