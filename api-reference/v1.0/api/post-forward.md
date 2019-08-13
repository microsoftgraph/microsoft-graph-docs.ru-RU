---
title: 'post: forward'
description: 'Переадресация публикации получателю. Вы можете указать родительский сеанс связи и поток в запросе, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 226ab9aebc5dab0cca28a992ebe1e42b7cbb8c58
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375767"
---
# <a name="post-forward"></a><span data-ttu-id="b8915-104">post: forward</span><span class="sxs-lookup"><span data-stu-id="b8915-104">post: forward</span></span>

<span data-ttu-id="b8915-p102">Пересылка записи получателю. Вы можете указать в запросе родительскую беседу вместе с цепочкой или только родительскую цепочку.</span><span class="sxs-lookup"><span data-stu-id="b8915-p102">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b8915-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8915-107">Permissions</span></span>
<span data-ttu-id="b8915-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8915-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8915-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8915-110">Permission type</span></span>      | <span data-ttu-id="b8915-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8915-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8915-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8915-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b8915-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8915-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b8915-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8915-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8915-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8915-115">Not supported.</span></span>    |
|<span data-ttu-id="b8915-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8915-116">Application</span></span> | <span data-ttu-id="b8915-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8915-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8915-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8915-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="b8915-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8915-119">Request headers</span></span>
| <span data-ttu-id="b8915-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8915-120">Header</span></span>       | <span data-ttu-id="b8915-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b8915-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8915-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8915-122">Authorization</span></span>  | <span data-ttu-id="b8915-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8915-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8915-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b8915-125">Request body</span></span>
<span data-ttu-id="b8915-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b8915-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b8915-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="b8915-127">Parameter</span></span>    | <span data-ttu-id="b8915-128">Тип</span><span class="sxs-lookup"><span data-stu-id="b8915-128">Type</span></span>   |<span data-ttu-id="b8915-129">Описание</span><span class="sxs-lookup"><span data-stu-id="b8915-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8915-130">comment</span><span class="sxs-lookup"><span data-stu-id="b8915-130">comment</span></span>|<span data-ttu-id="b8915-131">String</span><span class="sxs-lookup"><span data-stu-id="b8915-131">String</span></span>|<span data-ttu-id="b8915-132">Необязательный комментарий, который пересылается вместе с записью.</span><span class="sxs-lookup"><span data-stu-id="b8915-132">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="b8915-133">toRecipients</span><span class="sxs-lookup"><span data-stu-id="b8915-133">toRecipients</span></span>|<span data-ttu-id="b8915-134">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="b8915-134">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="b8915-135">Получатели, которым пересылается цепочка.</span><span class="sxs-lookup"><span data-stu-id="b8915-135">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="b8915-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8915-136">Response</span></span>

<span data-ttu-id="b8915-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b8915-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8915-139">Пример</span><span class="sxs-lookup"><span data-stu-id="b8915-139">Example</span></span>
<span data-ttu-id="b8915-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b8915-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b8915-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8915-141">Request</span></span>
<span data-ttu-id="b8915-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8915-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b8915-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8915-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/forward
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b8915-144">C#</span><span class="sxs-lookup"><span data-stu-id="b8915-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8915-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8915-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b8915-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b8915-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b8915-147">Java</span><span class="sxs-lookup"><span data-stu-id="b8915-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b8915-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8915-148">Response</span></span>
<span data-ttu-id="b8915-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b8915-149">Here is an example of the response.</span></span>
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
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
