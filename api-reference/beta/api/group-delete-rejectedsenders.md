---
title: Удаление объекта rejectedSender
description: Удаление пользователя или группы из списка отклоненных отправителей.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 8050be767bb2950eb1ebaf6d41a4c0b7c18c1270
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440640"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="6ef6d-103">Удаление объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="6ef6d-103">Remove rejectedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ef6d-104">Удаление пользователя или группы из списка отклоненных отправителей для указанной группы.</span><span class="sxs-lookup"><span data-stu-id="6ef6d-104">Remove a user or group from the rejected-senders list of the specified group.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ef6d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ef6d-105">Permissions</span></span>
<span data-ttu-id="6ef6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ef6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6ef6d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ef6d-108">Permission type</span></span>                        | <span data-ttu-id="6ef6d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ef6d-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="6ef6d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ef6d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6ef6d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ef6d-111">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="6ef6d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ef6d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ef6d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ef6d-113">Not supported.</span></span> |
| <span data-ttu-id="6ef6d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ef6d-114">Application</span></span>                            | <span data-ttu-id="6ef6d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ef6d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ef6d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ef6d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="6ef6d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ef6d-117">Request headers</span></span>

| <span data-ttu-id="6ef6d-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ef6d-118">Header</span></span>         | <span data-ttu-id="6ef6d-119">Значение</span><span class="sxs-lookup"><span data-stu-id="6ef6d-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="6ef6d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ef6d-120">Authorization</span></span>  | <span data-ttu-id="6ef6d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ef6d-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="6ef6d-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6ef6d-123">Request body</span></span>
<span data-ttu-id="6ef6d-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ef6d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ef6d-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ef6d-125">Response</span></span>
<span data-ttu-id="6ef6d-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6ef6d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6ef6d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="6ef6d-128">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="6ef6d-129">Пример 1: Удаление пользователя из списка отклоненных отправителей группы.</span><span class="sxs-lookup"><span data-stu-id="6ef6d-129">Example 1: Remove a user from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="6ef6d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ef6d-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6ef6d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ef6d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6ef6d-132">C#</span><span class="sxs-lookup"><span data-stu-id="6ef6d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-user-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ef6d-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="6ef6d-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-user-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6ef6d-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6ef6d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-user-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6ef6d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ef6d-135">Response</span></span>
<span data-ttu-id="6ef6d-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6ef6d-136">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="6ef6d-137">Пример 2: Удаление группы из списка отклоненных отправителей группы.</span><span class="sxs-lookup"><span data-stu-id="6ef6d-137">Example 2: Remove a group from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="6ef6d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ef6d-138">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6ef6d-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ef6d-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6ef6d-140">C#</span><span class="sxs-lookup"><span data-stu-id="6ef6d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-group-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ef6d-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="6ef6d-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-group-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6ef6d-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6ef6d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-group-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6ef6d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ef6d-143">Response</span></span>
<span data-ttu-id="6ef6d-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6ef6d-144">The following is an example of the response.</span></span> 
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
