---
title: 'message: createReply'
description: 'Создание черновика ответного сообщения для включения комментария или обновления любого свойства сообщения '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 80a8a81f226ab1990d784e4c82e665c54affee32
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415129"
---
# <a name="message-createreply"></a><span data-ttu-id="73f32-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="73f32-103">message: createReply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73f32-104">Создание черновика ответного сообщения, чтобы добавить комментарий или обновить любые свойства сообщения одновременно в одном вызове **createReply**.</span><span class="sxs-lookup"><span data-stu-id="73f32-104">Create a draft of a reply message to include a comment or update any message properties all in one **createReply** call.</span></span> <span data-ttu-id="73f32-105">После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.</span><span class="sxs-lookup"><span data-stu-id="73f32-105">You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="73f32-106">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="73f32-106">**Note**</span></span>

- <span data-ttu-id="73f32-107">Можно указать либо свойство Comment, либо свойство **Body** для `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="73f32-107">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="73f32-108">Если указать и то, и другое, будет возвращена ошибка неправильного запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="73f32-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="73f32-109">Если параметр **replyTo** указан в исходном сообщении, в формате сообщения Интернета ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), необходимо отправить ответ получателям в **replyTo**, а не получателям **из**.</span><span class="sxs-lookup"><span data-stu-id="73f32-109">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="73f32-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73f32-110">Permissions</span></span>
<span data-ttu-id="73f32-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73f32-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73f32-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73f32-113">Permission type</span></span>      | <span data-ttu-id="73f32-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73f32-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73f32-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73f32-115">Delegated (work or school account)</span></span> | <span data-ttu-id="73f32-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73f32-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="73f32-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73f32-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73f32-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73f32-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="73f32-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73f32-119">Application</span></span> | <span data-ttu-id="73f32-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73f32-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="73f32-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73f32-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="73f32-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73f32-122">Request headers</span></span>
| <span data-ttu-id="73f32-123">Имя</span><span class="sxs-lookup"><span data-stu-id="73f32-123">Name</span></span>       | <span data-ttu-id="73f32-124">Тип</span><span class="sxs-lookup"><span data-stu-id="73f32-124">Type</span></span> | <span data-ttu-id="73f32-125">Описание</span><span class="sxs-lookup"><span data-stu-id="73f32-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="73f32-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="73f32-126">Authorization</span></span>  | <span data-ttu-id="73f32-127">string</span><span class="sxs-lookup"><span data-stu-id="73f32-127">string</span></span>  | <span data-ttu-id="73f32-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73f32-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73f32-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73f32-130">Content-Type</span></span> | <span data-ttu-id="73f32-131">string</span><span class="sxs-lookup"><span data-stu-id="73f32-131">string</span></span>  | <span data-ttu-id="73f32-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73f32-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73f32-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73f32-134">Request body</span></span>
<span data-ttu-id="73f32-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="73f32-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="73f32-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="73f32-136">Parameter</span></span>    | <span data-ttu-id="73f32-137">Тип</span><span class="sxs-lookup"><span data-stu-id="73f32-137">Type</span></span>   |<span data-ttu-id="73f32-138">Описание</span><span class="sxs-lookup"><span data-stu-id="73f32-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73f32-139">comment</span><span class="sxs-lookup"><span data-stu-id="73f32-139">comment</span></span>|<span data-ttu-id="73f32-140">String</span><span class="sxs-lookup"><span data-stu-id="73f32-140">String</span></span>|<span data-ttu-id="73f32-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="73f32-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="73f32-143">message</span><span class="sxs-lookup"><span data-stu-id="73f32-143">message</span></span>|[<span data-ttu-id="73f32-144">message</span><span class="sxs-lookup"><span data-stu-id="73f32-144">message</span></span>](../resources/message.md)|<span data-ttu-id="73f32-145">Все доступные для записи свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="73f32-145">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="73f32-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="73f32-146">Response</span></span>

<span data-ttu-id="73f32-147">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="73f32-147">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73f32-148">Пример</span><span class="sxs-lookup"><span data-stu-id="73f32-148">Example</span></span>
<span data-ttu-id="73f32-149">В приведенном ниже примере создается черновик ответа, в тексте запроса добавляется комментарий и получатель.</span><span class="sxs-lookup"><span data-stu-id="73f32-149">The following example creates a reply draft, adds a comment and a recipient in the request body.</span></span>
##### <a name="request"></a><span data-ttu-id="73f32-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="73f32-150">Request</span></span>
<span data-ttu-id="73f32-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73f32-151">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="73f32-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="73f32-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/createReply
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
  "comment": "Samantha, Randi, would you name the group if the project is approved, please?" 
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73f32-153">C#</span><span class="sxs-lookup"><span data-stu-id="73f32-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73f32-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73f32-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73f32-155">Цель — C</span><span class="sxs-lookup"><span data-stu-id="73f32-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="73f32-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="73f32-156">Response</span></span>
<span data-ttu-id="73f32-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73f32-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKoAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DO\"",
  "id": "AAMkADA1MTAAAH5JKoAAA=",
  "subject": "RE: Let's start a group",
  "Body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body>Samantha, Randi, would you name the group if the project is approved, please?\r\n<b>From:</b> Samantha Booth<br>\r\n<b>Sent:</b> Friday, March 4, 2016 12:23:35 AM<br>\r\n<b>To:</b> Admin<br>\r\n<b>Subject:</b> Re: Let's start a group</font>\r\n<p>That's a great idea!<br>\r\n</body>\r\n</html>"
  },
  "sender": {
    "emailAddress": {
      "name": "Admin",
      "address": "admin@contoso.onmicrosoft.com"
    }
  },
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com"
      }
    },
    {
      "emailAddress": {
        "name": "Randi Welch",
        "address": "randiw@contoso.onmicrosoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
