---
title: Список accessPackageAssignmentPolicies
description: Извлечение списка объектов accessPackageAssignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: be973adb399d60846282acd55f9d44d5968af7ce
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439711"
---
# <a name="list-accesspackageassignmentpolicies"></a><span data-ttu-id="19f2e-103">Список accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="19f2e-103">List accessPackageAssignmentPolicies</span></span>

<span data-ttu-id="19f2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19f2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19f2e-105">В [управлении правами Azure AD](../resources/entitlementmanagement-root.md)извлекайте список объектов [accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="19f2e-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects.</span></span> <span data-ttu-id="19f2e-106">Если делегированная пользователь находится в роли каталога, в итоговом списке содержатся все политики назначения, которые вызывающий имеет доступ к считыву, во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="19f2e-106">If the delegated user is in a directory role, the resulting list includes all the assignment policies that the caller has access to read, across all catalogs and access packages.</span></span>  <span data-ttu-id="19f2e-107">Если делегированная пользователь является менеджером пакетов доступа или владельцем каталога, он [](accesspackage-list.md) должен вместо этого получить политики для пакетов доступа, которые они могут прочитать с помощью пакетов доступа к спискам, в том числе в качестве параметра `$expand=accessPackageAssignmentPolicies` запроса.</span><span class="sxs-lookup"><span data-stu-id="19f2e-107">If the delegated user is an access package manager or catalog owner, they should instead retrieve the policies for the access packages they can read with [list accessPackages](accesspackage-list.md) by including `$expand=accessPackageAssignmentPolicies` as a query parameter.</span></span>

## <a name="permissions"></a><span data-ttu-id="19f2e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19f2e-108">Permissions</span></span>

<span data-ttu-id="19f2e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19f2e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19f2e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19f2e-111">Permission type</span></span>                        | <span data-ttu-id="19f2e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19f2e-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="19f2e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19f2e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="19f2e-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19f2e-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="19f2e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19f2e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19f2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19f2e-116">Not supported.</span></span> |
| <span data-ttu-id="19f2e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="19f2e-117">Application</span></span>                            | <span data-ttu-id="19f2e-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19f2e-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19f2e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19f2e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19f2e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="19f2e-120">Optional query parameters</span></span>

<span data-ttu-id="19f2e-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="19f2e-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="19f2e-122">Например, чтобы получить политику назначения пакета доступа с заданным именем отображения, `$filter=displayName eq 'Employee sales support'` включайте в запрос.</span><span class="sxs-lookup"><span data-stu-id="19f2e-122">For example, to retrieve an access package assignment policy with a specified display name, include `$filter=displayName eq 'Employee sales support'` in the query.</span></span> <span data-ttu-id="19f2e-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="19f2e-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="19f2e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19f2e-124">Request headers</span></span>

| <span data-ttu-id="19f2e-125">Имя</span><span class="sxs-lookup"><span data-stu-id="19f2e-125">Name</span></span>      |<span data-ttu-id="19f2e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="19f2e-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="19f2e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="19f2e-127">Authorization</span></span> | <span data-ttu-id="19f2e-128">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="19f2e-128">Bearer \{token\}.</span></span> <span data-ttu-id="19f2e-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="19f2e-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19f2e-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19f2e-130">Request body</span></span>

<span data-ttu-id="19f2e-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19f2e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19f2e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="19f2e-132">Response</span></span>

<span data-ttu-id="19f2e-133">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="19f2e-133">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19f2e-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="19f2e-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="19f2e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="19f2e-135">Request</span></span>

<span data-ttu-id="19f2e-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19f2e-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="19f2e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="19f2e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```
# <a name="c"></a>[<span data-ttu-id="19f2e-138">C#</span><span class="sxs-lookup"><span data-stu-id="19f2e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19f2e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19f2e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19f2e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19f2e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="19f2e-141">Java</span><span class="sxs-lookup"><span data-stu-id="19f2e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="19f2e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="19f2e-142">Response</span></span>

<span data-ttu-id="19f2e-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="19f2e-143">The following is an example of the response.</span></span>

> <span data-ttu-id="19f2e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19f2e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
      "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
      "displayName": "All Users",
      "description": "All users can request for access to the directory.",
      "canExtend": false,
      "durationInDays": 365,
      "accessReviewSettings": null
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


