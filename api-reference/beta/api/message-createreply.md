---
title: 'message: createReply'
description: 'Создание черновика сообщения ответа, чтобы добавить примечание или обновить все свойства сообщения '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 45dfd80be469d6a921eb70ba54f468b531eeb047
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873447"
---
# <a name="message-createreply"></a><span data-ttu-id="c9a63-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="c9a63-103">message: createReply</span></span>

> <span data-ttu-id="c9a63-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c9a63-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9a63-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9a63-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9a63-106">Создание черновика сообщения ответа, чтобы добавить примечание или обновить все свойства сообщения в одном вызове **createReply** .</span><span class="sxs-lookup"><span data-stu-id="c9a63-106">Create a draft of a reply message to include a comment or update any message properties all in one **createReply** call.</span></span> <span data-ttu-id="c9a63-107">После этого можно [Обновить](../api/message-update.md) или [Отправить](../api/message-send.md) черновик.</span><span class="sxs-lookup"><span data-stu-id="c9a63-107">You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="c9a63-108">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="c9a63-108">**Note**</span></span>

- <span data-ttu-id="c9a63-109">Можно указать комментарий или свойству **body** `message` параметр.</span><span class="sxs-lookup"><span data-stu-id="c9a63-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="c9a63-110">Указание оба возвратит ошибку HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="c9a63-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="c9a63-111">Если указано **replyTo** в исходное сообщение в формат сообщений Интернета ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), следует отправить ответ в список получателей в **replyTo**и не получателей в **из**.</span><span class="sxs-lookup"><span data-stu-id="c9a63-111">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c9a63-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9a63-112">Permissions</span></span>
<span data-ttu-id="c9a63-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9a63-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9a63-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9a63-115">Permission type</span></span>      | <span data-ttu-id="c9a63-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9a63-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9a63-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9a63-117">Delegated (work or school account)</span></span> | <span data-ttu-id="c9a63-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9a63-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c9a63-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9a63-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9a63-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9a63-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c9a63-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9a63-121">Application</span></span> | <span data-ttu-id="c9a63-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9a63-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9a63-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9a63-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="c9a63-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9a63-124">Request headers</span></span>
| <span data-ttu-id="c9a63-125">Имя</span><span class="sxs-lookup"><span data-stu-id="c9a63-125">Name</span></span>       | <span data-ttu-id="c9a63-126">Тип</span><span class="sxs-lookup"><span data-stu-id="c9a63-126">Type</span></span> | <span data-ttu-id="c9a63-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c9a63-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c9a63-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9a63-128">Authorization</span></span>  | <span data-ttu-id="c9a63-129">string</span><span class="sxs-lookup"><span data-stu-id="c9a63-129">string</span></span>  | <span data-ttu-id="c9a63-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9a63-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c9a63-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c9a63-132">Content-Type</span></span> | <span data-ttu-id="c9a63-133">string</span><span class="sxs-lookup"><span data-stu-id="c9a63-133">string</span></span>  | <span data-ttu-id="c9a63-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9a63-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9a63-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9a63-136">Request body</span></span>
<span data-ttu-id="c9a63-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c9a63-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c9a63-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="c9a63-138">Parameter</span></span>    | <span data-ttu-id="c9a63-139">Тип</span><span class="sxs-lookup"><span data-stu-id="c9a63-139">Type</span></span>   |<span data-ttu-id="c9a63-140">Описание</span><span class="sxs-lookup"><span data-stu-id="c9a63-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9a63-141">comment</span><span class="sxs-lookup"><span data-stu-id="c9a63-141">comment</span></span>|<span data-ttu-id="c9a63-142">String</span><span class="sxs-lookup"><span data-stu-id="c9a63-142">String</span></span>|<span data-ttu-id="c9a63-p107">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="c9a63-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="c9a63-145">message</span><span class="sxs-lookup"><span data-stu-id="c9a63-145">message</span></span>|[<span data-ttu-id="c9a63-146">message</span><span class="sxs-lookup"><span data-stu-id="c9a63-146">message</span></span>](../resources/message.md)|<span data-ttu-id="c9a63-147">Любой доступный свойства для обновления в ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="c9a63-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="c9a63-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9a63-148">Response</span></span>

<span data-ttu-id="c9a63-149">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c9a63-149">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9a63-150">Пример</span><span class="sxs-lookup"><span data-stu-id="c9a63-150">Example</span></span>
<span data-ttu-id="c9a63-151">Следующий пример создает ответ черновиков, добавляется комментарий и получателя в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="c9a63-151">The following example creates a reply draft, adds a comment and a recipient in the request body.</span></span>
##### <a name="request"></a><span data-ttu-id="c9a63-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9a63-152">Request</span></span>
<span data-ttu-id="c9a63-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9a63-153">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c9a63-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9a63-154">Response</span></span>
<span data-ttu-id="c9a63-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c9a63-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
