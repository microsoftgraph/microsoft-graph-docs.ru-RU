---
title: Перечисление объектов windowsUpdateForBusinessConfiguration
description: Перечисление свойств и связей объектов windowsUpdateForBusinessConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d3da41b3b29fb7cc65b643435299b0302d2aa6e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396919"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="18d42-103">Перечисление объектов windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="18d42-103">List windowsUpdateForBusinessConfigurations</span></span>

> <span data-ttu-id="18d42-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="18d42-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="18d42-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18d42-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18d42-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18d42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18d42-107">Перечисление свойств и связей объектов [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18d42-107">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18d42-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="18d42-108">Prerequisites</span></span>
<span data-ttu-id="18d42-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="18d42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="18d42-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18d42-111">Permission type</span></span>|<span data-ttu-id="18d42-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18d42-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18d42-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18d42-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18d42-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="18d42-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="18d42-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18d42-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18d42-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18d42-116">Not supported.</span></span>|
|<span data-ttu-id="18d42-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18d42-117">Application</span></span>|<span data-ttu-id="18d42-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18d42-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18d42-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18d42-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="18d42-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18d42-120">Request headers</span></span>
|<span data-ttu-id="18d42-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18d42-121">Header</span></span>|<span data-ttu-id="18d42-122">Значение</span><span class="sxs-lookup"><span data-stu-id="18d42-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18d42-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18d42-123">Authorization</span></span>|<span data-ttu-id="18d42-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="18d42-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18d42-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18d42-125">Accept</span></span>|<span data-ttu-id="18d42-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18d42-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18d42-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18d42-127">Request body</span></span>
<span data-ttu-id="18d42-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18d42-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18d42-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="18d42-129">Response</span></span>
<span data-ttu-id="18d42-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="18d42-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18d42-131">Пример</span><span class="sxs-lookup"><span data-stu-id="18d42-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="18d42-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="18d42-132">Request</span></span>
<span data-ttu-id="18d42-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18d42-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="18d42-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="18d42-134">Response</span></span>
<span data-ttu-id="18d42-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="18d42-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2185

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
  ]
}
```




