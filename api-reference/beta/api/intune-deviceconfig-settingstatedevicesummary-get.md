---
title: Get settingStateDeviceSummary
description: Чтение свойств и связей объекта settingStateDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4228a644b5bd214db3977554528555d6a3163c6c
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792662"
---
# <a name="get-settingstatedevicesummary"></a><span data-ttu-id="2acf7-103">Get settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="2acf7-103">Get settingStateDeviceSummary</span></span>

<span data-ttu-id="2acf7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2acf7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2acf7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2acf7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2acf7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2acf7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2acf7-107">Чтение свойств и связей объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="2acf7-107">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2acf7-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2acf7-108">Prerequisites</span></span>
<span data-ttu-id="2acf7-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="2acf7-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2acf7-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2acf7-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2acf7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2acf7-111">Permission type</span></span>|<span data-ttu-id="2acf7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2acf7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2acf7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2acf7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2acf7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2acf7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2acf7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2acf7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2acf7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2acf7-116">Not supported.</span></span>|
|<span data-ttu-id="2acf7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2acf7-117">Application</span></span>|<span data-ttu-id="2acf7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2acf7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2acf7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2acf7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2acf7-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2acf7-120">Optional query parameters</span></span>
<span data-ttu-id="2acf7-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2acf7-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2acf7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2acf7-122">Request headers</span></span>
|<span data-ttu-id="2acf7-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2acf7-123">Header</span></span>|<span data-ttu-id="2acf7-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2acf7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2acf7-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2acf7-125">Authorization</span></span>|<span data-ttu-id="2acf7-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2acf7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2acf7-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2acf7-127">Accept</span></span>|<span data-ttu-id="2acf7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2acf7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2acf7-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2acf7-129">Request body</span></span>
<span data-ttu-id="2acf7-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2acf7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2acf7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2acf7-131">Response</span></span>
<span data-ttu-id="2acf7-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2acf7-132">If successful, this method returns a `200 OK` response code and [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2acf7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2acf7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2acf7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2acf7-134">Request</span></span>
<span data-ttu-id="2acf7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2acf7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="2acf7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2acf7-136">Response</span></span>
<span data-ttu-id="2acf7-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="2acf7-137">Here is an example of the response.</span></span> <span data-ttu-id="2acf7-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="2acf7-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2acf7-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="2acf7-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": {
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
}
```



