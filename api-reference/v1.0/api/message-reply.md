---
title: 'message: reply'
description: Ответ отправителю сообщения. Затем сообщение сохраняется в папке "Отправленные".
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 61e11f763a4ebfa5fda64cffb661e39649469f8d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444612"
---
# <a name="message-reply"></a><span data-ttu-id="6e85d-104">message: reply</span><span class="sxs-lookup"><span data-stu-id="6e85d-104">message: reply</span></span>

<span data-ttu-id="6e85d-p102">Ответ отправителю сообщения. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="6e85d-p102">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e85d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e85d-107">Permissions</span></span>
<span data-ttu-id="6e85d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e85d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e85d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e85d-110">Permission type</span></span>      | <span data-ttu-id="6e85d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e85d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e85d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e85d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6e85d-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="6e85d-113">Mail.Send</span></span>    |
|<span data-ttu-id="6e85d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e85d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e85d-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="6e85d-115">Mail.Send</span></span>    |
|<span data-ttu-id="6e85d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e85d-116">Application</span></span> | <span data-ttu-id="6e85d-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="6e85d-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e85d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e85d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="6e85d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e85d-119">Request headers</span></span>
| <span data-ttu-id="6e85d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6e85d-120">Name</span></span>       | <span data-ttu-id="6e85d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6e85d-121">Type</span></span> | <span data-ttu-id="6e85d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6e85d-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6e85d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e85d-123">Authorization</span></span>  | <span data-ttu-id="6e85d-124">string</span><span class="sxs-lookup"><span data-stu-id="6e85d-124">string</span></span>  | <span data-ttu-id="6e85d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e85d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6e85d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e85d-127">Content-Type</span></span> | <span data-ttu-id="6e85d-128">string</span><span class="sxs-lookup"><span data-stu-id="6e85d-128">string</span></span>  | <span data-ttu-id="6e85d-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e85d-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e85d-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e85d-131">Request body</span></span>
<span data-ttu-id="6e85d-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6e85d-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6e85d-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="6e85d-133">Parameter</span></span>    | <span data-ttu-id="6e85d-134">Тип</span><span class="sxs-lookup"><span data-stu-id="6e85d-134">Type</span></span>   |<span data-ttu-id="6e85d-135">Описание</span><span class="sxs-lookup"><span data-stu-id="6e85d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e85d-136">comment</span><span class="sxs-lookup"><span data-stu-id="6e85d-136">comment</span></span>|<span data-ttu-id="6e85d-137">String</span><span class="sxs-lookup"><span data-stu-id="6e85d-137">String</span></span>|<span data-ttu-id="6e85d-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="6e85d-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="6e85d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e85d-140">Response</span></span>

<span data-ttu-id="6e85d-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6e85d-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e85d-143">Пример</span><span class="sxs-lookup"><span data-stu-id="6e85d-143">Example</span></span>
<span data-ttu-id="6e85d-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6e85d-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6e85d-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e85d-145">Request</span></span>
<span data-ttu-id="6e85d-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e85d-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6e85d-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e85d-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/reply
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6e85d-148">C#</span><span class="sxs-lookup"><span data-stu-id="6e85d-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6e85d-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="6e85d-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6e85d-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6e85d-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6e85d-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e85d-151">Response</span></span>
##### <a name="response"></a><span data-ttu-id="6e85d-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e85d-152">Response</span></span>
<span data-ttu-id="6e85d-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6e85d-153">Here is an example of the response.</span></span>
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
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
