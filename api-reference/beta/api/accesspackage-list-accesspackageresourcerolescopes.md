---
title: Список accessPackageResourceRoleScopes
description: Извлечение списка объектов accesspackageresourcerolescope.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d2376d9eb4aaf0bd8ab58b0dd5cbbb131e36a01c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038644"
---
# <a name="list-accesspackageresourcerolescopes"></a><span data-ttu-id="b7c4e-103">Список accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="b7c4e-103">List accessPackageResourceRoleScopes</span></span>

<span data-ttu-id="b7c4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7c4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7c4e-105">Извлечение пакета доступа со списком [объектов accessPackageResourceRoleScope.](../resources/accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="b7c4e-105">Retrieve an access package with a list of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects.</span></span>  <span data-ttu-id="b7c4e-106">Каждый объект ссылок на [accessPackageResourceRole](../resources/accesspackageresourcerole.md) и [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span><span class="sxs-lookup"><span data-stu-id="b7c4e-106">Each object links to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) and an [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b7c4e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7c4e-107">Permissions</span></span>

<span data-ttu-id="b7c4e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7c4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7c4e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7c4e-110">Permission type</span></span>                        | <span data-ttu-id="b7c4e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7c4e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b7c4e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7c4e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7c4e-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7c4e-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="b7c4e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7c4e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7c4e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7c4e-115">Not supported.</span></span> |
| <span data-ttu-id="b7c4e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7c4e-116">Application</span></span>                            | <span data-ttu-id="b7c4e-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7c4e-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7c4e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7c4e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages/{id}?$expand=accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7c4e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b7c4e-119">Optional query parameters</span></span>

<span data-ttu-id="b7c4e-120">Этот метод использует параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b7c4e-120">This method uses OData query parameters to customize the response.</span></span> <span data-ttu-id="b7c4e-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b7c4e-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7c4e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7c4e-122">Request headers</span></span>

| <span data-ttu-id="b7c4e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b7c4e-123">Name</span></span>      |<span data-ttu-id="b7c4e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b7c4e-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b7c4e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7c4e-125">Authorization</span></span> | <span data-ttu-id="b7c4e-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7c4e-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7c4e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7c4e-128">Request body</span></span>

<span data-ttu-id="b7c4e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7c4e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7c4e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7c4e-130">Response</span></span>

<span data-ttu-id="b7c4e-131">В случае успеха этот метод возвращает код отклика и `200 OK` [accessPackage,](../resources/accesspackage.md) содержащий коллекцию объектов [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b7c4e-131">If successful, this method returns a `200 OK` response code and an [accessPackage](../resources/accesspackage.md) containing a collection of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7c4e-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="b7c4e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b7c4e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7c4e-133">Request</span></span>

<span data-ttu-id="b7c4e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7c4e-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b7c4e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7c4e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerolescopes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}?$expand=accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)
```
# <a name="c"></a>[<span data-ttu-id="b7c4e-136">C#</span><span class="sxs-lookup"><span data-stu-id="b7c4e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourcerolescopes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7c4e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7c4e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourcerolescopes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7c4e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7c4e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourcerolescopes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b7c4e-139">Java</span><span class="sxs-lookup"><span data-stu-id="b7c4e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourcerolescopes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b7c4e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7c4e-140">Response</span></span>

<span data-ttu-id="b7c4e-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b7c4e-141">The following is an example of the response.</span></span>

> <span data-ttu-id="b7c4e-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b7c4e-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "id": "933a4822-aed1-445b-9623-62116cd07a39",
    "catalogId": "32efb28c-9a7a-446c-986b-ca6528c6669d",
    "displayName": "Test Package 9-9",
    "description": "Test Package 9-9",
    "isHidden": false,
    "accessPackageResourceRoleScopes": [
        {
            "id": "70113acf-4dcb-453f-b517-2394598d974e_22bfd707-ab6f-404f-b0b5-a5e6f5d0ba36",
            "createdBy": "alice@contoso.com",
            "createdDateTime": "2019-09-09T19:54:14.853Z",
            "modifiedBy": "alice@contoso.com",
            "modifiedDateTime": "2019-09-09T19:54:14.853Z",
            "accessPackageResourceRole": {
                "id": "70113acf-4dcb-453f-b517-2394598d974e",
                "displayName": "Owner",
                "originSystem": "origin-type",
                "originId": "Owner_7b56ede0-9b58-40bd-b11e-b3d18fc32698"
            },
            "accessPackageResourceScope": {
                "id": "22bfd707-ab6f-404f-b0b5-a5e6f5d0ba36",
                "displayName": "Root",
                "description": "Root Scope",
                "originId": "7b56ede0-9b58-40bd-b11e-b3d18fc32698",
                "originSystem": "origin-type",
                "isRootScope": true
            }
        }
    ]
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRoleScopes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


