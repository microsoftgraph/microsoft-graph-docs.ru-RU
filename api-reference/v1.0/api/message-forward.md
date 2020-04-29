---
title: 'message: forward'
description: Пересылка сообщения. Сообщение сохраняется в папке "Отправленные".
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 086d411091e4476837a531daad93db6b7da3e587
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43361525"
---
# <a name="message-forward"></a><span data-ttu-id="8e07f-104">message: forward</span><span class="sxs-lookup"><span data-stu-id="8e07f-104">message: forward</span></span>

<span data-ttu-id="8e07f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e07f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e07f-p102">Пересылка сообщения. Сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="8e07f-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e07f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e07f-108">Permissions</span></span>
<span data-ttu-id="8e07f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e07f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e07f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e07f-111">Permission type</span></span>      | <span data-ttu-id="8e07f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e07f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e07f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e07f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8e07f-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8e07f-114">Mail.Send</span></span>    |
|<span data-ttu-id="8e07f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e07f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e07f-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8e07f-116">Mail.Send</span></span>    |
|<span data-ttu-id="8e07f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e07f-117">Application</span></span> | <span data-ttu-id="8e07f-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8e07f-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e07f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e07f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="8e07f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e07f-120">Request headers</span></span>
| <span data-ttu-id="8e07f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8e07f-121">Name</span></span>       | <span data-ttu-id="8e07f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="8e07f-122">Type</span></span> | <span data-ttu-id="8e07f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8e07f-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8e07f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e07f-124">Authorization</span></span>  | <span data-ttu-id="8e07f-125">string</span><span class="sxs-lookup"><span data-stu-id="8e07f-125">string</span></span>  | <span data-ttu-id="8e07f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e07f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e07f-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8e07f-128">Content-Type</span></span> | <span data-ttu-id="8e07f-129">string</span><span class="sxs-lookup"><span data-stu-id="8e07f-129">string</span></span>  | <span data-ttu-id="8e07f-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e07f-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e07f-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e07f-132">Request body</span></span>
<span data-ttu-id="8e07f-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8e07f-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8e07f-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="8e07f-134">Parameter</span></span>    | <span data-ttu-id="8e07f-135">Тип</span><span class="sxs-lookup"><span data-stu-id="8e07f-135">Type</span></span>   |<span data-ttu-id="8e07f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8e07f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e07f-137">comment</span><span class="sxs-lookup"><span data-stu-id="8e07f-137">comment</span></span>|<span data-ttu-id="8e07f-138">String</span><span class="sxs-lookup"><span data-stu-id="8e07f-138">String</span></span>|<span data-ttu-id="8e07f-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="8e07f-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="8e07f-141">toRecipients</span><span class="sxs-lookup"><span data-stu-id="8e07f-141">toRecipients</span></span>|<span data-ttu-id="8e07f-142">Коллекция объектов [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="8e07f-142">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="8e07f-143">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="8e07f-143">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="8e07f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e07f-144">Response</span></span>

<span data-ttu-id="8e07f-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8e07f-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e07f-147">Пример</span><span class="sxs-lookup"><span data-stu-id="8e07f-147">Example</span></span>
<span data-ttu-id="8e07f-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8e07f-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8e07f-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e07f-149">Request</span></span>
<span data-ttu-id="8e07f-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e07f-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e07f-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e07f-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8e07f-152">C#</span><span class="sxs-lookup"><span data-stu-id="8e07f-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e07f-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e07f-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e07f-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e07f-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e07f-155">Java</span><span class="sxs-lookup"><span data-stu-id="8e07f-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8e07f-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e07f-156">Response</span></span>
##### <a name="response"></a><span data-ttu-id="8e07f-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e07f-157">Response</span></span>
<span data-ttu-id="8e07f-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e07f-158">Here is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
