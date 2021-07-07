---
title: Удаление unifiedRoleAssignment
description: Удаление объекта unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 96bff141cc3f4dfb779335100a49a8fdf99edb00
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317072"
---
# <a name="delete-unifiedroleassignment"></a><span data-ttu-id="81bb3-103">Удаление unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="81bb3-103">Delete unifiedRoleAssignment</span></span>

<span data-ttu-id="81bb3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81bb3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81bb3-105">Удаление [объекта unifiedRoleAssignment.](../resources/unifiedRoleAssignment.md)</span><span class="sxs-lookup"><span data-stu-id="81bb3-105">Delete a [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="81bb3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81bb3-106">Permissions</span></span>

<span data-ttu-id="81bb3-107">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="81bb3-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="81bb3-108">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81bb3-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81bb3-109">Поддерживаемый поставщик</span><span class="sxs-lookup"><span data-stu-id="81bb3-109">Supported provider</span></span>      | <span data-ttu-id="81bb3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81bb3-110">Delegated (work or school account)</span></span>  | <span data-ttu-id="81bb3-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81bb3-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81bb3-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81bb3-112">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="81bb3-113">Каталог</span><span class="sxs-lookup"><span data-stu-id="81bb3-113">Directory</span></span> | <span data-ttu-id="81bb3-114">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="81bb3-114">RoleManagement.ReadWrite.Directory</span></span> | <span data-ttu-id="81bb3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81bb3-115">Not supported.</span></span>| <span data-ttu-id="81bb3-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="81bb3-116">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="81bb3-117">Управление правами</span><span class="sxs-lookup"><span data-stu-id="81bb3-117">Entitlement management</span></span> | <span data-ttu-id="81bb3-118">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81bb3-118">EntitlementManagement.ReadWrite.All</span></span> | <span data-ttu-id="81bb3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81bb3-119">Not supported.</span></span> | <span data-ttu-id="81bb3-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81bb3-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81bb3-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81bb3-121">HTTP request</span></span>

<span data-ttu-id="81bb3-122">Удаление назначения ролей у поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="81bb3-122">Remove a role assignment from a directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleAssignments/{id}
```

<span data-ttu-id="81bb3-123">Удаление назначения роли у поставщика управления правами:</span><span class="sxs-lookup"><span data-stu-id="81bb3-123">Remove a role assignment from the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/entitlementManagement/roleAssignments/{id}
```


## <a name="request-headers"></a><span data-ttu-id="81bb3-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81bb3-124">Request headers</span></span>

| <span data-ttu-id="81bb3-125">Имя</span><span class="sxs-lookup"><span data-stu-id="81bb3-125">Name</span></span>          | <span data-ttu-id="81bb3-126">Описание</span><span class="sxs-lookup"><span data-stu-id="81bb3-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="81bb3-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81bb3-127">Authorization</span></span> | <span data-ttu-id="81bb3-128">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="81bb3-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="81bb3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81bb3-129">Request body</span></span>

<span data-ttu-id="81bb3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81bb3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81bb3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="81bb3-131">Response</span></span>

<span data-ttu-id="81bb3-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="81bb3-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81bb3-134">Пример</span><span class="sxs-lookup"><span data-stu-id="81bb3-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="81bb3-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="81bb3-135">Request</span></span>

<span data-ttu-id="81bb3-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81bb3-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="81bb3-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="81bb3-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="81bb3-138">C#</span><span class="sxs-lookup"><span data-stu-id="81bb3-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81bb3-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81bb3-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81bb3-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81bb3-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81bb3-141">Java</span><span class="sxs-lookup"><span data-stu-id="81bb3-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="81bb3-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="81bb3-142">Response</span></span>

<span data-ttu-id="81bb3-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="81bb3-143">The following is an example of the response.</span></span>

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


