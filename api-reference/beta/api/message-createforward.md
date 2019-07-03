---
title: 'message: createForward'
description: 'Создание черновика переадресации сообщений для включения комментария или обновления любых свойств сообщения  '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0b1ce182e58d5e2033b1e9cac0f1025df1dd6e89
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448280"
---
# <a name="message-createforward"></a><span data-ttu-id="a884e-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="a884e-103">message: createForward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a884e-104">Создание черновика переадресации сообщений для включения комментария или обновления любых свойств сообщения</span><span class="sxs-lookup"><span data-stu-id="a884e-104">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="a884e-105">все в одном вызове **createForward** .</span><span class="sxs-lookup"><span data-stu-id="a884e-105">all in one **createForward** call.</span></span> <span data-ttu-id="a884e-106">Затем вы можете [Отправить](../api/message-send.md) черновик сообщения.</span><span class="sxs-lookup"><span data-stu-id="a884e-106">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="a884e-107">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="a884e-107">**Note**</span></span>

- <span data-ttu-id="a884e-108">Можно указать либо свойство Comment, либо свойство **Body** для `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="a884e-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="a884e-109">Если указать и то, и другое, будет возвращена ошибка неправильного запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="a884e-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="a884e-110">Необходимо указать либо параметр, `toRecipients` либо свойство **toRecipients** `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="a884e-110">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="a884e-111">Если указать оба параметра или не указывать ни один из них, будет возвращена ошибка ошибки запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="a884e-111">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="a884e-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a884e-112">Permissions</span></span>
<span data-ttu-id="a884e-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a884e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a884e-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a884e-115">Permission type</span></span>      | <span data-ttu-id="a884e-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a884e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a884e-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a884e-117">Delegated (work or school account)</span></span> | <span data-ttu-id="a884e-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a884e-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a884e-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a884e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a884e-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a884e-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a884e-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a884e-121">Application</span></span> | <span data-ttu-id="a884e-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a884e-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a884e-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a884e-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="a884e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a884e-124">Request headers</span></span>
| <span data-ttu-id="a884e-125">Имя</span><span class="sxs-lookup"><span data-stu-id="a884e-125">Name</span></span>       | <span data-ttu-id="a884e-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a884e-126">Type</span></span> | <span data-ttu-id="a884e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a884e-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a884e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a884e-128">Authorization</span></span>  | <span data-ttu-id="a884e-129">string</span><span class="sxs-lookup"><span data-stu-id="a884e-129">string</span></span>  | <span data-ttu-id="a884e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a884e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a884e-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a884e-132">Content-Type</span></span> | <span data-ttu-id="a884e-133">string</span><span class="sxs-lookup"><span data-stu-id="a884e-133">string</span></span>  | <span data-ttu-id="a884e-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a884e-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a884e-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a884e-136">Request body</span></span>
<span data-ttu-id="a884e-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a884e-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a884e-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="a884e-138">Parameter</span></span>    | <span data-ttu-id="a884e-139">Тип</span><span class="sxs-lookup"><span data-stu-id="a884e-139">Type</span></span>   |<span data-ttu-id="a884e-140">Описание</span><span class="sxs-lookup"><span data-stu-id="a884e-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a884e-141">comment</span><span class="sxs-lookup"><span data-stu-id="a884e-141">comment</span></span>|<span data-ttu-id="a884e-142">String</span><span class="sxs-lookup"><span data-stu-id="a884e-142">String</span></span>|<span data-ttu-id="a884e-p107">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="a884e-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="a884e-145">toRecipients</span><span class="sxs-lookup"><span data-stu-id="a884e-145">toRecipients</span></span>|<span data-ttu-id="a884e-146">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="a884e-146">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="a884e-147">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="a884e-147">The list of recipients.</span></span>|
|<span data-ttu-id="a884e-148">message</span><span class="sxs-lookup"><span data-stu-id="a884e-148">message</span></span>|[<span data-ttu-id="a884e-149">message</span><span class="sxs-lookup"><span data-stu-id="a884e-149">message</span></span>](../resources/message.md)|<span data-ttu-id="a884e-150">Все доступные для записи свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="a884e-150">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="a884e-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="a884e-151">Response</span></span>

<span data-ttu-id="a884e-152">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a884e-152">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a884e-153">Пример</span><span class="sxs-lookup"><span data-stu-id="a884e-153">Example</span></span>
<span data-ttu-id="a884e-154">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a884e-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a884e-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="a884e-155">Request</span></span>
<span data-ttu-id="a884e-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a884e-156">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a884e-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="a884e-157">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a884e-158">C#</span><span class="sxs-lookup"><span data-stu-id="a884e-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createforward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a884e-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="a884e-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createforward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a884e-160">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a884e-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createforward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a884e-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="a884e-161">Response</span></span>
<span data-ttu-id="a884e-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a884e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
