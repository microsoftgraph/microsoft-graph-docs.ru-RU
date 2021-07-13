---
title: Get cloudPcDevice
description: Ознакомьтесь с свойствами и отношениями объекта cloudPcDevice.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 26d9b438bf366a0a3b4b367bc96ea74441d5324d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402496"
---
# <a name="get-cloudpcdevice"></a><span data-ttu-id="7bf59-103">Get cloudPcDevice</span><span class="sxs-lookup"><span data-stu-id="7bf59-103">Get cloudPcDevice</span></span>
<span data-ttu-id="7bf59-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="7bf59-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bf59-105">Ознакомьтесь с свойствами и отношениями объекта [cloudPcDevice.](../resources/managedtenants-cloudpcdevice.md)</span><span class="sxs-lookup"><span data-stu-id="7bf59-105">Read the properties and relationships of a [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bf59-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bf59-106">Permissions</span></span>
<span data-ttu-id="7bf59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bf59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bf59-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bf59-109">Permission type</span></span>|<span data-ttu-id="7bf59-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bf59-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bf59-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bf59-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7bf59-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bf59-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="7bf59-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bf59-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bf59-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bf59-114">Not supported.</span></span>|
|<span data-ttu-id="7bf59-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bf59-115">Application</span></span>|<span data-ttu-id="7bf59-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bf59-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bf59-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bf59-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcDevices/{cloudPcDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7bf59-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7bf59-118">Optional query parameters</span></span>
<span data-ttu-id="7bf59-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="7bf59-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bf59-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bf59-120">Request headers</span></span>
|<span data-ttu-id="7bf59-121">Имя</span><span class="sxs-lookup"><span data-stu-id="7bf59-121">Name</span></span>|<span data-ttu-id="7bf59-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7bf59-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7bf59-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bf59-123">Authorization</span></span>|<span data-ttu-id="7bf59-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bf59-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bf59-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7bf59-126">Request body</span></span>
<span data-ttu-id="7bf59-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7bf59-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bf59-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bf59-128">Response</span></span>

<span data-ttu-id="7bf59-129">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7bf59-129">If successful, this method returns a `200 OK` response code and a [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7bf59-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="7bf59-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7bf59-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bf59-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_cloudpcdevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcDevices/{cloudPcDeviceId}
```


### <a name="response"></a><span data-ttu-id="7bf59-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bf59-132">Response</span></span>
><span data-ttu-id="7bf59-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7bf59-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.cloudPcDevice"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.managedTenants.cloudPcDevice",
    "id": "1307ab1b-63ee-4942-bdef-bcd4f415c635",
    "lastUpdated": "2021-07-10T23:05:03.2564744Z",
    "policyId": "",
    "displayName": "device01",
    "managedDeviceId": "",
    "managedDeviceName": "",
    "userPrincipalName": "sally@lucernepublishing001.onmicrosoft.com",
    "servicePlanName": "CloudPC_Standard",
    "status": "NotProvisioned",
    "tenantId": "aa060093-1e81-45b4-bebc-652713194ef7",
    "tenantDisplayName": "Lucerne Publishing",
    "lastRefreshedDateTime": "2021-07-10T23:05:03.2564744Z",
    "provisioningPolicyId": "",
    "cloudPcStatus": "NotProvisioned"
}
```
