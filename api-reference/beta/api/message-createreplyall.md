---
title: 'message: createReplyAll'
description: 'Создание черновика сообщения "ответить всем" для включения комментария или обновления любых свойств сообщения '
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 992cc883a99bcd5877035fc8dd8faee8b7604c12
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981580"
---
# <a name="message-createreplyall"></a><span data-ttu-id="196cd-103">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="196cd-103">message: createReplyAll</span></span>

<span data-ttu-id="196cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="196cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="196cd-105">Создание черновика сообщения "Ответить всем", чтобы добавить комментарий или обновить любые свойства сообщения одновременно в одном вызове **createReplyAll**.</span><span class="sxs-lookup"><span data-stu-id="196cd-105">Create a draft of a reply-all message to include a comment or update any message properties, all in one **createReplyAll** call.</span></span> <span data-ttu-id="196cd-106">После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.</span><span class="sxs-lookup"><span data-stu-id="196cd-106">You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="196cd-107">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="196cd-107">**Note**</span></span>

- <span data-ttu-id="196cd-108">Можно указать либо свойство Comment, либо свойство **Body** для `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="196cd-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="196cd-109">Если указать и то, и другое, будет возвращена ошибка неправильного запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="196cd-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="196cd-110">Если свойство **replyTo** указано в исходном сообщении, в формате Интернет-сообщений ( [RFC 2822](https://www.rfc-editor.org/info/rfc2822)), необходимо отправить ответ получателям в</span><span class="sxs-lookup"><span data-stu-id="196cd-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="196cd-111">свойства **replyTo** и **toRecipients** , а не получатели в свойствах **from** и **toRecipients** .</span><span class="sxs-lookup"><span data-stu-id="196cd-111">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="196cd-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="196cd-112">Permissions</span></span>
<span data-ttu-id="196cd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="196cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="196cd-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="196cd-115">Permission type</span></span>      | <span data-ttu-id="196cd-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="196cd-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="196cd-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="196cd-117">Delegated (work or school account)</span></span> | <span data-ttu-id="196cd-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="196cd-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="196cd-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="196cd-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="196cd-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="196cd-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="196cd-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="196cd-121">Application</span></span> | <span data-ttu-id="196cd-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="196cd-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="196cd-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="196cd-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="196cd-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="196cd-124">Request headers</span></span>
| <span data-ttu-id="196cd-125">Имя</span><span class="sxs-lookup"><span data-stu-id="196cd-125">Name</span></span>       | <span data-ttu-id="196cd-126">Тип</span><span class="sxs-lookup"><span data-stu-id="196cd-126">Type</span></span> | <span data-ttu-id="196cd-127">Описание</span><span class="sxs-lookup"><span data-stu-id="196cd-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="196cd-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="196cd-128">Authorization</span></span>  | <span data-ttu-id="196cd-129">string</span><span class="sxs-lookup"><span data-stu-id="196cd-129">string</span></span>  | <span data-ttu-id="196cd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="196cd-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="196cd-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="196cd-132">Content-Type</span></span> | <span data-ttu-id="196cd-133">string</span><span class="sxs-lookup"><span data-stu-id="196cd-133">string</span></span>  | <span data-ttu-id="196cd-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="196cd-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="196cd-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="196cd-136">Request body</span></span>
<span data-ttu-id="196cd-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="196cd-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="196cd-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="196cd-138">Parameter</span></span>    | <span data-ttu-id="196cd-139">Тип</span><span class="sxs-lookup"><span data-stu-id="196cd-139">Type</span></span>   |<span data-ttu-id="196cd-140">Описание</span><span class="sxs-lookup"><span data-stu-id="196cd-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="196cd-141">comment</span><span class="sxs-lookup"><span data-stu-id="196cd-141">comment</span></span>|<span data-ttu-id="196cd-142">String</span><span class="sxs-lookup"><span data-stu-id="196cd-142">String</span></span>|<span data-ttu-id="196cd-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="196cd-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="196cd-145">message</span><span class="sxs-lookup"><span data-stu-id="196cd-145">message</span></span>|[<span data-ttu-id="196cd-146">message</span><span class="sxs-lookup"><span data-stu-id="196cd-146">message</span></span>](../resources/message.md)|<span data-ttu-id="196cd-147">Все доступные для записи свойства, которые необходимо обновить в сообщении "ответить всем".</span><span class="sxs-lookup"><span data-stu-id="196cd-147">Any writeable properties to update in the reply-all message.</span></span>|

## <a name="response"></a><span data-ttu-id="196cd-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="196cd-148">Response</span></span>

<span data-ttu-id="196cd-149">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="196cd-149">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="196cd-150">Пример</span><span class="sxs-lookup"><span data-stu-id="196cd-150">Example</span></span>
<span data-ttu-id="196cd-151">В следующем примере создается черновик для ответа ALL и добавляется вложение и комментарий в одном вызове **createReplyAll** .</span><span class="sxs-lookup"><span data-stu-id="196cd-151">The following example creates a draft to reply all, and adds an attachment and comment all in one **createReplyAll** call.</span></span>
##### <a name="request"></a><span data-ttu-id="196cd-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="196cd-152">Request</span></span>
<span data-ttu-id="196cd-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="196cd-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="196cd-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="196cd-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/createReplyAll
Content-Type: application/json

{
    "message":{
      "attachments": [ 
        { 
          "@odata.type": "#microsoft.graph.fileAttachment", 
          "name": "guidelines.txt", 
          "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk=" 
        } 
      ]
    },
    "comment": "if the project gets approved, please take a look at the attached guidelines before you decide on the name." 
}
```
# <a name="c"></a>[<span data-ttu-id="196cd-155">C#</span><span class="sxs-lookup"><span data-stu-id="196cd-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreplyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="196cd-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="196cd-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreplyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="196cd-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="196cd-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreplyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="196cd-158">Java</span><span class="sxs-lookup"><span data-stu-id="196cd-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreplyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="196cd-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="196cd-159">Response</span></span>
<span data-ttu-id="196cd-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="196cd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKpAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DP\"",
  "id": "AAMkADA1MTAAAH5JKpAAA=",
  "subject": "RE: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body dir=\"ltr\">\r\nif the project gets approved, please take a look at the attached guidelines before you decide on the name.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:36:32 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group\r\n<div>Samantha, Randi, would you name the group please?\r\n<b>From:</b> Samantha Booth<br>\r\n<b>Sent:</b> Friday, March 4, 2016 12:23:35 AM<br>\r\n<b>To:</b> Admin<br>\r\n<b>Subject:</b> Re: Let's start a group</font>\r\n</body>\r\n</html>"
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
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


