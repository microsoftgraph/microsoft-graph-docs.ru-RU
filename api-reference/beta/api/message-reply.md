---
title: 'message: reply'
description: 'Ответ отправителю сообщения, добавление комментария или изменение любых обновляемых свойств одновременно в одном вызове **reply**. '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2c79861fbb452ac593d8a97d6c78a6a70d435631
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415003"
---
# <a name="message-reply"></a><span data-ttu-id="ada95-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="ada95-103">message: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ada95-104">Ответ отправителю сообщения, добавление комментария или изменение любых обновляемых свойств одновременно в одном вызове **reply**.</span><span class="sxs-lookup"><span data-stu-id="ada95-104">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call.</span></span> <span data-ttu-id="ada95-105">После этого сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="ada95-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="ada95-106">Кроме того, вы можете [создать черновик ответного сообщения](../api/message-createreply.md) , чтобы добавить комментарий или обновить все свойства сообщения, а затем [Отправить](../api/message-send.md) ответ.</span><span class="sxs-lookup"><span data-stu-id="ada95-106">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="ada95-107">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="ada95-107">**Note**</span></span>

- <span data-ttu-id="ada95-108">Можно указать либо свойство Comment, либо свойство **Body** для `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="ada95-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="ada95-109">Если указать и то, и другое, будет возвращена ошибка неправильного запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="ada95-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="ada95-110">Если свойство **replyTo** указано в исходном сообщении, в формате Интернет-сообщений ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), необходимо отправить ответ получателям в **replyTo** , а не получателю в свойстве **from** .</span><span class="sxs-lookup"><span data-stu-id="ada95-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="ada95-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ada95-111">Permissions</span></span>
<span data-ttu-id="ada95-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ada95-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ada95-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ada95-114">Permission type</span></span>      | <span data-ttu-id="ada95-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ada95-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ada95-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ada95-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ada95-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ada95-117">Mail.Send</span></span>    |
|<span data-ttu-id="ada95-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ada95-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ada95-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ada95-119">Mail.Send</span></span>    |
|<span data-ttu-id="ada95-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ada95-120">Application</span></span> | <span data-ttu-id="ada95-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ada95-121">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="ada95-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ada95-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="ada95-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ada95-123">Request headers</span></span>
| <span data-ttu-id="ada95-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ada95-124">Name</span></span>       | <span data-ttu-id="ada95-125">Тип</span><span class="sxs-lookup"><span data-stu-id="ada95-125">Type</span></span> | <span data-ttu-id="ada95-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ada95-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ada95-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ada95-127">Authorization</span></span>  | <span data-ttu-id="ada95-128">string</span><span class="sxs-lookup"><span data-stu-id="ada95-128">string</span></span>  | <span data-ttu-id="ada95-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ada95-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ada95-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ada95-131">Content-Type</span></span> | <span data-ttu-id="ada95-132">string</span><span class="sxs-lookup"><span data-stu-id="ada95-132">string</span></span>  | <span data-ttu-id="ada95-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ada95-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ada95-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ada95-135">Request body</span></span>
<span data-ttu-id="ada95-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ada95-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ada95-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="ada95-137">Parameter</span></span>    | <span data-ttu-id="ada95-138">Тип</span><span class="sxs-lookup"><span data-stu-id="ada95-138">Type</span></span>   |<span data-ttu-id="ada95-139">Описание</span><span class="sxs-lookup"><span data-stu-id="ada95-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ada95-140">comment</span><span class="sxs-lookup"><span data-stu-id="ada95-140">comment</span></span>|<span data-ttu-id="ada95-141">String</span><span class="sxs-lookup"><span data-stu-id="ada95-141">String</span></span>|<span data-ttu-id="ada95-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="ada95-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="ada95-144">message</span><span class="sxs-lookup"><span data-stu-id="ada95-144">message</span></span>|[<span data-ttu-id="ada95-145">message</span><span class="sxs-lookup"><span data-stu-id="ada95-145">message</span></span>](../resources/message.md)|<span data-ttu-id="ada95-146">Все доступные для записи свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="ada95-146">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="ada95-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="ada95-147">Response</span></span>

<span data-ttu-id="ada95-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ada95-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ada95-150">Пример</span><span class="sxs-lookup"><span data-stu-id="ada95-150">Example</span></span>
<span data-ttu-id="ada95-151">Приведенный ниже пример включает комментарий и добавляет получателя в ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="ada95-151">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="ada95-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="ada95-152">Request</span></span>
<span data-ttu-id="ada95-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ada95-153">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ada95-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="ada95-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_reply"
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ada95-155">C#</span><span class="sxs-lookup"><span data-stu-id="ada95-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ada95-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ada95-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ada95-157">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ada95-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ada95-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="ada95-158">Response</span></span>
<span data-ttu-id="ada95-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ada95-159">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
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
