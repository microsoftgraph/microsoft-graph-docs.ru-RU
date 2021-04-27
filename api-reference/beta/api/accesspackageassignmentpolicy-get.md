---
title: Получить accessPackageAssignmentPolicy
description: Извлечение свойств и связей объекта accessPackageAassignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8b3f98108aa18221a513b6dc187fa1ed68b7017b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048626"
---
# <a name="get-accesspackageassignmentpolicy"></a><span data-ttu-id="40cd4-103">Получить accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="40cd4-103">Get accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="40cd4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40cd4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40cd4-105">В [управлении правами Azure AD](../resources/entitlementmanagement-root.md)извлекайте свойства и связи объекта [accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="40cd4-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40cd4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40cd4-106">Permissions</span></span>

<span data-ttu-id="40cd4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40cd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40cd4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40cd4-109">Permission type</span></span>                        | <span data-ttu-id="40cd4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40cd4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="40cd4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40cd4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="40cd4-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40cd4-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="40cd4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40cd4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40cd4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40cd4-114">Not supported.</span></span> |
| <span data-ttu-id="40cd4-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="40cd4-115">Application</span></span>                            | <span data-ttu-id="40cd4-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40cd4-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40cd4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40cd4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40cd4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="40cd4-118">Optional query parameters</span></span>

<span data-ttu-id="40cd4-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="40cd4-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="40cd4-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="40cd4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="40cd4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40cd4-121">Request headers</span></span>

| <span data-ttu-id="40cd4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="40cd4-122">Name</span></span>      |<span data-ttu-id="40cd4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="40cd4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="40cd4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40cd4-124">Authorization</span></span> | <span data-ttu-id="40cd4-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40cd4-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40cd4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40cd4-127">Request body</span></span>

<span data-ttu-id="40cd4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40cd4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40cd4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="40cd4-129">Response</span></span>

<span data-ttu-id="40cd4-130">В случае успешного выполнения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="40cd4-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40cd4-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="40cd4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40cd4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="40cd4-132">Request</span></span>

<span data-ttu-id="40cd4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40cd4-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="40cd4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="40cd4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="40cd4-135">C#</span><span class="sxs-lookup"><span data-stu-id="40cd4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40cd4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40cd4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40cd4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40cd4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40cd4-138">Java</span><span class="sxs-lookup"><span data-stu-id="40cd4-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="40cd4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="40cd4-139">Response</span></span>

<span data-ttu-id="40cd4-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="40cd4-140">The following is an example of the response.</span></span>

> <span data-ttu-id="40cd4-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="40cd4-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


