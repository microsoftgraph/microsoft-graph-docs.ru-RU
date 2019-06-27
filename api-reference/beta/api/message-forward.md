---
title: 'message: forward'
description: 'Пересылка сообщения, Добавление комментария или изменение любых обновляемых свойств  '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 65da496594c2b3bca70410552166be7a4ed55fcb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266082"
---
# <a name="message-forward"></a><span data-ttu-id="a726c-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="a726c-103">message: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a726c-104">Пересылка сообщения, Добавление комментария или изменение любых обновляемых свойств</span><span class="sxs-lookup"><span data-stu-id="a726c-104">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="a726c-105">все в одном **переадресации** звонка.</span><span class="sxs-lookup"><span data-stu-id="a726c-105">all in one **forward** call.</span></span> <span data-ttu-id="a726c-106">Сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="a726c-106">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="a726c-107">Кроме того, вы можете [создать черновик переадресации](../api/message-createforward.md) , чтобы включить комментарий или обновить все свойства сообщения, а затем [Отправить](../api/message-send.md) черновик сообщения.</span><span class="sxs-lookup"><span data-stu-id="a726c-107">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="a726c-108">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="a726c-108">**Note**</span></span>

- <span data-ttu-id="a726c-109">Можно указать либо свойство Comment, либо свойство **Body** для `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="a726c-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="a726c-110">Если указать и то, и другое, будет возвращена ошибка неправильного запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="a726c-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="a726c-111">Необходимо указать либо параметр, `toRecipients` либо свойство **toRecipients** `message` параметра.</span><span class="sxs-lookup"><span data-stu-id="a726c-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="a726c-112">Если указать оба параметра или не указывать ни один из них, будет возвращена ошибка ошибки запроса HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="a726c-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="a726c-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a726c-113">Permissions</span></span>
<span data-ttu-id="a726c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a726c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a726c-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a726c-116">Permission type</span></span>      | <span data-ttu-id="a726c-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a726c-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a726c-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a726c-118">Delegated (work or school account)</span></span> | <span data-ttu-id="a726c-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a726c-119">Mail.Send</span></span>    |
|<span data-ttu-id="a726c-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a726c-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a726c-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a726c-121">Mail.Send</span></span>    |
|<span data-ttu-id="a726c-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a726c-122">Application</span></span> | <span data-ttu-id="a726c-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a726c-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="a726c-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a726c-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="a726c-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a726c-125">Request headers</span></span>
| <span data-ttu-id="a726c-126">Имя</span><span class="sxs-lookup"><span data-stu-id="a726c-126">Name</span></span>       | <span data-ttu-id="a726c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a726c-127">Type</span></span> | <span data-ttu-id="a726c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a726c-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a726c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="a726c-129">Authorization</span></span>  | <span data-ttu-id="a726c-130">string</span><span class="sxs-lookup"><span data-stu-id="a726c-130">string</span></span>  | <span data-ttu-id="a726c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a726c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a726c-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a726c-133">Content-Type</span></span> | <span data-ttu-id="a726c-134">string</span><span class="sxs-lookup"><span data-stu-id="a726c-134">string</span></span>  | <span data-ttu-id="a726c-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a726c-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a726c-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a726c-137">Request body</span></span>
<span data-ttu-id="a726c-138">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a726c-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a726c-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="a726c-139">Parameter</span></span>    | <span data-ttu-id="a726c-140">Тип</span><span class="sxs-lookup"><span data-stu-id="a726c-140">Type</span></span>   |<span data-ttu-id="a726c-141">Описание</span><span class="sxs-lookup"><span data-stu-id="a726c-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a726c-142">comment</span><span class="sxs-lookup"><span data-stu-id="a726c-142">comment</span></span>|<span data-ttu-id="a726c-143">String</span><span class="sxs-lookup"><span data-stu-id="a726c-143">String</span></span>|<span data-ttu-id="a726c-p107">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="a726c-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="a726c-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="a726c-146">toRecipients</span></span>|<span data-ttu-id="a726c-147">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="a726c-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="a726c-148">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="a726c-148">The list of recipients.</span></span>|
|<span data-ttu-id="a726c-149">message</span><span class="sxs-lookup"><span data-stu-id="a726c-149">message</span></span>|[<span data-ttu-id="a726c-150">message</span><span class="sxs-lookup"><span data-stu-id="a726c-150">message</span></span>](../resources/message.md)|<span data-ttu-id="a726c-151">Все доступные для записи свойства, которые необходимо обновить в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="a726c-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="a726c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="a726c-152">Response</span></span>

<span data-ttu-id="a726c-p108">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a726c-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a726c-155">Пример</span><span class="sxs-lookup"><span data-stu-id="a726c-155">Example</span></span>
<span data-ttu-id="a726c-156">В примере ниже показано, как задать для свойства **исделиверирецеиптрекуестед** значение true, добавить комментарий и переслать сообщение.</span><span class="sxs-lookup"><span data-stu-id="a726c-156">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="a726c-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="a726c-157">Request</span></span>
<span data-ttu-id="a726c-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a726c-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a726c-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="a726c-159">Response</span></span>
<span data-ttu-id="a726c-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a726c-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a726c-161">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a726c-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a726c-162">C#</span><span class="sxs-lookup"><span data-stu-id="a726c-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_forward-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a726c-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="a726c-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_forward-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a726c-164">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a726c-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_forward-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/message-forward.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/message-forward.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-forward.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
