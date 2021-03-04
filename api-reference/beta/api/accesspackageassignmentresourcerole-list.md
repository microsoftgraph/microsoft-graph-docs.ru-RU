---
title: Список accessPackageAssignmentResourceRoles
description: Извлечение списка объектов accessPackageAssignmentResourceRole.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e1d6c10437f4fa0c2eee26026dca3d323bf3bdd0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439627"
---
# <a name="list-accesspackageassignmentresourceroles"></a><span data-ttu-id="9e0bc-103">Список accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="9e0bc-103">List accessPackageAssignmentResourceRoles</span></span>

<span data-ttu-id="9e0bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e0bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e0bc-105">Извлечение списка [объектов accessPackageAssignmentResourceRole.](../resources/accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="9e0bc-105">Retrieve a list of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects.</span></span>  <span data-ttu-id="9e0bc-106">В итоговом списке содержатся все роли ресурсов всех назначений, которые вызываемая имеет доступ к считыву, во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="9e0bc-106">The resulting list includes all the resource roles of all assignments that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e0bc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e0bc-107">Permissions</span></span>

<span data-ttu-id="9e0bc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e0bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e0bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e0bc-110">Permission type</span></span>                        | <span data-ttu-id="9e0bc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e0bc-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9e0bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e0bc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e0bc-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e0bc-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9e0bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e0bc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e0bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e0bc-115">Not supported.</span></span> |
| <span data-ttu-id="9e0bc-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9e0bc-116">Application</span></span>                            | <span data-ttu-id="9e0bc-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e0bc-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e0bc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e0bc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e0bc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9e0bc-119">Optional query parameters</span></span>

<span data-ttu-id="9e0bc-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="9e0bc-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9e0bc-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9e0bc-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="9e0bc-122">Например, чтобы получить только роли ресурсов назначения пакета доступа для конкретного пользователя, можно включить запрос с фильтром, нацеленным на объект ID этого `?$expand=accessPackageSubject&$filter=accessPackageSubject/objectId+eq+'9b835e5c-bf18-4ad9-8556-9b1ea0019c6b'` пользователя.</span><span class="sxs-lookup"><span data-stu-id="9e0bc-122">For example, to retrieve only access package assignment resource roles for a particular user, you can include a query with a filter targeting the object ID of that user `?$expand=accessPackageSubject&$filter=accessPackageSubject/objectId+eq+'9b835e5c-bf18-4ad9-8556-9b1ea0019c6b'`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="9e0bc-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e0bc-123">Request headers</span></span>

| <span data-ttu-id="9e0bc-124">Имя</span><span class="sxs-lookup"><span data-stu-id="9e0bc-124">Name</span></span>      |<span data-ttu-id="9e0bc-125">Описание</span><span class="sxs-lookup"><span data-stu-id="9e0bc-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9e0bc-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e0bc-126">Authorization</span></span> | <span data-ttu-id="9e0bc-127">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="9e0bc-127">Bearer \{token\}.</span></span> <span data-ttu-id="9e0bc-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9e0bc-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e0bc-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9e0bc-129">Request body</span></span>

<span data-ttu-id="9e0bc-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e0bc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e0bc-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e0bc-131">Response</span></span>

<span data-ttu-id="9e0bc-132">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9e0bc-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e0bc-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="9e0bc-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9e0bc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e0bc-134">Request</span></span>

<span data-ttu-id="9e0bc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e0bc-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e0bc-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e0bc-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```
# <a name="c"></a>[<span data-ttu-id="9e0bc-137">C#</span><span class="sxs-lookup"><span data-stu-id="9e0bc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e0bc-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e0bc-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e0bc-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e0bc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9e0bc-140">Java</span><span class="sxs-lookup"><span data-stu-id="9e0bc-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentresourceroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9e0bc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e0bc-141">Response</span></span>

<span data-ttu-id="9e0bc-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9e0bc-142">The following is an example of the response.</span></span>

> <span data-ttu-id="9e0bc-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e0bc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1bf101d2-4d9c-437f-bbf5-3d13d98f5479",
      "originId": "originId-value",
      "originSystem": "SharePointOnline",
      "status": "Fulfilled"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentResourceRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


