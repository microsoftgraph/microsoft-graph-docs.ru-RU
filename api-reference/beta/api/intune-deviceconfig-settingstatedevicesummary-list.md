---
title: Перечисление объектов settingStateDeviceSummary
description: Список свойств и связей объектов settingStateDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db24698dc3d043a0568e40020871d366103eb302
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792655"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="af4cb-103">Перечисление объектов settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="af4cb-103">List settingStateDeviceSummaries</span></span>

<span data-ttu-id="af4cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af4cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af4cb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af4cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af4cb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af4cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af4cb-107">Список свойств и связей объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="af4cb-107">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af4cb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="af4cb-108">Prerequisites</span></span>
<span data-ttu-id="af4cb-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="af4cb-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="af4cb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af4cb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af4cb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af4cb-111">Permission type</span></span>|<span data-ttu-id="af4cb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af4cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af4cb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af4cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af4cb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="af4cb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="af4cb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af4cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af4cb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af4cb-116">Not supported.</span></span>|
|<span data-ttu-id="af4cb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af4cb-117">Application</span></span>|<span data-ttu-id="af4cb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="af4cb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af4cb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af4cb-119">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="af4cb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="af4cb-120">Request headers</span></span>
|<span data-ttu-id="af4cb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af4cb-121">Header</span></span>|<span data-ttu-id="af4cb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="af4cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af4cb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af4cb-123">Authorization</span></span>|<span data-ttu-id="af4cb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af4cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af4cb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="af4cb-125">Accept</span></span>|<span data-ttu-id="af4cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af4cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af4cb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="af4cb-127">Request body</span></span>
<span data-ttu-id="af4cb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="af4cb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af4cb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="af4cb-129">Response</span></span>
<span data-ttu-id="af4cb-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af4cb-130">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af4cb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="af4cb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="af4cb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="af4cb-132">Request</span></span>
<span data-ttu-id="af4cb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af4cb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="af4cb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="af4cb-134">Response</span></span>
<span data-ttu-id="af4cb-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="af4cb-135">Here is an example of the response.</span></span> <span data-ttu-id="af4cb-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="af4cb-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="af4cb-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="af4cb-137">All of the properties will be returned from an actual call.</span></span>
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



