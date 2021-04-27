---
title: 'message: createForward'
description: 'Создайте проект сообщения, чтобы включить комментарий или обновить свойства сообщений  '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: dd0802fa9443067fe4db9edd53783b800d81ce8c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052175"
---
# <a name="message-createforward"></a><span data-ttu-id="948fe-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="948fe-103">message: createForward</span></span>

<span data-ttu-id="948fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="948fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="948fe-105">Создайте проект сообщения, чтобы включить комментарий или обновить свойства сообщений</span><span class="sxs-lookup"><span data-stu-id="948fe-105">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="948fe-106">все в одном **вызове createForward.**</span><span class="sxs-lookup"><span data-stu-id="948fe-106">all in one **createForward** call.</span></span> <span data-ttu-id="948fe-107">Затем можно [отправить черновик](../api/message-send.md) сообщения.</span><span class="sxs-lookup"><span data-stu-id="948fe-107">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="948fe-108">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="948fe-108">**Note**</span></span>

- <span data-ttu-id="948fe-109">Вы можете указать комментарий или **свойство** тела `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="948fe-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="948fe-110">При указании обоих возвращается ошибка http 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="948fe-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="948fe-111">Необходимо указать параметр `toRecipients` или **свойство toRecipients** `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="948fe-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="948fe-112">Указание обоих или указаний не возвращает ошибку http 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="948fe-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="948fe-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="948fe-113">Permissions</span></span>
<span data-ttu-id="948fe-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="948fe-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="948fe-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="948fe-116">Permission type</span></span>      | <span data-ttu-id="948fe-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="948fe-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="948fe-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="948fe-118">Delegated (work or school account)</span></span> | <span data-ttu-id="948fe-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="948fe-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="948fe-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="948fe-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="948fe-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="948fe-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="948fe-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="948fe-122">Application</span></span> | <span data-ttu-id="948fe-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="948fe-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="948fe-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="948fe-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="948fe-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="948fe-125">Request headers</span></span>
| <span data-ttu-id="948fe-126">Имя</span><span class="sxs-lookup"><span data-stu-id="948fe-126">Name</span></span>       | <span data-ttu-id="948fe-127">Тип</span><span class="sxs-lookup"><span data-stu-id="948fe-127">Type</span></span> | <span data-ttu-id="948fe-128">Описание</span><span class="sxs-lookup"><span data-stu-id="948fe-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="948fe-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="948fe-129">Authorization</span></span>  | <span data-ttu-id="948fe-130">string</span><span class="sxs-lookup"><span data-stu-id="948fe-130">string</span></span>  | <span data-ttu-id="948fe-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="948fe-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="948fe-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="948fe-133">Content-Type</span></span> | <span data-ttu-id="948fe-134">string</span><span class="sxs-lookup"><span data-stu-id="948fe-134">string</span></span>  | <span data-ttu-id="948fe-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="948fe-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="948fe-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="948fe-137">Request body</span></span>
<span data-ttu-id="948fe-138">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="948fe-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="948fe-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="948fe-139">Parameter</span></span>    | <span data-ttu-id="948fe-140">Тип</span><span class="sxs-lookup"><span data-stu-id="948fe-140">Type</span></span>   |<span data-ttu-id="948fe-141">Описание</span><span class="sxs-lookup"><span data-stu-id="948fe-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="948fe-142">comment</span><span class="sxs-lookup"><span data-stu-id="948fe-142">comment</span></span>|<span data-ttu-id="948fe-143">String</span><span class="sxs-lookup"><span data-stu-id="948fe-143">String</span></span>|<span data-ttu-id="948fe-p107">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="948fe-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="948fe-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="948fe-146">toRecipients</span></span>|<span data-ttu-id="948fe-147">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="948fe-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="948fe-148">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="948fe-148">The list of recipients.</span></span>|
|<span data-ttu-id="948fe-149">message</span><span class="sxs-lookup"><span data-stu-id="948fe-149">message</span></span>|[<span data-ttu-id="948fe-150">message</span><span class="sxs-lookup"><span data-stu-id="948fe-150">message</span></span>](../resources/message.md)|<span data-ttu-id="948fe-151">Любые свойства, которые можно записать для обновления в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="948fe-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="948fe-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="948fe-152">Response</span></span>

<span data-ttu-id="948fe-153">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="948fe-153">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="948fe-154">Пример</span><span class="sxs-lookup"><span data-stu-id="948fe-154">Example</span></span>
<span data-ttu-id="948fe-155">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="948fe-155">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="948fe-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="948fe-156">Request</span></span>
<span data-ttu-id="948fe-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="948fe-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="948fe-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="948fe-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/createForward
Content-Type: application/json

{
  "message":{  
    "isDeliveryReceiptRequested": true,
    "toRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ]
  },
  "comment": "Dana, just want to make sure you get this; you'll need this if the project gets approved." 
}
```
# <a name="c"></a>[<span data-ttu-id="948fe-159">C#</span><span class="sxs-lookup"><span data-stu-id="948fe-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createforward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="948fe-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="948fe-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createforward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="948fe-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="948fe-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createforward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="948fe-162">Java</span><span class="sxs-lookup"><span data-stu-id="948fe-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createforward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="948fe-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="948fe-163">Response</span></span>
<span data-ttu-id="948fe-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="948fe-164">Here is an example of the response.</span></span> <span data-ttu-id="948fe-165">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="948fe-165">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 272

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKqAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DQ\"",
  "id": "AAMkADA1MTAAAH5JKqAAA=",
  "subject": "FW: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body>\r\nDana, just want to make sure you get this; you'll need this if the project gets approved.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:47:54 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group</body>\r\n</html>\r\n"
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
        "name": "Dana Swope",
        "address": "danas@contoso.onmicrosoft.com"
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
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


