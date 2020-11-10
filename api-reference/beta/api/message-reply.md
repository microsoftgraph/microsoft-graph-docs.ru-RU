---
title: 'message: reply'
description: 'Ответ отправителю сообщения, добавление комментария или изменение любых обновляемых свойств одновременно в одном вызове **reply**. '
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7b9ea1532eb932e99325b22e8c664879089b0f1d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967413"
---
# <a name="message-reply"></a><span data-ttu-id="7c20c-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="7c20c-103">message: reply</span></span>

<span data-ttu-id="7c20c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c20c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c20c-105">Ответ отправителю сообщения, добавление комментария или изменение любых обновляемых свойств одновременно в одном вызове **reply**.</span><span class="sxs-lookup"><span data-stu-id="7c20c-105">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call.</span></span> <span data-ttu-id="7c20c-106">После этого сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="7c20c-106">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="7c20c-107">Кроме того, вы можете [создать черновик ответного сообщения](../api/message-createreply.md) , чтобы добавить комментарий или обновить все свойства сообщения, а затем [Отправить](../api/message-send.md) ответ.</span><span class="sxs-lookup"><span data-stu-id="7c20c-107">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="7c20c-108">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="7c20c-108">**Note**</span></span>

- <span data-ttu-id="7c20c-109">Можно указать либо свойство Comment, либо свойство **Body** для `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="7c20c-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="7c20c-110">Если указать и то, и другое, будет возвращена ошибка неправильного запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="7c20c-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="7c20c-111">Если свойство **replyTo** указано в исходном сообщении, в формате Интернет-сообщений ( [RFC 2822](https://www.rfc-editor.org/info/rfc2822)), необходимо отправить ответ получателям в **replyTo** , а не получателю в свойстве **from** .</span><span class="sxs-lookup"><span data-stu-id="7c20c-111">If the **replyTo** property is specified in the original message, per Internet Message Format ( [RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="7c20c-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c20c-112">Permissions</span></span>
<span data-ttu-id="7c20c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c20c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c20c-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c20c-115">Permission type</span></span>      | <span data-ttu-id="7c20c-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c20c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c20c-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c20c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="7c20c-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7c20c-118">Mail.Send</span></span>    |
|<span data-ttu-id="7c20c-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c20c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c20c-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7c20c-120">Mail.Send</span></span>    |
|<span data-ttu-id="7c20c-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c20c-121">Application</span></span> | <span data-ttu-id="7c20c-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7c20c-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c20c-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c20c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="7c20c-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c20c-124">Request headers</span></span>
| <span data-ttu-id="7c20c-125">Имя</span><span class="sxs-lookup"><span data-stu-id="7c20c-125">Name</span></span>       | <span data-ttu-id="7c20c-126">Тип</span><span class="sxs-lookup"><span data-stu-id="7c20c-126">Type</span></span> | <span data-ttu-id="7c20c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="7c20c-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7c20c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c20c-128">Authorization</span></span>  | <span data-ttu-id="7c20c-129">string</span><span class="sxs-lookup"><span data-stu-id="7c20c-129">string</span></span>  | <span data-ttu-id="7c20c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c20c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7c20c-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c20c-132">Content-Type</span></span> | <span data-ttu-id="7c20c-133">string</span><span class="sxs-lookup"><span data-stu-id="7c20c-133">string</span></span>  | <span data-ttu-id="7c20c-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c20c-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c20c-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c20c-136">Request body</span></span>
<span data-ttu-id="7c20c-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7c20c-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7c20c-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="7c20c-138">Parameter</span></span>    | <span data-ttu-id="7c20c-139">Тип</span><span class="sxs-lookup"><span data-stu-id="7c20c-139">Type</span></span>   |<span data-ttu-id="7c20c-140">Описание</span><span class="sxs-lookup"><span data-stu-id="7c20c-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c20c-141">comment</span><span class="sxs-lookup"><span data-stu-id="7c20c-141">comment</span></span>|<span data-ttu-id="7c20c-142">String</span><span class="sxs-lookup"><span data-stu-id="7c20c-142">String</span></span>|<span data-ttu-id="7c20c-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="7c20c-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="7c20c-145">message</span><span class="sxs-lookup"><span data-stu-id="7c20c-145">message</span></span>|[<span data-ttu-id="7c20c-146">message</span><span class="sxs-lookup"><span data-stu-id="7c20c-146">message</span></span>](../resources/message.md)|<span data-ttu-id="7c20c-147">Все доступные для записи свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="7c20c-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="7c20c-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c20c-148">Response</span></span>

<span data-ttu-id="7c20c-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7c20c-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c20c-151">Пример</span><span class="sxs-lookup"><span data-stu-id="7c20c-151">Example</span></span>
<span data-ttu-id="7c20c-152">Приведенный ниже пример включает комментарий и добавляет получателя в ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="7c20c-152">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="7c20c-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c20c-153">Request</span></span>
<span data-ttu-id="7c20c-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c20c-154">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7c20c-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c20c-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7c20c-156">C#</span><span class="sxs-lookup"><span data-stu-id="7c20c-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c20c-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c20c-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c20c-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c20c-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c20c-159">Java</span><span class="sxs-lookup"><span data-stu-id="7c20c-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-reply-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7c20c-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c20c-160">Response</span></span>
<span data-ttu-id="7c20c-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7c20c-161">Here is an example of the response.</span></span>
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


