---
title: 'message: forward'
description: 'Переслать сообщение, добавить комментарий или изменить любые обновляемые свойства  '
ms.openlocfilehash: 3edb96a90c99f1bc9eb2d8499e9cda83774a7ab3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082418"
---
# <a name="message-forward"></a><span data-ttu-id="e11dd-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="e11dd-103">message: forward</span></span>

> <span data-ttu-id="e11dd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e11dd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e11dd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e11dd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e11dd-106">Переслать сообщение, добавить комментарий или изменить любые обновляемые свойства</span><span class="sxs-lookup"><span data-stu-id="e11dd-106">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="e11dd-107">все в одной **переадресовывать** вызова.</span><span class="sxs-lookup"><span data-stu-id="e11dd-107">all in one **forward** call.</span></span> <span data-ttu-id="e11dd-108">Сообщение сохраняется в папке «Отправленные».</span><span class="sxs-lookup"><span data-stu-id="e11dd-108">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="e11dd-109">Кроме того можно первого [создания переслать сообщение черновиков](../api/message-createforward.md) добавить примечание или обновить все свойства сообщений, а затем [Отправить](../api/message-send.md) сообщение черновиков.</span><span class="sxs-lookup"><span data-stu-id="e11dd-109">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="e11dd-110">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="e11dd-110">**Note**</span></span>

- <span data-ttu-id="e11dd-111">Можно указать комментарий или свойству **body** `message` параметр.</span><span class="sxs-lookup"><span data-stu-id="e11dd-111">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="e11dd-112">Указание оба возвратит ошибку HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="e11dd-112">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="e11dd-113">Необходимо указать либо `toRecipients` параметр или свойство **toRecipients** `message` параметр.</span><span class="sxs-lookup"><span data-stu-id="e11dd-113">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="e11dd-114">Указание оба или указан ни один из них возвратит ошибку HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="e11dd-114">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="e11dd-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e11dd-115">Permissions</span></span>
<span data-ttu-id="e11dd-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e11dd-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e11dd-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e11dd-118">Permission type</span></span>      | <span data-ttu-id="e11dd-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e11dd-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e11dd-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e11dd-120">Delegated (work or school account)</span></span> | <span data-ttu-id="e11dd-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e11dd-121">Mail.Send</span></span>    |
|<span data-ttu-id="e11dd-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e11dd-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e11dd-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e11dd-123">Mail.Send</span></span>    |
|<span data-ttu-id="e11dd-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e11dd-124">Application</span></span> | <span data-ttu-id="e11dd-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e11dd-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="e11dd-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e11dd-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="e11dd-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e11dd-127">Request headers</span></span>
| <span data-ttu-id="e11dd-128">Имя</span><span class="sxs-lookup"><span data-stu-id="e11dd-128">Name</span></span>       | <span data-ttu-id="e11dd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e11dd-129">Type</span></span> | <span data-ttu-id="e11dd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e11dd-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e11dd-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="e11dd-131">Authorization</span></span>  | <span data-ttu-id="e11dd-132">string</span><span class="sxs-lookup"><span data-stu-id="e11dd-132">string</span></span>  | <span data-ttu-id="e11dd-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e11dd-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e11dd-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e11dd-135">Content-Type</span></span> | <span data-ttu-id="e11dd-136">string</span><span class="sxs-lookup"><span data-stu-id="e11dd-136">string</span></span>  | <span data-ttu-id="e11dd-p107">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e11dd-p107">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e11dd-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e11dd-139">Request body</span></span>
<span data-ttu-id="e11dd-140">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e11dd-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e11dd-141">Параметр</span><span class="sxs-lookup"><span data-stu-id="e11dd-141">Parameter</span></span>    | <span data-ttu-id="e11dd-142">Тип</span><span class="sxs-lookup"><span data-stu-id="e11dd-142">Type</span></span>   |<span data-ttu-id="e11dd-143">Описание</span><span class="sxs-lookup"><span data-stu-id="e11dd-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e11dd-144">comment</span><span class="sxs-lookup"><span data-stu-id="e11dd-144">comment</span></span>|<span data-ttu-id="e11dd-145">String</span><span class="sxs-lookup"><span data-stu-id="e11dd-145">String</span></span>|<span data-ttu-id="e11dd-p108">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="e11dd-p108">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="e11dd-148">toRecipients</span><span class="sxs-lookup"><span data-stu-id="e11dd-148">toRecipients</span></span>|<span data-ttu-id="e11dd-149">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="e11dd-149">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="e11dd-150">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="e11dd-150">The list of recipients.</span></span>|
|<span data-ttu-id="e11dd-151">message</span><span class="sxs-lookup"><span data-stu-id="e11dd-151">message</span></span>|[<span data-ttu-id="e11dd-152">message</span><span class="sxs-lookup"><span data-stu-id="e11dd-152">message</span></span>](../resources/message.md)|<span data-ttu-id="e11dd-153">Любой доступный свойства для обновления в ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="e11dd-153">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="e11dd-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="e11dd-154">Response</span></span>

<span data-ttu-id="e11dd-p109">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e11dd-p109">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e11dd-157">Пример</span><span class="sxs-lookup"><span data-stu-id="e11dd-157">Example</span></span>
<span data-ttu-id="e11dd-158">В следующем примере задается свойство **isDeliveryReceiptRequested** имеет значение true, добавляется комментарий и перенаправляет сообщение.</span><span class="sxs-lookup"><span data-stu-id="e11dd-158">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="e11dd-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="e11dd-159">Request</span></span>
<span data-ttu-id="e11dd-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e11dd-160">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="e11dd-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="e11dd-161">Response</span></span>
<span data-ttu-id="e11dd-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e11dd-162">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
