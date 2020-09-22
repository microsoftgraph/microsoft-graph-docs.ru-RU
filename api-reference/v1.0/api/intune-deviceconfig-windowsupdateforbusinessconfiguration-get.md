---
title: Get windowsUpdateForBusinessConfiguration
description: Чтение свойств и связей объекта windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 694789eaa45a11b186cff30061972e1c756396f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063214"
---
# <a name="get-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="87c7e-103">Get windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="87c7e-103">Get windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="87c7e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87c7e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87c7e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87c7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87c7e-106">Чтение свойств и связей объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87c7e-106">Read properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87c7e-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="87c7e-107">Prerequisites</span></span>
<span data-ttu-id="87c7e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87c7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87c7e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87c7e-110">Permission type</span></span>|<span data-ttu-id="87c7e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87c7e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87c7e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87c7e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="87c7e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87c7e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87c7e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87c7e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87c7e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87c7e-115">Not supported.</span></span>|
|<span data-ttu-id="87c7e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87c7e-116">Application</span></span>|<span data-ttu-id="87c7e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87c7e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87c7e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87c7e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87c7e-119">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="87c7e-119">Optional query parameters</span></span>
<span data-ttu-id="87c7e-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="87c7e-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87c7e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87c7e-121">Request headers</span></span>
|<span data-ttu-id="87c7e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87c7e-122">Header</span></span>|<span data-ttu-id="87c7e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="87c7e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87c7e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="87c7e-124">Authorization</span></span>|<span data-ttu-id="87c7e-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87c7e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87c7e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="87c7e-126">Accept</span></span>|<span data-ttu-id="87c7e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="87c7e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87c7e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="87c7e-128">Request body</span></span>
<span data-ttu-id="87c7e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87c7e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87c7e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="87c7e-130">Response</span></span>
<span data-ttu-id="87c7e-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="87c7e-131">If successful, this method returns a `200 OK` response code and [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87c7e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="87c7e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="87c7e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="87c7e-133">Request</span></span>
<span data-ttu-id="87c7e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87c7e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="87c7e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="87c7e-135">Response</span></span>
<span data-ttu-id="87c7e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="87c7e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1149

{
  "value": {
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
}
```









