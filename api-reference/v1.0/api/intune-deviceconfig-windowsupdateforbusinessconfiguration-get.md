---
title: Get windowsUpdateForBusinessConfiguration
description: Чтение свойств и связей объекта windowsUpdateForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b13f12c48d9a3bf5fdfc8d50874be07906b39220
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809263"
---
# <a name="get-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="fae40-103">Get windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="fae40-103">Get windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="fae40-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fae40-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fae40-105">Чтение свойств и связей объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fae40-105">Read properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fae40-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fae40-106">Prerequisites</span></span>
<span data-ttu-id="fae40-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fae40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fae40-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fae40-109">Permission type</span></span>|<span data-ttu-id="fae40-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fae40-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fae40-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fae40-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fae40-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fae40-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fae40-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fae40-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fae40-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fae40-114">Not supported.</span></span>|
|<span data-ttu-id="fae40-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fae40-115">Application</span></span>|<span data-ttu-id="fae40-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fae40-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fae40-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fae40-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fae40-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fae40-118">Optional query parameters</span></span>
<span data-ttu-id="fae40-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fae40-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fae40-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fae40-120">Request headers</span></span>
|<span data-ttu-id="fae40-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fae40-121">Header</span></span>|<span data-ttu-id="fae40-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fae40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fae40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fae40-123">Authorization</span></span>|<span data-ttu-id="fae40-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fae40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fae40-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fae40-125">Accept</span></span>|<span data-ttu-id="fae40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fae40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fae40-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fae40-127">Request body</span></span>
<span data-ttu-id="fae40-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fae40-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fae40-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="fae40-129">Response</span></span>
<span data-ttu-id="fae40-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fae40-130">If successful, this method returns a `200 OK` response code and [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fae40-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fae40-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fae40-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fae40-132">Request</span></span>
<span data-ttu-id="fae40-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fae40-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="fae40-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="fae40-134">Response</span></span>
<span data-ttu-id="fae40-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fae40-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



