---
title: Список accessPackageResourceRoles
description: Извлечение списка объектов accessPackageResourceRole.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 29e83c3254cfa4931f3faeb869d6312335565019
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048570"
---
# <a name="list-accesspackageresourceroles"></a><span data-ttu-id="ed706-103">Список accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="ed706-103">List accessPackageResourceRoles</span></span>

<span data-ttu-id="ed706-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed706-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed706-105">Извлечение списка [объектов accessPackageResourceRole](../resources/accesspackageresourcerole.md) [accessPackageResource](../resources/accesspackageresource.md) в [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="ed706-105">Retrieve a list of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects of an [accessPackageResource](../resources/accesspackageresource.md) in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="ed706-106">Этот список ролей может быть использован звонивцом для выбора роли, которая необходима при создании [accessPackageResourceRoleScope.](accesspackage-post-accesspackageresourcerolescopes.md)</span><span class="sxs-lookup"><span data-stu-id="ed706-106">This list of roles can then be used by the caller to select a role, which is needed when subsequently [creating an accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed706-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed706-107">Permissions</span></span>

<span data-ttu-id="ed706-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed706-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed706-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed706-110">Permission type</span></span>                        | <span data-ttu-id="ed706-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed706-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ed706-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed706-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed706-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed706-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ed706-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed706-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed706-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed706-115">Not supported.</span></span> |
| <span data-ttu-id="ed706-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ed706-116">Application</span></span>                            | <span data-ttu-id="ed706-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed706-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed706-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed706-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{catalogId}/accessPackageResourceRoles?$filter=(originSystem+eq+%27{originSystemType}%27+and+accessPackageResource/id+eq+%27{resourceId}%27)&$expand=accessPackageResource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed706-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ed706-119">Optional query parameters</span></span>

<span data-ttu-id="ed706-120">Этот метод использует параметры запроса OData для построения ответа.</span><span class="sxs-lookup"><span data-stu-id="ed706-120">This method uses OData query parameters to construct the response.</span></span> <span data-ttu-id="ed706-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ed706-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed706-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed706-122">Request headers</span></span>

| <span data-ttu-id="ed706-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ed706-123">Name</span></span>      |<span data-ttu-id="ed706-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ed706-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ed706-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ed706-125">Authorization</span></span> | <span data-ttu-id="ed706-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed706-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed706-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed706-128">Request body</span></span>

<span data-ttu-id="ed706-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ed706-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed706-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed706-130">Response</span></span>

<span data-ttu-id="ed706-131">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [accessPackageResourceRole](../resources/accesspackageresourcerole.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ed706-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed706-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="ed706-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed706-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed706-133">Request</span></span>

<span data-ttu-id="ed706-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed706-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ed706-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed706-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/15d889df-3eb8-4e9b-bfb4-b1908849aec4/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%27a35bef72-a8aa-4ca3-af30-f6b2ece7208f%27)&$expand=accessPackageResource
```
# <a name="c"></a>[<span data-ttu-id="ed706-136">C#</span><span class="sxs-lookup"><span data-stu-id="ed706-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed706-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed706-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed706-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed706-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed706-139">Java</span><span class="sxs-lookup"><span data-stu-id="ed706-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourceroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ed706-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed706-140">Response</span></span>

<span data-ttu-id="ed706-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ed706-141">The following is an example of the response.</span></span>

> <span data-ttu-id="ed706-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ed706-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "displayName": "Member",
      "description": "description-value",
      "originId": "originId-value",
      "originSystem": "originSystem-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


