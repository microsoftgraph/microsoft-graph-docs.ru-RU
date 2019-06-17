---
title: Перечисление объектов settingStateDeviceSummary
description: Список свойств и связей объектов settingStateDeviceSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05e7007e795a7b174b89574576a4f40c9a8f0d6f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962892"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="0b3ac-103">Перечисление объектов settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="0b3ac-103">List settingStateDeviceSummaries</span></span>

> <span data-ttu-id="0b3ac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b3ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b3ac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b3ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b3ac-106">Список свойств и связей объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="0b3ac-106">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b3ac-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0b3ac-107">Prerequisites</span></span>
<span data-ttu-id="0b3ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b3ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b3ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b3ac-110">Permission type</span></span>|<span data-ttu-id="0b3ac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b3ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b3ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b3ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b3ac-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b3ac-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0b3ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b3ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b3ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b3ac-115">Not supported.</span></span>|
|<span data-ttu-id="0b3ac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b3ac-116">Application</span></span>|<span data-ttu-id="0b3ac-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b3ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b3ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b3ac-118">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="0b3ac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b3ac-119">Request headers</span></span>
|<span data-ttu-id="0b3ac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b3ac-120">Header</span></span>|<span data-ttu-id="0b3ac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0b3ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b3ac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b3ac-122">Authorization</span></span>|<span data-ttu-id="0b3ac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b3ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b3ac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0b3ac-124">Accept</span></span>|<span data-ttu-id="0b3ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b3ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b3ac-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0b3ac-126">Request body</span></span>
<span data-ttu-id="0b3ac-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b3ac-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b3ac-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0b3ac-128">Response</span></span>
<span data-ttu-id="0b3ac-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0b3ac-129">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b3ac-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0b3ac-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b3ac-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b3ac-131">Request</span></span>
<span data-ttu-id="0b3ac-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b3ac-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="0b3ac-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b3ac-133">Response</span></span>
<span data-ttu-id="0b3ac-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b3ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





