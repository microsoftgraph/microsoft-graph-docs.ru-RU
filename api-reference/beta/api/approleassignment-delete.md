---
title: Удаление объекта AppRoleAssignment
description: Удаление Аппролеассигнмент.
localization_priority: Normal
ms.openlocfilehash: 578780b4bd760a17269619e0a8a1f755b4f66b7a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856947"
---
# <a name="delete-approleassignment"></a><span data-ttu-id="a37cc-103">Удаление объекта AppRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a37cc-103">Delete appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a37cc-104">Удаление Аппролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="a37cc-104">Delete appRoleAssignment.</span></span>
## <a name="permissions"></a><span data-ttu-id="a37cc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a37cc-105">Permissions</span></span>
<span data-ttu-id="a37cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a37cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a37cc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a37cc-108">Permission type</span></span>      | <span data-ttu-id="a37cc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a37cc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a37cc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a37cc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a37cc-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a37cc-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a37cc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a37cc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a37cc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a37cc-113">Not supported.</span></span>    |
|<span data-ttu-id="a37cc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a37cc-114">Application</span></span> | <span data-ttu-id="a37cc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a37cc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a37cc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a37cc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/appRoleAssignments/{id}
DELETE /servicePrincipals/{id}/appRoleAssignedTo
DELETE /groups/{id}/appRoleAssignments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="a37cc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a37cc-117">Request headers</span></span>
| <span data-ttu-id="a37cc-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a37cc-118">Name</span></span>       | <span data-ttu-id="a37cc-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a37cc-119">Type</span></span> | <span data-ttu-id="a37cc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a37cc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a37cc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a37cc-121">Authorization</span></span>  | <span data-ttu-id="a37cc-122">string</span><span class="sxs-lookup"><span data-stu-id="a37cc-122">string</span></span>  | <span data-ttu-id="a37cc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a37cc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a37cc-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a37cc-125">Request body</span></span>
<span data-ttu-id="a37cc-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a37cc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a37cc-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a37cc-127">Response</span></span>

<span data-ttu-id="a37cc-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a37cc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a37cc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a37cc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a37cc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a37cc-131">Request</span></span>
<span data-ttu-id="a37cc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a37cc-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a37cc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a37cc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_approleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a37cc-134">C#</span><span class="sxs-lookup"><span data-stu-id="a37cc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a37cc-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="a37cc-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a37cc-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a37cc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a37cc-137">Java</span><span class="sxs-lookup"><span data-stu-id="a37cc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a37cc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a37cc-138">Response</span></span>
<span data-ttu-id="a37cc-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a37cc-139">Here is an example of the response.</span></span> 
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
