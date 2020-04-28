---
title: Удаление объекта AppRoleAssignment
description: Удаление Аппролеассигнмент.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 9a8c0d6f2ff76e8c95190cce52cecd8c19fd6b8a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441391"
---
# <a name="delete-approleassignment"></a><span data-ttu-id="788fb-103">Удаление объекта AppRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="788fb-103">Delete appRoleAssignment</span></span>

<span data-ttu-id="788fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="788fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="788fb-105">Удаление Аппролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="788fb-105">Delete appRoleAssignment.</span></span>
## <a name="permissions"></a><span data-ttu-id="788fb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="788fb-106">Permissions</span></span>
<span data-ttu-id="788fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="788fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="788fb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="788fb-109">Permission type</span></span>      | <span data-ttu-id="788fb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="788fb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="788fb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="788fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="788fb-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="788fb-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="788fb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="788fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="788fb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="788fb-114">Not supported.</span></span>    |
|<span data-ttu-id="788fb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="788fb-115">Application</span></span> | <span data-ttu-id="788fb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="788fb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="788fb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="788fb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/appRoleAssignments/{id}
DELETE /groups/{id}/appRoleAssignments/{id}
DELETE /servicePrincipals/{id}/appRoleAssignments/{id}
DELETE /servicePrincipals/{id}/appRoleAssignedTo/{id}

```
## <a name="request-headers"></a><span data-ttu-id="788fb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="788fb-118">Request headers</span></span>
| <span data-ttu-id="788fb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="788fb-119">Name</span></span>       | <span data-ttu-id="788fb-120">Тип</span><span class="sxs-lookup"><span data-stu-id="788fb-120">Type</span></span> | <span data-ttu-id="788fb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="788fb-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="788fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="788fb-122">Authorization</span></span>  | <span data-ttu-id="788fb-123">string</span><span class="sxs-lookup"><span data-stu-id="788fb-123">string</span></span>  | <span data-ttu-id="788fb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="788fb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="788fb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="788fb-126">Request body</span></span>
<span data-ttu-id="788fb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="788fb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="788fb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="788fb-128">Response</span></span>

<span data-ttu-id="788fb-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="788fb-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="788fb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="788fb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="788fb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="788fb-132">Request</span></span>
<span data-ttu-id="788fb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="788fb-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="788fb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="788fb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_approleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignedTo/{id}
```
# <a name="c"></a>[<span data-ttu-id="788fb-135">C#</span><span class="sxs-lookup"><span data-stu-id="788fb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="788fb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="788fb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="788fb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="788fb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="788fb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="788fb-138">Response</span></span>
<span data-ttu-id="788fb-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="788fb-139">Here is an example of the response.</span></span> 
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
  "description": "Delete appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
