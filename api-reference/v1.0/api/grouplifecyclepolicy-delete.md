---
title: Удаление groupLifecyclePolicy
description: Удаление объекта groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a8d73413c07eb00e45f266facf27cd1fe3c87400
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516888"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="320f7-103">Удаление groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="320f7-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="320f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="320f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="320f7-105">Удаление объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="320f7-105">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="320f7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="320f7-106">Permissions</span></span>

<span data-ttu-id="320f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="320f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="320f7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="320f7-109">Permission type</span></span>      | <span data-ttu-id="320f7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="320f7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="320f7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="320f7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="320f7-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="320f7-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="320f7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="320f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="320f7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="320f7-114">Not supported.</span></span>    |
|<span data-ttu-id="320f7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="320f7-115">Application</span></span> | <span data-ttu-id="320f7-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="320f7-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="320f7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="320f7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="320f7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="320f7-118">Request headers</span></span>

| <span data-ttu-id="320f7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="320f7-119">Name</span></span> | <span data-ttu-id="320f7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="320f7-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="320f7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="320f7-121">Authorization</span></span> | <span data-ttu-id="320f7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="320f7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="320f7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="320f7-124">Content-Type</span></span>  | <span data-ttu-id="320f7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="320f7-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="320f7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="320f7-126">Request body</span></span>
<span data-ttu-id="320f7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="320f7-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="320f7-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="320f7-128">Response</span></span>

<span data-ttu-id="320f7-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="320f7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="320f7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="320f7-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="320f7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="320f7-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="320f7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="320f7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="320f7-134">C#</span><span class="sxs-lookup"><span data-stu-id="320f7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="320f7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="320f7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="320f7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="320f7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="320f7-137">Java</span><span class="sxs-lookup"><span data-stu-id="320f7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-grouplifecyclepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="320f7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="320f7-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
