---
title: 'conversationThread: reply'
description: 'Ответ на цепочку в беседе группы и добавление в нее новой записи. Вы можете указать родительскую беседу. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 39d49f07a588b4b97b44739794a29c51489dcf48
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002688"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="40ecf-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="40ecf-104">conversationThread: reply</span></span>

<span data-ttu-id="40ecf-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40ecf-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40ecf-p102">Ответ на цепочку в беседе группы и добавление в нее новой записи. Вы можете указать в запросе всю родительскую беседу или только цепочку.</span><span class="sxs-lookup"><span data-stu-id="40ecf-p102">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="40ecf-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40ecf-108">Permissions</span></span>
<span data-ttu-id="40ecf-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40ecf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40ecf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40ecf-111">Permission type</span></span>      | <span data-ttu-id="40ecf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40ecf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40ecf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40ecf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="40ecf-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40ecf-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="40ecf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40ecf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40ecf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40ecf-116">Not supported.</span></span>    |
|<span data-ttu-id="40ecf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40ecf-117">Application</span></span> | <span data-ttu-id="40ecf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40ecf-118">Not supported.</span></span>    |

## <a name="http-request"></a><span data-ttu-id="40ecf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40ecf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="40ecf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40ecf-120">Request headers</span></span>
| <span data-ttu-id="40ecf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40ecf-121">Header</span></span>       | <span data-ttu-id="40ecf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="40ecf-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40ecf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40ecf-123">Authorization</span></span>  | <span data-ttu-id="40ecf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40ecf-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="40ecf-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40ecf-126">Content-Type</span></span>  | <span data-ttu-id="40ecf-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40ecf-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40ecf-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40ecf-129">Request body</span></span>
<span data-ttu-id="40ecf-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="40ecf-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="40ecf-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="40ecf-131">Parameter</span></span>    | <span data-ttu-id="40ecf-132">Тип</span><span class="sxs-lookup"><span data-stu-id="40ecf-132">Type</span></span>   |<span data-ttu-id="40ecf-133">Описание</span><span class="sxs-lookup"><span data-stu-id="40ecf-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40ecf-134">post</span><span class="sxs-lookup"><span data-stu-id="40ecf-134">post</span></span>|[<span data-ttu-id="40ecf-135">post</span><span class="sxs-lookup"><span data-stu-id="40ecf-135">post</span></span>](../resources/post.md)|<span data-ttu-id="40ecf-136">Новая запись для ответа.</span><span class="sxs-lookup"><span data-stu-id="40ecf-136">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="40ecf-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="40ecf-137">Response</span></span>

<span data-ttu-id="40ecf-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="40ecf-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40ecf-140">Пример</span><span class="sxs-lookup"><span data-stu-id="40ecf-140">Example</span></span>
<span data-ttu-id="40ecf-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="40ecf-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="40ecf-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="40ecf-142">Request</span></span>
<span data-ttu-id="40ecf-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40ecf-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="40ecf-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="40ecf-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="40ecf-145">C#</span><span class="sxs-lookup"><span data-stu-id="40ecf-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/conversationthread-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40ecf-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40ecf-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/conversationthread-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="40ecf-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="40ecf-147">Response</span></span>
<span data-ttu-id="40ecf-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="40ecf-148">Here is an example of the response.</span></span>
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


