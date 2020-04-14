---
title: Get windows10TeamGeneralConfiguration
description: Чтение свойств и связей объекта windows10TeamGeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b5c3e931090f066e8ae84cca9fd12f64b7eeb55a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43338127"
---
# <a name="get-windows10teamgeneralconfiguration"></a><span data-ttu-id="4ce22-103">Get windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ce22-103">Get windows10TeamGeneralConfiguration</span></span>

<span data-ttu-id="4ce22-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ce22-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ce22-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ce22-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ce22-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ce22-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ce22-107">Чтение свойств и связей объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ce22-107">Read properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ce22-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4ce22-108">Prerequisites</span></span>
<span data-ttu-id="4ce22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ce22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ce22-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ce22-111">Permission type</span></span>|<span data-ttu-id="4ce22-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ce22-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ce22-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ce22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ce22-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ce22-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4ce22-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ce22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ce22-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ce22-116">Not supported.</span></span>|
|<span data-ttu-id="4ce22-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="4ce22-117">Application</span></span>|<span data-ttu-id="4ce22-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ce22-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ce22-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ce22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ce22-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ce22-120">Optional query parameters</span></span>
<span data-ttu-id="4ce22-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4ce22-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ce22-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ce22-122">Request headers</span></span>
|<span data-ttu-id="4ce22-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ce22-123">Header</span></span>|<span data-ttu-id="4ce22-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4ce22-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ce22-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ce22-125">Authorization</span></span>|<span data-ttu-id="4ce22-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ce22-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ce22-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4ce22-127">Accept</span></span>|<span data-ttu-id="4ce22-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4ce22-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ce22-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ce22-129">Request body</span></span>
<span data-ttu-id="4ce22-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ce22-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ce22-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ce22-131">Response</span></span>
<span data-ttu-id="4ce22-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4ce22-132">If successful, this method returns a `200 OK` response code and [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ce22-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4ce22-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ce22-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ce22-134">Request</span></span>
<span data-ttu-id="4ce22-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ce22-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="4ce22-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ce22-136">Response</span></span>
<span data-ttu-id="4ce22-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ce22-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2310

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
    "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
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
    "azureOperationalInsightsBlockTelemetry": true,
    "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
    "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
    "connectAppBlockAutoLaunch": true,
    "maintenanceWindowBlocked": true,
    "maintenanceWindowDurationInHours": 0,
    "maintenanceWindowStartTime": "11:59:09.3130000",
    "miracastChannel": "one",
    "miracastBlocked": true,
    "miracastRequirePin": true,
    "settingsBlockMyMeetingsAndFiles": true,
    "settingsBlockSessionResume": true,
    "settingsBlockSigninSuggestions": true,
    "settingsDefaultVolume": 5,
    "settingsScreenTimeoutInMinutes": 14,
    "settingsSessionTimeoutInMinutes": 15,
    "settingsSleepTimeoutInMinutes": 13,
    "welcomeScreenBlockAutomaticWakeUp": true,
    "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
    "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
  }
}
```



