---
title: Перечисление объектов settingStateDeviceSummary
description: Список свойств и связей объектов settingStateDeviceSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9deff69a6a2c97888bec7830bc60e3a0220d84bf
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38083013"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="30c3a-103">Перечисление объектов settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="30c3a-103">List settingStateDeviceSummaries</span></span>

> <span data-ttu-id="30c3a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30c3a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30c3a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30c3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30c3a-106">Список свойств и связей объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="30c3a-106">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30c3a-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="30c3a-107">Prerequisites</span></span>
<span data-ttu-id="30c3a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30c3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30c3a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30c3a-110">Permission type</span></span>|<span data-ttu-id="30c3a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30c3a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30c3a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30c3a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30c3a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="30c3a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="30c3a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30c3a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30c3a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30c3a-115">Not supported.</span></span>|
|<span data-ttu-id="30c3a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30c3a-116">Application</span></span>|<span data-ttu-id="30c3a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="30c3a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30c3a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30c3a-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="30c3a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="30c3a-119">Request headers</span></span>
|<span data-ttu-id="30c3a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30c3a-120">Header</span></span>|<span data-ttu-id="30c3a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="30c3a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30c3a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30c3a-122">Authorization</span></span>|<span data-ttu-id="30c3a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30c3a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30c3a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="30c3a-124">Accept</span></span>|<span data-ttu-id="30c3a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="30c3a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30c3a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30c3a-126">Request body</span></span>
<span data-ttu-id="30c3a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30c3a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30c3a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="30c3a-128">Response</span></span>
<span data-ttu-id="30c3a-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30c3a-129">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30c3a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="30c3a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="30c3a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="30c3a-131">Request</span></span>
<span data-ttu-id="30c3a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30c3a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="30c3a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="30c3a-133">Response</span></span>
<span data-ttu-id="30c3a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30c3a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






