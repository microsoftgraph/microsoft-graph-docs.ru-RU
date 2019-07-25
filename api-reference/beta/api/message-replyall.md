---
title: 'message: replyAll'
description: 'Ответить всем получателям сообщения, указав комментарий и изменив все обновляемые свойства '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ac96da92aba17ae81a14382cd018762abb24bbfb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879569"
---
# <a name="message-replyall"></a><span data-ttu-id="821b1-103">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="821b1-103">message: replyAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="821b1-104">Ответить всем получателям сообщения, указав комментарий и изменив все обновляемые свойства для этого ответа с помощью метода **replyAll** .</span><span class="sxs-lookup"><span data-stu-id="821b1-104">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="821b1-105">После этого сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="821b1-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="821b1-106">Кроме того, вы можете [создать черновик "ответить всем"](../api/message-createreplyall.md) , чтобы включить комментарий или обновить все свойства сообщения, а затем [Отправить](../api/message-send.md) ответ.</span><span class="sxs-lookup"><span data-stu-id="821b1-106">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="821b1-107">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="821b1-107">**Note**</span></span>

- <span data-ttu-id="821b1-108">Можно указать либо свойство Comment, либо свойство **Body** для `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="821b1-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="821b1-109">Если указать и то, и другое, будет возвращена ошибка неправильного запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="821b1-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="821b1-110">Если свойство **replyTo** указано в исходном сообщении, в формате Интернет-сообщений ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), необходимо отправить ответ получателям в</span><span class="sxs-lookup"><span data-stu-id="821b1-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="821b1-111">свойства **replyTo** и **toRecipients** , а не получатели в свойствах **from** и **toRecipients** .</span><span class="sxs-lookup"><span data-stu-id="821b1-111">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="821b1-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="821b1-112">Permissions</span></span>
<span data-ttu-id="821b1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="821b1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="821b1-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="821b1-115">Permission type</span></span>      | <span data-ttu-id="821b1-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="821b1-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="821b1-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="821b1-117">Delegated (work or school account)</span></span> | <span data-ttu-id="821b1-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="821b1-118">Mail.Send</span></span>    |
|<span data-ttu-id="821b1-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="821b1-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="821b1-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="821b1-120">Mail.Send</span></span>    |
|<span data-ttu-id="821b1-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="821b1-121">Application</span></span> | <span data-ttu-id="821b1-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="821b1-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="821b1-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="821b1-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="821b1-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="821b1-124">Request headers</span></span>
| <span data-ttu-id="821b1-125">Имя</span><span class="sxs-lookup"><span data-stu-id="821b1-125">Name</span></span>       | <span data-ttu-id="821b1-126">Тип</span><span class="sxs-lookup"><span data-stu-id="821b1-126">Type</span></span> | <span data-ttu-id="821b1-127">Описание</span><span class="sxs-lookup"><span data-stu-id="821b1-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="821b1-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="821b1-128">Authorization</span></span>  | <span data-ttu-id="821b1-129">string</span><span class="sxs-lookup"><span data-stu-id="821b1-129">string</span></span>  | <span data-ttu-id="821b1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="821b1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="821b1-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="821b1-132">Content-Type</span></span> | <span data-ttu-id="821b1-133">string</span><span class="sxs-lookup"><span data-stu-id="821b1-133">string</span></span>  | <span data-ttu-id="821b1-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="821b1-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="821b1-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="821b1-136">Request body</span></span>
<span data-ttu-id="821b1-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="821b1-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="821b1-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="821b1-138">Parameter</span></span>    | <span data-ttu-id="821b1-139">Тип</span><span class="sxs-lookup"><span data-stu-id="821b1-139">Type</span></span>   |<span data-ttu-id="821b1-140">Описание</span><span class="sxs-lookup"><span data-stu-id="821b1-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="821b1-141">comment</span><span class="sxs-lookup"><span data-stu-id="821b1-141">comment</span></span>|<span data-ttu-id="821b1-142">String</span><span class="sxs-lookup"><span data-stu-id="821b1-142">String</span></span>|<span data-ttu-id="821b1-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="821b1-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="821b1-145">message</span><span class="sxs-lookup"><span data-stu-id="821b1-145">message</span></span>|[<span data-ttu-id="821b1-146">message</span><span class="sxs-lookup"><span data-stu-id="821b1-146">message</span></span>](../resources/message.md)|<span data-ttu-id="821b1-147">Все доступные для записи свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="821b1-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="821b1-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="821b1-148">Response</span></span>

<span data-ttu-id="821b1-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="821b1-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="821b1-151">Пример</span><span class="sxs-lookup"><span data-stu-id="821b1-151">Example</span></span>
<span data-ttu-id="821b1-152">Приведенный ниже пример включает комментарий и добавляет вложение в сообщение Reply — All.</span><span class="sxs-lookup"><span data-stu-id="821b1-152">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="821b1-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="821b1-153">Request</span></span>
<span data-ttu-id="821b1-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="821b1-154">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="821b1-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="821b1-155">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="821b1-156">C#</span><span class="sxs-lookup"><span data-stu-id="821b1-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="821b1-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="821b1-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="821b1-158">Цель — C</span><span class="sxs-lookup"><span data-stu-id="821b1-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="821b1-159">Java</span><span class="sxs-lookup"><span data-stu-id="821b1-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="821b1-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="821b1-160">Response</span></span>
<span data-ttu-id="821b1-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="821b1-161">Here is an example of the response.</span></span>
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
