---
title: Удаление объекта rejectedSender
description: Удаление пользователя или группы из списка отклоненных отправителей.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a43b4876b73b33693f8c3d49102b02f5a468bb8f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323523"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="9aa53-103">Удаление объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="9aa53-103">Remove rejectedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9aa53-104">Удаление пользователя или группы из списка отклоненных отправителей для указанной группы.</span><span class="sxs-lookup"><span data-stu-id="9aa53-104">Remove a user or group from the rejected-senders list of the specified group.</span></span>

## <a name="permissions"></a><span data-ttu-id="9aa53-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9aa53-105">Permissions</span></span>
<span data-ttu-id="9aa53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9aa53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9aa53-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9aa53-108">Permission type</span></span>                        | <span data-ttu-id="9aa53-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9aa53-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="9aa53-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9aa53-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9aa53-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9aa53-111">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="9aa53-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9aa53-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9aa53-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9aa53-113">Not supported.</span></span> |
| <span data-ttu-id="9aa53-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9aa53-114">Application</span></span>                            | <span data-ttu-id="9aa53-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9aa53-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9aa53-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9aa53-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="9aa53-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9aa53-117">Request headers</span></span>

| <span data-ttu-id="9aa53-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9aa53-118">Header</span></span>         | <span data-ttu-id="9aa53-119">Значение</span><span class="sxs-lookup"><span data-stu-id="9aa53-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="9aa53-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9aa53-120">Authorization</span></span>  | <span data-ttu-id="9aa53-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9aa53-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="9aa53-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9aa53-123">Request body</span></span>
<span data-ttu-id="9aa53-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9aa53-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9aa53-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="9aa53-125">Response</span></span>
<span data-ttu-id="9aa53-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9aa53-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9aa53-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="9aa53-128">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="9aa53-129">Пример 1: Удаление пользователя из списка отклоненных отправителей группы.</span><span class="sxs-lookup"><span data-stu-id="9aa53-129">Example 1: Remove a user from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="9aa53-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9aa53-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9aa53-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9aa53-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9aa53-132">C#</span><span class="sxs-lookup"><span data-stu-id="9aa53-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-user-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9aa53-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9aa53-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-user-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9aa53-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9aa53-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-user-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9aa53-135">Java</span><span class="sxs-lookup"><span data-stu-id="9aa53-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-user-from-rejectedsenderslist-of-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9aa53-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9aa53-136">Response</span></span>
<span data-ttu-id="9aa53-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9aa53-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="9aa53-138">Пример 2: Удаление группы из списка отклоненных отправителей группы.</span><span class="sxs-lookup"><span data-stu-id="9aa53-138">Example 2: Remove a group from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="9aa53-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9aa53-139">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9aa53-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="9aa53-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9aa53-141">C#</span><span class="sxs-lookup"><span data-stu-id="9aa53-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-group-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9aa53-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9aa53-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-group-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9aa53-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9aa53-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-group-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9aa53-144">Java</span><span class="sxs-lookup"><span data-stu-id="9aa53-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-group-from-rejectedsenderslist-of-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9aa53-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9aa53-145">Response</span></span>
<span data-ttu-id="9aa53-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9aa53-146">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
