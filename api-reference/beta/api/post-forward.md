---
title: 'post: forward'
description: 'Переадресация публикации получателю. Вы можете указать родительский сеанс связи и поток в запросе, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2095e5a22ed15ff5444f424da475cda314925e37
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980461"
---
# <a name="post-forward"></a><span data-ttu-id="22d45-104">post: forward</span><span class="sxs-lookup"><span data-stu-id="22d45-104">post: forward</span></span>

<span data-ttu-id="22d45-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22d45-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22d45-p102">Пересылка записи получателю. Вы можете указать в запросе родительскую беседу вместе с цепочкой или только родительскую цепочку.</span><span class="sxs-lookup"><span data-stu-id="22d45-p102">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="22d45-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22d45-108">Permissions</span></span>
<span data-ttu-id="22d45-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22d45-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22d45-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22d45-111">Permission type</span></span>      | <span data-ttu-id="22d45-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22d45-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22d45-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22d45-113">Delegated (work or school account)</span></span> | <span data-ttu-id="22d45-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22d45-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="22d45-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22d45-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22d45-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22d45-116">Not supported.</span></span>    |
|<span data-ttu-id="22d45-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22d45-117">Application</span></span> | <span data-ttu-id="22d45-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22d45-118">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22d45-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22d45-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="22d45-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22d45-120">Request headers</span></span>
| <span data-ttu-id="22d45-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22d45-121">Header</span></span>       | <span data-ttu-id="22d45-122">Значение</span><span class="sxs-lookup"><span data-stu-id="22d45-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="22d45-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22d45-123">Authorization</span></span>  | <span data-ttu-id="22d45-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22d45-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="22d45-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22d45-126">Request body</span></span>
<span data-ttu-id="22d45-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="22d45-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="22d45-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="22d45-128">Parameter</span></span>    | <span data-ttu-id="22d45-129">Тип</span><span class="sxs-lookup"><span data-stu-id="22d45-129">Type</span></span>   |<span data-ttu-id="22d45-130">Описание</span><span class="sxs-lookup"><span data-stu-id="22d45-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22d45-131">comment</span><span class="sxs-lookup"><span data-stu-id="22d45-131">comment</span></span>|<span data-ttu-id="22d45-132">String</span><span class="sxs-lookup"><span data-stu-id="22d45-132">String</span></span>|<span data-ttu-id="22d45-133">Необязательный комментарий, который пересылается вместе с записью.</span><span class="sxs-lookup"><span data-stu-id="22d45-133">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="22d45-134">toRecipients</span><span class="sxs-lookup"><span data-stu-id="22d45-134">toRecipients</span></span>|<span data-ttu-id="22d45-135">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="22d45-135">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="22d45-136">Получатели, которым пересылается цепочка.</span><span class="sxs-lookup"><span data-stu-id="22d45-136">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="22d45-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="22d45-137">Response</span></span>

<span data-ttu-id="22d45-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="22d45-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22d45-140">Пример</span><span class="sxs-lookup"><span data-stu-id="22d45-140">Example</span></span>
<span data-ttu-id="22d45-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="22d45-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="22d45-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="22d45-142">Request</span></span>
<span data-ttu-id="22d45-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22d45-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22d45-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="22d45-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/forward
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
# <a name="c"></a>[<span data-ttu-id="22d45-145">C#</span><span class="sxs-lookup"><span data-stu-id="22d45-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22d45-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22d45-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22d45-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22d45-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22d45-148">Java</span><span class="sxs-lookup"><span data-stu-id="22d45-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="22d45-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="22d45-149">Response</span></span>
<span data-ttu-id="22d45-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22d45-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


