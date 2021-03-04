---
title: Get aospDeviceOwnerDeviceConfiguration
description: Чтение свойств и связей объекта aospDeviceOwnerDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4beda8c8f41849565de72bbb33b9440d85bc2e32
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446780"
---
# <a name="get-aospdeviceownerdeviceconfiguration"></a><span data-ttu-id="646cb-103">Get aospDeviceOwnerDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="646cb-103">Get aospDeviceOwnerDeviceConfiguration</span></span>

<span data-ttu-id="646cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="646cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="646cb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="646cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="646cb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="646cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="646cb-107">Чтение свойств и связей [объекта aospDeviceOwnerDeviceConfiguration.](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="646cb-107">Read properties and relationships of the [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="646cb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="646cb-108">Prerequisites</span></span>
<span data-ttu-id="646cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="646cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="646cb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="646cb-111">Permission type</span></span>|<span data-ttu-id="646cb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="646cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="646cb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="646cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="646cb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="646cb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="646cb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="646cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="646cb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="646cb-116">Not supported.</span></span>|
|<span data-ttu-id="646cb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="646cb-117">Application</span></span>|<span data-ttu-id="646cb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="646cb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="646cb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="646cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="646cb-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="646cb-120">Optional query parameters</span></span>
<span data-ttu-id="646cb-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="646cb-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="646cb-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="646cb-122">Request headers</span></span>
|<span data-ttu-id="646cb-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="646cb-123">Header</span></span>|<span data-ttu-id="646cb-124">Значение</span><span class="sxs-lookup"><span data-stu-id="646cb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="646cb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="646cb-125">Authorization</span></span>|<span data-ttu-id="646cb-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="646cb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="646cb-127">Accept</span><span class="sxs-lookup"><span data-stu-id="646cb-127">Accept</span></span>|<span data-ttu-id="646cb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="646cb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="646cb-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="646cb-129">Request body</span></span>
<span data-ttu-id="646cb-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="646cb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="646cb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="646cb-131">Response</span></span>
<span data-ttu-id="646cb-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="646cb-132">If successful, this method returns a `200 OK` response code and [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="646cb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="646cb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="646cb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="646cb-134">Request</span></span>
<span data-ttu-id="646cb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="646cb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="646cb-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="646cb-136">Response</span></span>
<span data-ttu-id="646cb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="646cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2012

{
  "value": {
    "@odata.type": "#microsoft.graph.aospDeviceOwnerDeviceConfiguration",
    "id": "c9e83a69-3a69-c9e8-693a-e8c9693ae8c9",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "deviceManagementApplicabilityRuleOsEdition": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
      "osEditionTypes": [
        "windows10EnterpriseN"
      ],
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleOsVersion": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
      "minOSVersion": "Min OSVersion value",
      "maxOSVersion": "Max OSVersion value",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleDeviceMode": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
      "deviceMode": "sModeConfiguration",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "appsAllowInstallFromUnknownSources": true,
    "bluetoothBlocked": true,
    "bluetoothBlockConfiguration": true,
    "bluetoothBlockContactSharing": true,
    "cameraBlocked": true,
    "cellularBlockWiFiTethering": true,
    "factoryResetBlocked": true,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordRequiredType": "required",
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "screenCaptureBlocked": true,
    "securityAllowDebuggingFeatures": true,
    "storageAllowUsb": true,
    "storageBlockExternalMedia": true,
    "storageBlockUsbFileTransfer": true,
    "backupBlocked": true,
    "wifiBlockEditConfigurations": true
  }
}
```




