---
title: 'message: createForward'
description: 'Создание черновика переадресации сообщений для включения комментария или обновления любых свойств сообщения  '
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4f1ad719afb21a6e8fca724171029d4d924e4fd2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027673"
---
# <a name="message-createforward"></a><span data-ttu-id="2ef53-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="2ef53-103">message: createForward</span></span>

<span data-ttu-id="2ef53-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ef53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ef53-105">Создание черновика переадресации сообщений для включения комментария или обновления любых свойств сообщения</span><span class="sxs-lookup"><span data-stu-id="2ef53-105">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="2ef53-106">все в одном вызове **createForward** .</span><span class="sxs-lookup"><span data-stu-id="2ef53-106">all in one **createForward** call.</span></span> <span data-ttu-id="2ef53-107">Затем вы можете [Отправить](../api/message-send.md) черновик сообщения.</span><span class="sxs-lookup"><span data-stu-id="2ef53-107">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="2ef53-108">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="2ef53-108">**Note**</span></span>

- <span data-ttu-id="2ef53-109">Можно указать либо свойство Comment, либо свойство **Body** для `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="2ef53-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="2ef53-110">Если указать и то, и другое, будет возвращена ошибка неправильного запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="2ef53-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="2ef53-111">Необходимо указать либо параметр, `toRecipients` либо свойство **toRecipients** `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="2ef53-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="2ef53-112">Если указать оба параметра или не указывать ни один из них, будет возвращена ошибка ошибки запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="2ef53-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ef53-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ef53-113">Permissions</span></span>
<span data-ttu-id="2ef53-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ef53-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ef53-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ef53-116">Permission type</span></span>      | <span data-ttu-id="2ef53-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ef53-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ef53-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ef53-118">Delegated (work or school account)</span></span> | <span data-ttu-id="2ef53-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ef53-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2ef53-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ef53-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ef53-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ef53-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2ef53-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ef53-122">Application</span></span> | <span data-ttu-id="2ef53-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ef53-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ef53-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ef53-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="2ef53-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ef53-125">Request headers</span></span>
| <span data-ttu-id="2ef53-126">Имя</span><span class="sxs-lookup"><span data-stu-id="2ef53-126">Name</span></span>       | <span data-ttu-id="2ef53-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2ef53-127">Type</span></span> | <span data-ttu-id="2ef53-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2ef53-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2ef53-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ef53-129">Authorization</span></span>  | <span data-ttu-id="2ef53-130">string</span><span class="sxs-lookup"><span data-stu-id="2ef53-130">string</span></span>  | <span data-ttu-id="2ef53-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ef53-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2ef53-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ef53-133">Content-Type</span></span> | <span data-ttu-id="2ef53-134">string</span><span class="sxs-lookup"><span data-stu-id="2ef53-134">string</span></span>  | <span data-ttu-id="2ef53-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ef53-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ef53-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ef53-137">Request body</span></span>
<span data-ttu-id="2ef53-138">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2ef53-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2ef53-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="2ef53-139">Parameter</span></span>    | <span data-ttu-id="2ef53-140">Тип</span><span class="sxs-lookup"><span data-stu-id="2ef53-140">Type</span></span>   |<span data-ttu-id="2ef53-141">Описание</span><span class="sxs-lookup"><span data-stu-id="2ef53-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ef53-142">comment</span><span class="sxs-lookup"><span data-stu-id="2ef53-142">comment</span></span>|<span data-ttu-id="2ef53-143">String</span><span class="sxs-lookup"><span data-stu-id="2ef53-143">String</span></span>|<span data-ttu-id="2ef53-p107">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="2ef53-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="2ef53-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="2ef53-146">toRecipients</span></span>|<span data-ttu-id="2ef53-147">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="2ef53-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="2ef53-148">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="2ef53-148">The list of recipients.</span></span>|
|<span data-ttu-id="2ef53-149">message</span><span class="sxs-lookup"><span data-stu-id="2ef53-149">message</span></span>|[<span data-ttu-id="2ef53-150">message</span><span class="sxs-lookup"><span data-stu-id="2ef53-150">message</span></span>](../resources/message.md)|<span data-ttu-id="2ef53-151">Все доступные для записи свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="2ef53-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="2ef53-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ef53-152">Response</span></span>

<span data-ttu-id="2ef53-153">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2ef53-153">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ef53-154">Пример</span><span class="sxs-lookup"><span data-stu-id="2ef53-154">Example</span></span>
<span data-ttu-id="2ef53-155">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2ef53-155">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2ef53-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ef53-156">Request</span></span>
<span data-ttu-id="2ef53-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ef53-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ef53-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef53-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2ef53-159">C#</span><span class="sxs-lookup"><span data-stu-id="2ef53-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createforward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ef53-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ef53-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createforward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ef53-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ef53-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createforward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2ef53-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ef53-162">Response</span></span>
<span data-ttu-id="2ef53-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ef53-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


