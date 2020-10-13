---
title: Список ПермиссионгрантполиЦиес
description: Получение списка объектов Пермиссионгрантполици.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: a57f443ab8c278f601fac0a488164a61e64411da
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433688"
---
# <a name="list-permissiongrantpolicies"></a><span data-ttu-id="2d2e4-103">Список ПермиссионгрантполиЦиес</span><span class="sxs-lookup"><span data-stu-id="2d2e4-103">List permissionGrantPolicies</span></span>

<span data-ttu-id="2d2e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d2e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d2e4-105">Получение списка объектов [пермиссионгрантполици](../resources/permissiongrantpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="2d2e4-105">Retrieve the list of [permissionGrantPolicy](../resources/permissiongrantpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d2e4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d2e4-106">Permissions</span></span>

<span data-ttu-id="2d2e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d2e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d2e4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d2e4-109">Permission type</span></span>                        | <span data-ttu-id="2d2e4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d2e4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2d2e4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d2e4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d2e4-112">Policy. Read. Пермиссионгрант, Policy. ReadWrite. Пермиссионгрант</span><span class="sxs-lookup"><span data-stu-id="2d2e4-112">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="2d2e4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d2e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d2e4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d2e4-114">Not supported.</span></span> |
| <span data-ttu-id="2d2e4-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="2d2e4-115">Application</span></span>                            | <span data-ttu-id="2d2e4-116">Policy. Read. Пермиссионгрант, Policy. ReadWrite. Пермиссионгрант</span><span class="sxs-lookup"><span data-stu-id="2d2e4-116">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d2e4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d2e4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/permissionGrantPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2d2e4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2d2e4-118">Optional query parameters</span></span>

<span data-ttu-id="2d2e4-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2d2e4-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d2e4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d2e4-120">Request headers</span></span>

| <span data-ttu-id="2d2e4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2d2e4-121">Name</span></span>           | <span data-ttu-id="2d2e4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2d2e4-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="2d2e4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d2e4-123">Authorization</span></span>  | <span data-ttu-id="2d2e4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d2e4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2d2e4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d2e4-126">Request body</span></span>

<span data-ttu-id="2d2e4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2d2e4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d2e4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d2e4-128">Response</span></span>

<span data-ttu-id="2d2e4-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [пермиссионгрантполици](../resources/permissiongrantpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2d2e4-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantPolicy](../resources/permissiongrantpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d2e4-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="2d2e4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d2e4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d2e4-131">Request</span></span>

<span data-ttu-id="2d2e4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d2e4-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_permissiongrantpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/permissionGrantPolicies
```

### <a name="response"></a><span data-ttu-id="2d2e4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d2e4-133">Response</span></span>

<span data-ttu-id="2d2e4-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2d2e4-134">The following is an example of the response.</span></span>

> <span data-ttu-id="2d2e4-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d2e4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
