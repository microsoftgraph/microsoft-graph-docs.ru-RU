---
title: Удаление объекта rejectedSender
description: Удалите пользователя или группу из списка отклоненных отправителей.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 14bdcef8d41d204e3c3ae6f3de08a3d1cc53a5ff
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681856"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="5698d-103">Удаление объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="5698d-103">Remove rejectedSender</span></span>

<span data-ttu-id="5698d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5698d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5698d-105">Удалите пользователя или группу из списка отклоненных отправителей указанной группы.</span><span class="sxs-lookup"><span data-stu-id="5698d-105">Remove a user or group from the rejected-senders list of the specified group.</span></span>

## <a name="permissions"></a><span data-ttu-id="5698d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5698d-106">Permissions</span></span>
<span data-ttu-id="5698d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5698d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5698d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5698d-109">Permission type</span></span>                        | <span data-ttu-id="5698d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5698d-110">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="5698d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5698d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5698d-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5698d-112">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="5698d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5698d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5698d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5698d-114">Not supported.</span></span> |
| <span data-ttu-id="5698d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5698d-115">Application</span></span>                            | <span data-ttu-id="5698d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5698d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5698d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5698d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="5698d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5698d-118">Request headers</span></span>

| <span data-ttu-id="5698d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5698d-119">Header</span></span>         | <span data-ttu-id="5698d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5698d-120">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="5698d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5698d-121">Authorization</span></span>  | <span data-ttu-id="5698d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5698d-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="5698d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5698d-124">Request body</span></span>
<span data-ttu-id="5698d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5698d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5698d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5698d-126">Response</span></span>
<span data-ttu-id="5698d-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5698d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5698d-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="5698d-129">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="5698d-130">Пример 1. Удаление пользователя из списка отклоненных отправителей группы.</span><span class="sxs-lookup"><span data-stu-id="5698d-130">Example 1: Remove a user from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="5698d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5698d-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5698d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5698d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="5698d-133">C#</span><span class="sxs-lookup"><span data-stu-id="5698d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-user-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5698d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5698d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-user-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5698d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5698d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-user-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5698d-136">Java</span><span class="sxs-lookup"><span data-stu-id="5698d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-user-from-rejectedsenderslist-of-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5698d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5698d-137">Response</span></span>
<span data-ttu-id="5698d-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5698d-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="5698d-139">Пример 2. Удаление группы из списка отклоненных отправителей группы.</span><span class="sxs-lookup"><span data-stu-id="5698d-139">Example 2: Remove a group from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="5698d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="5698d-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5698d-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="5698d-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```
# <a name="c"></a>[<span data-ttu-id="5698d-142">C#</span><span class="sxs-lookup"><span data-stu-id="5698d-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-group-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5698d-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5698d-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-group-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5698d-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5698d-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-group-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5698d-145">Java</span><span class="sxs-lookup"><span data-stu-id="5698d-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-group-from-rejectedsenderslist-of-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5698d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="5698d-146">Response</span></span>
<span data-ttu-id="5698d-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5698d-147">The following is an example of the response.</span></span> 
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


