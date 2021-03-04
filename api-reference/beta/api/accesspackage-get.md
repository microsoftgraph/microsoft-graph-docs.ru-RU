---
title: Получить accessPackage
description: Извлечение свойств и связей объекта accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 17d501e950205ca1003dfdabad9cd67d503807d3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439837"
---
# <a name="get-accesspackage"></a><span data-ttu-id="cf8a2-103">Получить accessPackage</span><span class="sxs-lookup"><span data-stu-id="cf8a2-103">Get accessPackage</span></span>

<span data-ttu-id="cf8a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf8a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf8a2-105">Извлечение свойств и связей объекта [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="cf8a2-105">Retrieve the properties and relationships of an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf8a2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf8a2-106">Permissions</span></span>

<span data-ttu-id="cf8a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf8a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf8a2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf8a2-109">Permission type</span></span>                        | <span data-ttu-id="cf8a2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf8a2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cf8a2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf8a2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf8a2-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf8a2-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="cf8a2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf8a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf8a2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf8a2-114">Not supported.</span></span> |
| <span data-ttu-id="cf8a2-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="cf8a2-115">Application</span></span>                            | <span data-ttu-id="cf8a2-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf8a2-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf8a2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf8a2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf8a2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cf8a2-118">Optional query parameters</span></span>

<span data-ttu-id="cf8a2-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cf8a2-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cf8a2-120">Например, чтобы получить политики пакета доступа, добавьте `$expand=accessPackageAssignmentPolicies` .</span><span class="sxs-lookup"><span data-stu-id="cf8a2-120">For example, to retrieve the access package policies, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="cf8a2-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cf8a2-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf8a2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf8a2-122">Request headers</span></span>

| <span data-ttu-id="cf8a2-123">Имя</span><span class="sxs-lookup"><span data-stu-id="cf8a2-123">Name</span></span>      |<span data-ttu-id="cf8a2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="cf8a2-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cf8a2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf8a2-125">Authorization</span></span> | <span data-ttu-id="cf8a2-126">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="cf8a2-126">Bearer \{token\}.</span></span> <span data-ttu-id="cf8a2-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="cf8a2-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf8a2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cf8a2-128">Request body</span></span>

<span data-ttu-id="cf8a2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf8a2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf8a2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf8a2-130">Response</span></span>

<span data-ttu-id="cf8a2-131">В случае успешной работы этот метод возвращает код отклика и запрашиваемого объекта `200 OK` [accessPackage](../resources/accesspackage.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cf8a2-131">If successful, this method returns a `200 OK` response code and the requested [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cf8a2-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="cf8a2-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cf8a2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf8a2-133">Request</span></span>

<span data-ttu-id="cf8a2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf8a2-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf8a2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf8a2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackage"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```
# <a name="c"></a>[<span data-ttu-id="cf8a2-136">C#</span><span class="sxs-lookup"><span data-stu-id="cf8a2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf8a2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf8a2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf8a2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf8a2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf8a2-139">Java</span><span class="sxs-lookup"><span data-stu-id="cf8a2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cf8a2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf8a2-140">Response</span></span>

<span data-ttu-id="cf8a2-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cf8a2-141">The following is an example of the response.</span></span>

> <span data-ttu-id="cf8a2-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf8a2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package",
    "displayName":"Access package for testing",
    "isHidden":false,
    "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
    "isRoleScopesVisible":false,
    "createdDateTime":"2019-01-27T18:19:50.74Z",
    "modifiedDateTime":"2019-01-27T18:19:50.74Z",
    "createdBy":"TestGA@example.com",
    "modifiedBy":"TestGA@example.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


