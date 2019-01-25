---
title: 'message: reply'
description: 'Отправителю сообщения, добавьте комментарий или изменить любые обновляемые свойства в вызове один **ответ** . '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6461d9735459ff9cf956820b00bb61a4d42d1ec0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519012"
---
# <a name="message-reply"></a><span data-ttu-id="d272b-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="d272b-103">message: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d272b-104">Отправителю сообщения, добавьте комментарий или изменить любые обновляемые свойства в вызове один **ответ** .</span><span class="sxs-lookup"><span data-stu-id="d272b-104">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call.</span></span> <span data-ttu-id="d272b-105">Затем сообщение сохраняется в папке «Отправленные».</span><span class="sxs-lookup"><span data-stu-id="d272b-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="d272b-106">Кроме того можно первого [Создание черновика ответное сообщение](../api/message-createreply.md) для добавить примечание или обновите все свойства сообщений, а затем [Отправить](../api/message-send.md) его.</span><span class="sxs-lookup"><span data-stu-id="d272b-106">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="d272b-107">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="d272b-107">**Note**</span></span>

- <span data-ttu-id="d272b-108">Можно указать комментарий или свойству **body** `message` параметр.</span><span class="sxs-lookup"><span data-stu-id="d272b-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="d272b-109">Указание оба возвратит ошибку HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="d272b-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="d272b-110">Если свойство **replyTo** указано в исходное сообщение в формат сообщений Интернета ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), следует отправить ответ в список получателей в **replyTo** и не получателя в свойстве **из** .</span><span class="sxs-lookup"><span data-stu-id="d272b-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="d272b-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d272b-111">Permissions</span></span>
<span data-ttu-id="d272b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d272b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d272b-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d272b-114">Permission type</span></span>      | <span data-ttu-id="d272b-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d272b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d272b-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d272b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d272b-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d272b-117">Mail.Send</span></span>    |
|<span data-ttu-id="d272b-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d272b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d272b-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d272b-119">Mail.Send</span></span>    |
|<span data-ttu-id="d272b-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d272b-120">Application</span></span> | <span data-ttu-id="d272b-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d272b-121">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="d272b-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d272b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="d272b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d272b-123">Request headers</span></span>
| <span data-ttu-id="d272b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d272b-124">Name</span></span>       | <span data-ttu-id="d272b-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d272b-125">Type</span></span> | <span data-ttu-id="d272b-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d272b-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d272b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d272b-127">Authorization</span></span>  | <span data-ttu-id="d272b-128">string</span><span class="sxs-lookup"><span data-stu-id="d272b-128">string</span></span>  | <span data-ttu-id="d272b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d272b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d272b-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d272b-131">Content-Type</span></span> | <span data-ttu-id="d272b-132">string</span><span class="sxs-lookup"><span data-stu-id="d272b-132">string</span></span>  | <span data-ttu-id="d272b-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d272b-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d272b-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d272b-135">Request body</span></span>
<span data-ttu-id="d272b-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d272b-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d272b-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="d272b-137">Parameter</span></span>    | <span data-ttu-id="d272b-138">Тип</span><span class="sxs-lookup"><span data-stu-id="d272b-138">Type</span></span>   |<span data-ttu-id="d272b-139">Описание</span><span class="sxs-lookup"><span data-stu-id="d272b-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d272b-140">comment</span><span class="sxs-lookup"><span data-stu-id="d272b-140">comment</span></span>|<span data-ttu-id="d272b-141">String</span><span class="sxs-lookup"><span data-stu-id="d272b-141">String</span></span>|<span data-ttu-id="d272b-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="d272b-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="d272b-144">message</span><span class="sxs-lookup"><span data-stu-id="d272b-144">message</span></span>|[<span data-ttu-id="d272b-145">message</span><span class="sxs-lookup"><span data-stu-id="d272b-145">message</span></span>](../resources/message.md)|<span data-ttu-id="d272b-146">Любой доступный свойства для обновления в ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="d272b-146">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="d272b-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="d272b-147">Response</span></span>

<span data-ttu-id="d272b-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d272b-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d272b-150">Пример</span><span class="sxs-lookup"><span data-stu-id="d272b-150">Example</span></span>
<span data-ttu-id="d272b-151">В следующем примере включает в себя комментария и добавляет получателя сообщения ответа.</span><span class="sxs-lookup"><span data-stu-id="d272b-151">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="d272b-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="d272b-152">Request</span></span>
<span data-ttu-id="d272b-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d272b-153">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d272b-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="d272b-154">Response</span></span>
<span data-ttu-id="d272b-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d272b-155">Here is an example of the response.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/message-reply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
