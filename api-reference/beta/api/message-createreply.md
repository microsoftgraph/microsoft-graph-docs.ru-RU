---
title: 'message: createReply'
description: 'Создание черновика ответного сообщения для включения комментария или обновления любого свойства сообщения '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 8c117eda36feda59db0fd3d9a599ce65a705d4c5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598342"
---
# <a name="message-createreply"></a><span data-ttu-id="0eb8a-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="0eb8a-103">message: createReply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0eb8a-104">Создание черновика ответного сообщения, чтобы добавить комментарий или обновить любые свойства сообщения одновременно в одном вызове **createReply**.</span><span class="sxs-lookup"><span data-stu-id="0eb8a-104">Create a draft of a reply message to include a comment or update any message properties all in one **createReply** call.</span></span> <span data-ttu-id="0eb8a-105">После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.</span><span class="sxs-lookup"><span data-stu-id="0eb8a-105">You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="0eb8a-106">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="0eb8a-106">**Note**</span></span>

- <span data-ttu-id="0eb8a-107">Можно указать либо свойство Comment, либо свойство **Body** для `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="0eb8a-107">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="0eb8a-108">Если указать и то, и другое, будет возвращена ошибка неправильного запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="0eb8a-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="0eb8a-109">Если параметр **replyTo** указан в исходном сообщении, в формате сообщения Интернета ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), необходимо отправить ответ получателям в **replyTo**, а не получателям **из**.</span><span class="sxs-lookup"><span data-stu-id="0eb8a-109">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0eb8a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0eb8a-110">Permissions</span></span>
<span data-ttu-id="0eb8a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0eb8a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0eb8a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0eb8a-113">Permission type</span></span>      | <span data-ttu-id="0eb8a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0eb8a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0eb8a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0eb8a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0eb8a-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0eb8a-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0eb8a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0eb8a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0eb8a-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0eb8a-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0eb8a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0eb8a-119">Application</span></span> | <span data-ttu-id="0eb8a-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0eb8a-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0eb8a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0eb8a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="0eb8a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0eb8a-122">Request headers</span></span>
| <span data-ttu-id="0eb8a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="0eb8a-123">Name</span></span>       | <span data-ttu-id="0eb8a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="0eb8a-124">Type</span></span> | <span data-ttu-id="0eb8a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0eb8a-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0eb8a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0eb8a-126">Authorization</span></span>  | <span data-ttu-id="0eb8a-127">string</span><span class="sxs-lookup"><span data-stu-id="0eb8a-127">string</span></span>  | <span data-ttu-id="0eb8a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0eb8a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0eb8a-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0eb8a-130">Content-Type</span></span> | <span data-ttu-id="0eb8a-131">string</span><span class="sxs-lookup"><span data-stu-id="0eb8a-131">string</span></span>  | <span data-ttu-id="0eb8a-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0eb8a-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0eb8a-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0eb8a-134">Request body</span></span>
<span data-ttu-id="0eb8a-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0eb8a-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0eb8a-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="0eb8a-136">Parameter</span></span>    | <span data-ttu-id="0eb8a-137">Тип</span><span class="sxs-lookup"><span data-stu-id="0eb8a-137">Type</span></span>   |<span data-ttu-id="0eb8a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="0eb8a-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0eb8a-139">comment</span><span class="sxs-lookup"><span data-stu-id="0eb8a-139">comment</span></span>|<span data-ttu-id="0eb8a-140">String</span><span class="sxs-lookup"><span data-stu-id="0eb8a-140">String</span></span>|<span data-ttu-id="0eb8a-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="0eb8a-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="0eb8a-143">message</span><span class="sxs-lookup"><span data-stu-id="0eb8a-143">message</span></span>|[<span data-ttu-id="0eb8a-144">message</span><span class="sxs-lookup"><span data-stu-id="0eb8a-144">message</span></span>](../resources/message.md)|<span data-ttu-id="0eb8a-145">Все доступные для записи свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="0eb8a-145">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="0eb8a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eb8a-146">Response</span></span>

<span data-ttu-id="0eb8a-147">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0eb8a-147">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0eb8a-148">Пример</span><span class="sxs-lookup"><span data-stu-id="0eb8a-148">Example</span></span>
<span data-ttu-id="0eb8a-149">В приведенном ниже примере создается черновик ответа, в тексте запроса добавляется комментарий и получатель.</span><span class="sxs-lookup"><span data-stu-id="0eb8a-149">The following example creates a reply draft, adds a comment and a recipient in the request body.</span></span>
##### <a name="request"></a><span data-ttu-id="0eb8a-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="0eb8a-150">Request</span></span>
<span data-ttu-id="0eb8a-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0eb8a-151">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0eb8a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eb8a-152">Response</span></span>
<span data-ttu-id="0eb8a-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0eb8a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0eb8a-156">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="0eb8a-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0eb8a-157">Языках</span><span class="sxs-lookup"><span data-stu-id="0eb8a-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_createreply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0eb8a-158">Язык</span><span class="sxs-lookup"><span data-stu-id="0eb8a-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_createreply-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/message-createreply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-createreply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
