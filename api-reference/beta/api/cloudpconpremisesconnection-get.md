---
title: Получение Клаудпконпремисесконнектион
description: Чтение свойств и связей объекта Клаудпконпремисесконнектион.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 24c5be1f4e05a91b52821b24ab76885f63124c2c
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378467"
---
# <a name="get-cloudpconpremisesconnection"></a><span data-ttu-id="2b9a0-103">Получение Клаудпконпремисесконнектион</span><span class="sxs-lookup"><span data-stu-id="2b9a0-103">Get cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="2b9a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b9a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b9a0-105">Чтение свойств и связей объекта [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="2b9a0-105">Read the properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b9a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b9a0-106">Permissions</span></span>

<span data-ttu-id="2b9a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b9a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b9a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b9a0-109">Permission type</span></span>| <span data-ttu-id="2b9a0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b9a0-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="2b9a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b9a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2b9a0-112">Клаудпк. ReadWrite. ALL, Клаудпк. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="2b9a0-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="2b9a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b9a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b9a0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b9a0-114">Not supported.</span></span>|
|<span data-ttu-id="2b9a0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b9a0-115">Application</span></span>| <span data-ttu-id="2b9a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b9a0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b9a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b9a0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b9a0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b9a0-118">Optional query parameters</span></span>

<span data-ttu-id="2b9a0-119">Этот метод поддерживает `$select` параметр запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2b9a0-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="2b9a0-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2b9a0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b9a0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b9a0-121">Request headers</span></span>

| <span data-ttu-id="2b9a0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2b9a0-122">Name</span></span>          | <span data-ttu-id="2b9a0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2b9a0-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2b9a0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b9a0-124">Authorization</span></span> | <span data-ttu-id="2b9a0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b9a0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b9a0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b9a0-127">Request body</span></span>

<span data-ttu-id="2b9a0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b9a0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b9a0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b9a0-129">Response</span></span>

<span data-ttu-id="2b9a0-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b9a0-130">If successful, this method returns a `200 OK` response code and a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b9a0-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="2b9a0-131">Examples</span></span>

### <a name="example-1-get-the-default-properties-of-an-on-premises-connection"></a><span data-ttu-id="2b9a0-132">Пример 1: получение свойств по умолчанию локального подключения</span><span class="sxs-lookup"><span data-stu-id="2b9a0-132">Example 1: Get the default properties of an on-premises connection</span></span>

#### <a name="request"></a><span data-ttu-id="2b9a0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b9a0-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

#### <a name="response"></a><span data-ttu-id="2b9a0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b9a0-134">Response</span></span>

<span data-ttu-id="2b9a0-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2b9a0-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
    "id": "9ec90ff8-fd63-4fb9-ab5a-aa4fdccffff",
    "displayName": "Display Name value",
    "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
    "subscriptionName": "Subscription Name value",
    "adDomainName": "Active Directory Domain Name value",
    "adDomainUsername": "Active Directory Domain User Name value",
    "organizationalUnit": "Organization Unit value",
    "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
    "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
    "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default",
    "healthCheckStatus": "running",
    "inUse": false
  }
}
```

### <a name="example-2-get-the-selected-properties-of-an-on-premises-connection-including-healthcheckstatusdetails"></a><span data-ttu-id="2b9a0-136">Пример 2: Получение выбранных свойств локального подключения, включая Хеалсчеккстатусдетаилс</span><span class="sxs-lookup"><span data-stu-id="2b9a0-136">Example 2: Get the selected properties of an on-premises connection, including healthCheckStatusDetails</span></span>

#### <a name="request"></a><span data-ttu-id="2b9a0-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b9a0-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection_withDetails"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}?$select=id,displayName,subscriptionId,subscriptionName,adDomainName,adDomainUsername,organizationalUnit,virtualNetworkId,subnetId,healthCheckStatus,healthCheckStatusDetails,inUse
```

#### <a name="response"></a><span data-ttu-id="2b9a0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b9a0-138">Response</span></span>

<span data-ttu-id="2b9a0-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2b9a0-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
    "id": "9ec90ff8-fd63-4fb9-ab5a-aa4fdccffff",
    "displayName": "Display Name value",
    "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
    "subscriptionName": "Subscription Name value",
    "adDomainName": "Active Directory Domain Name value",
    "adDomainUsername": "Active Directory Domain User Name value",
    "organizationalUnit": "Organization Unit value",
    "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
    "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
    "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default",
    "healthCheckStatus": "failed",
    "healthCheckStatusDetails": {
      "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionStatusDetails",
      "startDateTime": "2020-11-03T12:43:14Z",
      "endDateTime": "2020-11-03T12:43:32Z",
      "healthChecks": [
        {
          "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
          "status": "failed",
          "displayName": "Display Name value",
          "startDateTime": "2020-11-03T12:43:14Z",
          "endDateTime": "2020-11-03T12:43:15Z",
          "errorType": "dnsCheckFqdnNotFound",
          "recommendedAction": "We did not find the provided domain name; please re-enter",
          "additionalDdetails": null
        },
        {
          "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
          "status": "passed",
          "displayName": "Display Name value",
          "startDateTime": "2020-11-03T12:43:15Z",
          "endDateTime": "2020-11-03T12:43:26Z",
          "errorType": null,
          "recommendedAction": null,
          "additionalDetails": null
        },
        {
          "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
          "status": "failed",
          "displayName": "Display Name value",
          "startDateTime": "2020-11-03T12:43:27Z",
          "endDateTime": "2020-11-03T12:43:32Z",
          "errorType": "endpointConnectivityCheckUrlNotWhitelisted",
          "recommendedAction": "Recommended Action value",
          "additionaldDetails": "Additional Details value"
        },
        {
          "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
          "status": "passed",
          "displayName": "Display Name value",
          "startDateTime": null,
          "endDateTime": null,
          "errorType": null,
          "recommendedAction": null,
          "additionaldDetails": null
        }
      ]
    },
    "inUse": false
  }
}
```
