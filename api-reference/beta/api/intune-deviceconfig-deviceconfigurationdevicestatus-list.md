---
title: Перечисление объектов deviceConfigurationDeviceStatus
description: Список свойств и связей объектов deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cce92f80f686e7e97fe69d023b34a3599bc47387
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131619"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="b4775-103">Перечисление объектов deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b4775-103">List deviceConfigurationDeviceStatuses</span></span>

<span data-ttu-id="b4775-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4775-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4775-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4775-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4775-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4775-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4775-107">Список свойств и связей объектов [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b4775-107">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4775-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b4775-108">Prerequisites</span></span>
<span data-ttu-id="b4775-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4775-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4775-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4775-111">Permission type</span></span>|<span data-ttu-id="b4775-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4775-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4775-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4775-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4775-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4775-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4775-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4775-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4775-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4775-116">Not supported.</span></span>|
|<span data-ttu-id="b4775-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b4775-117">Application</span></span>|<span data-ttu-id="b4775-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4775-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4775-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4775-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b4775-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b4775-120">Request headers</span></span>
|<span data-ttu-id="b4775-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4775-121">Header</span></span>|<span data-ttu-id="b4775-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b4775-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4775-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4775-123">Authorization</span></span>|<span data-ttu-id="b4775-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4775-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4775-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b4775-125">Accept</span></span>|<span data-ttu-id="b4775-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4775-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4775-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4775-127">Request body</span></span>
<span data-ttu-id="b4775-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4775-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4775-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4775-129">Response</span></span>
<span data-ttu-id="b4775-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4775-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4775-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b4775-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4775-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4775-132">Request</span></span>
<span data-ttu-id="b4775-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4775-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="b4775-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4775-134">Response</span></span>
<span data-ttu-id="b4775-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4775-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 569

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
      "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "platform": 8,
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




