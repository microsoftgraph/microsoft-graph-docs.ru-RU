---
title: 'message: replyAll'
description: 'Ответить всем получателям сообщения, указав комментарий и изменив все обновляемые свойства '
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 53d28496fbb0b82732d4d3aedecf6d9de62199ae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448503"
---
# <a name="message-replyall"></a><span data-ttu-id="0d28f-103">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="0d28f-103">message: replyAll</span></span>

<span data-ttu-id="0d28f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d28f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d28f-105">Ответить всем получателям сообщения, указав комментарий и изменив все обновляемые свойства для этого ответа с помощью метода **replyAll** .</span><span class="sxs-lookup"><span data-stu-id="0d28f-105">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="0d28f-106">После этого сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="0d28f-106">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="0d28f-107">Кроме того, вы можете [создать черновик "ответить всем"](../api/message-createreplyall.md) , чтобы включить комментарий или обновить все свойства сообщения, а затем [Отправить](../api/message-send.md) ответ.</span><span class="sxs-lookup"><span data-stu-id="0d28f-107">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="0d28f-108">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="0d28f-108">**Note**</span></span>

- <span data-ttu-id="0d28f-109">Можно указать либо свойство Comment, либо свойство **Body** для `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="0d28f-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="0d28f-110">Если указать и то, и другое, будет возвращена ошибка неправильного запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="0d28f-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="0d28f-111">Если свойство **replyTo** указано в исходном сообщении, в формате Интернет-сообщений ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), необходимо отправить ответ получателям в</span><span class="sxs-lookup"><span data-stu-id="0d28f-111">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="0d28f-112">свойства **replyTo** и **toRecipients** , а не получатели в свойствах **from** и **toRecipients** .</span><span class="sxs-lookup"><span data-stu-id="0d28f-112">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="0d28f-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d28f-113">Permissions</span></span>
<span data-ttu-id="0d28f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d28f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d28f-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d28f-116">Permission type</span></span>      | <span data-ttu-id="0d28f-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d28f-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d28f-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d28f-118">Delegated (work or school account)</span></span> | <span data-ttu-id="0d28f-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0d28f-119">Mail.Send</span></span>    |
|<span data-ttu-id="0d28f-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d28f-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d28f-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0d28f-121">Mail.Send</span></span>    |
|<span data-ttu-id="0d28f-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d28f-122">Application</span></span> | <span data-ttu-id="0d28f-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0d28f-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d28f-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d28f-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="0d28f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d28f-125">Request headers</span></span>
| <span data-ttu-id="0d28f-126">Имя</span><span class="sxs-lookup"><span data-stu-id="0d28f-126">Name</span></span>       | <span data-ttu-id="0d28f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="0d28f-127">Type</span></span> | <span data-ttu-id="0d28f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0d28f-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0d28f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d28f-129">Authorization</span></span>  | <span data-ttu-id="0d28f-130">string</span><span class="sxs-lookup"><span data-stu-id="0d28f-130">string</span></span>  | <span data-ttu-id="0d28f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d28f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0d28f-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d28f-133">Content-Type</span></span> | <span data-ttu-id="0d28f-134">string</span><span class="sxs-lookup"><span data-stu-id="0d28f-134">string</span></span>  | <span data-ttu-id="0d28f-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d28f-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d28f-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d28f-137">Request body</span></span>
<span data-ttu-id="0d28f-138">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0d28f-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0d28f-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="0d28f-139">Parameter</span></span>    | <span data-ttu-id="0d28f-140">Тип</span><span class="sxs-lookup"><span data-stu-id="0d28f-140">Type</span></span>   |<span data-ttu-id="0d28f-141">Описание</span><span class="sxs-lookup"><span data-stu-id="0d28f-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d28f-142">comment</span><span class="sxs-lookup"><span data-stu-id="0d28f-142">comment</span></span>|<span data-ttu-id="0d28f-143">String</span><span class="sxs-lookup"><span data-stu-id="0d28f-143">String</span></span>|<span data-ttu-id="0d28f-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="0d28f-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="0d28f-146">message</span><span class="sxs-lookup"><span data-stu-id="0d28f-146">message</span></span>|[<span data-ttu-id="0d28f-147">message</span><span class="sxs-lookup"><span data-stu-id="0d28f-147">message</span></span>](../resources/message.md)|<span data-ttu-id="0d28f-148">Все доступные для записи свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="0d28f-148">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="0d28f-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d28f-149">Response</span></span>

<span data-ttu-id="0d28f-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0d28f-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d28f-152">Пример</span><span class="sxs-lookup"><span data-stu-id="0d28f-152">Example</span></span>
<span data-ttu-id="0d28f-153">Приведенный ниже пример включает комментарий и добавляет вложение в сообщение Reply — All.</span><span class="sxs-lookup"><span data-stu-id="0d28f-153">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="0d28f-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d28f-154">Request</span></span>
<span data-ttu-id="0d28f-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d28f-155">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d28f-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d28f-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll
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
    "comment": "Please take a look at the attached guidelines before you decide on the name." 
}
```
# <a name="c"></a>[<span data-ttu-id="0d28f-157">C#</span><span class="sxs-lookup"><span data-stu-id="0d28f-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d28f-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d28f-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d28f-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d28f-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="0d28f-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d28f-160">Response</span></span>
<span data-ttu-id="0d28f-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0d28f-161">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
