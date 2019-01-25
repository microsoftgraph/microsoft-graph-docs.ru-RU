---
title: 'message: createForward'
description: 'Создание прямого черновик сообщения добавить примечание или обновить все свойства сообщения  '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2c750ac0dd8f6a6226161701950bd879025f9641
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519530"
---
# <a name="message-createforward"></a><span data-ttu-id="6186f-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="6186f-103">message: createForward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6186f-104">Создание прямого черновик сообщения добавить примечание или обновить все свойства сообщения</span><span class="sxs-lookup"><span data-stu-id="6186f-104">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="6186f-105">в вызове одной **createForward** .</span><span class="sxs-lookup"><span data-stu-id="6186f-105">all in one **createForward** call.</span></span> <span data-ttu-id="6186f-106">После этого можно [Отправить](../api/message-send.md) сообщение черновиков.</span><span class="sxs-lookup"><span data-stu-id="6186f-106">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="6186f-107">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="6186f-107">**Note**</span></span>

- <span data-ttu-id="6186f-108">Можно указать комментарий или свойству **body** `message` параметр.</span><span class="sxs-lookup"><span data-stu-id="6186f-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="6186f-109">Указание оба возвратит ошибку HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="6186f-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="6186f-110">Необходимо указать либо `toRecipients` параметр или свойство **toRecipients** `message` параметр.</span><span class="sxs-lookup"><span data-stu-id="6186f-110">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="6186f-111">Указание оба или указан ни один из них возвратит ошибку HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="6186f-111">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="6186f-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6186f-112">Permissions</span></span>
<span data-ttu-id="6186f-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6186f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6186f-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6186f-115">Permission type</span></span>      | <span data-ttu-id="6186f-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6186f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6186f-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6186f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="6186f-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6186f-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6186f-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6186f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6186f-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6186f-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6186f-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6186f-121">Application</span></span> | <span data-ttu-id="6186f-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6186f-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6186f-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6186f-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="6186f-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6186f-124">Request headers</span></span>
| <span data-ttu-id="6186f-125">Имя</span><span class="sxs-lookup"><span data-stu-id="6186f-125">Name</span></span>       | <span data-ttu-id="6186f-126">Тип</span><span class="sxs-lookup"><span data-stu-id="6186f-126">Type</span></span> | <span data-ttu-id="6186f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="6186f-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6186f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="6186f-128">Authorization</span></span>  | <span data-ttu-id="6186f-129">string</span><span class="sxs-lookup"><span data-stu-id="6186f-129">string</span></span>  | <span data-ttu-id="6186f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6186f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6186f-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6186f-132">Content-Type</span></span> | <span data-ttu-id="6186f-133">string</span><span class="sxs-lookup"><span data-stu-id="6186f-133">string</span></span>  | <span data-ttu-id="6186f-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6186f-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6186f-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6186f-136">Request body</span></span>
<span data-ttu-id="6186f-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6186f-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6186f-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="6186f-138">Parameter</span></span>    | <span data-ttu-id="6186f-139">Тип</span><span class="sxs-lookup"><span data-stu-id="6186f-139">Type</span></span>   |<span data-ttu-id="6186f-140">Описание</span><span class="sxs-lookup"><span data-stu-id="6186f-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6186f-141">comment</span><span class="sxs-lookup"><span data-stu-id="6186f-141">comment</span></span>|<span data-ttu-id="6186f-142">String</span><span class="sxs-lookup"><span data-stu-id="6186f-142">String</span></span>|<span data-ttu-id="6186f-p107">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="6186f-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="6186f-145">toRecipients</span><span class="sxs-lookup"><span data-stu-id="6186f-145">toRecipients</span></span>|<span data-ttu-id="6186f-146">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="6186f-146">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="6186f-147">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="6186f-147">The list of recipients.</span></span>|
|<span data-ttu-id="6186f-148">message</span><span class="sxs-lookup"><span data-stu-id="6186f-148">message</span></span>|[<span data-ttu-id="6186f-149">message</span><span class="sxs-lookup"><span data-stu-id="6186f-149">message</span></span>](../resources/message.md)|<span data-ttu-id="6186f-150">Любой доступный свойства для обновления в ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="6186f-150">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="6186f-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="6186f-151">Response</span></span>

<span data-ttu-id="6186f-152">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6186f-152">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6186f-153">Пример</span><span class="sxs-lookup"><span data-stu-id="6186f-153">Example</span></span>
<span data-ttu-id="6186f-154">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6186f-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6186f-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="6186f-155">Request</span></span>
<span data-ttu-id="6186f-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6186f-156">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6186f-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="6186f-157">Response</span></span>
<span data-ttu-id="6186f-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6186f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-createforward.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
