---
title: Список accessPackageAssignmentRequests
description: Извлечение списка объектов accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d5ce1ca824f104de9058be4ed748d5b87a731e71
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53466938"
---
# <a name="list-accesspackageassignmentrequests"></a><span data-ttu-id="f3509-103">Список accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="f3509-103">List accessPackageAssignmentRequests</span></span>

<span data-ttu-id="f3509-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3509-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3509-105">В [управлении правами Azure AD](../resources/entitlementmanagement-root.md)извлекайте список объектов [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f3509-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.</span></span>  <span data-ttu-id="f3509-106">В итоговом списке содержатся все запросы на назначение, текущие и просроченные, которые вызываемая имеет доступ к считывке во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="f3509-106">The resulting list includes all the assignment requests, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3509-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3509-107">Permissions</span></span>

<span data-ttu-id="f3509-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3509-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f3509-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3509-110">Permission type</span></span>                        | <span data-ttu-id="f3509-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3509-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f3509-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3509-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f3509-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3509-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="f3509-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3509-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3509-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3509-115">Not supported.</span></span> |
| <span data-ttu-id="f3509-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f3509-116">Application</span></span>                            | <span data-ttu-id="f3509-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3509-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3509-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3509-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3509-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f3509-119">Optional query parameters</span></span>

<span data-ttu-id="f3509-120">Этот метод поддерживает параметры `$expand` `$filter` запроса oData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f3509-120">This method supports the `$expand` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="f3509-121">Например, чтобы получить пакет доступа каждого запроса, включайте `$expand=accessPackage` в запрос.</span><span class="sxs-lookup"><span data-stu-id="f3509-121">For example, to retrieve the access package of each request, include `$expand=accessPackage` in the query.</span></span>  <span data-ttu-id="f3509-122">Чтобы получить только запросы для определенного пакета доступа, включайте в запрос фильтр, например `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'` .</span><span class="sxs-lookup"><span data-stu-id="f3509-122">To retrieve only requests for a specific access package, include in the query a filter such as `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'`.</span></span>  <span data-ttu-id="f3509-123">Чтобы получить результат назначения, включайте `$expand=accessPackageAssignment` запрос.</span><span class="sxs-lookup"><span data-stu-id="f3509-123">To retrieve the resulting assignment, include `$expand=accessPackageAssignment` in the query.</span></span>  <span data-ttu-id="f3509-124">Дополнительные сведения о запрашиваемом запросе `$expand=requestor` включайте в запрос.</span><span class="sxs-lookup"><span data-stu-id="f3509-124">To obtain more details on the requestor, include `$expand=requestor` in the query.</span></span>
<span data-ttu-id="f3509-125">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f3509-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3509-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3509-126">Request headers</span></span>

| <span data-ttu-id="f3509-127">Имя</span><span class="sxs-lookup"><span data-stu-id="f3509-127">Name</span></span>      |<span data-ttu-id="f3509-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f3509-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f3509-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3509-129">Authorization</span></span> | <span data-ttu-id="f3509-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3509-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3509-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3509-132">Request body</span></span>

<span data-ttu-id="f3509-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3509-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3509-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3509-134">Response</span></span>

<span data-ttu-id="f3509-135">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f3509-135">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f3509-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="f3509-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f3509-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3509-137">Request</span></span>

<span data-ttu-id="f3509-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3509-138">The following is an example of the request.</span></span> <span data-ttu-id="f3509-139">URI запроса включает только возврат запросов в определенном состоянии, а также возвращение сведений о запрашиваемом и связанной с ним `$filter` `$expand` организации.</span><span class="sxs-lookup"><span data-stu-id="f3509-139">The request URI includes `$filter` to only return requests in a particular state, and `$expand` to return details of the requestor and their connected organization as well.</span></span>

# <a name="http"></a>[<span data-ttu-id="f3509-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3509-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests?$expand=requestor($expand=connectedOrganization)&$filter=(requestState eq 'PendingApproval')
```
# <a name="c"></a>[<span data-ttu-id="f3509-141">C#</span><span class="sxs-lookup"><span data-stu-id="f3509-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f3509-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3509-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f3509-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f3509-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f3509-144">Java</span><span class="sxs-lookup"><span data-stu-id="f3509-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f3509-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3509-145">Response</span></span>

<span data-ttu-id="f3509-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f3509-146">The following is an example of the response.</span></span>

> <span data-ttu-id="f3509-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f3509-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "433dafca-5047-4614-95f7-a03510b1ded3",
      "requestType": "UserAdd",
      "requestState": "PendingApproval",
      "createdDateTime": "2019-10-25T22:55:11.623Z",
      "justification": "Need access",
      "answers": [],
      "requestor": {
        "connectedOrganizationId": "c3c2adbc-a863-437f-9383-ee578665317d",
        "id": "ba7ef0fb-e16f-474b-87aa-02815d061e67",
        "displayName": "displayname",
        "email": "displayname@example.com",
        "type": "User",
        "connectedOrganization": {
          "id": "c3c2adbc-a863-437f-9383-ee578665317d",
          "displayName": "example"
        }
      }
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

