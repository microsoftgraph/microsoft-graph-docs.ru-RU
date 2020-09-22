---
title: Удаление объекта rejectedSender
description: Удаление пользователя или группы из списка отклоненных отправителей.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2a66eb00c414a1566a98f80e957898416047a3ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002286"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="39c72-103">Удаление объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="39c72-103">Remove rejectedSender</span></span>

<span data-ttu-id="39c72-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39c72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39c72-105">Удаление пользователя или группы из списка отклоненных отправителей для указанной группы.</span><span class="sxs-lookup"><span data-stu-id="39c72-105">Remove a user or group from the rejected-senders list of the specified group.</span></span>

## <a name="permissions"></a><span data-ttu-id="39c72-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39c72-106">Permissions</span></span>
<span data-ttu-id="39c72-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39c72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39c72-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39c72-109">Permission type</span></span>                        | <span data-ttu-id="39c72-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39c72-110">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="39c72-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39c72-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="39c72-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39c72-112">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="39c72-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39c72-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39c72-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39c72-114">Not supported.</span></span> |
| <span data-ttu-id="39c72-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39c72-115">Application</span></span>                            | <span data-ttu-id="39c72-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39c72-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39c72-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39c72-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="39c72-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39c72-118">Request headers</span></span>

| <span data-ttu-id="39c72-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39c72-119">Header</span></span>         | <span data-ttu-id="39c72-120">Значение</span><span class="sxs-lookup"><span data-stu-id="39c72-120">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="39c72-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39c72-121">Authorization</span></span>  | <span data-ttu-id="39c72-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39c72-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="39c72-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="39c72-124">Request body</span></span>
<span data-ttu-id="39c72-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39c72-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39c72-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="39c72-126">Response</span></span>
<span data-ttu-id="39c72-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="39c72-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="39c72-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="39c72-129">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="39c72-130">Пример 1: Удаление пользователя из списка отклоненных отправителей группы.</span><span class="sxs-lookup"><span data-stu-id="39c72-130">Example 1: Remove a user from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="39c72-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="39c72-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="39c72-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="39c72-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="39c72-133">C#</span><span class="sxs-lookup"><span data-stu-id="39c72-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-user-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39c72-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39c72-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-user-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39c72-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39c72-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-user-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="39c72-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="39c72-136">Response</span></span>
<span data-ttu-id="39c72-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="39c72-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="39c72-138">Пример 2: Удаление группы из списка отклоненных отправителей группы.</span><span class="sxs-lookup"><span data-stu-id="39c72-138">Example 2: Remove a group from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="39c72-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="39c72-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="39c72-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="39c72-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```
# <a name="c"></a>[<span data-ttu-id="39c72-141">C#</span><span class="sxs-lookup"><span data-stu-id="39c72-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-group-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39c72-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39c72-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-group-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39c72-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39c72-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-group-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="39c72-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="39c72-144">Response</span></span>
<span data-ttu-id="39c72-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="39c72-145">The following is an example of the response.</span></span> 
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


