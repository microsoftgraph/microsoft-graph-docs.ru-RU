---
title: Удаление Унифиедролеассигнмент
description: Удаление объекта Унифиедролеассигнмент.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f11d0017c9dc7ac403f40ee8e913b489bf3969e7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978164"
---
# <a name="delete-unifiedroleassignment"></a><span data-ttu-id="d244f-103">Удаление Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="d244f-103">Delete unifiedRoleAssignment</span></span>

<span data-ttu-id="d244f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d244f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d244f-105">Удаление объекта [унифиедролеассигнмент](../resources/unifiedRoleAssignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d244f-105">Delete a [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d244f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d244f-106">Permissions</span></span>

<span data-ttu-id="d244f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d244f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d244f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d244f-109">Permission type</span></span>                        | <span data-ttu-id="d244f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d244f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d244f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d244f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d244f-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="d244f-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="d244f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d244f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d244f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d244f-114">Not supported.</span></span> |
| <span data-ttu-id="d244f-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d244f-115">Application</span></span>                            | <span data-ttu-id="d244f-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="d244f-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="d244f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d244f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d244f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d244f-118">Request headers</span></span>

| <span data-ttu-id="d244f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d244f-119">Name</span></span>          | <span data-ttu-id="d244f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d244f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d244f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d244f-121">Authorization</span></span> | <span data-ttu-id="d244f-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="d244f-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d244f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d244f-123">Request body</span></span>

<span data-ttu-id="d244f-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d244f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d244f-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="d244f-125">Response</span></span>

<span data-ttu-id="d244f-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d244f-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d244f-128">Пример</span><span class="sxs-lookup"><span data-stu-id="d244f-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="d244f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d244f-129">Request</span></span>

<span data-ttu-id="d244f-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d244f-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d244f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="d244f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="d244f-132">C#</span><span class="sxs-lookup"><span data-stu-id="d244f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d244f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d244f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d244f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d244f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d244f-135">Java</span><span class="sxs-lookup"><span data-stu-id="d244f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d244f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d244f-136">Response</span></span>

<span data-ttu-id="d244f-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d244f-137">The following is an example of the response.</span></span>

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


