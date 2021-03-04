---
title: Получить accessPackageAssignmentPolicy
description: Извлечение свойств и связей объекта accessPackageAassignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8ab969653cd9787ed51a9269fa9060b2e2e07d9c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439732"
---
# <a name="get-accesspackageassignmentpolicy"></a><span data-ttu-id="0eaec-103">Получить accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="0eaec-103">Get accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="0eaec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0eaec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0eaec-105">В [управлении правами Azure AD](../resources/entitlementmanagement-root.md)извлекайте свойства и связи объекта [accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0eaec-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0eaec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0eaec-106">Permissions</span></span>

<span data-ttu-id="0eaec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0eaec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0eaec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0eaec-109">Permission type</span></span>                        | <span data-ttu-id="0eaec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0eaec-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0eaec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0eaec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0eaec-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eaec-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="0eaec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0eaec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0eaec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eaec-114">Not supported.</span></span> |
| <span data-ttu-id="0eaec-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0eaec-115">Application</span></span>                            | <span data-ttu-id="0eaec-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eaec-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0eaec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0eaec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0eaec-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0eaec-118">Optional query parameters</span></span>

<span data-ttu-id="0eaec-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0eaec-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0eaec-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0eaec-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0eaec-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0eaec-121">Request headers</span></span>

| <span data-ttu-id="0eaec-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0eaec-122">Name</span></span>      |<span data-ttu-id="0eaec-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0eaec-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0eaec-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0eaec-124">Authorization</span></span> | <span data-ttu-id="0eaec-125">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="0eaec-125">Bearer \{token\}.</span></span> <span data-ttu-id="0eaec-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="0eaec-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0eaec-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0eaec-127">Request body</span></span>

<span data-ttu-id="0eaec-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0eaec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0eaec-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eaec-129">Response</span></span>

<span data-ttu-id="0eaec-130">В случае успешного выполнения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0eaec-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0eaec-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="0eaec-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0eaec-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0eaec-132">Request</span></span>

<span data-ttu-id="0eaec-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0eaec-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0eaec-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0eaec-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="0eaec-135">C#</span><span class="sxs-lookup"><span data-stu-id="0eaec-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0eaec-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0eaec-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0eaec-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0eaec-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0eaec-138">Java</span><span class="sxs-lookup"><span data-stu-id="0eaec-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0eaec-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eaec-139">Response</span></span>

<span data-ttu-id="0eaec-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0eaec-140">The following is an example of the response.</span></span>

> <span data-ttu-id="0eaec-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0eaec-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
  "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
  "displayName": "All Users",
  "description": "All users in the directory can request access.",
  "canExtend": false,
  "durationInDays": 365,
  "accessReviewSettings": null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


