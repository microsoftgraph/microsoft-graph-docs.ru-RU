---
title: 'message: createReply'
description: 'Создание черновика ответного сообщения с комментарием или обновлением свойств сообщения '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d2943f5a822ce02c3fc4c8fd1e6ae34e6d6f7b98
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134732"
---
# <a name="message-createreply"></a><span data-ttu-id="10dc4-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="10dc4-103">message: createReply</span></span>

<span data-ttu-id="10dc4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10dc4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10dc4-105">Создание черновика ответного сообщения, чтобы добавить комментарий или обновить любые свойства сообщения одновременно в одном вызове **createReply**.</span><span class="sxs-lookup"><span data-stu-id="10dc4-105">Create a draft of a reply message to include a comment or update any message properties all in one **createReply** call.</span></span> <span data-ttu-id="10dc4-106">После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.</span><span class="sxs-lookup"><span data-stu-id="10dc4-106">You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="10dc4-107">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="10dc4-107">**Note**</span></span>

- <span data-ttu-id="10dc4-108">Можно указать комментарий или свойство **body** `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="10dc4-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="10dc4-109">Если указать оба этих запроса, будет возвращена ошибка "HTTP 400 Bad Request".</span><span class="sxs-lookup"><span data-stu-id="10dc4-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="10dc4-110">Если **replyTo** указан в исходном сообщении в формате интернет-сообщений [(RFC 2822),](https://www.rfc-editor.org/info/rfc2822)необходимо отправить ответ получателям в **replyTo,** а не получателям из **.**</span><span class="sxs-lookup"><span data-stu-id="10dc4-110">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="10dc4-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10dc4-111">Permissions</span></span>
<span data-ttu-id="10dc4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10dc4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10dc4-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10dc4-114">Permission type</span></span>      | <span data-ttu-id="10dc4-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10dc4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10dc4-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10dc4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="10dc4-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10dc4-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="10dc4-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10dc4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10dc4-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10dc4-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="10dc4-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10dc4-120">Application</span></span> | <span data-ttu-id="10dc4-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10dc4-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="10dc4-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10dc4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="10dc4-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10dc4-123">Request headers</span></span>
| <span data-ttu-id="10dc4-124">Имя</span><span class="sxs-lookup"><span data-stu-id="10dc4-124">Name</span></span>       | <span data-ttu-id="10dc4-125">Тип</span><span class="sxs-lookup"><span data-stu-id="10dc4-125">Type</span></span> | <span data-ttu-id="10dc4-126">Описание</span><span class="sxs-lookup"><span data-stu-id="10dc4-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="10dc4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="10dc4-127">Authorization</span></span>  | <span data-ttu-id="10dc4-128">string</span><span class="sxs-lookup"><span data-stu-id="10dc4-128">string</span></span>  | <span data-ttu-id="10dc4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10dc4-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="10dc4-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10dc4-131">Content-Type</span></span> | <span data-ttu-id="10dc4-132">string</span><span class="sxs-lookup"><span data-stu-id="10dc4-132">string</span></span>  | <span data-ttu-id="10dc4-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10dc4-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10dc4-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10dc4-135">Request body</span></span>
<span data-ttu-id="10dc4-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="10dc4-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="10dc4-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="10dc4-137">Parameter</span></span>    | <span data-ttu-id="10dc4-138">Тип</span><span class="sxs-lookup"><span data-stu-id="10dc4-138">Type</span></span>   |<span data-ttu-id="10dc4-139">Описание</span><span class="sxs-lookup"><span data-stu-id="10dc4-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10dc4-140">comment</span><span class="sxs-lookup"><span data-stu-id="10dc4-140">comment</span></span>|<span data-ttu-id="10dc4-141">String</span><span class="sxs-lookup"><span data-stu-id="10dc4-141">String</span></span>|<span data-ttu-id="10dc4-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="10dc4-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="10dc4-144">message</span><span class="sxs-lookup"><span data-stu-id="10dc4-144">message</span></span>|[<span data-ttu-id="10dc4-145">message</span><span class="sxs-lookup"><span data-stu-id="10dc4-145">message</span></span>](../resources/message.md)|<span data-ttu-id="10dc4-146">Любые записаемые свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="10dc4-146">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="10dc4-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="10dc4-147">Response</span></span>

<span data-ttu-id="10dc4-148">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="10dc4-148">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10dc4-149">Пример</span><span class="sxs-lookup"><span data-stu-id="10dc4-149">Example</span></span>
<span data-ttu-id="10dc4-150">В следующем примере создается черновик ответа, добавляется комментарий и получатель в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="10dc4-150">The following example creates a reply draft, adds a comment and a recipient in the request body.</span></span>
##### <a name="request"></a><span data-ttu-id="10dc4-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="10dc4-151">Request</span></span>
<span data-ttu-id="10dc4-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10dc4-152">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="10dc4-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="10dc4-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="10dc4-154">C#</span><span class="sxs-lookup"><span data-stu-id="10dc4-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10dc4-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10dc4-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10dc4-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10dc4-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10dc4-157">Java</span><span class="sxs-lookup"><span data-stu-id="10dc4-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="10dc4-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="10dc4-158">Response</span></span>
<span data-ttu-id="10dc4-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10dc4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


