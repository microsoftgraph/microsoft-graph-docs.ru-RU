---
title: Удаление groupLifecyclePolicy
description: Удаление объекта groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4d829c027c492de55dbcedc8850826e41ec13273
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888482"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="b98dc-103">Удаление groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b98dc-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="b98dc-104">Удаление объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b98dc-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b98dc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b98dc-105">Permissions</span></span>

<span data-ttu-id="b98dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b98dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b98dc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b98dc-108">Permission type</span></span>      | <span data-ttu-id="b98dc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b98dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b98dc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b98dc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b98dc-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b98dc-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="b98dc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b98dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b98dc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b98dc-113">Not supported.</span></span>    |
|<span data-ttu-id="b98dc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b98dc-114">Application</span></span> | <span data-ttu-id="b98dc-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b98dc-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b98dc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b98dc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="b98dc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b98dc-117">Request headers</span></span>

| <span data-ttu-id="b98dc-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b98dc-118">Name</span></span> | <span data-ttu-id="b98dc-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b98dc-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b98dc-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b98dc-120">Authorization</span></span> | <span data-ttu-id="b98dc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b98dc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b98dc-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b98dc-123">Content-Type</span></span>  | <span data-ttu-id="b98dc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b98dc-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b98dc-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b98dc-125">Request body</span></span>
<span data-ttu-id="b98dc-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b98dc-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b98dc-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b98dc-127">Response</span></span>

<span data-ttu-id="b98dc-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b98dc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b98dc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b98dc-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b98dc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b98dc-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b98dc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b98dc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b98dc-133">C#</span><span class="sxs-lookup"><span data-stu-id="b98dc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b98dc-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="b98dc-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b98dc-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b98dc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b98dc-136">Java</span><span class="sxs-lookup"><span data-stu-id="b98dc-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-grouplifecyclepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b98dc-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b98dc-137">Response</span></span>

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
