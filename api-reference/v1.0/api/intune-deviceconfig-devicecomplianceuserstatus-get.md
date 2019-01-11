---
title: Get deviceComplianceUserStatus
description: Чтение свойств и связей объекта deviceComplianceUserStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5b1e091b61e467575035669bd87670927688f437
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804846"
---
# <a name="get-devicecomplianceuserstatus"></a><span data-ttu-id="7d91a-103">Get deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="7d91a-103">Get deviceComplianceUserStatus</span></span>

> <span data-ttu-id="7d91a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7d91a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d91a-105">Чтение свойств и связей объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="7d91a-105">Read properties and relationships of the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d91a-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7d91a-106">Prerequisites</span></span>
<span data-ttu-id="7d91a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d91a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d91a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d91a-109">Permission type</span></span>|<span data-ttu-id="7d91a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d91a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d91a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d91a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7d91a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d91a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7d91a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d91a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d91a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d91a-114">Not supported.</span></span>|
|<span data-ttu-id="7d91a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d91a-115">Application</span></span>|<span data-ttu-id="7d91a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d91a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d91a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d91a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d91a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7d91a-118">Optional query parameters</span></span>
<span data-ttu-id="7d91a-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7d91a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7d91a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d91a-120">Request headers</span></span>
|<span data-ttu-id="7d91a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d91a-121">Header</span></span>|<span data-ttu-id="7d91a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7d91a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d91a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d91a-123">Authorization</span></span>|<span data-ttu-id="7d91a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7d91a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d91a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d91a-125">Accept</span></span>|<span data-ttu-id="7d91a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d91a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d91a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7d91a-127">Request body</span></span>
<span data-ttu-id="7d91a-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d91a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d91a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="7d91a-129">Response</span></span>
<span data-ttu-id="7d91a-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7d91a-130">If successful, this method returns a `200 OK` response code and [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d91a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7d91a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7d91a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d91a-132">Request</span></span>
<span data-ttu-id="7d91a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d91a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

### <a name="response"></a><span data-ttu-id="7d91a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="7d91a-134">Response</span></span>
<span data-ttu-id="7d91a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7d91a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 369

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
    "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
    "userDisplayName": "User Display Name value",
    "devicesCount": 12,
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



