---
title: Перечисление объектов windowsUpdateForBusinessConfiguration
description: Перечисление свойств и связей объектов windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1a9ce0a56d2491c331e7abd74bdbbbab58100f75
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753785"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="cde2e-103">Перечисление объектов windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="cde2e-103">List windowsUpdateForBusinessConfigurations</span></span>

<span data-ttu-id="cde2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cde2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cde2e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cde2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cde2e-106">Перечисление свойств и связей объектов [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cde2e-106">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cde2e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cde2e-107">Prerequisites</span></span>
<span data-ttu-id="cde2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cde2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cde2e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cde2e-110">Permission type</span></span>|<span data-ttu-id="cde2e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cde2e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cde2e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cde2e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cde2e-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cde2e-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cde2e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cde2e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cde2e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cde2e-115">Not supported.</span></span>|
|<span data-ttu-id="cde2e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="cde2e-116">Application</span></span>|<span data-ttu-id="cde2e-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cde2e-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cde2e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cde2e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cde2e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cde2e-119">Request headers</span></span>
|<span data-ttu-id="cde2e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cde2e-120">Header</span></span>|<span data-ttu-id="cde2e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cde2e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cde2e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cde2e-122">Authorization</span></span>|<span data-ttu-id="cde2e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cde2e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cde2e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cde2e-124">Accept</span></span>|<span data-ttu-id="cde2e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cde2e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cde2e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cde2e-126">Request body</span></span>
<span data-ttu-id="cde2e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cde2e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cde2e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="cde2e-128">Response</span></span>
<span data-ttu-id="cde2e-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cde2e-129">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cde2e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cde2e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cde2e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cde2e-131">Request</span></span>
<span data-ttu-id="cde2e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cde2e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="cde2e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cde2e-133">Response</span></span>
<span data-ttu-id="cde2e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cde2e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




