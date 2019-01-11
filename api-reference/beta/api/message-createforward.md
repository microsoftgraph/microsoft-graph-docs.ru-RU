---
title: 'message: createForward'
description: 'Создание прямого черновик сообщения добавить примечание или обновить все свойства сообщения  '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 7d8fa7fa70970e2bb1a5b506d768b3d04311c911
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817670"
---
# <a name="message-createforward"></a><span data-ttu-id="f7b3d-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="f7b3d-103">message: createForward</span></span>

> <span data-ttu-id="f7b3d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7b3d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f7b3d-106">Создание прямого черновик сообщения добавить примечание или обновить все свойства сообщения</span><span class="sxs-lookup"><span data-stu-id="f7b3d-106">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="f7b3d-107">в вызове одной **createForward** .</span><span class="sxs-lookup"><span data-stu-id="f7b3d-107">all in one **createForward** call.</span></span> <span data-ttu-id="f7b3d-108">После этого можно [Отправить](../api/message-send.md) сообщение черновиков.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-108">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="f7b3d-109">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="f7b3d-109">**Note**</span></span>

- <span data-ttu-id="f7b3d-110">Можно указать комментарий или свойству **body** `message` параметр.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="f7b3d-111">Указание оба возвратит ошибку HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="f7b3d-112">Необходимо указать либо `toRecipients` параметр или свойство **toRecipients** `message` параметр.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-112">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="f7b3d-113">Указание оба или указан ни один из них возвратит ошибку HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-113">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7b3d-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7b3d-114">Permissions</span></span>
<span data-ttu-id="f7b3d-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7b3d-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7b3d-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7b3d-117">Permission type</span></span>      | <span data-ttu-id="f7b3d-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7b3d-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7b3d-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7b3d-119">Delegated (work or school account)</span></span> | <span data-ttu-id="f7b3d-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7b3d-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f7b3d-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7b3d-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7b3d-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7b3d-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f7b3d-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7b3d-123">Application</span></span> | <span data-ttu-id="f7b3d-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7b3d-124">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7b3d-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7b3d-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="f7b3d-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7b3d-126">Request headers</span></span>
| <span data-ttu-id="f7b3d-127">Имя</span><span class="sxs-lookup"><span data-stu-id="f7b3d-127">Name</span></span>       | <span data-ttu-id="f7b3d-128">Тип</span><span class="sxs-lookup"><span data-stu-id="f7b3d-128">Type</span></span> | <span data-ttu-id="f7b3d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="f7b3d-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f7b3d-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7b3d-130">Authorization</span></span>  | <span data-ttu-id="f7b3d-131">string</span><span class="sxs-lookup"><span data-stu-id="f7b3d-131">string</span></span>  | <span data-ttu-id="f7b3d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7b3d-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7b3d-134">Content-Type</span></span> | <span data-ttu-id="f7b3d-135">string</span><span class="sxs-lookup"><span data-stu-id="f7b3d-135">string</span></span>  | <span data-ttu-id="f7b3d-p107">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-p107">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7b3d-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7b3d-138">Request body</span></span>
<span data-ttu-id="f7b3d-139">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7b3d-140">Параметр</span><span class="sxs-lookup"><span data-stu-id="f7b3d-140">Parameter</span></span>    | <span data-ttu-id="f7b3d-141">Тип</span><span class="sxs-lookup"><span data-stu-id="f7b3d-141">Type</span></span>   |<span data-ttu-id="f7b3d-142">Описание</span><span class="sxs-lookup"><span data-stu-id="f7b3d-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7b3d-143">comment</span><span class="sxs-lookup"><span data-stu-id="f7b3d-143">comment</span></span>|<span data-ttu-id="f7b3d-144">String</span><span class="sxs-lookup"><span data-stu-id="f7b3d-144">String</span></span>|<span data-ttu-id="f7b3d-p108">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-p108">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="f7b3d-147">toRecipients</span><span class="sxs-lookup"><span data-stu-id="f7b3d-147">toRecipients</span></span>|<span data-ttu-id="f7b3d-148">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="f7b3d-148">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="f7b3d-149">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-149">The list of recipients.</span></span>|
|<span data-ttu-id="f7b3d-150">message</span><span class="sxs-lookup"><span data-stu-id="f7b3d-150">message</span></span>|[<span data-ttu-id="f7b3d-151">message</span><span class="sxs-lookup"><span data-stu-id="f7b3d-151">message</span></span>](../resources/message.md)|<span data-ttu-id="f7b3d-152">Любой доступный свойства для обновления в ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-152">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="f7b3d-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7b3d-153">Response</span></span>

<span data-ttu-id="f7b3d-154">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-154">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7b3d-155">Пример</span><span class="sxs-lookup"><span data-stu-id="f7b3d-155">Example</span></span>
<span data-ttu-id="f7b3d-156">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f7b3d-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7b3d-157">Request</span></span>
<span data-ttu-id="f7b3d-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/createForward
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
  "comment": "Dana, just want to make sure you get this; you'll need this if the project gets approved." 
}
```

##### <a name="response"></a><span data-ttu-id="f7b3d-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7b3d-159">Response</span></span>
<span data-ttu-id="f7b3d-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f7b3d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 272

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKqAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DQ\"",
  "id": "AAMkADA1MTAAAH5JKqAAA=",
  "subject": "FW: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body>\r\nDana, just want to make sure you get this; you'll need this if the project gets approved.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:47:54 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group</body>\r\n</html>\r\n"
  },
  "sender": {
    "emailAddress": {
      "name": "Admin",
      "address": "admin@contoso.onmicrosoft.com"
    }
  },
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "name": "Dana Swope",
        "address": "danas@contoso.onmicrosoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
