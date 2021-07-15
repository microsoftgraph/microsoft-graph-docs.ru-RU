---
title: Список клиентов
description: Получите список объектов клиента и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 2ffea17f39ee0db99b3b9aa964c73ccd5763f909
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440789"
---
# <a name="list-tenants"></a><span data-ttu-id="02055-103">Список клиентов</span><span class="sxs-lookup"><span data-stu-id="02055-103">List tenants</span></span>
<span data-ttu-id="02055-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="02055-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02055-105">Получите список объектов [клиента](../resources/managedtenants-tenant.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="02055-105">Get a list of the [tenant](../resources/managedtenants-tenant.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="02055-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02055-106">Permissions</span></span>
<span data-ttu-id="02055-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02055-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02055-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02055-109">Permission type</span></span>|<span data-ttu-id="02055-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02055-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02055-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02055-111">Delegated (work or school account)</span></span>|<span data-ttu-id="02055-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02055-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="02055-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02055-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02055-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02055-114">Not supported.</span></span>|
|<span data-ttu-id="02055-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02055-115">Application</span></span>|<span data-ttu-id="02055-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02055-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02055-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02055-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02055-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="02055-118">Optional query parameters</span></span>
<span data-ttu-id="02055-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="02055-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02055-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02055-120">Request headers</span></span>
|<span data-ttu-id="02055-121">Имя</span><span class="sxs-lookup"><span data-stu-id="02055-121">Name</span></span>|<span data-ttu-id="02055-122">Описание</span><span class="sxs-lookup"><span data-stu-id="02055-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="02055-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02055-123">Authorization</span></span>|<span data-ttu-id="02055-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02055-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02055-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02055-126">Request body</span></span>
<span data-ttu-id="02055-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02055-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02055-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="02055-128">Response</span></span>

<span data-ttu-id="02055-129">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` клиента в тексте ответа. [](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="02055-129">If successful, this method returns a `200 OK` response code and a collection of [tenant](../resources/managedtenants-tenant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02055-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="02055-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02055-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="02055-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="02055-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="02055-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tenant"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants
```
# <a name="c"></a>[<span data-ttu-id="02055-133">C#</span><span class="sxs-lookup"><span data-stu-id="02055-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tenant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02055-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02055-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tenant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02055-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02055-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tenant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02055-136">Java</span><span class="sxs-lookup"><span data-stu-id="02055-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tenant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="02055-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="02055-137">Response</span></span>
><span data-ttu-id="02055-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="02055-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenant)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "contract": {
        "displayName": "Fourth Coffee",
        "defaultDomainName": "fourthcoffe01.onmicrosoft.com",
        "contractType": 2
      },
      "tenantStatusInformation": {
        "onboardingStatus": "ineligible",
        "onboardingDateTime": "2012-02-20T00:00:00Z",
        "onboardedByUserId": "",
        "offboardedDateTime": "2012-02-20T00:00:00Z",
        "offboardedBy": "",
        "delegatedPrivilegeStatus": "delegatedAdminPrivileges",
        "workloadStatuses": [
          {
            "displayName": "Device Management",
            "onboardingStatus": "onboarded",
            "onboardedDateTime": "2012-02-20T00:00:00Z",
            "offboardedDateTime": null
          },
          {
            "displayName": "Cloud PC",
            "onboardingStatus": "notOnboarded",
            "onboardedDateTime": "2012-02-20T00:00:00Z",
            "offboardedDateTime": null
          }
        ]
      },
      "createdDateTime": "2012-02-20T00:00:00Z",
      "lastUpdatedDatetime": "2021-02-20T00:00:00Z"
    }
  ]
}
```
