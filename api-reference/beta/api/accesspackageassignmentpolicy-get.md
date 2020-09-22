---
title: Получение Акцесспаккажеассигнментполици
description: Получение свойств и связей объекта Акцесспаккажеаассигнментполици.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bcb7bba0753347d483b8d68b74ba58b27291c25f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983909"
---
# <a name="get-accesspackageassignmentpolicy"></a><span data-ttu-id="4c3e5-103">Получение Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="4c3e5-103">Get accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="4c3e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c3e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c3e5-105">В разделе [Управление обслуживанием Azure AD](../resources/entitlementmanagement-root.md)извлекаются свойства и связи объекта [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="4c3e5-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c3e5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c3e5-106">Permissions</span></span>

<span data-ttu-id="4c3e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c3e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c3e5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c3e5-109">Permission type</span></span>                        | <span data-ttu-id="4c3e5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c3e5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4c3e5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c3e5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c3e5-112">Ентитлементманажемент. Read. ALL, Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4c3e5-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="4c3e5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c3e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c3e5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-114">Not supported.</span></span> |
| <span data-ttu-id="4c3e5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c3e5-115">Application</span></span>                            | <span data-ttu-id="4c3e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c3e5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c3e5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4c3e5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4c3e5-118">Optional query parameters</span></span>

<span data-ttu-id="4c3e5-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4c3e5-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4c3e5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c3e5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c3e5-121">Request headers</span></span>

| <span data-ttu-id="4c3e5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4c3e5-122">Name</span></span>      |<span data-ttu-id="4c3e5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4c3e5-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4c3e5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c3e5-124">Authorization</span></span> | <span data-ttu-id="4c3e5-125">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-125">Bearer \{token\}.</span></span> <span data-ttu-id="4c3e5-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c3e5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c3e5-127">Request body</span></span>

<span data-ttu-id="4c3e5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c3e5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c3e5-129">Response</span></span>

<span data-ttu-id="4c3e5-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c3e5-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="4c3e5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c3e5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c3e5-132">Request</span></span>

<span data-ttu-id="4c3e5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c3e5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c3e5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="4c3e5-135">C#</span><span class="sxs-lookup"><span data-stu-id="4c3e5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c3e5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c3e5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c3e5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c3e5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4c3e5-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c3e5-138">Response</span></span>

<span data-ttu-id="4c3e5-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-139">The following is an example of the response.</span></span>

> <span data-ttu-id="4c3e5-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


