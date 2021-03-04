---
title: Создание accessPackageResourceRoleScope
description: Создайте новый accessPackageResourceRoleScope для добавления роли ресурса в пакет доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ffaedc45cc512b554fda3ce4dd06794fba716b16
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439811"
---
# <a name="create-accesspackageresourcerolescope"></a><span data-ttu-id="9e05d-103">Создание accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="9e05d-103">Create accessPackageResourceRoleScope</span></span>

<span data-ttu-id="9e05d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e05d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e05d-105">Создайте [новый accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) для добавления роли ресурса в пакет доступа.</span><span class="sxs-lookup"><span data-stu-id="9e05d-105">Create a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) for adding a resource role to an access package.</span></span>  <span data-ttu-id="9e05d-106">Ресурс пакета доступа уже должен существовать в каталоге пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="9e05d-106">The access package resource must already exist in the access package catalog.</span></span>  <span data-ttu-id="9e05d-107">Все последующие запросы на назначение пакета доступа к этому пакету доступа будут включать эту роль ресурса.</span><span class="sxs-lookup"><span data-stu-id="9e05d-107">Any subsequent access package assignment requests to this access package will include this resource role.</span></span>  

## <a name="permissions"></a><span data-ttu-id="9e05d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e05d-108">Permissions</span></span>

<span data-ttu-id="9e05d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e05d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e05d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e05d-111">Permission type</span></span>                        | <span data-ttu-id="9e05d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e05d-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9e05d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e05d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e05d-114">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e05d-114">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9e05d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e05d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e05d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e05d-116">Not supported.</span></span> |
| <span data-ttu-id="9e05d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9e05d-117">Application</span></span>                            | <span data-ttu-id="9e05d-118">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e05d-118">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e05d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e05d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
```

## <a name="request-headers"></a><span data-ttu-id="9e05d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e05d-120">Request headers</span></span>

| <span data-ttu-id="9e05d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9e05d-121">Name</span></span>          | <span data-ttu-id="9e05d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9e05d-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9e05d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e05d-123">Authorization</span></span> | <span data-ttu-id="9e05d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e05d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9e05d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9e05d-126">Content-Type</span></span>  | <span data-ttu-id="9e05d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e05d-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9e05d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e05d-129">Request body</span></span>

<span data-ttu-id="9e05d-130">В теле запроса устройте представление JSON объекта [accessPackageResourceRoleScope.](../resources/accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="9e05d-130">In the request body, supply a JSON representation of an [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.</span></span>  <span data-ttu-id="9e05d-131">Включив в объект связи с [accessPackageResourceRole](../resources/accesspackageresourcerole.md) и [accessPackageResourceScope.](../resources/accesspackageresourcescope.md)</span><span class="sxs-lookup"><span data-stu-id="9e05d-131">Include in the object the relationships to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) and [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span></span>  

## <a name="response"></a><span data-ttu-id="9e05d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e05d-132">Response</span></span>

<span data-ttu-id="9e05d-133">В случае успешной работы этот метод возвращает код ответа из 200 серий и новый [объект accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9e05d-133">If successful, this method returns a 200-series response code and a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e05d-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="9e05d-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9e05d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e05d-135">Request</span></span>

<span data-ttu-id="9e05d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e05d-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e05d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e05d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerolescope_from_accesspackage"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
Content-type: application/json

{
  "accessPackageResourceRole":{
    "originId":"Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca",
    "displayName":"Member",
    "originSystem":"AadGroup",
    "accessPackageResource":{"id":"1d08498d-72a1-403f-8511-6b1f875746a0","resourceType":"O365 Group","originId":"b31fe1f1-3651-488f-bd9a-1711887fd4ca","originSystem":"AadGroup"}
  },
 "accessPackageResourceScope":{
   "originId":"b31fe1f1-3651-488f-bd9a-1711887fd4ca","originSystem":"AadGroup"
 }
}
```
# <a name="c"></a>[<span data-ttu-id="9e05d-138">C#</span><span class="sxs-lookup"><span data-stu-id="9e05d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerolescope-from-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e05d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e05d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerolescope-from-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e05d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e05d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerolescope-from-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9e05d-141">Java</span><span class="sxs-lookup"><span data-stu-id="9e05d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerolescope-from-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9e05d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e05d-142">Response</span></span>

<span data-ttu-id="9e05d-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9e05d-143">The following is an example of the response.</span></span>

> <span data-ttu-id="9e05d-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9e05d-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageResourceRoleScopes/$entity",
    "id": "ad5c7636-e481-4528-991f-198e3b38dd56_ffd4004a-f4a9-4b22-b027-759e55c0d1db",
    "createdBy": "admin@example.com",
    "createdDateTime": "2019-12-11T01:35:26.4754081Z",
    "modifiedBy": "admin@example.com",
    "modifiedDateTime": "2019-12-11T01:35:26.4754081Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageResourceRoleScope",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


