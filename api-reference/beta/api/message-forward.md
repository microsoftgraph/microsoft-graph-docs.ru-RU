---
title: 'message: forward'
description: 'Переслать сообщение, добавить комментарий или изменить любые обновляемые свойства  '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ed3d51c28e6fe0404b5cb26fb17f6d8ed3bba212
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508890"
---
# <a name="message-forward"></a><span data-ttu-id="27804-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="27804-103">message: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27804-104">Переслать сообщение, добавить комментарий или изменить любые обновляемые свойства</span><span class="sxs-lookup"><span data-stu-id="27804-104">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="27804-105">все в одной **переадресовывать** вызова.</span><span class="sxs-lookup"><span data-stu-id="27804-105">all in one **forward** call.</span></span> <span data-ttu-id="27804-106">Сообщение сохраняется в папке «Отправленные».</span><span class="sxs-lookup"><span data-stu-id="27804-106">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="27804-107">Кроме того можно первого [создания переслать сообщение черновиков](../api/message-createforward.md) добавить примечание или обновить все свойства сообщений, а затем [Отправить](../api/message-send.md) сообщение черновиков.</span><span class="sxs-lookup"><span data-stu-id="27804-107">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="27804-108">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="27804-108">**Note**</span></span>

- <span data-ttu-id="27804-109">Можно указать комментарий или свойству **body** `message` параметр.</span><span class="sxs-lookup"><span data-stu-id="27804-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="27804-110">Указание оба возвратит ошибку HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="27804-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="27804-111">Необходимо указать либо `toRecipients` параметр или свойство **toRecipients** `message` параметр.</span><span class="sxs-lookup"><span data-stu-id="27804-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="27804-112">Указание оба или указан ни один из них возвратит ошибку HTTP 400 Bad Request.</span><span class="sxs-lookup"><span data-stu-id="27804-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="27804-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27804-113">Permissions</span></span>
<span data-ttu-id="27804-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27804-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27804-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27804-116">Permission type</span></span>      | <span data-ttu-id="27804-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27804-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27804-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27804-118">Delegated (work or school account)</span></span> | <span data-ttu-id="27804-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="27804-119">Mail.Send</span></span>    |
|<span data-ttu-id="27804-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27804-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27804-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="27804-121">Mail.Send</span></span>    |
|<span data-ttu-id="27804-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27804-122">Application</span></span> | <span data-ttu-id="27804-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="27804-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="27804-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27804-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="27804-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27804-125">Request headers</span></span>
| <span data-ttu-id="27804-126">Имя</span><span class="sxs-lookup"><span data-stu-id="27804-126">Name</span></span>       | <span data-ttu-id="27804-127">Тип</span><span class="sxs-lookup"><span data-stu-id="27804-127">Type</span></span> | <span data-ttu-id="27804-128">Описание</span><span class="sxs-lookup"><span data-stu-id="27804-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="27804-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="27804-129">Authorization</span></span>  | <span data-ttu-id="27804-130">string</span><span class="sxs-lookup"><span data-stu-id="27804-130">string</span></span>  | <span data-ttu-id="27804-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27804-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27804-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27804-133">Content-Type</span></span> | <span data-ttu-id="27804-134">string</span><span class="sxs-lookup"><span data-stu-id="27804-134">string</span></span>  | <span data-ttu-id="27804-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27804-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27804-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27804-137">Request body</span></span>
<span data-ttu-id="27804-138">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="27804-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="27804-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="27804-139">Parameter</span></span>    | <span data-ttu-id="27804-140">Тип</span><span class="sxs-lookup"><span data-stu-id="27804-140">Type</span></span>   |<span data-ttu-id="27804-141">Описание</span><span class="sxs-lookup"><span data-stu-id="27804-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27804-142">comment</span><span class="sxs-lookup"><span data-stu-id="27804-142">comment</span></span>|<span data-ttu-id="27804-143">String</span><span class="sxs-lookup"><span data-stu-id="27804-143">String</span></span>|<span data-ttu-id="27804-p107">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="27804-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="27804-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="27804-146">toRecipients</span></span>|<span data-ttu-id="27804-147">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="27804-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="27804-148">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="27804-148">The list of recipients.</span></span>|
|<span data-ttu-id="27804-149">message</span><span class="sxs-lookup"><span data-stu-id="27804-149">message</span></span>|[<span data-ttu-id="27804-150">message</span><span class="sxs-lookup"><span data-stu-id="27804-150">message</span></span>](../resources/message.md)|<span data-ttu-id="27804-151">Любой доступный свойства для обновления в ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="27804-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="27804-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="27804-152">Response</span></span>

<span data-ttu-id="27804-p108">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="27804-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27804-155">Пример</span><span class="sxs-lookup"><span data-stu-id="27804-155">Example</span></span>
<span data-ttu-id="27804-156">В следующем примере задается свойство **isDeliveryReceiptRequested** имеет значение true, добавляется комментарий и перенаправляет сообщение.</span><span class="sxs-lookup"><span data-stu-id="27804-156">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="27804-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="27804-157">Request</span></span>
<span data-ttu-id="27804-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27804-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="27804-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="27804-159">Response</span></span>
<span data-ttu-id="27804-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27804-160">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-forward.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
