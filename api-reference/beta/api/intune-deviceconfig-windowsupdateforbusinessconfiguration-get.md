---
title: Get windowsUpdateForBusinessConfiguration
description: Чтение свойств и связей объекта windowsUpdateForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 872846a4a9d72fa4b685a51a6727fb794ce3c75b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162743"
---
# <a name="get-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="87f44-103">Get windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="87f44-103">Get windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="87f44-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87f44-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87f44-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87f44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87f44-106">Чтение свойств и связей объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87f44-106">Read properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87f44-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="87f44-107">Prerequisites</span></span>
<span data-ttu-id="87f44-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="87f44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="87f44-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87f44-110">Permission type</span></span>|<span data-ttu-id="87f44-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87f44-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87f44-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87f44-112">Delegated (work or school account)</span></span>|<span data-ttu-id="87f44-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87f44-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87f44-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87f44-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87f44-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87f44-115">Not supported.</span></span>|
|<span data-ttu-id="87f44-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87f44-116">Application</span></span>|<span data-ttu-id="87f44-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87f44-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87f44-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87f44-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87f44-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="87f44-119">Optional query parameters</span></span>
<span data-ttu-id="87f44-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="87f44-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87f44-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87f44-121">Request headers</span></span>
|<span data-ttu-id="87f44-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87f44-122">Header</span></span>|<span data-ttu-id="87f44-123">Значение</span><span class="sxs-lookup"><span data-stu-id="87f44-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87f44-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87f44-124">Authorization</span></span>|<span data-ttu-id="87f44-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="87f44-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87f44-126">Accept</span><span class="sxs-lookup"><span data-stu-id="87f44-126">Accept</span></span>|<span data-ttu-id="87f44-127">application/json</span><span class="sxs-lookup"><span data-stu-id="87f44-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87f44-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87f44-128">Request body</span></span>
<span data-ttu-id="87f44-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87f44-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87f44-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="87f44-130">Response</span></span>
<span data-ttu-id="87f44-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="87f44-131">If successful, this method returns a `200 OK` response code and [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87f44-132">Пример</span><span class="sxs-lookup"><span data-stu-id="87f44-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="87f44-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="87f44-133">Request</span></span>
<span data-ttu-id="87f44-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87f44-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="87f44-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="87f44-135">Response</span></span>
<span data-ttu-id="87f44-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="87f44-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2083

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
    "id": "4928dd6a-dd6a-4928-6add-28496add2849",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
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
    "autoRestartNotificationDismissal": "automatic",
    "scheduleRestartWarningInHours": 13,
    "scheduleImminentRestartWarningInMinutes": 7,
    "userPauseAccess": "enabled"
  }
}
```




