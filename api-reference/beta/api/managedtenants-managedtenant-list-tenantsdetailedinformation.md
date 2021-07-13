---
title: Список tenantDetailedInformation
description: Получите список объектов tenantDetailedInformation и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e9c1bfd7b460dbb093b308aa2b3f9d19ffe18f81
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403084"
---
# <a name="list-tenantdetailedinformation"></a><span data-ttu-id="0a3a1-103">Список tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="0a3a1-103">List tenantDetailedInformation</span></span>
<span data-ttu-id="0a3a1-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="0a3a1-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a3a1-105">Получите список объектов [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="0a3a1-105">Get a list of the [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a3a1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a3a1-106">Permissions</span></span>
<span data-ttu-id="0a3a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a3a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a3a1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a3a1-109">Permission type</span></span>|<span data-ttu-id="0a3a1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a3a1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a3a1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a3a1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0a3a1-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a3a1-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="0a3a1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a3a1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a3a1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a3a1-114">Not supported.</span></span>|
|<span data-ttu-id="0a3a1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a3a1-115">Application</span></span>|<span data-ttu-id="0a3a1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a3a1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a3a1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a3a1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantsDetailedInformation
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a3a1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0a3a1-118">Optional query parameters</span></span>
<span data-ttu-id="0a3a1-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="0a3a1-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a3a1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a3a1-120">Request headers</span></span>
|<span data-ttu-id="0a3a1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0a3a1-121">Name</span></span>|<span data-ttu-id="0a3a1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0a3a1-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0a3a1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a3a1-123">Authorization</span></span>|<span data-ttu-id="0a3a1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a3a1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a3a1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a3a1-126">Request body</span></span>
<span data-ttu-id="0a3a1-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a3a1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a3a1-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a3a1-128">Response</span></span>

<span data-ttu-id="0a3a1-129">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0a3a1-129">If successful, this method returns a `200 OK` response code and a collection of [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0a3a1-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="0a3a1-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0a3a1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a3a1-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_tenantdetailedinformation"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantsDetailedInformation
```


### <a name="response"></a><span data-ttu-id="0a3a1-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a3a1-132">Response</span></span>
><span data-ttu-id="0a3a1-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0a3a1-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenantDetailedInformation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/managedTenants/$metadata#tenantDetailedInformation",
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "companyName": "Fourth Coffee",
      "defaultDomainName": "fourthcoffee001.onmicrosoft.com",
      "countryName": "United States",
      "countryCode": "US",
      "city": "Redmond",
      "region": "NA",
      "verticalName": "Software",
      "industryName": "Computer",
      "segmentName": "Service"
    },
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "companyName": "Consolidated Messenger",
      "defaultDomainName": "consoldiatedmessenger001.onmicrosoft.com",
      "countryName": "United States",
      "countryCode": "US",
      "city": "Redmond",
      "region": "NA",
      "verticalName": "Software",
      "industryName": "Computer",
      "segmentName": "Service"
    }
  ]
}
```
