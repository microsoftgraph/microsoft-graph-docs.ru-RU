---
title: 'post: forward'
description: 'Переадресация публикации получателю. Вы можете указать родительский сеанс связи и поток в запросе, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 50090aa86676b544e93818d5b0058517c58b85fe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445165"
---
# <a name="post-forward"></a><span data-ttu-id="cc889-104">post: forward</span><span class="sxs-lookup"><span data-stu-id="cc889-104">post: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc889-p102">Пересылка записи получателю. Вы можете указать в запросе родительскую беседу вместе с цепочкой или только родительскую цепочку.</span><span class="sxs-lookup"><span data-stu-id="cc889-p102">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="cc889-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc889-107">Permissions</span></span>
<span data-ttu-id="cc889-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc889-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc889-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc889-110">Permission type</span></span>      | <span data-ttu-id="cc889-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc889-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc889-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc889-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cc889-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc889-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc889-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc889-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc889-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc889-115">Not supported.</span></span>    |
|<span data-ttu-id="cc889-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc889-116">Application</span></span> | <span data-ttu-id="cc889-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc889-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc889-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc889-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="cc889-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc889-119">Request headers</span></span>
| <span data-ttu-id="cc889-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc889-120">Header</span></span>       | <span data-ttu-id="cc889-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cc889-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc889-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc889-122">Authorization</span></span>  | <span data-ttu-id="cc889-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc889-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc889-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cc889-125">Request body</span></span>
<span data-ttu-id="cc889-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cc889-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cc889-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="cc889-127">Parameter</span></span>    | <span data-ttu-id="cc889-128">Тип</span><span class="sxs-lookup"><span data-stu-id="cc889-128">Type</span></span>   |<span data-ttu-id="cc889-129">Описание</span><span class="sxs-lookup"><span data-stu-id="cc889-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc889-130">comment</span><span class="sxs-lookup"><span data-stu-id="cc889-130">comment</span></span>|<span data-ttu-id="cc889-131">String</span><span class="sxs-lookup"><span data-stu-id="cc889-131">String</span></span>|<span data-ttu-id="cc889-132">Необязательный комментарий, который пересылается вместе с записью.</span><span class="sxs-lookup"><span data-stu-id="cc889-132">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="cc889-133">toRecipients</span><span class="sxs-lookup"><span data-stu-id="cc889-133">toRecipients</span></span>|<span data-ttu-id="cc889-134">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="cc889-134">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="cc889-135">Получатели, которым пересылается цепочка.</span><span class="sxs-lookup"><span data-stu-id="cc889-135">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="cc889-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc889-136">Response</span></span>

<span data-ttu-id="cc889-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cc889-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc889-139">Пример</span><span class="sxs-lookup"><span data-stu-id="cc889-139">Example</span></span>
<span data-ttu-id="cc889-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cc889-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cc889-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc889-141">Request</span></span>
<span data-ttu-id="cc889-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc889-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cc889-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc889-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="cc889-144">C#</span><span class="sxs-lookup"><span data-stu-id="cc889-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc889-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="cc889-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cc889-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cc889-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cc889-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc889-147">Response</span></span>
<span data-ttu-id="cc889-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc889-148">Here is an example of the response.</span></span>
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
