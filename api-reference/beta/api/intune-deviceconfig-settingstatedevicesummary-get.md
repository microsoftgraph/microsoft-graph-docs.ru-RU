---
title: Get settingStateDeviceSummary
description: Чтение свойств и связей объекта settingStateDeviceSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: afcc7b79d0456f30b22fb9b282e04d57659cdfd4
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533336"
---
# <a name="get-settingstatedevicesummary"></a><span data-ttu-id="2e888-103">Get settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="2e888-103">Get settingStateDeviceSummary</span></span>

> <span data-ttu-id="2e888-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e888-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e888-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e888-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e888-106">Чтение свойств и связей объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="2e888-106">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e888-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2e888-107">Prerequisites</span></span>
<span data-ttu-id="2e888-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e888-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e888-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e888-110">Permission type</span></span>|<span data-ttu-id="2e888-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e888-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e888-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e888-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2e888-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e888-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2e888-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e888-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e888-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e888-115">Not supported.</span></span>|
|<span data-ttu-id="2e888-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2e888-116">Application</span></span>|<span data-ttu-id="2e888-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e888-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e888-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e888-118">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e888-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2e888-119">Optional query parameters</span></span>
<span data-ttu-id="2e888-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2e888-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e888-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e888-121">Request headers</span></span>
|<span data-ttu-id="2e888-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e888-122">Header</span></span>|<span data-ttu-id="2e888-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2e888-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e888-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e888-124">Authorization</span></span>|<span data-ttu-id="2e888-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e888-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e888-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2e888-126">Accept</span></span>|<span data-ttu-id="2e888-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2e888-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e888-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e888-128">Request body</span></span>
<span data-ttu-id="2e888-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e888-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e888-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e888-130">Response</span></span>
<span data-ttu-id="2e888-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2e888-131">If successful, this method returns a `200 OK` response code and [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e888-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2e888-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e888-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e888-133">Request</span></span>
<span data-ttu-id="2e888-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e888-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="2e888-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e888-135">Response</span></span>
<span data-ttu-id="2e888-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e888-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






