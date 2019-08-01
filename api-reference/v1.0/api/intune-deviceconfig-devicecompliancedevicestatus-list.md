---
title: List deviceComplianceDeviceStatuses
description: Перечисление свойств и связей объектов deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4020550623102063aadfb8d21fdc665d1b087673
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997794"
---
# <a name="list-devicecompliancedevicestatuses"></a><span data-ttu-id="a5a1c-103">List deviceComplianceDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a5a1c-103">List deviceComplianceDeviceStatuses</span></span>

> <span data-ttu-id="a5a1c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5a1c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5a1c-105">Перечисление свойств и связей объектов [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="a5a1c-105">List properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5a1c-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a5a1c-106">Prerequisites</span></span>
<span data-ttu-id="a5a1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5a1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5a1c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5a1c-109">Permission type</span></span>|<span data-ttu-id="a5a1c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5a1c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5a1c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5a1c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a5a1c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5a1c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a5a1c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5a1c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5a1c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5a1c-114">Not supported.</span></span>|
|<span data-ttu-id="a5a1c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5a1c-115">Application</span></span>|<span data-ttu-id="a5a1c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5a1c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5a1c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5a1c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a5a1c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5a1c-118">Request headers</span></span>
|<span data-ttu-id="a5a1c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5a1c-119">Header</span></span>|<span data-ttu-id="a5a1c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a5a1c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5a1c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5a1c-121">Authorization</span></span>|<span data-ttu-id="a5a1c-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5a1c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5a1c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a5a1c-123">Accept</span></span>|<span data-ttu-id="a5a1c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a5a1c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5a1c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a5a1c-125">Request body</span></span>
<span data-ttu-id="a5a1c-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5a1c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5a1c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5a1c-127">Response</span></span>
<span data-ttu-id="a5a1c-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a5a1c-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5a1c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a5a1c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5a1c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5a1c-130">Request</span></span>
<span data-ttu-id="a5a1c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5a1c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="a5a1c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5a1c-132">Response</span></span>
<span data-ttu-id="a5a1c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5a1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 544

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
      "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



