---
title: Удаление unifiedRoleAssignmentMultiple
description: Удаление объекта Унифиедролеассигнментмултипле.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 89c81e4dd63a892553d59f715c62620db5ae0895
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978138"
---
# <a name="delete-unifiedroleassignmentmultiple"></a><span data-ttu-id="0400d-103">Удаление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="0400d-103">Delete unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="0400d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0400d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0400d-105">Удаление объекта [унифиедролеассигнментмултипле](../resources/unifiedroleassignmentmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="0400d-105">Delete a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="0400d-106">Это относится к приложению RBAC, которое поддерживает несколько субъектов и областей.</span><span class="sxs-lookup"><span data-stu-id="0400d-106">This is applicable for a RBAC application that supports multiple principals and scopes.</span></span> <span data-ttu-id="0400d-107">Microsoft Intune это приложение.</span><span class="sxs-lookup"><span data-stu-id="0400d-107">Microsoft Intune is such an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="0400d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0400d-108">Permissions</span></span>

<span data-ttu-id="0400d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0400d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0400d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0400d-111">Permission type</span></span> | <span data-ttu-id="0400d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0400d-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="0400d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0400d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0400d-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0400d-114">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="0400d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0400d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0400d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0400d-116">Not supported.</span></span> |
| <span data-ttu-id="0400d-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="0400d-117">Application</span></span> | <span data-ttu-id="0400d-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0400d-118">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0400d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0400d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0400d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0400d-120">Request headers</span></span>

| <span data-ttu-id="0400d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0400d-121">Name</span></span> | <span data-ttu-id="0400d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0400d-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="0400d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0400d-123">Authorization</span></span> | <span data-ttu-id="0400d-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="0400d-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0400d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0400d-125">Request body</span></span>

<span data-ttu-id="0400d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0400d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0400d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0400d-127">Response</span></span>

<span data-ttu-id="0400d-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0400d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0400d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0400d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0400d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0400d-131">Request</span></span>

<span data-ttu-id="0400d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0400d-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0400d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0400d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="0400d-134">C#</span><span class="sxs-lookup"><span data-stu-id="0400d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0400d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0400d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0400d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0400d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0400d-137">Java</span><span class="sxs-lookup"><span data-stu-id="0400d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0400d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0400d-138">Response</span></span>

<span data-ttu-id="0400d-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0400d-139">The following is an example of the response.</span></span>

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


