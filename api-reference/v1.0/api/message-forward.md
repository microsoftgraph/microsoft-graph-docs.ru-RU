---
title: 'message: forward'
description: Пересылка сообщения. Сообщение сохраняется в папке "Отправленные".
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f3d568d4e519ab17d39bd01eabe28830ea29d17c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374766"
---
# <a name="message-forward"></a><span data-ttu-id="c991e-104">message: forward</span><span class="sxs-lookup"><span data-stu-id="c991e-104">message: forward</span></span>

<span data-ttu-id="c991e-p102">Пересылка сообщения. Сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="c991e-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="c991e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c991e-107">Permissions</span></span>
<span data-ttu-id="c991e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c991e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c991e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c991e-110">Permission type</span></span>      | <span data-ttu-id="c991e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c991e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c991e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c991e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c991e-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c991e-113">Mail.Send</span></span>    |
|<span data-ttu-id="c991e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c991e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c991e-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c991e-115">Mail.Send</span></span>    |
|<span data-ttu-id="c991e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c991e-116">Application</span></span> | <span data-ttu-id="c991e-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c991e-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="c991e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c991e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="c991e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c991e-119">Request headers</span></span>
| <span data-ttu-id="c991e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c991e-120">Name</span></span>       | <span data-ttu-id="c991e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c991e-121">Type</span></span> | <span data-ttu-id="c991e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c991e-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c991e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c991e-123">Authorization</span></span>  | <span data-ttu-id="c991e-124">string</span><span class="sxs-lookup"><span data-stu-id="c991e-124">string</span></span>  | <span data-ttu-id="c991e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c991e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c991e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c991e-127">Content-Type</span></span> | <span data-ttu-id="c991e-128">string</span><span class="sxs-lookup"><span data-stu-id="c991e-128">string</span></span>  | <span data-ttu-id="c991e-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c991e-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c991e-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c991e-131">Request body</span></span>
<span data-ttu-id="c991e-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c991e-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c991e-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="c991e-133">Parameter</span></span>    | <span data-ttu-id="c991e-134">Тип</span><span class="sxs-lookup"><span data-stu-id="c991e-134">Type</span></span>   |<span data-ttu-id="c991e-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c991e-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c991e-136">comment</span><span class="sxs-lookup"><span data-stu-id="c991e-136">comment</span></span>|<span data-ttu-id="c991e-137">String</span><span class="sxs-lookup"><span data-stu-id="c991e-137">String</span></span>|<span data-ttu-id="c991e-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="c991e-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="c991e-140">toRecipients</span><span class="sxs-lookup"><span data-stu-id="c991e-140">toRecipients</span></span>|<span data-ttu-id="c991e-141">Коллекция объектов [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="c991e-141">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="c991e-142">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="c991e-142">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="c991e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c991e-143">Response</span></span>

<span data-ttu-id="c991e-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c991e-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c991e-146">Пример</span><span class="sxs-lookup"><span data-stu-id="c991e-146">Example</span></span>
<span data-ttu-id="c991e-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c991e-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c991e-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c991e-148">Request</span></span>
<span data-ttu-id="c991e-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c991e-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c991e-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="c991e-150">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c991e-151">C#</span><span class="sxs-lookup"><span data-stu-id="c991e-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c991e-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c991e-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c991e-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c991e-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c991e-154">Java</span><span class="sxs-lookup"><span data-stu-id="c991e-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c991e-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="c991e-155">Response</span></span>
##### <a name="response"></a><span data-ttu-id="c991e-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="c991e-156">Response</span></span>
<span data-ttu-id="c991e-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c991e-157">Here is an example of the response.</span></span>
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
