---
title: 'message: forward'
description: Пересылка сообщения. Сообщение сохраняется в папке "Отправленные".
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 12409685e21b338a86b392f32449b006a0e958f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960548"
---
# <a name="message-forward"></a><span data-ttu-id="4bcc7-104">message: forward</span><span class="sxs-lookup"><span data-stu-id="4bcc7-104">message: forward</span></span>

<span data-ttu-id="4bcc7-p102">Пересылка сообщения. Сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="4bcc7-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bcc7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4bcc7-107">Permissions</span></span>
<span data-ttu-id="4bcc7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bcc7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bcc7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bcc7-110">Permission type</span></span>      | <span data-ttu-id="4bcc7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bcc7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bcc7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bcc7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4bcc7-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="4bcc7-113">Mail.Send</span></span>    |
|<span data-ttu-id="4bcc7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bcc7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bcc7-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="4bcc7-115">Mail.Send</span></span>    |
|<span data-ttu-id="4bcc7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bcc7-116">Application</span></span> | <span data-ttu-id="4bcc7-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="4bcc7-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bcc7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bcc7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="4bcc7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bcc7-119">Request headers</span></span>
| <span data-ttu-id="4bcc7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4bcc7-120">Name</span></span>       | <span data-ttu-id="4bcc7-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4bcc7-121">Type</span></span> | <span data-ttu-id="4bcc7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4bcc7-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4bcc7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bcc7-123">Authorization</span></span>  | <span data-ttu-id="4bcc7-124">строка</span><span class="sxs-lookup"><span data-stu-id="4bcc7-124">string</span></span>  | <span data-ttu-id="4bcc7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bcc7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4bcc7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4bcc7-127">Content-Type</span></span> | <span data-ttu-id="4bcc7-128">строка</span><span class="sxs-lookup"><span data-stu-id="4bcc7-128">string</span></span>  | <span data-ttu-id="4bcc7-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bcc7-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bcc7-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4bcc7-131">Request body</span></span>
<span data-ttu-id="4bcc7-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4bcc7-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4bcc7-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="4bcc7-133">Parameter</span></span>    | <span data-ttu-id="4bcc7-134">Тип</span><span class="sxs-lookup"><span data-stu-id="4bcc7-134">Type</span></span>   |<span data-ttu-id="4bcc7-135">Описание</span><span class="sxs-lookup"><span data-stu-id="4bcc7-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bcc7-136">comment</span><span class="sxs-lookup"><span data-stu-id="4bcc7-136">comment</span></span>|<span data-ttu-id="4bcc7-137">String</span><span class="sxs-lookup"><span data-stu-id="4bcc7-137">String</span></span>|<span data-ttu-id="4bcc7-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="4bcc7-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="4bcc7-140">toRecipients</span><span class="sxs-lookup"><span data-stu-id="4bcc7-140">toRecipients</span></span>|<span data-ttu-id="4bcc7-141">Коллекция объектов [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="4bcc7-141">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="4bcc7-142">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="4bcc7-142">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="4bcc7-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bcc7-143">Response</span></span>

<span data-ttu-id="4bcc7-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4bcc7-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bcc7-146">Пример</span><span class="sxs-lookup"><span data-stu-id="4bcc7-146">Example</span></span>
<span data-ttu-id="4bcc7-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4bcc7-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4bcc7-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bcc7-148">Request</span></span>
<span data-ttu-id="4bcc7-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bcc7-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="4bcc7-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bcc7-150">Response</span></span>
##### <a name="response"></a><span data-ttu-id="4bcc7-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bcc7-151">Response</span></span>
<span data-ttu-id="4bcc7-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4bcc7-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
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
