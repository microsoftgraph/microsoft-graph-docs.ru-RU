---
title: 'message: replyAll'
description: Ответ всем получателям сообщения. Затем сообщение сохраняется в папке "Отправленные".
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 07ea6c8846139f6209b188d12cf60273c0838b29
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43355096"
---
# <a name="message-replyall"></a><span data-ttu-id="75c98-104">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="75c98-104">message: replyAll</span></span>

<span data-ttu-id="75c98-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75c98-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75c98-p102">Ответ всем получателям сообщения. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="75c98-p102">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="75c98-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75c98-108">Permissions</span></span>
<span data-ttu-id="75c98-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75c98-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75c98-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75c98-111">Permission type</span></span>      | <span data-ttu-id="75c98-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75c98-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75c98-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75c98-113">Delegated (work or school account)</span></span> | <span data-ttu-id="75c98-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="75c98-114">Mail.Send</span></span>    |
|<span data-ttu-id="75c98-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75c98-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75c98-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="75c98-116">Mail.Send</span></span>    |
|<span data-ttu-id="75c98-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75c98-117">Application</span></span> | <span data-ttu-id="75c98-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="75c98-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="75c98-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75c98-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="75c98-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75c98-120">Request headers</span></span>
| <span data-ttu-id="75c98-121">Имя</span><span class="sxs-lookup"><span data-stu-id="75c98-121">Name</span></span>       | <span data-ttu-id="75c98-122">Тип</span><span class="sxs-lookup"><span data-stu-id="75c98-122">Type</span></span> | <span data-ttu-id="75c98-123">Описание</span><span class="sxs-lookup"><span data-stu-id="75c98-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="75c98-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="75c98-124">Authorization</span></span>  | <span data-ttu-id="75c98-125">string</span><span class="sxs-lookup"><span data-stu-id="75c98-125">string</span></span>  | <span data-ttu-id="75c98-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75c98-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75c98-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75c98-128">Content-Type</span></span> | <span data-ttu-id="75c98-129">string</span><span class="sxs-lookup"><span data-stu-id="75c98-129">string</span></span>  | <span data-ttu-id="75c98-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75c98-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75c98-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75c98-132">Request body</span></span>
<span data-ttu-id="75c98-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="75c98-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="75c98-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="75c98-134">Parameter</span></span>    | <span data-ttu-id="75c98-135">Тип</span><span class="sxs-lookup"><span data-stu-id="75c98-135">Type</span></span>   |<span data-ttu-id="75c98-136">Описание</span><span class="sxs-lookup"><span data-stu-id="75c98-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75c98-137">comment</span><span class="sxs-lookup"><span data-stu-id="75c98-137">comment</span></span>|<span data-ttu-id="75c98-138">String</span><span class="sxs-lookup"><span data-stu-id="75c98-138">String</span></span>|<span data-ttu-id="75c98-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="75c98-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="75c98-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="75c98-141">Response</span></span>

<span data-ttu-id="75c98-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="75c98-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75c98-144">Пример</span><span class="sxs-lookup"><span data-stu-id="75c98-144">Example</span></span>
<span data-ttu-id="75c98-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="75c98-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="75c98-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="75c98-146">Request</span></span>
<span data-ttu-id="75c98-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75c98-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="75c98-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="75c98-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="75c98-149">C#</span><span class="sxs-lookup"><span data-stu-id="75c98-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75c98-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75c98-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75c98-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75c98-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75c98-152">Java</span><span class="sxs-lookup"><span data-stu-id="75c98-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="75c98-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="75c98-153">Response</span></span>
<span data-ttu-id="75c98-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="75c98-154">Here is an example of the response.</span></span>
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
