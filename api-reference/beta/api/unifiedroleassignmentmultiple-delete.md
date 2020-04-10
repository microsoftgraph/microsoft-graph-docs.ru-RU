---
title: Удаление unifiedRoleAssignmentMultiple
description: Удаление объекта Унифиедролеассигнментмултипле.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f4df58deab010d6cb7b5374210ebde1aad2eb6d2
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218985"
---
# <a name="delete-unifiedroleassignmentmultiple"></a><span data-ttu-id="55162-103">Удаление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="55162-103">Delete unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="55162-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55162-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55162-105">Удаление объекта [унифиедролеассигнментмултипле](../resources/unifiedroleassignmentmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="55162-105">Delete a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="55162-106">Это относится к приложению RBAC, которое поддерживает несколько субъектов и областей.</span><span class="sxs-lookup"><span data-stu-id="55162-106">This is applicable for a RBAC application that supports multiple principals and scopes.</span></span> <span data-ttu-id="55162-107">Microsoft Intune это приложение.</span><span class="sxs-lookup"><span data-stu-id="55162-107">Microsoft Intune is such an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="55162-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55162-108">Permissions</span></span>

<span data-ttu-id="55162-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55162-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55162-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55162-111">Permission type</span></span> | <span data-ttu-id="55162-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55162-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="55162-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55162-113">Delegated (work or school account)</span></span> | <span data-ttu-id="55162-114">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="55162-114">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="55162-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55162-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55162-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55162-116">Not supported.</span></span> |
| <span data-ttu-id="55162-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55162-117">Application</span></span> | <span data-ttu-id="55162-118">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="55162-118">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="55162-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55162-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="55162-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55162-120">Request headers</span></span>

| <span data-ttu-id="55162-121">Имя</span><span class="sxs-lookup"><span data-stu-id="55162-121">Name</span></span> | <span data-ttu-id="55162-122">Описание</span><span class="sxs-lookup"><span data-stu-id="55162-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="55162-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55162-123">Authorization</span></span> | <span data-ttu-id="55162-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="55162-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="55162-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55162-125">Request body</span></span>

<span data-ttu-id="55162-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55162-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55162-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="55162-127">Response</span></span>

<span data-ttu-id="55162-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="55162-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55162-130">Пример</span><span class="sxs-lookup"><span data-stu-id="55162-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="55162-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="55162-131">Request</span></span>

<span data-ttu-id="55162-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55162-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="55162-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="55162-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="55162-134">C#</span><span class="sxs-lookup"><span data-stu-id="55162-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55162-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55162-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55162-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55162-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="55162-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="55162-137">Response</span></span>

<span data-ttu-id="55162-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="55162-138">The following is an example of the response.</span></span>

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
  "description": "Delete unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
