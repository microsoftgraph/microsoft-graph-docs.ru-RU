---
title: Список accessPackageAssignmentRequests
description: Извлечение списка объектов accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a455b4ecddbc264446ffbb8909b06b0f3b66997f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439686"
---
# <a name="list-accesspackageassignmentrequests"></a><span data-ttu-id="51de1-103">Список accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="51de1-103">List accessPackageAssignmentRequests</span></span>

<span data-ttu-id="51de1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51de1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51de1-105">В [управлении правами Azure AD](../resources/entitlementmanagement-root.md)извлекайте список объектов [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="51de1-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.</span></span>  <span data-ttu-id="51de1-106">В итоговом списке содержатся все запросы на назначение, текущие и просроченные, которые вызываемая имеет доступ к считывке во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="51de1-106">The resulting list includes all the assignment requests, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="51de1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51de1-107">Permissions</span></span>

<span data-ttu-id="51de1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51de1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51de1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51de1-110">Permission type</span></span>                        | <span data-ttu-id="51de1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51de1-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="51de1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51de1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="51de1-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51de1-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="51de1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51de1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51de1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51de1-115">Not supported.</span></span> |
| <span data-ttu-id="51de1-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="51de1-116">Application</span></span>                            | <span data-ttu-id="51de1-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51de1-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51de1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51de1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51de1-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51de1-119">Optional query parameters</span></span>

<span data-ttu-id="51de1-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="51de1-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="51de1-121">Например, чтобы получить пакет доступа каждого запроса, включайте `$expand=accessPackage` в запрос.</span><span class="sxs-lookup"><span data-stu-id="51de1-121">For example, to retrieve the access package of each request, include `$expand=accessPackage` in the query.</span></span>  <span data-ttu-id="51de1-122">Чтобы получить только запросы для определенного пакета доступа, включайте в запрос фильтр, например `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'` .</span><span class="sxs-lookup"><span data-stu-id="51de1-122">To retrieve only requests for a specific access package, include in the query a filter such as `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'`.</span></span>  <span data-ttu-id="51de1-123">Чтобы получить результат назначения, включайте `$expand=accessPackageAssignment` запрос.</span><span class="sxs-lookup"><span data-stu-id="51de1-123">To retrieve the resulting assignment, include `$expand=accessPackageAssignment` in the query.</span></span>
<span data-ttu-id="51de1-124">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="51de1-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="51de1-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51de1-125">Request headers</span></span>

| <span data-ttu-id="51de1-126">Имя</span><span class="sxs-lookup"><span data-stu-id="51de1-126">Name</span></span>      |<span data-ttu-id="51de1-127">Описание</span><span class="sxs-lookup"><span data-stu-id="51de1-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="51de1-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="51de1-128">Authorization</span></span> | <span data-ttu-id="51de1-129">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="51de1-129">Bearer \{token\}.</span></span> <span data-ttu-id="51de1-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="51de1-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51de1-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51de1-131">Request body</span></span>

<span data-ttu-id="51de1-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51de1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51de1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="51de1-133">Response</span></span>

<span data-ttu-id="51de1-134">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="51de1-134">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51de1-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="51de1-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="51de1-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="51de1-136">Request</span></span>

<span data-ttu-id="51de1-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51de1-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51de1-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="51de1-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```
# <a name="c"></a>[<span data-ttu-id="51de1-139">C#</span><span class="sxs-lookup"><span data-stu-id="51de1-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51de1-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51de1-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51de1-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51de1-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51de1-142">Java</span><span class="sxs-lookup"><span data-stu-id="51de1-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="51de1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="51de1-143">Response</span></span>

<span data-ttu-id="51de1-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51de1-144">The following is an example of the response.</span></span>

> <span data-ttu-id="51de1-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51de1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "requestType": "AdminAdd",
      "requestState": "Delivered",
      "requestStatus": "Fulfilled",
      "isValidationOnly": false,
      "createdDateTime": "2019-10-25T22:55:11.623Z"
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


