---
title: 'message: replyAll'
description: Ответ всем получателям сообщения. Затем сообщение сохраняется в папке "Отправленные".
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2596dfcf93895dc152673bc2e7e89a3f7380b322
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374689"
---
# <a name="message-replyall"></a><span data-ttu-id="5b6a2-104">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="5b6a2-104">message: replyAll</span></span>

<span data-ttu-id="5b6a2-p102">Ответ всем получателям сообщения. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="5b6a2-p102">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b6a2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b6a2-107">Permissions</span></span>
<span data-ttu-id="5b6a2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b6a2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b6a2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b6a2-110">Permission type</span></span>      | <span data-ttu-id="5b6a2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b6a2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b6a2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b6a2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5b6a2-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="5b6a2-113">Mail.Send</span></span>    |
|<span data-ttu-id="5b6a2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b6a2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b6a2-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="5b6a2-115">Mail.Send</span></span>    |
|<span data-ttu-id="5b6a2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b6a2-116">Application</span></span> | <span data-ttu-id="5b6a2-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="5b6a2-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b6a2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b6a2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="5b6a2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b6a2-119">Request headers</span></span>
| <span data-ttu-id="5b6a2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5b6a2-120">Name</span></span>       | <span data-ttu-id="5b6a2-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5b6a2-121">Type</span></span> | <span data-ttu-id="5b6a2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5b6a2-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5b6a2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b6a2-123">Authorization</span></span>  | <span data-ttu-id="5b6a2-124">string</span><span class="sxs-lookup"><span data-stu-id="5b6a2-124">string</span></span>  | <span data-ttu-id="5b6a2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b6a2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b6a2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b6a2-127">Content-Type</span></span> | <span data-ttu-id="5b6a2-128">string</span><span class="sxs-lookup"><span data-stu-id="5b6a2-128">string</span></span>  | <span data-ttu-id="5b6a2-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b6a2-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b6a2-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b6a2-131">Request body</span></span>
<span data-ttu-id="5b6a2-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5b6a2-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5b6a2-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="5b6a2-133">Parameter</span></span>    | <span data-ttu-id="5b6a2-134">Тип</span><span class="sxs-lookup"><span data-stu-id="5b6a2-134">Type</span></span>   |<span data-ttu-id="5b6a2-135">Описание</span><span class="sxs-lookup"><span data-stu-id="5b6a2-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b6a2-136">comment</span><span class="sxs-lookup"><span data-stu-id="5b6a2-136">comment</span></span>|<span data-ttu-id="5b6a2-137">String</span><span class="sxs-lookup"><span data-stu-id="5b6a2-137">String</span></span>|<span data-ttu-id="5b6a2-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="5b6a2-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="5b6a2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b6a2-140">Response</span></span>

<span data-ttu-id="5b6a2-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5b6a2-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b6a2-143">Пример</span><span class="sxs-lookup"><span data-stu-id="5b6a2-143">Example</span></span>
<span data-ttu-id="5b6a2-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5b6a2-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5b6a2-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b6a2-145">Request</span></span>
<span data-ttu-id="5b6a2-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b6a2-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5b6a2-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b6a2-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/replyAll
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5b6a2-148">C#</span><span class="sxs-lookup"><span data-stu-id="5b6a2-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b6a2-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b6a2-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5b6a2-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5b6a2-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5b6a2-151">Java</span><span class="sxs-lookup"><span data-stu-id="5b6a2-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="5b6a2-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b6a2-152">Response</span></span>
<span data-ttu-id="5b6a2-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b6a2-153">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
