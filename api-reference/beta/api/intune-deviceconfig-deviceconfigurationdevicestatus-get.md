---
title: Get deviceConfigurationDeviceStatus
description: Чтение свойств и связей объекта deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0b1e6033fc6d21d3a24f22cc6a1897abb921b4c
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792942"
---
# <a name="get-deviceconfigurationdevicestatus"></a><span data-ttu-id="2c095-103">Get deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="2c095-103">Get deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="2c095-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c095-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c095-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c095-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c095-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c095-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c095-107">Чтение свойств и связей объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="2c095-107">Read properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c095-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2c095-108">Prerequisites</span></span>
<span data-ttu-id="2c095-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c095-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c095-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c095-111">Permission type</span></span>|<span data-ttu-id="2c095-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c095-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c095-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c095-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2c095-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c095-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2c095-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c095-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c095-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c095-116">Not supported.</span></span>|
|<span data-ttu-id="2c095-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c095-117">Application</span></span>|<span data-ttu-id="2c095-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c095-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c095-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c095-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c095-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2c095-120">Optional query parameters</span></span>
<span data-ttu-id="2c095-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2c095-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c095-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c095-122">Request headers</span></span>
|<span data-ttu-id="2c095-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c095-123">Header</span></span>|<span data-ttu-id="2c095-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2c095-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c095-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c095-125">Authorization</span></span>|<span data-ttu-id="2c095-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c095-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c095-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2c095-127">Accept</span></span>|<span data-ttu-id="2c095-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2c095-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c095-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c095-129">Request body</span></span>
<span data-ttu-id="2c095-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2c095-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c095-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c095-131">Response</span></span>
<span data-ttu-id="2c095-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2c095-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c095-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2c095-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c095-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c095-134">Request</span></span>
<span data-ttu-id="2c095-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c095-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="2c095-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c095-136">Response</span></span>
<span data-ttu-id="2c095-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c095-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 535

{
  "value": {
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
}
```



