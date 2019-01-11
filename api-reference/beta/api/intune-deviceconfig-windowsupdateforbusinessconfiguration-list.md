---
title: Перечисление объектов windowsUpdateForBusinessConfiguration
description: Перечисление свойств и связей объектов windowsUpdateForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3ba7e3558d4b1e1b45f73ae7ab919546a8a759f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889511"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="5529b-103">Перечисление объектов windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="5529b-103">List windowsUpdateForBusinessConfigurations</span></span>

> <span data-ttu-id="5529b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5529b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5529b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5529b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5529b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5529b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5529b-107">Перечисление свойств и связей объектов [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5529b-107">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5529b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5529b-108">Prerequisites</span></span>
<span data-ttu-id="5529b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5529b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5529b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5529b-111">Permission type</span></span>|<span data-ttu-id="5529b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5529b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5529b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5529b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5529b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5529b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5529b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5529b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5529b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5529b-116">Not supported.</span></span>|
|<span data-ttu-id="5529b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5529b-117">Application</span></span>|<span data-ttu-id="5529b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5529b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5529b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5529b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5529b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5529b-120">Request headers</span></span>
|<span data-ttu-id="5529b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5529b-121">Header</span></span>|<span data-ttu-id="5529b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5529b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5529b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5529b-123">Authorization</span></span>|<span data-ttu-id="5529b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5529b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5529b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5529b-125">Accept</span></span>|<span data-ttu-id="5529b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5529b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5529b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5529b-127">Request body</span></span>
<span data-ttu-id="5529b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5529b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5529b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5529b-129">Response</span></span>
<span data-ttu-id="5529b-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5529b-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5529b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5529b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="5529b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5529b-132">Request</span></span>
<span data-ttu-id="5529b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5529b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="5529b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="5529b-134">Response</span></span>
<span data-ttu-id="5529b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5529b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2176

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
      "qualityUpdatesPauseStartDateTime": "Quality Updates Pause Start Date Time value",
      "featureUpdatesPauseStartDateTime": "Feature Updates Pause Start Date Time value",
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
      "scheduleImminentRestartWarningInMinutes": 7
    }
  ]
}
```





