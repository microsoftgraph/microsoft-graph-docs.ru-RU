---
title: 'message: replyAll'
description: 'Ответить всем получателям сообщения, указав комментария и изменение любые обновляемые свойства '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 05f552676400196aed275c32020bcdf5211d0e31
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528615"
---
# <a name="message-replyall"></a><span data-ttu-id="147af-103">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="147af-103">message: replyAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="147af-104">Ответить всем получателям сообщения, указав комментария и изменение любого обновляемых свойств для ответа с помощью метода **replyAll** .</span><span class="sxs-lookup"><span data-stu-id="147af-104">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="147af-105">Затем сообщение сохраняется в папке «Отправленные».</span><span class="sxs-lookup"><span data-stu-id="147af-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="147af-106">Кроме того можно первого [создания сообщения ответить всем черновиков](../api/message-createreplyall.md) добавить примечание или обновить все свойства сообщений, а затем [Отправить](../api/message-send.md) его.</span><span class="sxs-lookup"><span data-stu-id="147af-106">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="147af-107">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="147af-107">**Note**</span></span>

- <span data-ttu-id="147af-108">Можно указать комментарий или свойству **body** `message` параметр.</span><span class="sxs-lookup"><span data-stu-id="147af-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="147af-109">Указание оба возвратит ошибку HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="147af-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="147af-110">Если свойство **replyTo** указано в исходное сообщение в формат сообщений Интернета ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), следует отправить ответ в список получателей в</span><span class="sxs-lookup"><span data-stu-id="147af-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="147af-111">свойства **replyTo** и **toRecipients** , а не в список получателей в свойства **из** и **toRecipients** .</span><span class="sxs-lookup"><span data-stu-id="147af-111">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="147af-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="147af-112">Permissions</span></span>
<span data-ttu-id="147af-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="147af-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="147af-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="147af-115">Permission type</span></span>      | <span data-ttu-id="147af-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="147af-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="147af-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="147af-117">Delegated (work or school account)</span></span> | <span data-ttu-id="147af-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="147af-118">Mail.Send</span></span>    |
|<span data-ttu-id="147af-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="147af-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="147af-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="147af-120">Mail.Send</span></span>    |
|<span data-ttu-id="147af-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="147af-121">Application</span></span> | <span data-ttu-id="147af-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="147af-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="147af-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="147af-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="147af-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="147af-124">Request headers</span></span>
| <span data-ttu-id="147af-125">Имя</span><span class="sxs-lookup"><span data-stu-id="147af-125">Name</span></span>       | <span data-ttu-id="147af-126">Тип</span><span class="sxs-lookup"><span data-stu-id="147af-126">Type</span></span> | <span data-ttu-id="147af-127">Описание</span><span class="sxs-lookup"><span data-stu-id="147af-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="147af-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="147af-128">Authorization</span></span>  | <span data-ttu-id="147af-129">string</span><span class="sxs-lookup"><span data-stu-id="147af-129">string</span></span>  | <span data-ttu-id="147af-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="147af-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="147af-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="147af-132">Content-Type</span></span> | <span data-ttu-id="147af-133">string</span><span class="sxs-lookup"><span data-stu-id="147af-133">string</span></span>  | <span data-ttu-id="147af-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="147af-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="147af-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="147af-136">Request body</span></span>
<span data-ttu-id="147af-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="147af-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="147af-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="147af-138">Parameter</span></span>    | <span data-ttu-id="147af-139">Тип</span><span class="sxs-lookup"><span data-stu-id="147af-139">Type</span></span>   |<span data-ttu-id="147af-140">Описание</span><span class="sxs-lookup"><span data-stu-id="147af-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="147af-141">comment</span><span class="sxs-lookup"><span data-stu-id="147af-141">comment</span></span>|<span data-ttu-id="147af-142">String</span><span class="sxs-lookup"><span data-stu-id="147af-142">String</span></span>|<span data-ttu-id="147af-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="147af-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="147af-145">message</span><span class="sxs-lookup"><span data-stu-id="147af-145">message</span></span>|[<span data-ttu-id="147af-146">message</span><span class="sxs-lookup"><span data-stu-id="147af-146">message</span></span>](../resources/message.md)|<span data-ttu-id="147af-147">Любой доступный свойства для обновления в ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="147af-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="147af-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="147af-148">Response</span></span>

<span data-ttu-id="147af-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="147af-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="147af-151">Пример</span><span class="sxs-lookup"><span data-stu-id="147af-151">Example</span></span>
<span data-ttu-id="147af-152">Следующий пример включает в себя комментария и добавляет вложения в сообщение ответить всем.</span><span class="sxs-lookup"><span data-stu-id="147af-152">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="147af-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="147af-153">Request</span></span>
<span data-ttu-id="147af-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="147af-154">Here is an example of the request.</span></span>
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


##### <a name="response"></a><span data-ttu-id="147af-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="147af-155">Response</span></span>
<span data-ttu-id="147af-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="147af-156">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/message-replyall.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
