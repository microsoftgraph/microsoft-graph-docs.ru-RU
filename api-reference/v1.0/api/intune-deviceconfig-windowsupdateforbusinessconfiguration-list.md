---
title: Перечисление объектов windowsUpdateForBusinessConfiguration
description: Перечисление свойств и связей объектов windowsUpdateForBusinessConfiguration.
ms.openlocfilehash: b2242e0a53203f2699a90050af88a16480c7fd4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026160"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="03890-103">Перечисление объектов windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="03890-103">List windowsUpdateForBusinessConfigurations</span></span>

> <span data-ttu-id="03890-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="03890-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03890-105">Перечисление свойств и связей объектов [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03890-105">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="03890-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="03890-106">Prerequisites</span></span>
<span data-ttu-id="03890-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03890-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03890-109">Permission type</span></span>|<span data-ttu-id="03890-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03890-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03890-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03890-111">Delegated (work or school account)</span></span>|<span data-ttu-id="03890-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="03890-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="03890-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03890-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03890-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03890-114">Not supported.</span></span>|
|<span data-ttu-id="03890-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03890-115">Application</span></span>|<span data-ttu-id="03890-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03890-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03890-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03890-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="03890-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03890-118">Request headers</span></span>
|<span data-ttu-id="03890-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03890-119">Header</span></span>|<span data-ttu-id="03890-120">Значение</span><span class="sxs-lookup"><span data-stu-id="03890-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03890-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="03890-121">Authorization</span></span>|<span data-ttu-id="03890-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="03890-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03890-123">Accept</span><span class="sxs-lookup"><span data-stu-id="03890-123">Accept</span></span>|<span data-ttu-id="03890-124">application/json</span><span class="sxs-lookup"><span data-stu-id="03890-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03890-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03890-125">Request body</span></span>
<span data-ttu-id="03890-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03890-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03890-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="03890-127">Response</span></span>
<span data-ttu-id="03890-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="03890-128">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03890-129">Пример</span><span class="sxs-lookup"><span data-stu-id="03890-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="03890-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="03890-130">Request</span></span>
<span data-ttu-id="03890-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03890-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="03890-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="03890-132">Response</span></span>
<span data-ttu-id="03890-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="03890-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1211

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
      "id": "4928dd6a-dd6a-4928-6add-28496add2849",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
      "businessReadyUpdatesOnly": "all"
    }
  ]
}
```



