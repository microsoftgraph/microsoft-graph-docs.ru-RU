---
title: Получение Клаудпконпремисесконнектион
description: Чтение свойств и связей объекта Клаудпконпремисесконнектион.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: e7e70e6ff0f5ea8badb314c1a5fa915d2f657a6b
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563410"
---
# <a name="get-cloudpconpremisesconnection"></a><span data-ttu-id="efd61-103">Получение Клаудпконпремисесконнектион</span><span class="sxs-lookup"><span data-stu-id="efd61-103">Get cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="efd61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efd61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efd61-105">Чтение свойств и связей объекта [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="efd61-105">Read the properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="efd61-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="efd61-106">Permissions</span></span>

<span data-ttu-id="efd61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efd61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efd61-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efd61-109">Permission type</span></span>| <span data-ttu-id="efd61-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="efd61-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="efd61-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efd61-111">Delegated (work or school account)</span></span>|<span data-ttu-id="efd61-112">Клаудпк. ReadWrite. ALL, Клаудпк. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="efd61-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="efd61-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efd61-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efd61-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efd61-114">Not supported.</span></span>|
|<span data-ttu-id="efd61-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efd61-115">Application</span></span>| <span data-ttu-id="efd61-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efd61-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efd61-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efd61-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="efd61-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="efd61-118">Optional query parameters</span></span>

<span data-ttu-id="efd61-119">Этот метод поддерживает `$select` параметр запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="efd61-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="efd61-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="efd61-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="efd61-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efd61-121">Request headers</span></span>

| <span data-ttu-id="efd61-122">Имя</span><span class="sxs-lookup"><span data-stu-id="efd61-122">Name</span></span>          | <span data-ttu-id="efd61-123">Описание</span><span class="sxs-lookup"><span data-stu-id="efd61-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="efd61-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efd61-124">Authorization</span></span> | <span data-ttu-id="efd61-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efd61-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="efd61-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efd61-127">Request body</span></span>

<span data-ttu-id="efd61-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="efd61-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efd61-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="efd61-129">Response</span></span>

<span data-ttu-id="efd61-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="efd61-130">If successful, this method returns a `200 OK` response code and a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="efd61-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="efd61-131">Examples</span></span>

### <a name="example-1-get-the-default-properties-of-an-on-premises-connection"></a><span data-ttu-id="efd61-132">Пример 1: получение свойств по умолчанию локального подключения</span><span class="sxs-lookup"><span data-stu-id="efd61-132">Example 1: Get the default properties of an on-premises connection</span></span>

#### <a name="request"></a><span data-ttu-id="efd61-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="efd61-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="efd61-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="efd61-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```
# <a name="c"></a>[<span data-ttu-id="efd61-135">C#</span><span class="sxs-lookup"><span data-stu-id="efd61-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpconpremisesconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="efd61-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="efd61-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpconpremisesconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="efd61-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="efd61-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpconpremisesconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="efd61-138">Java</span><span class="sxs-lookup"><span data-stu-id="efd61-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpconpremisesconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="efd61-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="efd61-139">Response</span></span>

<span data-ttu-id="efd61-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="efd61-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-the-selected-properties-of-an-on-premises-connection-including-healthcheckstatusdetails"></a><span data-ttu-id="efd61-141">Пример 2: Получение выбранных свойств локального подключения, включая Хеалсчеккстатусдетаилс</span><span class="sxs-lookup"><span data-stu-id="efd61-141">Example 2: Get the selected properties of an on-premises connection, including healthCheckStatusDetails</span></span>

#### <a name="request"></a><span data-ttu-id="efd61-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="efd61-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="efd61-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="efd61-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection_withDetails"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}?$select=id,displayName,subscriptionId,subscriptionName,adDomainName,adDomainUsername,organizationalUnit,virtualNetworkId,subnetId,healthCheckStatus,healthCheckStatusDetails,inUse
```
# <a name="c"></a>[<span data-ttu-id="efd61-144">C#</span><span class="sxs-lookup"><span data-stu-id="efd61-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpconpremisesconnection-withdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="efd61-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="efd61-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpconpremisesconnection-withdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="efd61-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="efd61-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpconpremisesconnection-withdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="efd61-147">Java</span><span class="sxs-lookup"><span data-stu-id="efd61-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpconpremisesconnection-withdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="efd61-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="efd61-148">Response</span></span>

<span data-ttu-id="efd61-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="efd61-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
