---
title: 'message: forward'
description: 'Пересылка сообщения, Добавление комментария или изменение любых обновляемых свойств  '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9b4e9ee3e2b0c97971e12143263a33e2241f876c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346928"
---
# <a name="message-forward"></a><span data-ttu-id="8be87-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="8be87-103">message: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8be87-104">Пересылка сообщения, Добавление комментария или изменение любых обновляемых свойств</span><span class="sxs-lookup"><span data-stu-id="8be87-104">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="8be87-105">все в одном **переадресации** звонка.</span><span class="sxs-lookup"><span data-stu-id="8be87-105">all in one **forward** call.</span></span> <span data-ttu-id="8be87-106">Сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="8be87-106">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="8be87-107">Кроме того, вы можете [создать черновик переадресации](../api/message-createforward.md) , чтобы включить комментарий или обновить все свойства сообщения, а затем [Отправить](../api/message-send.md) черновик сообщения.</span><span class="sxs-lookup"><span data-stu-id="8be87-107">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="8be87-108">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="8be87-108">**Note**</span></span>

- <span data-ttu-id="8be87-109">Можно указать либо свойство Comment, либо свойство **Body** для `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="8be87-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="8be87-110">Если указать и то, и другое, будет возвращена ошибка неправильного запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="8be87-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="8be87-111">Необходимо указать либо параметр, `toRecipients` либо свойство **toRecipients** `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="8be87-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="8be87-112">Если указать оба параметра или не указывать ни один из них, будет возвращена ошибка ошибки запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="8be87-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="8be87-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8be87-113">Permissions</span></span>
<span data-ttu-id="8be87-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8be87-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8be87-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8be87-116">Permission type</span></span>      | <span data-ttu-id="8be87-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8be87-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8be87-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8be87-118">Delegated (work or school account)</span></span> | <span data-ttu-id="8be87-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8be87-119">Mail.Send</span></span>    |
|<span data-ttu-id="8be87-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8be87-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8be87-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8be87-121">Mail.Send</span></span>    |
|<span data-ttu-id="8be87-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8be87-122">Application</span></span> | <span data-ttu-id="8be87-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8be87-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="8be87-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8be87-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="8be87-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8be87-125">Request headers</span></span>
| <span data-ttu-id="8be87-126">Имя</span><span class="sxs-lookup"><span data-stu-id="8be87-126">Name</span></span>       | <span data-ttu-id="8be87-127">Тип</span><span class="sxs-lookup"><span data-stu-id="8be87-127">Type</span></span> | <span data-ttu-id="8be87-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8be87-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8be87-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="8be87-129">Authorization</span></span>  | <span data-ttu-id="8be87-130">string</span><span class="sxs-lookup"><span data-stu-id="8be87-130">string</span></span>  | <span data-ttu-id="8be87-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8be87-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8be87-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8be87-133">Content-Type</span></span> | <span data-ttu-id="8be87-134">string</span><span class="sxs-lookup"><span data-stu-id="8be87-134">string</span></span>  | <span data-ttu-id="8be87-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8be87-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8be87-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8be87-137">Request body</span></span>
<span data-ttu-id="8be87-138">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8be87-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8be87-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="8be87-139">Parameter</span></span>    | <span data-ttu-id="8be87-140">Тип</span><span class="sxs-lookup"><span data-stu-id="8be87-140">Type</span></span>   |<span data-ttu-id="8be87-141">Описание</span><span class="sxs-lookup"><span data-stu-id="8be87-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8be87-142">comment</span><span class="sxs-lookup"><span data-stu-id="8be87-142">comment</span></span>|<span data-ttu-id="8be87-143">String</span><span class="sxs-lookup"><span data-stu-id="8be87-143">String</span></span>|<span data-ttu-id="8be87-p107">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="8be87-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="8be87-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="8be87-146">toRecipients</span></span>|<span data-ttu-id="8be87-147">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="8be87-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="8be87-148">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="8be87-148">The list of recipients.</span></span>|
|<span data-ttu-id="8be87-149">message</span><span class="sxs-lookup"><span data-stu-id="8be87-149">message</span></span>|[<span data-ttu-id="8be87-150">message</span><span class="sxs-lookup"><span data-stu-id="8be87-150">message</span></span>](../resources/message.md)|<span data-ttu-id="8be87-151">Все доступные для записи свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="8be87-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="8be87-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="8be87-152">Response</span></span>

<span data-ttu-id="8be87-p108">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8be87-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8be87-155">Пример</span><span class="sxs-lookup"><span data-stu-id="8be87-155">Example</span></span>
<span data-ttu-id="8be87-156">В примере ниже показано, как задать для свойства **исделиверирецеиптрекуестед** значение true, добавить комментарий и переслать сообщение.</span><span class="sxs-lookup"><span data-stu-id="8be87-156">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="8be87-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="8be87-157">Request</span></span>
<span data-ttu-id="8be87-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8be87-158">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8be87-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="8be87-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward
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
  "comment": "Dana, just want to make sure you get this." 
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8be87-160">C#</span><span class="sxs-lookup"><span data-stu-id="8be87-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8be87-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8be87-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8be87-162">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8be87-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8be87-163">Java</span><span class="sxs-lookup"><span data-stu-id="8be87-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8be87-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="8be87-164">Response</span></span>
<span data-ttu-id="8be87-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8be87-165">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
