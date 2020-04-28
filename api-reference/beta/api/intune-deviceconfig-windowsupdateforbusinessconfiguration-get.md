---
title: Get windowsUpdateForBusinessConfiguration
description: Чтение свойств и связей объекта windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a69f853967927996519bcf8e00f4f389cc186035
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43428531"
---
# <a name="get-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="81cf2-103">Get windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="81cf2-103">Get windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="81cf2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81cf2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81cf2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81cf2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81cf2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81cf2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81cf2-107">Чтение свойств и связей объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81cf2-107">Read properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81cf2-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="81cf2-108">Prerequisites</span></span>
<span data-ttu-id="81cf2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81cf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81cf2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81cf2-111">Permission type</span></span>|<span data-ttu-id="81cf2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="81cf2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81cf2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81cf2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81cf2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="81cf2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="81cf2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81cf2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81cf2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81cf2-116">Not supported.</span></span>|
|<span data-ttu-id="81cf2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81cf2-117">Application</span></span>|<span data-ttu-id="81cf2-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="81cf2-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81cf2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81cf2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81cf2-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="81cf2-120">Optional query parameters</span></span>
<span data-ttu-id="81cf2-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="81cf2-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81cf2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81cf2-122">Request headers</span></span>
|<span data-ttu-id="81cf2-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81cf2-123">Header</span></span>|<span data-ttu-id="81cf2-124">Значение</span><span class="sxs-lookup"><span data-stu-id="81cf2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81cf2-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81cf2-125">Authorization</span></span>|<span data-ttu-id="81cf2-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81cf2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81cf2-127">Accept</span><span class="sxs-lookup"><span data-stu-id="81cf2-127">Accept</span></span>|<span data-ttu-id="81cf2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="81cf2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81cf2-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="81cf2-129">Request body</span></span>
<span data-ttu-id="81cf2-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81cf2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81cf2-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="81cf2-131">Response</span></span>
<span data-ttu-id="81cf2-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="81cf2-132">If successful, this method returns a `200 OK` response code and [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81cf2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="81cf2-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="81cf2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="81cf2-134">Request</span></span>
<span data-ttu-id="81cf2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81cf2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="81cf2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="81cf2-136">Response</span></span>
<span data-ttu-id="81cf2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="81cf2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3173

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
    "id": "4928dd6a-dd6a-4928-6add-28496add2849",
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
    "deliveryOptimizationMode": "httpOnly",
    "prereleaseFeatures": "settingsOnly",
    "automaticUpdateMode": "notifyDownload",
    "microsoftUpdateServiceAllowed": true,
    "driversExcluded": true,
    "installationSchedule": {
      "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
      "scheduledInstallDay": "everyday",
      "scheduledInstallTime": "11:59:31.3170000"
    },
    "qualityUpdatesDeferralPeriodInDays": 2,
    "featureUpdatesDeferralPeriodInDays": 2,
    "qualityUpdatesPaused": true,
    "featureUpdatesPaused": true,
    "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
    "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
    "businessReadyUpdatesOnly": "all",
    "skipChecksBeforeRestart": true,
    "updateWeeks": "firstWeek",
    "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
    "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
    "featureUpdatesRollbackWindowInDays": 2,
    "qualityUpdatesWillBeRolledBack": true,
    "featureUpdatesWillBeRolledBack": true,
    "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
    "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
    "engagedRestartDeadlineInDays": 12,
    "engagedRestartSnoozeScheduleInDays": 2,
    "engagedRestartTransitionScheduleInDays": 6,
    "deadlineForFeatureUpdatesInDays": 15,
    "deadlineForQualityUpdatesInDays": 15,
    "deadlineGracePeriodInDays": 9,
    "postponeRebootUntilAfterDeadline": true,
    "autoRestartNotificationDismissal": "automatic",
    "scheduleRestartWarningInHours": 13,
    "scheduleImminentRestartWarningInMinutes": 7,
    "userPauseAccess": "enabled",
    "userWindowsUpdateScanAccess": "enabled",
    "updateNotificationLevel": "defaultNotifications"
  }
}
```



