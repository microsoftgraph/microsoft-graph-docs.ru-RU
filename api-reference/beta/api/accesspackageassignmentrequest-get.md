---
title: Получить accessPackageAssignmentRequest
description: Извлечение свойств и связей объекта accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0184e1146b6450cb5c500e8b377e817a42f82ff1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439690"
---
# <a name="get-accesspackageassignmentrequest"></a><span data-ttu-id="b25fc-103">Получить accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="b25fc-103">Get accessPackageAssignmentRequest</span></span>

<span data-ttu-id="b25fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b25fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b25fc-105">В [управлении правами Azure AD](../resources/entitlementmanagement-root.md)извлекайте свойства и связи объекта [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="b25fc-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an  [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b25fc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b25fc-106">Permissions</span></span>

<span data-ttu-id="b25fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b25fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b25fc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b25fc-109">Permission type</span></span>                        | <span data-ttu-id="b25fc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b25fc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b25fc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b25fc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b25fc-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b25fc-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="b25fc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b25fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b25fc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b25fc-114">Not supported.</span></span> |
| <span data-ttu-id="b25fc-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b25fc-115">Application</span></span>                            | <span data-ttu-id="b25fc-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b25fc-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b25fc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b25fc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b25fc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b25fc-118">Optional query parameters</span></span>

<span data-ttu-id="b25fc-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b25fc-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b25fc-120">Например, чтобы получить запрашиваемую посылку доступа, включайте `$expand=accessPackage` в запрос.</span><span class="sxs-lookup"><span data-stu-id="b25fc-120">For example, to retrieve the access package that was requested, include `$expand=accessPackage` in the query.</span></span> <span data-ttu-id="b25fc-121">Чтобы получить результат назначения, включайте `$expand=accessPackageAssignment` запрос.</span><span class="sxs-lookup"><span data-stu-id="b25fc-121">To retrieve the resulting assignment, include `$expand=accessPackageAssignment` in the query.</span></span>  <span data-ttu-id="b25fc-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b25fc-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b25fc-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b25fc-123">Request headers</span></span>

| <span data-ttu-id="b25fc-124">Имя</span><span class="sxs-lookup"><span data-stu-id="b25fc-124">Name</span></span>      |<span data-ttu-id="b25fc-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b25fc-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b25fc-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b25fc-126">Authorization</span></span> | <span data-ttu-id="b25fc-127">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="b25fc-127">Bearer \{token\}.</span></span> <span data-ttu-id="b25fc-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b25fc-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b25fc-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b25fc-129">Request body</span></span>

<span data-ttu-id="b25fc-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b25fc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b25fc-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b25fc-131">Response</span></span>

<span data-ttu-id="b25fc-132">В случае успешного выполнения этот метод возвращает код отклика и запрашиваемого объекта `200 OK` [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b25fc-132">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b25fc-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="b25fc-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b25fc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b25fc-134">Request</span></span>

<span data-ttu-id="b25fc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b25fc-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b25fc-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b25fc-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```
# <a name="c"></a>[<span data-ttu-id="b25fc-137">C#</span><span class="sxs-lookup"><span data-stu-id="b25fc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b25fc-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b25fc-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b25fc-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b25fc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b25fc-140">Java</span><span class="sxs-lookup"><span data-stu-id="b25fc-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b25fc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b25fc-141">Response</span></span>

<span data-ttu-id="b25fc-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b25fc-142">The following is an example of the response.</span></span>

> <span data-ttu-id="b25fc-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b25fc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "433dafca-5047-4614-95f7-a03510b1ded3",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "isValidationOnly": false,
  "createdDateTime": "2019-10-25T22:55:11.623Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


