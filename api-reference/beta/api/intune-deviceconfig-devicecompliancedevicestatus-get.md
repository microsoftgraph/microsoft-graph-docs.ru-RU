---
title: Get deviceComplianceDeviceStatus
description: Чтение свойств и связей объекта deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bad46ca2d3a62392d076bf6c2505025c19569804
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150052"
---
# <a name="get-devicecompliancedevicestatus"></a><span data-ttu-id="54aca-103">Get deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="54aca-103">Get deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="54aca-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54aca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54aca-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54aca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54aca-106">Чтение свойств и связей объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="54aca-106">Read properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54aca-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="54aca-107">Prerequisites</span></span>
<span data-ttu-id="54aca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="54aca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="54aca-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54aca-110">Permission type</span></span>|<span data-ttu-id="54aca-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="54aca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54aca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54aca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54aca-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="54aca-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="54aca-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54aca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54aca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54aca-115">Not supported.</span></span>|
|<span data-ttu-id="54aca-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54aca-116">Application</span></span>|<span data-ttu-id="54aca-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54aca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54aca-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54aca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54aca-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="54aca-119">Optional query parameters</span></span>
<span data-ttu-id="54aca-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="54aca-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54aca-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54aca-121">Request headers</span></span>
|<span data-ttu-id="54aca-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54aca-122">Header</span></span>|<span data-ttu-id="54aca-123">Значение</span><span class="sxs-lookup"><span data-stu-id="54aca-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54aca-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="54aca-124">Authorization</span></span>|<span data-ttu-id="54aca-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="54aca-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54aca-126">Accept</span><span class="sxs-lookup"><span data-stu-id="54aca-126">Accept</span></span>|<span data-ttu-id="54aca-127">application/json</span><span class="sxs-lookup"><span data-stu-id="54aca-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54aca-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54aca-128">Request body</span></span>
<span data-ttu-id="54aca-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54aca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54aca-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="54aca-130">Response</span></span>
<span data-ttu-id="54aca-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="54aca-131">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54aca-132">Пример</span><span class="sxs-lookup"><span data-stu-id="54aca-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="54aca-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="54aca-133">Request</span></span>
<span data-ttu-id="54aca-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54aca-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="54aca-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="54aca-135">Response</span></span>
<span data-ttu-id="54aca-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="54aca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 532

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
    "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "platform": 8,
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```




