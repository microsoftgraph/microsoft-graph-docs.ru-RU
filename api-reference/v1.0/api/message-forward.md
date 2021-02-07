---
title: 'message: forward'
description: Пересылка сообщения. Сообщение сохраняется в папке "Отправленные".
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bf50b58b215eb4ec277c79d15c89e159882ee831
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128388"
---
# <a name="message-forward"></a><span data-ttu-id="f7622-104">message: forward</span><span class="sxs-lookup"><span data-stu-id="f7622-104">message: forward</span></span>

<span data-ttu-id="f7622-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7622-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7622-p102">Пересылка сообщения. Сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="f7622-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7622-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7622-108">Permissions</span></span>
<span data-ttu-id="f7622-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7622-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7622-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7622-111">Permission type</span></span>      | <span data-ttu-id="f7622-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7622-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7622-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7622-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f7622-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f7622-114">Mail.Send</span></span>    |
|<span data-ttu-id="f7622-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7622-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7622-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f7622-116">Mail.Send</span></span>    |
|<span data-ttu-id="f7622-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7622-117">Application</span></span> | <span data-ttu-id="f7622-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f7622-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7622-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7622-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="f7622-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7622-120">Request headers</span></span>
| <span data-ttu-id="f7622-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f7622-121">Name</span></span>       | <span data-ttu-id="f7622-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f7622-122">Type</span></span> | <span data-ttu-id="f7622-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f7622-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f7622-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7622-124">Authorization</span></span>  | <span data-ttu-id="f7622-125">string</span><span class="sxs-lookup"><span data-stu-id="f7622-125">string</span></span>  | <span data-ttu-id="f7622-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7622-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7622-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7622-128">Content-Type</span></span> | <span data-ttu-id="f7622-129">string</span><span class="sxs-lookup"><span data-stu-id="f7622-129">string</span></span>  | <span data-ttu-id="f7622-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7622-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7622-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7622-132">Request body</span></span>
<span data-ttu-id="f7622-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f7622-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7622-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="f7622-134">Parameter</span></span>    | <span data-ttu-id="f7622-135">Тип</span><span class="sxs-lookup"><span data-stu-id="f7622-135">Type</span></span>   |<span data-ttu-id="f7622-136">Описание</span><span class="sxs-lookup"><span data-stu-id="f7622-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7622-137">comment</span><span class="sxs-lookup"><span data-stu-id="f7622-137">comment</span></span>|<span data-ttu-id="f7622-138">String</span><span class="sxs-lookup"><span data-stu-id="f7622-138">String</span></span>|<span data-ttu-id="f7622-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="f7622-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="f7622-141">toRecipients</span><span class="sxs-lookup"><span data-stu-id="f7622-141">toRecipients</span></span>|<span data-ttu-id="f7622-142">Коллекция объектов [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="f7622-142">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="f7622-143">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="f7622-143">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="f7622-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7622-144">Response</span></span>

<span data-ttu-id="f7622-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f7622-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7622-147">Пример</span><span class="sxs-lookup"><span data-stu-id="f7622-147">Example</span></span>
<span data-ttu-id="f7622-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f7622-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f7622-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7622-149">Request</span></span>
<span data-ttu-id="f7622-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7622-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7622-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7622-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f7622-152">C#</span><span class="sxs-lookup"><span data-stu-id="f7622-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7622-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7622-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7622-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7622-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7622-155">Java</span><span class="sxs-lookup"><span data-stu-id="f7622-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f7622-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7622-156">Response</span></span>
##### <a name="response"></a><span data-ttu-id="f7622-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7622-157">Response</span></span>
<span data-ttu-id="f7622-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7622-158">Here is an example of the response.</span></span>
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

