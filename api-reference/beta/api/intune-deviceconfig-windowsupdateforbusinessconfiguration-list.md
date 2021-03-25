---
title: Перечисление объектов windowsUpdateForBusinessConfiguration
description: Перечисление свойств и связей объектов windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 21968a002c6677e001744d29699e31f4662b8576
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154639"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="47f76-103">Перечисление объектов windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="47f76-103">List windowsUpdateForBusinessConfigurations</span></span>

<span data-ttu-id="47f76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47f76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47f76-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47f76-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47f76-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47f76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47f76-107">Перечисление свойств и связей объектов [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47f76-107">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47f76-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="47f76-108">Prerequisites</span></span>
<span data-ttu-id="47f76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47f76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47f76-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47f76-111">Permission type</span></span>|<span data-ttu-id="47f76-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47f76-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47f76-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47f76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47f76-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47f76-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47f76-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47f76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47f76-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47f76-116">Not supported.</span></span>|
|<span data-ttu-id="47f76-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="47f76-117">Application</span></span>|<span data-ttu-id="47f76-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47f76-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47f76-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47f76-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="47f76-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="47f76-120">Request headers</span></span>
|<span data-ttu-id="47f76-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47f76-121">Header</span></span>|<span data-ttu-id="47f76-122">Значение</span><span class="sxs-lookup"><span data-stu-id="47f76-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47f76-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47f76-123">Authorization</span></span>|<span data-ttu-id="47f76-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47f76-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47f76-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47f76-125">Accept</span></span>|<span data-ttu-id="47f76-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47f76-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47f76-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47f76-127">Request body</span></span>
<span data-ttu-id="47f76-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47f76-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47f76-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="47f76-129">Response</span></span>
<span data-ttu-id="47f76-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="47f76-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47f76-131">Пример</span><span class="sxs-lookup"><span data-stu-id="47f76-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="47f76-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="47f76-132">Request</span></span>
<span data-ttu-id="47f76-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47f76-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="47f76-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="47f76-134">Response</span></span>
<span data-ttu-id="47f76-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47f76-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3283

{
  "value": [
    {
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
      "qualityUpdatesPauseStartDate": "2016-12-31",
      "featureUpdatesPauseStartDate": "2016-12-31",
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
  ]
}
```




