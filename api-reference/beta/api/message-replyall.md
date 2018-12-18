---
title: 'message: replyAll'
description: 'Ответить всем получателям сообщения, указав комментария и изменение любые обновляемые свойства '
author: angelgolfer-ms
ms.openlocfilehash: 035212224bca5cb6d173be9ea447cf16406ebf36
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307191"
---
# <a name="message-replyall"></a><span data-ttu-id="a1702-103">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="a1702-103">message: replyAll</span></span>

> <span data-ttu-id="a1702-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a1702-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1702-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1702-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1702-106">Ответить всем получателям сообщения, указав комментария и изменение любого обновляемых свойств для ответа с помощью метода **replyAll** .</span><span class="sxs-lookup"><span data-stu-id="a1702-106">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="a1702-107">Затем сообщение сохраняется в папке «Отправленные».</span><span class="sxs-lookup"><span data-stu-id="a1702-107">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="a1702-108">Кроме того можно первого [создания сообщения ответить всем черновиков](../api/message-createreplyall.md) добавить примечание или обновить все свойства сообщений, а затем [Отправить](../api/message-send.md) его.</span><span class="sxs-lookup"><span data-stu-id="a1702-108">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="a1702-109">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="a1702-109">**Note**</span></span>

- <span data-ttu-id="a1702-110">Можно указать комментарий или свойству **body** `message` параметр.</span><span class="sxs-lookup"><span data-stu-id="a1702-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="a1702-111">Указание оба возвратит ошибку HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="a1702-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="a1702-112">Если свойство **replyTo** указано в исходное сообщение в формат сообщений Интернета ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), следует отправить ответ в список получателей в</span><span class="sxs-lookup"><span data-stu-id="a1702-112">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="a1702-113">свойства **replyTo** и **toRecipients** , а не в список получателей в свойства **из** и **toRecipients** .</span><span class="sxs-lookup"><span data-stu-id="a1702-113">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="a1702-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1702-114">Permissions</span></span>
<span data-ttu-id="a1702-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1702-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1702-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1702-117">Permission type</span></span>      | <span data-ttu-id="a1702-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1702-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1702-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1702-119">Delegated (work or school account)</span></span> | <span data-ttu-id="a1702-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a1702-120">Mail.Send</span></span>    |
|<span data-ttu-id="a1702-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1702-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1702-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a1702-122">Mail.Send</span></span>    |
|<span data-ttu-id="a1702-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1702-123">Application</span></span> | <span data-ttu-id="a1702-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a1702-124">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1702-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1702-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="a1702-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1702-126">Request headers</span></span>
| <span data-ttu-id="a1702-127">Имя</span><span class="sxs-lookup"><span data-stu-id="a1702-127">Name</span></span>       | <span data-ttu-id="a1702-128">Тип</span><span class="sxs-lookup"><span data-stu-id="a1702-128">Type</span></span> | <span data-ttu-id="a1702-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a1702-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a1702-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1702-130">Authorization</span></span>  | <span data-ttu-id="a1702-131">string</span><span class="sxs-lookup"><span data-stu-id="a1702-131">string</span></span>  | <span data-ttu-id="a1702-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1702-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a1702-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a1702-134">Content-Type</span></span> | <span data-ttu-id="a1702-135">string</span><span class="sxs-lookup"><span data-stu-id="a1702-135">string</span></span>  | <span data-ttu-id="a1702-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1702-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1702-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1702-138">Request body</span></span>
<span data-ttu-id="a1702-139">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a1702-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a1702-140">Параметр</span><span class="sxs-lookup"><span data-stu-id="a1702-140">Parameter</span></span>    | <span data-ttu-id="a1702-141">Тип</span><span class="sxs-lookup"><span data-stu-id="a1702-141">Type</span></span>   |<span data-ttu-id="a1702-142">Описание</span><span class="sxs-lookup"><span data-stu-id="a1702-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1702-143">comment</span><span class="sxs-lookup"><span data-stu-id="a1702-143">comment</span></span>|<span data-ttu-id="a1702-144">String</span><span class="sxs-lookup"><span data-stu-id="a1702-144">String</span></span>|<span data-ttu-id="a1702-p107">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="a1702-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="a1702-147">message</span><span class="sxs-lookup"><span data-stu-id="a1702-147">message</span></span>|[<span data-ttu-id="a1702-148">message</span><span class="sxs-lookup"><span data-stu-id="a1702-148">message</span></span>](../resources/message.md)|<span data-ttu-id="a1702-149">Любой доступный свойства для обновления в ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="a1702-149">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="a1702-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1702-150">Response</span></span>

<span data-ttu-id="a1702-p108">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a1702-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1702-153">Пример</span><span class="sxs-lookup"><span data-stu-id="a1702-153">Example</span></span>
<span data-ttu-id="a1702-154">Следующий пример включает в себя комментария и добавляет вложения в сообщение ответить всем.</span><span class="sxs-lookup"><span data-stu-id="a1702-154">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="a1702-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1702-155">Request</span></span>
<span data-ttu-id="a1702-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1702-156">Here is an example of the request.</span></span>
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


##### <a name="response"></a><span data-ttu-id="a1702-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1702-157">Response</span></span>
<span data-ttu-id="a1702-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a1702-158">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
