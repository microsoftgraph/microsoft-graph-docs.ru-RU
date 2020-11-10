---
title: Список АкцесспаккажеассигнментполиЦиес
description: Получение списка объектов Акцесспаккажеассигнментполици.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4220c2b6d92291d91d8ee6cfea36783550b91537
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952171"
---
# <a name="list-accesspackageassignmentpolicies"></a><span data-ttu-id="bad4d-103">Список АкцесспаккажеассигнментполиЦиес</span><span class="sxs-lookup"><span data-stu-id="bad4d-103">List accessPackageAssignmentPolicies</span></span>

<span data-ttu-id="bad4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bad4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bad4d-105">Получение списка объектов [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в [службе управления обслуживанием Azure AD](../resources/entitlementmanagement-root.md).</span><span class="sxs-lookup"><span data-stu-id="bad4d-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects.</span></span> <span data-ttu-id="bad4d-106">Если делегированный пользователь находится в роли каталога, полученный список включает все политики назначения, которые абонент имеет доступ для чтения, во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="bad4d-106">If the delegated user is in a directory role, the resulting list includes all the assignment policies that the caller has access to read, across all catalogs and access packages.</span></span>  <span data-ttu-id="bad4d-107">Если делегированный пользователь является диспетчером пакетов доступа или владельцем каталога, он должен вместо этого получать политики для пакетов доступа, которые они могут читать с помощью [List акцесспаккажес](accesspackage-list.md) , включая `$expand=accessPackageAssignmentPolicies` в качестве параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="bad4d-107">If the delegated user is an access package manager or catalog owner, they should instead retrieve the policies for the access packages they can read with [list accessPackages](accesspackage-list.md) by including `$expand=accessPackageAssignmentPolicies` as a query parameter.</span></span>

## <a name="permissions"></a><span data-ttu-id="bad4d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bad4d-108">Permissions</span></span>

<span data-ttu-id="bad4d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bad4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bad4d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bad4d-111">Permission type</span></span>                        | <span data-ttu-id="bad4d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bad4d-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bad4d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bad4d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bad4d-114">Ентитлементманажемент. Read. ALL, Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bad4d-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="bad4d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bad4d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bad4d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bad4d-116">Not supported.</span></span> |
| <span data-ttu-id="bad4d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bad4d-117">Application</span></span>                            | <span data-ttu-id="bad4d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bad4d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bad4d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bad4d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bad4d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bad4d-120">Optional query parameters</span></span>

<span data-ttu-id="bad4d-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bad4d-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bad4d-122">Например, чтобы получить политику назначения пакетов Access с указанным отображаемым именем, включите `$filter=displayName eq 'Employee sales support'` в запрос.</span><span class="sxs-lookup"><span data-stu-id="bad4d-122">For example, to retrieve an access package assignment policy with a specified display name, include `$filter=displayName eq 'Employee sales support'` in the query.</span></span> <span data-ttu-id="bad4d-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bad4d-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bad4d-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bad4d-124">Request headers</span></span>

| <span data-ttu-id="bad4d-125">Имя</span><span class="sxs-lookup"><span data-stu-id="bad4d-125">Name</span></span>      |<span data-ttu-id="bad4d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="bad4d-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bad4d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="bad4d-127">Authorization</span></span> | <span data-ttu-id="bad4d-128">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="bad4d-128">Bearer \{token\}.</span></span> <span data-ttu-id="bad4d-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="bad4d-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bad4d-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bad4d-130">Request body</span></span>

<span data-ttu-id="bad4d-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bad4d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bad4d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bad4d-132">Response</span></span>

<span data-ttu-id="bad4d-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bad4d-133">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bad4d-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="bad4d-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bad4d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="bad4d-135">Request</span></span>

<span data-ttu-id="bad4d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bad4d-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bad4d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="bad4d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```
# <a name="c"></a>[<span data-ttu-id="bad4d-138">C#</span><span class="sxs-lookup"><span data-stu-id="bad4d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bad4d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bad4d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bad4d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bad4d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bad4d-141">Java</span><span class="sxs-lookup"><span data-stu-id="bad4d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bad4d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="bad4d-142">Response</span></span>

<span data-ttu-id="bad4d-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bad4d-143">The following is an example of the response.</span></span>

> <span data-ttu-id="bad4d-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bad4d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
      "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
      "displayName": "All Users",
      "description": "All users can request for access to the directory.",
      "canExtend": false,
      "durationInDays": 365,
      "accessReviewSettings": null
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


