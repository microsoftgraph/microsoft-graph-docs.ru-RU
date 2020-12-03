---
title: Список ПермиссионгрантполиЦиес
description: Получение списка объектов Пермиссионгрантполици.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 755d2146907c77baa342a0f1b8abd4ea32b87df4
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524291"
---
# <a name="list-permissiongrantpolicies"></a><span data-ttu-id="e315a-103">Список ПермиссионгрантполиЦиес</span><span class="sxs-lookup"><span data-stu-id="e315a-103">List permissionGrantPolicies</span></span>

<span data-ttu-id="e315a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e315a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e315a-105">Получение списка объектов [пермиссионгрантполици](../resources/permissiongrantpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e315a-105">Retrieve the list of [permissionGrantPolicy](../resources/permissiongrantpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e315a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e315a-106">Permissions</span></span>

<span data-ttu-id="e315a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e315a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e315a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e315a-109">Permission type</span></span>                        | <span data-ttu-id="e315a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e315a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e315a-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e315a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e315a-112">Policy. Read. Пермиссионгрант, Policy. ReadWrite. Пермиссионгрант</span><span class="sxs-lookup"><span data-stu-id="e315a-112">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="e315a-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e315a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e315a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e315a-114">Not supported.</span></span> |
| <span data-ttu-id="e315a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e315a-115">Application</span></span>                            | <span data-ttu-id="e315a-116">Policy. Read. Пермиссионгрант, Policy. ReadWrite. Пермиссионгрант</span><span class="sxs-lookup"><span data-stu-id="e315a-116">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="e315a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e315a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/permissionGrantPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e315a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e315a-118">Optional query parameters</span></span>

<span data-ttu-id="e315a-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e315a-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e315a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e315a-120">Request headers</span></span>

| <span data-ttu-id="e315a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e315a-121">Name</span></span>           | <span data-ttu-id="e315a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e315a-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="e315a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e315a-123">Authorization</span></span>  | <span data-ttu-id="e315a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e315a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e315a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e315a-126">Request body</span></span>

<span data-ttu-id="e315a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e315a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e315a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e315a-128">Response</span></span>

<span data-ttu-id="e315a-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [пермиссионгрантполици](../resources/permissiongrantpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e315a-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantPolicy](../resources/permissiongrantpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e315a-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="e315a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e315a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e315a-131">Request</span></span>

<span data-ttu-id="e315a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e315a-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e315a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e315a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_permissiongrantpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies
```
# <a name="c"></a>[<span data-ttu-id="e315a-134">C#</span><span class="sxs-lookup"><span data-stu-id="e315a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-permissiongrantpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e315a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e315a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-permissiongrantpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e315a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e315a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-permissiongrantpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e315a-137">Java</span><span class="sxs-lookup"><span data-stu-id="e315a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-permissiongrantpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e315a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e315a-138">Response</span></span>

<span data-ttu-id="e315a-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e315a-139">The following is an example of the response.</span></span>

> <span data-ttu-id="e315a-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e315a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "tier-1",
      "displayName": "Tier 1 Help Desk",
      "description": "Custom permission grant policy for tier 1 help desk.",
      "includes": [
        {
          "id": "198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5",
          "permissionClassification": "low",
          "permissionType": "delegated",
          "resourceApplication": "any",
          "permissions": [ "all" ],
          "clientApplicationIds": [ "all" ],
          "clientApplicationTenantIds": [ "all" ],
          "clientApplicationPublisherIds": [ "all" ],
          "clientApplicationsFromVerifiedPublisherOnly": true
        }
      ],
      "excludes": []
    },
    {
      "id": "microsoft-company-admin",
      "displayName": "Company Admin Policy",
      "description": "Permissions consentable by Company Administrators.",
      "includes": [
        {
          "id": "1f06f3a1-42d3-4243-8fbc-5d0c30d4de4c",
          "permissionClassification": "all",
          "permissionType": "application",
          "resourceApplication": "any",
          "permissions": [ "all" ],
          "clientApplicationIds": [ "all" ],
          "clientApplicationTenantIds": [ "all" ],
          "clientApplicationPublisherIds": [ "all" ],
          "clientApplicationsFromVerifiedPublisherOnly": false
        },
        {
          "id": "08619a19-ae6f-406c-b9a0-ea6af1f1558d",
          "permissionClassification": "all",
          "permissionType": "delegated",
          "resourceApplication": "any",
          "permissions": [ "all" ],
          "clientApplicationIds": [ "all" ],
          "clientApplicationTenantIds": [ "all" ],
          "clientApplicationPublisherIds": [ "all" ],
          "clientApplicationsFromVerifiedPublisherOnly": false
        }
      ],
      "excludes": []
    }
  ]
}
```
