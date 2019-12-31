---
title: Создание Акцесспаккажересаурцеролескопе
description: Создайте новый Акцесспаккажересаурцеролескопе для добавления роли ресурса в пакет Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a05af5bb3290a17b8e732b75f771977c5126b368
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911585"
---
# <a name="create-accesspackageresourcerolescope"></a><span data-ttu-id="f0433-103">Создание Акцесспаккажересаурцеролескопе</span><span class="sxs-lookup"><span data-stu-id="f0433-103">Create accessPackageResourceRoleScope</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0433-104">Создайте новый [акцесспаккажересаурцеролескопе](../resources/accesspackageresourcerolescope.md) для добавления роли ресурса в пакет Access.</span><span class="sxs-lookup"><span data-stu-id="f0433-104">Create a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) for adding a resource role to an access package.</span></span>  <span data-ttu-id="f0433-105">Ресурс пакета Access уже должен существовать в каталоге пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="f0433-105">The access package resource must already exist in the access package catalog.</span></span>  <span data-ttu-id="f0433-106">Все последующие запросы на назначение пакетов доступа к этому пакету доступа будут включать эту роль ресурса.</span><span class="sxs-lookup"><span data-stu-id="f0433-106">Any subsequent access package assignment requests to this access package will include this resource role.</span></span>  

## <a name="permissions"></a><span data-ttu-id="f0433-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0433-107">Permissions</span></span>

<span data-ttu-id="f0433-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0433-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f0433-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0433-110">Permission type</span></span>                        | <span data-ttu-id="f0433-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0433-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f0433-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0433-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0433-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0433-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="f0433-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0433-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0433-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0433-115">Not supported.</span></span> |
| <span data-ttu-id="f0433-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0433-116">Application</span></span>                            | <span data-ttu-id="f0433-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0433-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0433-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0433-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
```

## <a name="request-headers"></a><span data-ttu-id="f0433-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0433-119">Request headers</span></span>

| <span data-ttu-id="f0433-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f0433-120">Name</span></span>          | <span data-ttu-id="f0433-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f0433-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f0433-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0433-122">Authorization</span></span> | <span data-ttu-id="f0433-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0433-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0433-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0433-125">Content-Type</span></span>  | <span data-ttu-id="f0433-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0433-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f0433-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0433-128">Request body</span></span>

<span data-ttu-id="f0433-129">В тексте запроса добавьте представление объекта [акцесспаккажересаурцеролескопе](../resources/accesspackageresourcerolescope.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0433-129">In the request body, supply a JSON representation of an [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.</span></span>  <span data-ttu-id="f0433-130">Включите в объект связи для [акцесспаккажересаурцероле](../resources/accesspackageresourcerole.md) и [акцесспаккажересаурцескопе](../resources/accesspackageresourcescope.md).</span><span class="sxs-lookup"><span data-stu-id="f0433-130">Include in the object the relationships to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) and [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span></span>  

## <a name="response"></a><span data-ttu-id="f0433-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0433-131">Response</span></span>

<span data-ttu-id="f0433-132">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажересаурцеролескопе](../resources/accesspackageresourcerolescope.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0433-132">If successful, this method returns a 200-series response code and a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0433-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="f0433-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f0433-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0433-134">Request</span></span>

<span data-ttu-id="f0433-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0433-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f0433-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0433-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f0433-137">C#</span><span class="sxs-lookup"><span data-stu-id="f0433-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerolescope-from-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f0433-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0433-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerolescope-from-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f0433-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0433-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerolescope-from-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f0433-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0433-140">Response</span></span>

<span data-ttu-id="f0433-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f0433-141">The following is an example of the response.</span></span>

> <span data-ttu-id="f0433-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f0433-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
