---
title: Get settingStateDeviceSummary
description: Чтение свойств и связей объекта settingStateDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8339515b11db7978d22995c19ee3b0c2e098e8a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129638"
---
# <a name="get-settingstatedevicesummary"></a><span data-ttu-id="4a7b4-103">Get settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="4a7b4-103">Get settingStateDeviceSummary</span></span>

<span data-ttu-id="4a7b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a7b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a7b4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a7b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a7b4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a7b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a7b4-107">Чтение свойств и связей объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4a7b4-107">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a7b4-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4a7b4-108">Prerequisites</span></span>
<span data-ttu-id="4a7b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a7b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a7b4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a7b4-111">Permission type</span></span>|<span data-ttu-id="4a7b4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a7b4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a7b4-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a7b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a7b4-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a7b4-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a7b4-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a7b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a7b4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a7b4-116">Not supported.</span></span>|
|<span data-ttu-id="4a7b4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4a7b4-117">Application</span></span>|<span data-ttu-id="4a7b4-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a7b4-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a7b4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a7b4-119">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a7b4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4a7b4-120">Optional query parameters</span></span>
<span data-ttu-id="4a7b4-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4a7b4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a7b4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a7b4-122">Request headers</span></span>
|<span data-ttu-id="4a7b4-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a7b4-123">Header</span></span>|<span data-ttu-id="4a7b4-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4a7b4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a7b4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a7b4-125">Authorization</span></span>|<span data-ttu-id="4a7b4-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a7b4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a7b4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4a7b4-127">Accept</span></span>|<span data-ttu-id="4a7b4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4a7b4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a7b4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a7b4-129">Request body</span></span>
<span data-ttu-id="4a7b4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a7b4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a7b4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a7b4-131">Response</span></span>
<span data-ttu-id="4a7b4-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4a7b4-132">If successful, this method returns a `200 OK` response code and [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a7b4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4a7b4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a7b4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a7b4-134">Request</span></span>
<span data-ttu-id="4a7b4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a7b4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="4a7b4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a7b4-136">Response</span></span>
<span data-ttu-id="4a7b4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a7b4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




