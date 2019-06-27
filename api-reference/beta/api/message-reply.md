---
title: 'message: reply'
description: 'Ответ отправителю сообщения, добавление комментария или изменение любых обновляемых свойств одновременно в одном вызове **reply**. '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b32a808b13c6133d47cc0c710b85fb9d5820cfb3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267888"
---
# <a name="message-reply"></a><span data-ttu-id="e7e29-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="e7e29-103">message: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7e29-104">Ответ отправителю сообщения, добавление комментария или изменение любых обновляемых свойств одновременно в одном вызове **reply**.</span><span class="sxs-lookup"><span data-stu-id="e7e29-104">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call.</span></span> <span data-ttu-id="e7e29-105">После этого сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="e7e29-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="e7e29-106">Кроме того, вы можете [создать черновик ответного сообщения](../api/message-createreply.md) , чтобы добавить комментарий или обновить все свойства сообщения, а затем [Отправить](../api/message-send.md) ответ.</span><span class="sxs-lookup"><span data-stu-id="e7e29-106">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="e7e29-107">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="e7e29-107">**Note**</span></span>

- <span data-ttu-id="e7e29-108">Можно указать либо свойство Comment, либо свойство **Body** для `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="e7e29-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="e7e29-109">Если указать и то, и другое, будет возвращена ошибка неправильного запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="e7e29-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="e7e29-110">Если свойство **replyTo** указано в исходном сообщении, в формате Интернет-сообщений ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), необходимо отправить ответ получателям в **replyTo** , а не получателю в свойстве **from** .</span><span class="sxs-lookup"><span data-stu-id="e7e29-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="e7e29-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7e29-111">Permissions</span></span>
<span data-ttu-id="e7e29-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7e29-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7e29-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7e29-114">Permission type</span></span>      | <span data-ttu-id="e7e29-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7e29-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7e29-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7e29-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e7e29-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e7e29-117">Mail.Send</span></span>    |
|<span data-ttu-id="e7e29-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7e29-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7e29-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e7e29-119">Mail.Send</span></span>    |
|<span data-ttu-id="e7e29-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7e29-120">Application</span></span> | <span data-ttu-id="e7e29-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e7e29-121">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7e29-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7e29-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="e7e29-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7e29-123">Request headers</span></span>
| <span data-ttu-id="e7e29-124">Имя</span><span class="sxs-lookup"><span data-stu-id="e7e29-124">Name</span></span>       | <span data-ttu-id="e7e29-125">Тип</span><span class="sxs-lookup"><span data-stu-id="e7e29-125">Type</span></span> | <span data-ttu-id="e7e29-126">Описание</span><span class="sxs-lookup"><span data-stu-id="e7e29-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e7e29-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7e29-127">Authorization</span></span>  | <span data-ttu-id="e7e29-128">string</span><span class="sxs-lookup"><span data-stu-id="e7e29-128">string</span></span>  | <span data-ttu-id="e7e29-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7e29-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7e29-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e7e29-131">Content-Type</span></span> | <span data-ttu-id="e7e29-132">string</span><span class="sxs-lookup"><span data-stu-id="e7e29-132">string</span></span>  | <span data-ttu-id="e7e29-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7e29-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7e29-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7e29-135">Request body</span></span>
<span data-ttu-id="e7e29-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e7e29-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e7e29-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="e7e29-137">Parameter</span></span>    | <span data-ttu-id="e7e29-138">Тип</span><span class="sxs-lookup"><span data-stu-id="e7e29-138">Type</span></span>   |<span data-ttu-id="e7e29-139">Описание</span><span class="sxs-lookup"><span data-stu-id="e7e29-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7e29-140">comment</span><span class="sxs-lookup"><span data-stu-id="e7e29-140">comment</span></span>|<span data-ttu-id="e7e29-141">String</span><span class="sxs-lookup"><span data-stu-id="e7e29-141">String</span></span>|<span data-ttu-id="e7e29-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="e7e29-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="e7e29-144">message</span><span class="sxs-lookup"><span data-stu-id="e7e29-144">message</span></span>|[<span data-ttu-id="e7e29-145">message</span><span class="sxs-lookup"><span data-stu-id="e7e29-145">message</span></span>](../resources/message.md)|<span data-ttu-id="e7e29-146">Все доступные для записи свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="e7e29-146">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="e7e29-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7e29-147">Response</span></span>

<span data-ttu-id="e7e29-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e7e29-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7e29-150">Пример</span><span class="sxs-lookup"><span data-stu-id="e7e29-150">Example</span></span>
<span data-ttu-id="e7e29-151">Приведенный ниже пример включает комментарий и добавляет получателя в ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="e7e29-151">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="e7e29-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7e29-152">Request</span></span>
<span data-ttu-id="e7e29-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7e29-153">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="e7e29-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7e29-154">Response</span></span>
<span data-ttu-id="e7e29-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e7e29-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e7e29-156">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="e7e29-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e7e29-157">C#</span><span class="sxs-lookup"><span data-stu-id="e7e29-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_reply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7e29-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="e7e29-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_reply-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e7e29-159">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e7e29-159">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_reply-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/message-reply.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/message-reply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-reply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
