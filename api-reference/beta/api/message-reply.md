---
title: 'message: reply'
description: 'Ответ отправителю сообщения, добавление комментария или изменение любых обновляемых свойств одновременно в одном вызове **reply**. '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c745cfaab60aae9395e2b8d720852a1d2b2b2a39
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333214"
---
# <a name="message-reply"></a><span data-ttu-id="660c0-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="660c0-103">message: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="660c0-104">Ответ отправителю сообщения, добавление комментария или изменение любых обновляемых свойств одновременно в одном вызове **reply**.</span><span class="sxs-lookup"><span data-stu-id="660c0-104">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call.</span></span> <span data-ttu-id="660c0-105">После этого сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="660c0-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="660c0-106">Кроме того, вы можете [создать черновик ответного сообщения](../api/message-createreply.md) , чтобы добавить комментарий или обновить все свойства сообщения, а затем [Отправить](../api/message-send.md) ответ.</span><span class="sxs-lookup"><span data-stu-id="660c0-106">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="660c0-107">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="660c0-107">**Note**</span></span>

- <span data-ttu-id="660c0-108">Можно указать либо свойство Comment, либо свойство **Body** для `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="660c0-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="660c0-109">Если указать и то, и другое, будет возвращена ошибка неПравильного запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="660c0-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="660c0-110">Если свойство **replyTo** указано в исходном сообщении, в формате Интернет-сообщений ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), необходимо отправить ответ получателям в **replyTo** , а не получателю в свойстве **from** .</span><span class="sxs-lookup"><span data-stu-id="660c0-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="660c0-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="660c0-111">Permissions</span></span>
<span data-ttu-id="660c0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="660c0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="660c0-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="660c0-114">Permission type</span></span>      | <span data-ttu-id="660c0-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="660c0-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="660c0-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="660c0-116">Delegated (work or school account)</span></span> | <span data-ttu-id="660c0-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="660c0-117">Mail.Send</span></span>    |
|<span data-ttu-id="660c0-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="660c0-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="660c0-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="660c0-119">Mail.Send</span></span>    |
|<span data-ttu-id="660c0-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="660c0-120">Application</span></span> | <span data-ttu-id="660c0-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="660c0-121">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="660c0-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="660c0-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="660c0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="660c0-123">Request headers</span></span>
| <span data-ttu-id="660c0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="660c0-124">Name</span></span>       | <span data-ttu-id="660c0-125">Тип</span><span class="sxs-lookup"><span data-stu-id="660c0-125">Type</span></span> | <span data-ttu-id="660c0-126">Описание</span><span class="sxs-lookup"><span data-stu-id="660c0-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="660c0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="660c0-127">Authorization</span></span>  | <span data-ttu-id="660c0-128">string</span><span class="sxs-lookup"><span data-stu-id="660c0-128">string</span></span>  | <span data-ttu-id="660c0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="660c0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="660c0-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="660c0-131">Content-Type</span></span> | <span data-ttu-id="660c0-132">string</span><span class="sxs-lookup"><span data-stu-id="660c0-132">string</span></span>  | <span data-ttu-id="660c0-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="660c0-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="660c0-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="660c0-135">Request body</span></span>
<span data-ttu-id="660c0-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="660c0-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="660c0-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="660c0-137">Parameter</span></span>    | <span data-ttu-id="660c0-138">Тип</span><span class="sxs-lookup"><span data-stu-id="660c0-138">Type</span></span>   |<span data-ttu-id="660c0-139">Описание</span><span class="sxs-lookup"><span data-stu-id="660c0-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="660c0-140">comment</span><span class="sxs-lookup"><span data-stu-id="660c0-140">comment</span></span>|<span data-ttu-id="660c0-141">String</span><span class="sxs-lookup"><span data-stu-id="660c0-141">String</span></span>|<span data-ttu-id="660c0-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="660c0-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="660c0-144">message</span><span class="sxs-lookup"><span data-stu-id="660c0-144">message</span></span>|[<span data-ttu-id="660c0-145">message</span><span class="sxs-lookup"><span data-stu-id="660c0-145">message</span></span>](../resources/message.md)|<span data-ttu-id="660c0-146">Все доступные для записи свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="660c0-146">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="660c0-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="660c0-147">Response</span></span>

<span data-ttu-id="660c0-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="660c0-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="660c0-150">Пример</span><span class="sxs-lookup"><span data-stu-id="660c0-150">Example</span></span>
<span data-ttu-id="660c0-151">Приведенный ниже пример включает комментарий и добавляет получателя в ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="660c0-151">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="660c0-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="660c0-152">Request</span></span>
<span data-ttu-id="660c0-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="660c0-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: application/json

{
  "message":{  
    "toRecipients":[
      {
        "emailAddress": {
          "address":"samanthab@contoso.onmicrosoft.com",
          "name":"Samantha Booth"
        }
      },
      {
        "emailAddress":{
          "address":"randiw@contoso.onmicrosoft.com",
          "name":"Randi Welch"
        }
      }
     ]
  },
  "comment": "Samantha, Randi, would you name the group please?" 
}
```

##### <a name="response"></a><span data-ttu-id="660c0-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="660c0-154">Response</span></span>
<span data-ttu-id="660c0-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="660c0-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
