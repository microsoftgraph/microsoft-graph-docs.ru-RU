---
title: 'message: createReplyAll'
description: 'Создание черновика сообщения ответить всем добавить примечание или обновить все свойства сообщения '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7f0b2631f02a94a7627e96e24308b135d70d20e1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922174"
---
# <a name="message-createreplyall"></a><span data-ttu-id="eba93-103">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="eba93-103">message: createReplyAll</span></span>

> <span data-ttu-id="eba93-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eba93-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eba93-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eba93-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eba93-106">Создание черновика сообщения ответить всем добавить примечание или обновить все свойства сообщения в одном вызове **createReplyAll** .</span><span class="sxs-lookup"><span data-stu-id="eba93-106">Create a draft of a reply-all message to include a comment or update any message properties, all in one **createReplyAll** call.</span></span> <span data-ttu-id="eba93-107">После этого можно [Обновить](../api/message-update.md) или [Отправить](../api/message-send.md) черновик.</span><span class="sxs-lookup"><span data-stu-id="eba93-107">You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="eba93-108">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="eba93-108">**Note**</span></span>

- <span data-ttu-id="eba93-109">Можно указать комментарий или свойству **body** `message` параметр.</span><span class="sxs-lookup"><span data-stu-id="eba93-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="eba93-110">Указание оба возвратит ошибку HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="eba93-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="eba93-111">Если свойство **replyTo** указано в исходное сообщение в формат сообщений Интернета ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), следует отправить ответ в список получателей в</span><span class="sxs-lookup"><span data-stu-id="eba93-111">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="eba93-112">свойства **replyTo** и **toRecipients** , а не в список получателей в свойства **из** и **toRecipients** .</span><span class="sxs-lookup"><span data-stu-id="eba93-112">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="eba93-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eba93-113">Permissions</span></span>
<span data-ttu-id="eba93-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eba93-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eba93-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eba93-116">Permission type</span></span>      | <span data-ttu-id="eba93-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eba93-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eba93-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eba93-118">Delegated (work or school account)</span></span> | <span data-ttu-id="eba93-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eba93-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eba93-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eba93-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eba93-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eba93-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eba93-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eba93-122">Application</span></span> | <span data-ttu-id="eba93-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eba93-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eba93-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eba93-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="eba93-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eba93-125">Request headers</span></span>
| <span data-ttu-id="eba93-126">Имя</span><span class="sxs-lookup"><span data-stu-id="eba93-126">Name</span></span>       | <span data-ttu-id="eba93-127">Тип</span><span class="sxs-lookup"><span data-stu-id="eba93-127">Type</span></span> | <span data-ttu-id="eba93-128">Описание</span><span class="sxs-lookup"><span data-stu-id="eba93-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eba93-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="eba93-129">Authorization</span></span>  | <span data-ttu-id="eba93-130">строка</span><span class="sxs-lookup"><span data-stu-id="eba93-130">string</span></span>  | <span data-ttu-id="eba93-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eba93-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eba93-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eba93-133">Content-Type</span></span> | <span data-ttu-id="eba93-134">строка</span><span class="sxs-lookup"><span data-stu-id="eba93-134">string</span></span>  | <span data-ttu-id="eba93-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eba93-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eba93-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eba93-137">Request body</span></span>
<span data-ttu-id="eba93-138">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="eba93-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eba93-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="eba93-139">Parameter</span></span>    | <span data-ttu-id="eba93-140">Тип</span><span class="sxs-lookup"><span data-stu-id="eba93-140">Type</span></span>   |<span data-ttu-id="eba93-141">Описание</span><span class="sxs-lookup"><span data-stu-id="eba93-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eba93-142">comment</span><span class="sxs-lookup"><span data-stu-id="eba93-142">comment</span></span>|<span data-ttu-id="eba93-143">String</span><span class="sxs-lookup"><span data-stu-id="eba93-143">String</span></span>|<span data-ttu-id="eba93-p107">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="eba93-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="eba93-146">message</span><span class="sxs-lookup"><span data-stu-id="eba93-146">message</span></span>|[<span data-ttu-id="eba93-147">message</span><span class="sxs-lookup"><span data-stu-id="eba93-147">message</span></span>](../resources/message.md)|<span data-ttu-id="eba93-148">Любой доступный свойства для обновления в сообщении ответить всем.</span><span class="sxs-lookup"><span data-stu-id="eba93-148">Any writeable properties to update in the reply-all message.</span></span>|

## <a name="response"></a><span data-ttu-id="eba93-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="eba93-149">Response</span></span>

<span data-ttu-id="eba93-150">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eba93-150">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eba93-151">Пример</span><span class="sxs-lookup"><span data-stu-id="eba93-151">Example</span></span>
<span data-ttu-id="eba93-152">В следующем примере создается черновиков, чтобы ответить всем и добавляет вложение и комментария в вызове одной **createReplyAll** .</span><span class="sxs-lookup"><span data-stu-id="eba93-152">The following example creates a draft to reply all, and adds an attachment and comment all in one **createReplyAll** call.</span></span>
##### <a name="request"></a><span data-ttu-id="eba93-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="eba93-153">Request</span></span>
<span data-ttu-id="eba93-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eba93-154">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="eba93-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="eba93-155">Response</span></span>
<span data-ttu-id="eba93-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="eba93-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
