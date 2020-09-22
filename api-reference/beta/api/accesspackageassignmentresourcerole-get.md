---
title: Получение Акцесспаккажеассигнментресаурцероле
description: Получение свойств и связей объекта Акцесспаккажеассигнментресаурцероле.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8d1f7b447bf9f920cd1074c24ec98aeeaf74b8af
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983832"
---
# <a name="get-accesspackageassignmentresourcerole"></a><span data-ttu-id="8c5eb-103">Получение Акцесспаккажеассигнментресаурцероле</span><span class="sxs-lookup"><span data-stu-id="8c5eb-103">Get accessPackageAssignmentResourceRole</span></span>

<span data-ttu-id="8c5eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c5eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c5eb-105">Получение свойств и связей объекта [акцесспаккажеассигнментресаурцероле](../resources/accesspackageassignmentresourcerole.md) .</span><span class="sxs-lookup"><span data-stu-id="8c5eb-105">Retrieve the properties and relationships of an [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c5eb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c5eb-106">Permissions</span></span>

<span data-ttu-id="8c5eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c5eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c5eb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c5eb-109">Permission type</span></span>                        | <span data-ttu-id="8c5eb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c5eb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8c5eb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c5eb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c5eb-112">Ентитлементманажемент. Read. ALL, Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8c5eb-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="8c5eb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c5eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c5eb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c5eb-114">Not supported.</span></span> |
| <span data-ttu-id="8c5eb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c5eb-115">Application</span></span>                            | <span data-ttu-id="8c5eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c5eb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c5eb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c5eb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c5eb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8c5eb-118">Optional query parameters</span></span>

<span data-ttu-id="8c5eb-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8c5eb-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8c5eb-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8c5eb-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c5eb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c5eb-121">Request headers</span></span>

| <span data-ttu-id="8c5eb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8c5eb-122">Name</span></span>      |<span data-ttu-id="8c5eb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8c5eb-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c5eb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c5eb-124">Authorization</span></span> | <span data-ttu-id="8c5eb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c5eb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c5eb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8c5eb-127">Request body</span></span>

<span data-ttu-id="8c5eb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c5eb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c5eb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c5eb-129">Response</span></span>

<span data-ttu-id="8c5eb-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [акцесспаккажеассигнментресаурцероле](../resources/accesspackageassignmentresourcerole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c5eb-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c5eb-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="8c5eb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c5eb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c5eb-132">Request</span></span>

<span data-ttu-id="8c5eb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c5eb-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c5eb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c5eb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourcerole"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```
# <a name="c"></a>[<span data-ttu-id="8c5eb-135">C#</span><span class="sxs-lookup"><span data-stu-id="8c5eb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentresourcerole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c5eb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c5eb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentresourcerole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c5eb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c5eb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentresourcerole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8c5eb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c5eb-138">Response</span></span>

<span data-ttu-id="8c5eb-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c5eb-139">The following is an example of the response.</span></span>

> <span data-ttu-id="8c5eb-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c5eb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1bf101d2-4d9c-437f-bbf5-3d13d98f5479",
  "originId": "originId-value",
  "originSystem": "SharePointOnline",
  "status": "Fulfilled"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentResourceRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


