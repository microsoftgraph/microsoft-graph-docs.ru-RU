---
title: Перечисление объектов settingStateDeviceSummary
description: Список свойств и связей объектов settingStateDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7807d5f7849db610b1fcb060c62ce4c760de376e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011468"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="d6eda-103">Перечисление объектов settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="d6eda-103">List settingStateDeviceSummaries</span></span>

<span data-ttu-id="d6eda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6eda-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6eda-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6eda-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6eda-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6eda-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6eda-107">Список свойств и связей объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d6eda-107">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6eda-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d6eda-108">Prerequisites</span></span>
<span data-ttu-id="d6eda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6eda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6eda-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6eda-111">Permission type</span></span>|<span data-ttu-id="d6eda-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6eda-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6eda-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6eda-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6eda-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6eda-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d6eda-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6eda-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6eda-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6eda-116">Not supported.</span></span>|
|<span data-ttu-id="d6eda-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d6eda-117">Application</span></span>|<span data-ttu-id="d6eda-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6eda-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6eda-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6eda-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="d6eda-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6eda-120">Request headers</span></span>
|<span data-ttu-id="d6eda-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6eda-121">Header</span></span>|<span data-ttu-id="d6eda-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d6eda-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6eda-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6eda-123">Authorization</span></span>|<span data-ttu-id="d6eda-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6eda-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6eda-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d6eda-125">Accept</span></span>|<span data-ttu-id="d6eda-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6eda-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6eda-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6eda-127">Request body</span></span>
<span data-ttu-id="d6eda-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6eda-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6eda-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6eda-129">Response</span></span>
<span data-ttu-id="d6eda-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6eda-130">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6eda-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d6eda-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6eda-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6eda-132">Request</span></span>
<span data-ttu-id="d6eda-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6eda-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="d6eda-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6eda-134">Response</span></span>
<span data-ttu-id="d6eda-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6eda-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
      "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
      "settingName": "Setting Name value",
      "instancePath": "Instance Path value",
      "unknownDeviceCount": 2,
      "notApplicableDeviceCount": 8,
      "compliantDeviceCount": 4,
      "remediatedDeviceCount": 5,
      "nonCompliantDeviceCount": 7,
      "errorDeviceCount": 0,
      "conflictDeviceCount": 3
    }
  ]
}
```






