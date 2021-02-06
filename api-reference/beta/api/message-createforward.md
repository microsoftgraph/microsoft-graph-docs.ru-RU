---
title: 'message: createForward'
description: 'Создание черновика переадментного сообщения с комментарием или обновлением свойств сообщения  '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e36487e3e25e4eac30c4c05987082b26b31601f3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136733"
---
# <a name="message-createforward"></a><span data-ttu-id="0190f-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="0190f-103">message: createForward</span></span>

<span data-ttu-id="0190f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0190f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0190f-105">Создание черновика переадментного сообщения с комментарием или обновлением свойств сообщения</span><span class="sxs-lookup"><span data-stu-id="0190f-105">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="0190f-106">все в одном **вызове createForward.**</span><span class="sxs-lookup"><span data-stu-id="0190f-106">all in one **createForward** call.</span></span> <span data-ttu-id="0190f-107">Затем можно отправить [черновик](../api/message-send.md) сообщения.</span><span class="sxs-lookup"><span data-stu-id="0190f-107">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="0190f-108">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="0190f-108">**Note**</span></span>

- <span data-ttu-id="0190f-109">Можно указать комментарий или свойство **body** `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="0190f-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="0190f-110">Если указать оба этих запроса, будет возвращена ошибка "HTTP 400 Bad Request".</span><span class="sxs-lookup"><span data-stu-id="0190f-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="0190f-111">Необходимо указать либо параметр, либо свойство `toRecipients` **toRecipients** `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="0190f-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="0190f-112">Если указать и то, и другое, не будет возвращена ошибка HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="0190f-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="0190f-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0190f-113">Permissions</span></span>
<span data-ttu-id="0190f-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0190f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0190f-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0190f-116">Permission type</span></span>      | <span data-ttu-id="0190f-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0190f-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0190f-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0190f-118">Delegated (work or school account)</span></span> | <span data-ttu-id="0190f-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0190f-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0190f-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0190f-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0190f-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0190f-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0190f-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0190f-122">Application</span></span> | <span data-ttu-id="0190f-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0190f-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0190f-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0190f-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="0190f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0190f-125">Request headers</span></span>
| <span data-ttu-id="0190f-126">Имя</span><span class="sxs-lookup"><span data-stu-id="0190f-126">Name</span></span>       | <span data-ttu-id="0190f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="0190f-127">Type</span></span> | <span data-ttu-id="0190f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0190f-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0190f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="0190f-129">Authorization</span></span>  | <span data-ttu-id="0190f-130">string</span><span class="sxs-lookup"><span data-stu-id="0190f-130">string</span></span>  | <span data-ttu-id="0190f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0190f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0190f-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0190f-133">Content-Type</span></span> | <span data-ttu-id="0190f-134">string</span><span class="sxs-lookup"><span data-stu-id="0190f-134">string</span></span>  | <span data-ttu-id="0190f-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0190f-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0190f-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0190f-137">Request body</span></span>
<span data-ttu-id="0190f-138">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0190f-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0190f-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="0190f-139">Parameter</span></span>    | <span data-ttu-id="0190f-140">Тип</span><span class="sxs-lookup"><span data-stu-id="0190f-140">Type</span></span>   |<span data-ttu-id="0190f-141">Описание</span><span class="sxs-lookup"><span data-stu-id="0190f-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0190f-142">comment</span><span class="sxs-lookup"><span data-stu-id="0190f-142">comment</span></span>|<span data-ttu-id="0190f-143">String</span><span class="sxs-lookup"><span data-stu-id="0190f-143">String</span></span>|<span data-ttu-id="0190f-p107">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="0190f-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="0190f-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="0190f-146">toRecipients</span></span>|<span data-ttu-id="0190f-147">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="0190f-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="0190f-148">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="0190f-148">The list of recipients.</span></span>|
|<span data-ttu-id="0190f-149">message</span><span class="sxs-lookup"><span data-stu-id="0190f-149">message</span></span>|[<span data-ttu-id="0190f-150">message</span><span class="sxs-lookup"><span data-stu-id="0190f-150">message</span></span>](../resources/message.md)|<span data-ttu-id="0190f-151">Любые записаемые свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="0190f-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="0190f-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="0190f-152">Response</span></span>

<span data-ttu-id="0190f-153">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0190f-153">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0190f-154">Пример</span><span class="sxs-lookup"><span data-stu-id="0190f-154">Example</span></span>
<span data-ttu-id="0190f-155">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0190f-155">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0190f-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="0190f-156">Request</span></span>
<span data-ttu-id="0190f-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0190f-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0190f-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="0190f-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0190f-159">C#</span><span class="sxs-lookup"><span data-stu-id="0190f-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createforward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0190f-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0190f-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createforward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0190f-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0190f-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createforward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0190f-162">Java</span><span class="sxs-lookup"><span data-stu-id="0190f-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createforward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0190f-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="0190f-163">Response</span></span>
<span data-ttu-id="0190f-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0190f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


