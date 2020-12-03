---
title: Список Клаудпконпремисесконнектион
description: Получение списка объектов Клаудпконпремисесконнектион и их свойств.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: b27ab1156309b47c9e613a9e37e32ffe69f79eb5
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563888"
---
# <a name="list-onpremisesconnections"></a><span data-ttu-id="531c7-103">Список Онпремисесконнектионс</span><span class="sxs-lookup"><span data-stu-id="531c7-103">List onPremisesConnections</span></span>

<span data-ttu-id="531c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="531c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="531c7-105">Список свойств и связей объектов [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="531c7-105">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="531c7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="531c7-106">Permissions</span></span>

<span data-ttu-id="531c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="531c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="531c7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="531c7-109">Permission type</span></span>|<span data-ttu-id="531c7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="531c7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="531c7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="531c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="531c7-112">Клаудпк. ReadWrite. ALL, Клаудпк. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="531c7-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="531c7-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="531c7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="531c7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="531c7-114">Not supported.</span></span>|
|<span data-ttu-id="531c7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="531c7-115">Application</span></span>|<span data-ttu-id="531c7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="531c7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="531c7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="531c7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/onPremisesConnections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="531c7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="531c7-118">Optional query parameters</span></span>

<span data-ttu-id="531c7-119">Этот метод поддерживает `$select` и `$filter` параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="531c7-119">This method supports `$select` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="531c7-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="531c7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="531c7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="531c7-121">Request headers</span></span>

| <span data-ttu-id="531c7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="531c7-122">Name</span></span>          | <span data-ttu-id="531c7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="531c7-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="531c7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="531c7-124">Authorization</span></span> | <span data-ttu-id="531c7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="531c7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="531c7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="531c7-127">Request body</span></span>

<span data-ttu-id="531c7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="531c7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="531c7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="531c7-129">Response</span></span>

<span data-ttu-id="531c7-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="531c7-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="531c7-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="531c7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="531c7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="531c7-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="531c7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="531c7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpconpremisesconnections"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections
```
# <a name="c"></a>[<span data-ttu-id="531c7-134">C#</span><span class="sxs-lookup"><span data-stu-id="531c7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpconpremisesconnections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="531c7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="531c7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpconpremisesconnections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="531c7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="531c7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpconpremisesconnections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="531c7-137">Java</span><span class="sxs-lookup"><span data-stu-id="531c7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpconpremisesconnections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="531c7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="531c7-138">Response</span></span>

<span data-ttu-id="531c7-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="531c7-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcOnPremisesConnection)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
      "id": "07f12770-a225-4957-9127-0d247cf4ffff",
      "displayName": "Display Name value",
      "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
      "subscriptionName": "Subscription Name value",
      "adDomainName": "Active Directory Domain Name value",
      "adDomainUsername": "Active Directory Domain User Name value",
      "organizationalUnit": "Organization Unit value",
      "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
      "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
      "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default",
      "healthCheckStatus": "passed",
      "inUse": false
    }
  ]
}
```
