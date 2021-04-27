---
title: Список accessPackageAssignmentPolicies
description: Извлечение списка объектов accessPackageAssignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e6c6d3bf4706dcac398cef182cf692aee511f07b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048633"
---
# <a name="list-accesspackageassignmentpolicies"></a><span data-ttu-id="009f4-103">Список accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="009f4-103">List accessPackageAssignmentPolicies</span></span>

<span data-ttu-id="009f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="009f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="009f4-105">В [управлении правами Azure AD](../resources/entitlementmanagement-root.md)извлекайте список объектов [accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="009f4-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects.</span></span> <span data-ttu-id="009f4-106">Если делегированная пользователь находится в роли каталога, в итоговом списке содержатся все политики назначения, которые вызывающий имеет доступ к считыву, во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="009f4-106">If the delegated user is in a directory role, the resulting list includes all the assignment policies that the caller has access to read, across all catalogs and access packages.</span></span>  <span data-ttu-id="009f4-107">Если делегированная пользователь является менеджером пакетов доступа или владельцем каталога, он [](accesspackage-list.md) должен вместо этого получить политики для пакетов доступа, которые они могут прочитать с помощью пакетов доступа к спискам, в том числе в качестве параметра `$expand=accessPackageAssignmentPolicies` запроса.</span><span class="sxs-lookup"><span data-stu-id="009f4-107">If the delegated user is an access package manager or catalog owner, they should instead retrieve the policies for the access packages they can read with [list accessPackages](accesspackage-list.md) by including `$expand=accessPackageAssignmentPolicies` as a query parameter.</span></span>

## <a name="permissions"></a><span data-ttu-id="009f4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="009f4-108">Permissions</span></span>

<span data-ttu-id="009f4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="009f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="009f4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="009f4-111">Permission type</span></span>                        | <span data-ttu-id="009f4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="009f4-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="009f4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="009f4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="009f4-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="009f4-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="009f4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="009f4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="009f4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="009f4-116">Not supported.</span></span> |
| <span data-ttu-id="009f4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="009f4-117">Application</span></span>                            | <span data-ttu-id="009f4-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="009f4-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="009f4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="009f4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="009f4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="009f4-120">Optional query parameters</span></span>

<span data-ttu-id="009f4-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="009f4-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="009f4-122">Например, чтобы получить политику назначения пакета доступа с заданным именем отображения, `$filter=displayName eq 'Employee sales support'` включайте в запрос.</span><span class="sxs-lookup"><span data-stu-id="009f4-122">For example, to retrieve an access package assignment policy with a specified display name, include `$filter=displayName eq 'Employee sales support'` in the query.</span></span> <span data-ttu-id="009f4-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="009f4-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="009f4-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="009f4-124">Request headers</span></span>

| <span data-ttu-id="009f4-125">Имя</span><span class="sxs-lookup"><span data-stu-id="009f4-125">Name</span></span>      |<span data-ttu-id="009f4-126">Описание</span><span class="sxs-lookup"><span data-stu-id="009f4-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="009f4-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="009f4-127">Authorization</span></span> | <span data-ttu-id="009f4-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="009f4-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="009f4-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="009f4-130">Request body</span></span>

<span data-ttu-id="009f4-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="009f4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="009f4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="009f4-132">Response</span></span>

<span data-ttu-id="009f4-133">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="009f4-133">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="009f4-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="009f4-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="009f4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="009f4-135">Request</span></span>

<span data-ttu-id="009f4-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="009f4-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="009f4-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="009f4-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```
# <a name="c"></a>[<span data-ttu-id="009f4-138">C#</span><span class="sxs-lookup"><span data-stu-id="009f4-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="009f4-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="009f4-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="009f4-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="009f4-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="009f4-141">Java</span><span class="sxs-lookup"><span data-stu-id="009f4-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="009f4-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="009f4-142">Response</span></span>

<span data-ttu-id="009f4-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="009f4-143">The following is an example of the response.</span></span>

> <span data-ttu-id="009f4-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="009f4-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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


