---
title: Получить accessPackageAssignmentRequest
description: Извлечение свойств и связей объекта accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 78340e93b202d4088b453e39594b84345a247cbe
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048605"
---
# <a name="get-accesspackageassignmentrequest"></a><span data-ttu-id="9648c-103">Получить accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9648c-103">Get accessPackageAssignmentRequest</span></span>

<span data-ttu-id="9648c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9648c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9648c-105">В [управлении правами Azure AD](../resources/entitlementmanagement-root.md)извлекайте свойства и связи объекта [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="9648c-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an  [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9648c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9648c-106">Permissions</span></span>

<span data-ttu-id="9648c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9648c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9648c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9648c-109">Permission type</span></span>                        | <span data-ttu-id="9648c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9648c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9648c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9648c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9648c-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9648c-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="9648c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9648c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9648c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9648c-114">Not supported.</span></span> |
| <span data-ttu-id="9648c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9648c-115">Application</span></span>                            | <span data-ttu-id="9648c-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9648c-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9648c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9648c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9648c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9648c-118">Optional query parameters</span></span>

<span data-ttu-id="9648c-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="9648c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9648c-120">Например, чтобы получить запрашиваемую посылку доступа, включайте `$expand=accessPackage` в запрос.</span><span class="sxs-lookup"><span data-stu-id="9648c-120">For example, to retrieve the access package that was requested, include `$expand=accessPackage` in the query.</span></span> <span data-ttu-id="9648c-121">Чтобы получить результат назначения, включайте `$expand=accessPackageAssignment` запрос.</span><span class="sxs-lookup"><span data-stu-id="9648c-121">To retrieve the resulting assignment, include `$expand=accessPackageAssignment` in the query.</span></span>  <span data-ttu-id="9648c-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9648c-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9648c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9648c-123">Request headers</span></span>

| <span data-ttu-id="9648c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="9648c-124">Name</span></span>      |<span data-ttu-id="9648c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="9648c-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9648c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9648c-126">Authorization</span></span> | <span data-ttu-id="9648c-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9648c-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9648c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9648c-129">Request body</span></span>

<span data-ttu-id="9648c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9648c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9648c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9648c-131">Response</span></span>

<span data-ttu-id="9648c-132">В случае успешного выполнения этот метод возвращает код отклика и запрашиваемого объекта `200 OK` [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9648c-132">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9648c-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="9648c-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9648c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9648c-134">Request</span></span>

<span data-ttu-id="9648c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9648c-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9648c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9648c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```
# <a name="c"></a>[<span data-ttu-id="9648c-137">C#</span><span class="sxs-lookup"><span data-stu-id="9648c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9648c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9648c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9648c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9648c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9648c-140">Java</span><span class="sxs-lookup"><span data-stu-id="9648c-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9648c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9648c-141">Response</span></span>

<span data-ttu-id="9648c-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9648c-142">The following is an example of the response.</span></span>

> <span data-ttu-id="9648c-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9648c-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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


