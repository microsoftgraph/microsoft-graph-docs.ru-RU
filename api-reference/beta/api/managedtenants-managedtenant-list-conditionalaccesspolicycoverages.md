---
title: Список conditionalAccessPolicyCoverages
description: Получите список объектов conditionalAccessPolicyCoverage и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 633a909778182a6da2ea04d9e37484db3cfdc286
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402418"
---
# <a name="list-conditionalaccesspolicycoverages"></a><span data-ttu-id="03139-103">Список conditionalAccessPolicyCoverages</span><span class="sxs-lookup"><span data-stu-id="03139-103">List conditionalAccessPolicyCoverages</span></span>
<span data-ttu-id="03139-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="03139-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03139-105">Получите список объектов [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="03139-105">Get a list of the [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) objects and their properties.</span></span> <span data-ttu-id="03139-106">Используйте эту операцию для списка Azure Active Directory политики условного доступа для всех клиентов, управляемых платформой управления с несколькими клиентами.</span><span class="sxs-lookup"><span data-stu-id="03139-106">Use this operation to list of Azure Active Directory conditional access policy coverage across all tenants that are being managed by the multi-tenant management platform.</span></span>

## <a name="permissions"></a><span data-ttu-id="03139-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03139-107">Permissions</span></span>
<span data-ttu-id="03139-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03139-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03139-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03139-110">Permission type</span></span>|<span data-ttu-id="03139-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03139-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03139-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03139-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03139-113">Policy.Read.All, Policy.ReadWrite.ConditionalAccess и Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="03139-113">Policy.Read.All, Policy.ReadWrite.ConditionalAccess, and Application.Read.All</span></span>|
|<span data-ttu-id="03139-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03139-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03139-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03139-115">Not supported.</span></span>|
|<span data-ttu-id="03139-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03139-116">Application</span></span>|<span data-ttu-id="03139-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03139-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03139-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03139-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/conditionalAccessPolicyCoverages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03139-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="03139-119">Optional query parameters</span></span>
<span data-ttu-id="03139-120">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="03139-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03139-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03139-121">Request headers</span></span>
|<span data-ttu-id="03139-122">Имя</span><span class="sxs-lookup"><span data-stu-id="03139-122">Name</span></span>|<span data-ttu-id="03139-123">Описание</span><span class="sxs-lookup"><span data-stu-id="03139-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="03139-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03139-124">Authorization</span></span>|<span data-ttu-id="03139-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03139-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03139-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03139-127">Request body</span></span>
<span data-ttu-id="03139-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03139-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03139-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="03139-129">Response</span></span>

<span data-ttu-id="03139-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="03139-130">If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03139-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="03139-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03139-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="03139-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_conditionalaccesspolicycoverage"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/conditionalAccessPolicyCoverages
```


### <a name="response"></a><span data-ttu-id="03139-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="03139-133">Response</span></span>
><span data-ttu-id="03139-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="03139-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.conditionalAccessPolicyCoverage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
      "id": "38227791-a88b-4fcc-81c5-58cf77668320",
      "conditionalAccessPolicyState": "enabled",
      "requiresDeviceCompliance": false,
      "latestPolicyModifiedDateTime": "2021-07-11T14:56:13.598304Z",
      "tenantDisplayName": "Consolidated Messenger"
    }
  ]
}
```
