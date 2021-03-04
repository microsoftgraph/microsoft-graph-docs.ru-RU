---
title: Удаление unifiedRoleAssignment
description: Удаление объекта unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 865d18f0278084ecf884ead909374eeccaaace54
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444891"
---
# <a name="delete-unifiedroleassignment"></a><span data-ttu-id="a28eb-103">Удаление unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a28eb-103">Delete unifiedRoleAssignment</span></span>

<span data-ttu-id="a28eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a28eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a28eb-105">Удаление [объекта unifiedRoleAssignment.](../resources/unifiedRoleAssignment.md)</span><span class="sxs-lookup"><span data-stu-id="a28eb-105">Delete a [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a28eb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a28eb-106">Permissions</span></span>

<span data-ttu-id="a28eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a28eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a28eb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a28eb-109">Permission type</span></span>                        | <span data-ttu-id="a28eb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a28eb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a28eb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a28eb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a28eb-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="a28eb-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="a28eb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a28eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a28eb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a28eb-114">Not supported.</span></span> |
| <span data-ttu-id="a28eb-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a28eb-115">Application</span></span>                            | <span data-ttu-id="a28eb-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="a28eb-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="a28eb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a28eb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a28eb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a28eb-118">Request headers</span></span>

| <span data-ttu-id="a28eb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a28eb-119">Name</span></span>          | <span data-ttu-id="a28eb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a28eb-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a28eb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a28eb-121">Authorization</span></span> | <span data-ttu-id="a28eb-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a28eb-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a28eb-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a28eb-123">Request body</span></span>

<span data-ttu-id="a28eb-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a28eb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a28eb-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a28eb-125">Response</span></span>

<span data-ttu-id="a28eb-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a28eb-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a28eb-128">Пример</span><span class="sxs-lookup"><span data-stu-id="a28eb-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="a28eb-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a28eb-129">Request</span></span>

<span data-ttu-id="a28eb-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a28eb-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a28eb-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="a28eb-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="a28eb-132">C#</span><span class="sxs-lookup"><span data-stu-id="a28eb-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a28eb-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a28eb-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a28eb-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a28eb-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a28eb-135">Java</span><span class="sxs-lookup"><span data-stu-id="a28eb-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a28eb-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a28eb-136">Response</span></span>

<span data-ttu-id="a28eb-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a28eb-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


