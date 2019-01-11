---
title: 'message: reply'
description: 'Отправителю сообщения, добавьте комментарий или изменить любые обновляемые свойства в вызове один **ответ** . '
localization_priority: Normal
ms.openlocfilehash: 3844969c8c4bbec9026aee8477db968d5a3b0e52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827463"
---
# <a name="message-reply"></a><span data-ttu-id="d9597-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="d9597-103">message: reply</span></span>

> <span data-ttu-id="d9597-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d9597-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9597-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9597-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9597-106">Отправителю сообщения, добавьте комментарий или изменить любые обновляемые свойства в вызове один **ответ** .</span><span class="sxs-lookup"><span data-stu-id="d9597-106">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call.</span></span> <span data-ttu-id="d9597-107">Затем сообщение сохраняется в папке «Отправленные».</span><span class="sxs-lookup"><span data-stu-id="d9597-107">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="d9597-108">Кроме того можно первого [Создание черновика ответное сообщение](../api/message-createreply.md) для добавить примечание или обновите все свойства сообщений, а затем [Отправить](../api/message-send.md) его.</span><span class="sxs-lookup"><span data-stu-id="d9597-108">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="d9597-109">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="d9597-109">**Note**</span></span>

- <span data-ttu-id="d9597-110">Можно указать комментарий или свойству **body** `message` параметр.</span><span class="sxs-lookup"><span data-stu-id="d9597-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="d9597-111">Указание оба возвратит ошибку HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="d9597-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="d9597-112">Если свойство **replyTo** указано в исходное сообщение в формат сообщений Интернета ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), следует отправить ответ в список получателей в **replyTo** и не получателя в свойстве **из** .</span><span class="sxs-lookup"><span data-stu-id="d9597-112">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="d9597-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9597-113">Permissions</span></span>
<span data-ttu-id="d9597-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9597-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9597-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9597-116">Permission type</span></span>      | <span data-ttu-id="d9597-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9597-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9597-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9597-118">Delegated (work or school account)</span></span> | <span data-ttu-id="d9597-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d9597-119">Mail.Send</span></span>    |
|<span data-ttu-id="d9597-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9597-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9597-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d9597-121">Mail.Send</span></span>    |
|<span data-ttu-id="d9597-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9597-122">Application</span></span> | <span data-ttu-id="d9597-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d9597-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9597-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9597-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="d9597-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9597-125">Request headers</span></span>
| <span data-ttu-id="d9597-126">Имя</span><span class="sxs-lookup"><span data-stu-id="d9597-126">Name</span></span>       | <span data-ttu-id="d9597-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d9597-127">Type</span></span> | <span data-ttu-id="d9597-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d9597-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d9597-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9597-129">Authorization</span></span>  | <span data-ttu-id="d9597-130">string</span><span class="sxs-lookup"><span data-stu-id="d9597-130">string</span></span>  | <span data-ttu-id="d9597-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9597-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d9597-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9597-133">Content-Type</span></span> | <span data-ttu-id="d9597-134">string</span><span class="sxs-lookup"><span data-stu-id="d9597-134">string</span></span>  | <span data-ttu-id="d9597-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9597-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9597-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d9597-137">Request body</span></span>
<span data-ttu-id="d9597-138">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d9597-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d9597-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="d9597-139">Parameter</span></span>    | <span data-ttu-id="d9597-140">Тип</span><span class="sxs-lookup"><span data-stu-id="d9597-140">Type</span></span>   |<span data-ttu-id="d9597-141">Описание</span><span class="sxs-lookup"><span data-stu-id="d9597-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9597-142">comment</span><span class="sxs-lookup"><span data-stu-id="d9597-142">comment</span></span>|<span data-ttu-id="d9597-143">String</span><span class="sxs-lookup"><span data-stu-id="d9597-143">String</span></span>|<span data-ttu-id="d9597-p107">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="d9597-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="d9597-146">message</span><span class="sxs-lookup"><span data-stu-id="d9597-146">message</span></span>|[<span data-ttu-id="d9597-147">message</span><span class="sxs-lookup"><span data-stu-id="d9597-147">message</span></span>](../resources/message.md)|<span data-ttu-id="d9597-148">Любой доступный свойства для обновления в ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="d9597-148">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="d9597-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9597-149">Response</span></span>

<span data-ttu-id="d9597-p108">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d9597-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9597-152">Пример</span><span class="sxs-lookup"><span data-stu-id="d9597-152">Example</span></span>
<span data-ttu-id="d9597-153">В следующем примере включает в себя комментария и добавляет получателя сообщения ответа.</span><span class="sxs-lookup"><span data-stu-id="d9597-153">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="d9597-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9597-154">Request</span></span>
<span data-ttu-id="d9597-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9597-155">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d9597-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9597-156">Response</span></span>
<span data-ttu-id="d9597-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d9597-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
