---
title: 'message: reply'
description: 'Ответ отправителю сообщения, добавление комментария или изменение любых обновляемых свойств одновременно в одном вызове **reply**. '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 39d03daf5a26d5617e4eca31ae7ba3799a5159c9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131161"
---
# <a name="message-reply"></a><span data-ttu-id="b9517-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="b9517-103">message: reply</span></span>

<span data-ttu-id="b9517-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9517-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9517-105">Ответ отправителю сообщения, добавление комментария или изменение любых обновляемых свойств одновременно в одном вызове **reply**.</span><span class="sxs-lookup"><span data-stu-id="b9517-105">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call.</span></span> <span data-ttu-id="b9517-106">После этого сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="b9517-106">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="b9517-107">Кроме того, сначала можно создать [черновик](../api/message-createreply.md) ответного сообщения, включив комментарий или обновив свойства сообщения, а затем [отправить](../api/message-send.md) ответ.</span><span class="sxs-lookup"><span data-stu-id="b9517-107">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="b9517-108">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="b9517-108">**Note**</span></span>

- <span data-ttu-id="b9517-109">Можно указать комментарий или свойство **body** `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="b9517-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="b9517-110">Если указать оба этих запроса, будет возвращена ошибка "HTTP 400 Bad Request".</span><span class="sxs-lookup"><span data-stu-id="b9517-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="b9517-111">Если свойство **replyTo** указано в исходном сообщении в формате интернет-сообщений [(RFC 2822),](https://www.rfc-editor.org/info/rfc2822)следует отправить ответ получателям в **replyTo,** а не получателю в свойстве **from.**</span><span class="sxs-lookup"><span data-stu-id="b9517-111">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="b9517-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9517-112">Permissions</span></span>
<span data-ttu-id="b9517-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9517-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9517-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9517-115">Permission type</span></span>      | <span data-ttu-id="b9517-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9517-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9517-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9517-117">Delegated (work or school account)</span></span> | <span data-ttu-id="b9517-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b9517-118">Mail.Send</span></span>    |
|<span data-ttu-id="b9517-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9517-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9517-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b9517-120">Mail.Send</span></span>    |
|<span data-ttu-id="b9517-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9517-121">Application</span></span> | <span data-ttu-id="b9517-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b9517-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9517-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9517-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="b9517-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9517-124">Request headers</span></span>
| <span data-ttu-id="b9517-125">Имя</span><span class="sxs-lookup"><span data-stu-id="b9517-125">Name</span></span>       | <span data-ttu-id="b9517-126">Тип</span><span class="sxs-lookup"><span data-stu-id="b9517-126">Type</span></span> | <span data-ttu-id="b9517-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b9517-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b9517-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9517-128">Authorization</span></span>  | <span data-ttu-id="b9517-129">string</span><span class="sxs-lookup"><span data-stu-id="b9517-129">string</span></span>  | <span data-ttu-id="b9517-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9517-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9517-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9517-132">Content-Type</span></span> | <span data-ttu-id="b9517-133">string</span><span class="sxs-lookup"><span data-stu-id="b9517-133">string</span></span>  | <span data-ttu-id="b9517-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9517-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9517-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9517-136">Request body</span></span>
<span data-ttu-id="b9517-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b9517-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9517-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="b9517-138">Parameter</span></span>    | <span data-ttu-id="b9517-139">Тип</span><span class="sxs-lookup"><span data-stu-id="b9517-139">Type</span></span>   |<span data-ttu-id="b9517-140">Описание</span><span class="sxs-lookup"><span data-stu-id="b9517-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9517-141">comment</span><span class="sxs-lookup"><span data-stu-id="b9517-141">comment</span></span>|<span data-ttu-id="b9517-142">String</span><span class="sxs-lookup"><span data-stu-id="b9517-142">String</span></span>|<span data-ttu-id="b9517-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="b9517-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="b9517-145">message</span><span class="sxs-lookup"><span data-stu-id="b9517-145">message</span></span>|[<span data-ttu-id="b9517-146">message</span><span class="sxs-lookup"><span data-stu-id="b9517-146">message</span></span>](../resources/message.md)|<span data-ttu-id="b9517-147">Любые записаемые свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="b9517-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="b9517-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9517-148">Response</span></span>

<span data-ttu-id="b9517-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b9517-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9517-151">Пример</span><span class="sxs-lookup"><span data-stu-id="b9517-151">Example</span></span>
<span data-ttu-id="b9517-152">В следующем примере содержится комментарий и получатель добавляется в ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="b9517-152">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="b9517-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9517-153">Request</span></span>
<span data-ttu-id="b9517-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9517-154">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9517-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9517-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b9517-156">C#</span><span class="sxs-lookup"><span data-stu-id="b9517-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9517-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9517-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9517-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9517-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9517-159">Java</span><span class="sxs-lookup"><span data-stu-id="b9517-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-reply-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b9517-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9517-160">Response</span></span>
<span data-ttu-id="b9517-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b9517-161">Here is an example of the response.</span></span>
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
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


