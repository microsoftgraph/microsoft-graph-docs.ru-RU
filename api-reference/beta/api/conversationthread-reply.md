---
title: 'conversationThread: reply'
description: 'Ответ на цепочку в беседе группы и добавление в нее новой записи. Вы можете указать родительскую беседу. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: af497789df7f32b1d6d2dfd57836ebed0356ced1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319694"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="40625-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="40625-104">conversationThread: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40625-p102">Ответ на цепочку в беседе группы и добавление в нее новой записи. Вы можете указать в запросе всю родительскую беседу или только цепочку.</span><span class="sxs-lookup"><span data-stu-id="40625-p102">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="40625-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40625-107">Permissions</span></span>
<span data-ttu-id="40625-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40625-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40625-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40625-110">Permission type</span></span>      | <span data-ttu-id="40625-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40625-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40625-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40625-112">Delegated (work or school account)</span></span> | <span data-ttu-id="40625-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40625-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="40625-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40625-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40625-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40625-115">Not supported.</span></span>    |
|<span data-ttu-id="40625-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40625-116">Application</span></span> | <span data-ttu-id="40625-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40625-117">Not supported.</span></span>    |

## <a name="http-request"></a><span data-ttu-id="40625-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40625-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="40625-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40625-119">Request headers</span></span>
| <span data-ttu-id="40625-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40625-120">Header</span></span>       | <span data-ttu-id="40625-121">Значение</span><span class="sxs-lookup"><span data-stu-id="40625-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40625-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40625-122">Authorization</span></span>  | <span data-ttu-id="40625-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40625-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="40625-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40625-125">Content-Type</span></span>  | <span data-ttu-id="40625-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40625-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40625-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40625-128">Request body</span></span>
<span data-ttu-id="40625-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="40625-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="40625-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="40625-130">Parameter</span></span>    | <span data-ttu-id="40625-131">Тип</span><span class="sxs-lookup"><span data-stu-id="40625-131">Type</span></span>   |<span data-ttu-id="40625-132">Описание</span><span class="sxs-lookup"><span data-stu-id="40625-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40625-133">post</span><span class="sxs-lookup"><span data-stu-id="40625-133">post</span></span>|[<span data-ttu-id="40625-134">post</span><span class="sxs-lookup"><span data-stu-id="40625-134">post</span></span>](../resources/post.md)|<span data-ttu-id="40625-135">Новая запись для ответа.</span><span class="sxs-lookup"><span data-stu-id="40625-135">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="40625-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="40625-136">Response</span></span>

<span data-ttu-id="40625-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="40625-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40625-139">Пример</span><span class="sxs-lookup"><span data-stu-id="40625-139">Example</span></span>
<span data-ttu-id="40625-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="40625-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="40625-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="40625-141">Request</span></span>
<span data-ttu-id="40625-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40625-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="40625-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="40625-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/reply
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="40625-144">C#</span><span class="sxs-lookup"><span data-stu-id="40625-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/conversationthread-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40625-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40625-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/conversationthread-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="40625-146">Java</span><span class="sxs-lookup"><span data-stu-id="40625-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/conversationthread-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="40625-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="40625-147">Response</span></span>
<span data-ttu-id="40625-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="40625-148">Here is an example of the response.</span></span>
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
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
