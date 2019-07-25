---
title: 'conversationThread: reply'
description: 'Ответ на цепочку в беседе группы и добавление в нее новой записи. Вы можете указать родительскую беседу. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 711a16aad7bae595eb4cc55f2cdc24ec784dfa69
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883603"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="96c50-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="96c50-104">conversationThread: reply</span></span>

<span data-ttu-id="96c50-p102">Ответ на цепочку в беседе группы и добавление в нее новой записи. Вы можете указать в запросе всю родительскую беседу или только цепочку.</span><span class="sxs-lookup"><span data-stu-id="96c50-p102">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="96c50-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96c50-107">Permissions</span></span>
<span data-ttu-id="96c50-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96c50-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96c50-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96c50-110">Permission type</span></span>      | <span data-ttu-id="96c50-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96c50-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96c50-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96c50-112">Delegated (work or school account)</span></span> | <span data-ttu-id="96c50-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96c50-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="96c50-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96c50-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96c50-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96c50-115">Not supported.</span></span>    |
|<span data-ttu-id="96c50-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96c50-116">Application</span></span> | <span data-ttu-id="96c50-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96c50-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96c50-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96c50-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="96c50-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96c50-119">Request headers</span></span>
| <span data-ttu-id="96c50-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96c50-120">Header</span></span>       | <span data-ttu-id="96c50-121">Значение</span><span class="sxs-lookup"><span data-stu-id="96c50-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="96c50-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96c50-122">Authorization</span></span>  | <span data-ttu-id="96c50-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96c50-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="96c50-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96c50-125">Content-Type</span></span>  | <span data-ttu-id="96c50-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96c50-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="96c50-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96c50-128">Request body</span></span>
<span data-ttu-id="96c50-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="96c50-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="96c50-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="96c50-130">Parameter</span></span>    | <span data-ttu-id="96c50-131">Тип</span><span class="sxs-lookup"><span data-stu-id="96c50-131">Type</span></span>   |<span data-ttu-id="96c50-132">Описание</span><span class="sxs-lookup"><span data-stu-id="96c50-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96c50-133">post</span><span class="sxs-lookup"><span data-stu-id="96c50-133">post</span></span>|[<span data-ttu-id="96c50-134">post</span><span class="sxs-lookup"><span data-stu-id="96c50-134">post</span></span>](../resources/post.md)|<span data-ttu-id="96c50-135">Новая запись для ответа.</span><span class="sxs-lookup"><span data-stu-id="96c50-135">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="96c50-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="96c50-136">Response</span></span>

<span data-ttu-id="96c50-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="96c50-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96c50-139">Пример</span><span class="sxs-lookup"><span data-stu-id="96c50-139">Example</span></span>
<span data-ttu-id="96c50-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="96c50-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="96c50-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="96c50-141">Request</span></span>
<span data-ttu-id="96c50-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96c50-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="96c50-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="96c50-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96c50-144">C#</span><span class="sxs-lookup"><span data-stu-id="96c50-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/conversationthread-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96c50-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="96c50-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/conversationthread-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="96c50-146">Java</span><span class="sxs-lookup"><span data-stu-id="96c50-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/conversationthread-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="96c50-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="96c50-147">Response</span></span>
<span data-ttu-id="96c50-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="96c50-148">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
