---
title: Get windowsUpdateForBusinessConfiguration
description: Чтение свойств и связей объекта windowsUpdateForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c66f7060dec6db43618046ad825e8fb9cbed0cff
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973742"
---
# <a name="get-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="1c182-103">Get windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c182-103">Get windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="1c182-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c182-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c182-105">Чтение свойств и связей объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c182-105">Read properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c182-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1c182-106">Prerequisites</span></span>
<span data-ttu-id="1c182-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c182-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c182-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c182-109">Permission type</span></span>|<span data-ttu-id="1c182-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c182-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c182-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c182-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1c182-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c182-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1c182-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c182-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c182-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c182-114">Not supported.</span></span>|
|<span data-ttu-id="1c182-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c182-115">Application</span></span>|<span data-ttu-id="1c182-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c182-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c182-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c182-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c182-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1c182-118">Optional query parameters</span></span>
<span data-ttu-id="1c182-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1c182-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c182-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c182-120">Request headers</span></span>
|<span data-ttu-id="1c182-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c182-121">Header</span></span>|<span data-ttu-id="1c182-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1c182-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c182-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c182-123">Authorization</span></span>|<span data-ttu-id="1c182-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c182-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c182-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1c182-125">Accept</span></span>|<span data-ttu-id="1c182-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c182-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c182-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c182-127">Request body</span></span>
<span data-ttu-id="1c182-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c182-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c182-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c182-129">Response</span></span>
<span data-ttu-id="1c182-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1c182-130">If successful, this method returns a `200 OK` response code and [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c182-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1c182-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c182-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c182-132">Request</span></span>
<span data-ttu-id="1c182-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c182-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="1c182-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c182-134">Response</span></span>
<span data-ttu-id="1c182-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c182-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



