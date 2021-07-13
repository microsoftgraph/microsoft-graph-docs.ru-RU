---
title: Список клиентов
description: Получите список объектов клиента и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: a837f1db5990322311c0718d47e888fafd64284e
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403088"
---
# <a name="list-tenants"></a><span data-ttu-id="2fcda-103">Список клиентов</span><span class="sxs-lookup"><span data-stu-id="2fcda-103">List tenants</span></span>
<span data-ttu-id="2fcda-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="2fcda-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fcda-105">Получите список объектов [клиента](../resources/managedtenants-tenant.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="2fcda-105">Get a list of the [tenant](../resources/managedtenants-tenant.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fcda-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2fcda-106">Permissions</span></span>
<span data-ttu-id="2fcda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fcda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fcda-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2fcda-109">Permission type</span></span>|<span data-ttu-id="2fcda-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2fcda-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fcda-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2fcda-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2fcda-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fcda-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="2fcda-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2fcda-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fcda-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fcda-114">Not supported.</span></span>|
|<span data-ttu-id="2fcda-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2fcda-115">Application</span></span>|<span data-ttu-id="2fcda-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fcda-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fcda-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2fcda-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2fcda-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2fcda-118">Optional query parameters</span></span>
<span data-ttu-id="2fcda-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="2fcda-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2fcda-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2fcda-120">Request headers</span></span>
|<span data-ttu-id="2fcda-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2fcda-121">Name</span></span>|<span data-ttu-id="2fcda-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2fcda-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2fcda-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2fcda-123">Authorization</span></span>|<span data-ttu-id="2fcda-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2fcda-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fcda-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2fcda-126">Request body</span></span>
<span data-ttu-id="2fcda-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2fcda-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fcda-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fcda-128">Response</span></span>

<span data-ttu-id="2fcda-129">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` клиента в тексте ответа. [](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="2fcda-129">If successful, this method returns a `200 OK` response code and a collection of [tenant](../resources/managedtenants-tenant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2fcda-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="2fcda-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2fcda-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fcda-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_tenant"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants
```


### <a name="response"></a><span data-ttu-id="2fcda-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fcda-132">Response</span></span>
><span data-ttu-id="2fcda-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2fcda-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
