---
title: 'message: replyAll'
description: 'Ответить всем получателям сообщения, указав комментарий и изменив все обновляемые свойства '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5215af70332977d1c7aef70ad9418287f7c0b46f
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536990"
---
# <a name="message-replyall"></a><span data-ttu-id="dc2ed-103">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="dc2ed-103">message: replyAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc2ed-104">Ответить всем получателям сообщения, указав комментарий и изменив все обновляемые свойства для этого ответа с помощью метода **replyAll** .</span><span class="sxs-lookup"><span data-stu-id="dc2ed-104">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="dc2ed-105">После этого сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="dc2ed-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="dc2ed-106">Кроме того, вы можете [создать черновик "ответить всем"](../api/message-createreplyall.md) , чтобы включить комментарий или обновить все свойства сообщения, а затем [Отправить](../api/message-send.md) ответ.</span><span class="sxs-lookup"><span data-stu-id="dc2ed-106">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="dc2ed-107">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="dc2ed-107">**Note**</span></span>

- <span data-ttu-id="dc2ed-108">Можно указать либо свойство Comment, либо свойство **Body** для `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="dc2ed-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="dc2ed-109">Если указать и то, и другое, будет возвращена ошибка неправильного запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="dc2ed-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="dc2ed-110">Если свойство **replyTo** указано в исходном сообщении, в формате Интернет-сообщений ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), необходимо отправить ответ получателям в</span><span class="sxs-lookup"><span data-stu-id="dc2ed-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="dc2ed-111">свойства **replyTo** и **toRecipients** , а не получатели в свойствах **from** и **toRecipients** .</span><span class="sxs-lookup"><span data-stu-id="dc2ed-111">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="dc2ed-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc2ed-112">Permissions</span></span>
<span data-ttu-id="dc2ed-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc2ed-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc2ed-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc2ed-115">Permission type</span></span>      | <span data-ttu-id="dc2ed-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc2ed-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc2ed-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc2ed-117">Delegated (work or school account)</span></span> | <span data-ttu-id="dc2ed-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="dc2ed-118">Mail.Send</span></span>    |
|<span data-ttu-id="dc2ed-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc2ed-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc2ed-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="dc2ed-120">Mail.Send</span></span>    |
|<span data-ttu-id="dc2ed-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc2ed-121">Application</span></span> | <span data-ttu-id="dc2ed-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="dc2ed-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc2ed-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc2ed-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="dc2ed-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc2ed-124">Request headers</span></span>
| <span data-ttu-id="dc2ed-125">Имя</span><span class="sxs-lookup"><span data-stu-id="dc2ed-125">Name</span></span>       | <span data-ttu-id="dc2ed-126">Тип</span><span class="sxs-lookup"><span data-stu-id="dc2ed-126">Type</span></span> | <span data-ttu-id="dc2ed-127">Описание</span><span class="sxs-lookup"><span data-stu-id="dc2ed-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dc2ed-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc2ed-128">Authorization</span></span>  | <span data-ttu-id="dc2ed-129">string</span><span class="sxs-lookup"><span data-stu-id="dc2ed-129">string</span></span>  | <span data-ttu-id="dc2ed-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc2ed-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc2ed-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc2ed-132">Content-Type</span></span> | <span data-ttu-id="dc2ed-133">string</span><span class="sxs-lookup"><span data-stu-id="dc2ed-133">string</span></span>  | <span data-ttu-id="dc2ed-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc2ed-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc2ed-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc2ed-136">Request body</span></span>
<span data-ttu-id="dc2ed-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dc2ed-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dc2ed-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="dc2ed-138">Parameter</span></span>    | <span data-ttu-id="dc2ed-139">Тип</span><span class="sxs-lookup"><span data-stu-id="dc2ed-139">Type</span></span>   |<span data-ttu-id="dc2ed-140">Описание</span><span class="sxs-lookup"><span data-stu-id="dc2ed-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc2ed-141">comment</span><span class="sxs-lookup"><span data-stu-id="dc2ed-141">comment</span></span>|<span data-ttu-id="dc2ed-142">String</span><span class="sxs-lookup"><span data-stu-id="dc2ed-142">String</span></span>|<span data-ttu-id="dc2ed-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="dc2ed-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="dc2ed-145">message</span><span class="sxs-lookup"><span data-stu-id="dc2ed-145">message</span></span>|[<span data-ttu-id="dc2ed-146">message</span><span class="sxs-lookup"><span data-stu-id="dc2ed-146">message</span></span>](../resources/message.md)|<span data-ttu-id="dc2ed-147">Все доступные для записи свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="dc2ed-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="dc2ed-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc2ed-148">Response</span></span>

<span data-ttu-id="dc2ed-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dc2ed-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc2ed-151">Пример</span><span class="sxs-lookup"><span data-stu-id="dc2ed-151">Example</span></span>
<span data-ttu-id="dc2ed-152">Приведенный ниже пример включает комментарий и добавляет вложение в сообщение Reply — All.</span><span class="sxs-lookup"><span data-stu-id="dc2ed-152">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="dc2ed-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc2ed-153">Request</span></span>
<span data-ttu-id="dc2ed-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc2ed-154">Here is an example of the request.</span></span>
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


##### <a name="response"></a><span data-ttu-id="dc2ed-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc2ed-155">Response</span></span>
<span data-ttu-id="dc2ed-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dc2ed-156">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dc2ed-157">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="dc2ed-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dc2ed-158">C#</span><span class="sxs-lookup"><span data-stu-id="dc2ed-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_replyall-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc2ed-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="dc2ed-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_replyall-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/message-replyall.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-replyall.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
