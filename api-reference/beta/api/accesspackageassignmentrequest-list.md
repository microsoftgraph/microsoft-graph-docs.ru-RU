---
title: Список accessPackageAssignmentRequests
description: Извлечение списка объектов accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 193e257656abbcc13ea54099cd8d09897ffdb340
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401015"
---
# <a name="list-accesspackageassignmentrequests"></a><span data-ttu-id="5eab4-103">Список accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="5eab4-103">List accessPackageAssignmentRequests</span></span>

<span data-ttu-id="5eab4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5eab4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5eab4-105">В [управлении правами Azure AD](../resources/entitlementmanagement-root.md)извлекайте список объектов [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="5eab4-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.</span></span>  <span data-ttu-id="5eab4-106">В итоговом списке содержатся все запросы на назначение, текущие и просроченные, которые вызываемая имеет доступ к считывке во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="5eab4-106">The resulting list includes all the assignment requests, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="5eab4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5eab4-107">Permissions</span></span>

<span data-ttu-id="5eab4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5eab4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5eab4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5eab4-110">Permission type</span></span>                        | <span data-ttu-id="5eab4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5eab4-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5eab4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5eab4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5eab4-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eab4-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="5eab4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5eab4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5eab4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eab4-115">Not supported.</span></span> |
| <span data-ttu-id="5eab4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5eab4-116">Application</span></span>                            | <span data-ttu-id="5eab4-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eab4-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5eab4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5eab4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5eab4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5eab4-119">Optional query parameters</span></span>

<span data-ttu-id="5eab4-120">Этот метод поддерживает параметры `$expand` `$filter` запроса oData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5eab4-120">This method supports the `$expand` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="5eab4-121">Например, чтобы получить пакет доступа каждого запроса, включайте `$expand=accessPackage` в запрос.</span><span class="sxs-lookup"><span data-stu-id="5eab4-121">For example, to retrieve the access package of each request, include `$expand=accessPackage` in the query.</span></span>  <span data-ttu-id="5eab4-122">Чтобы получить только запросы для определенного пакета доступа, включайте в запрос фильтр, например `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'` .</span><span class="sxs-lookup"><span data-stu-id="5eab4-122">To retrieve only requests for a specific access package, include in the query a filter such as `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'`.</span></span>  <span data-ttu-id="5eab4-123">Чтобы получить результат назначения, включайте `$expand=accessPackageAssignment` запрос.</span><span class="sxs-lookup"><span data-stu-id="5eab4-123">To retrieve the resulting assignment, include `$expand=accessPackageAssignment` in the query.</span></span>  <span data-ttu-id="5eab4-124">Дополнительные сведения о запрашиваемом запросе `$expand=requestor` включайте в запрос.</span><span class="sxs-lookup"><span data-stu-id="5eab4-124">To obtain more details on the requestor, include `$expand=requestor` in the query.</span></span>
<span data-ttu-id="5eab4-125">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5eab4-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5eab4-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5eab4-126">Request headers</span></span>

| <span data-ttu-id="5eab4-127">Имя</span><span class="sxs-lookup"><span data-stu-id="5eab4-127">Name</span></span>      |<span data-ttu-id="5eab4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5eab4-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5eab4-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5eab4-129">Authorization</span></span> | <span data-ttu-id="5eab4-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5eab4-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5eab4-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5eab4-132">Request body</span></span>

<span data-ttu-id="5eab4-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5eab4-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5eab4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eab4-134">Response</span></span>

<span data-ttu-id="5eab4-135">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5eab4-135">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5eab4-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="5eab4-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5eab4-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5eab4-137">Request</span></span>

<span data-ttu-id="5eab4-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5eab4-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5eab4-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="5eab4-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```
# <a name="c"></a>[<span data-ttu-id="5eab4-140">C#</span><span class="sxs-lookup"><span data-stu-id="5eab4-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5eab4-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5eab4-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5eab4-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5eab4-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5eab4-143">Java</span><span class="sxs-lookup"><span data-stu-id="5eab4-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5eab4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eab4-144">Response</span></span>

<span data-ttu-id="5eab4-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5eab4-145">The following is an example of the response.</span></span>

> <span data-ttu-id="5eab4-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5eab4-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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

