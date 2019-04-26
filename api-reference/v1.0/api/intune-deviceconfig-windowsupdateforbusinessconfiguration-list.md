---
title: Перечисление объектов windowsUpdateForBusinessConfiguration
description: Перечисление свойств и связей объектов windowsUpdateForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48be9818e5e7b93de30a67760ffe2f0ada5515a8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563513"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="3da43-103">Перечисление объектов windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="3da43-103">List windowsUpdateForBusinessConfigurations</span></span>

> <span data-ttu-id="3da43-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3da43-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3da43-105">Перечисление свойств и связей объектов [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3da43-105">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3da43-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3da43-106">Prerequisites</span></span>
<span data-ttu-id="3da43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3da43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3da43-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3da43-109">Permission type</span></span>|<span data-ttu-id="3da43-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3da43-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3da43-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3da43-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3da43-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3da43-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3da43-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3da43-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3da43-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3da43-114">Not supported.</span></span>|
|<span data-ttu-id="3da43-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3da43-115">Application</span></span>|<span data-ttu-id="3da43-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3da43-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3da43-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3da43-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3da43-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3da43-118">Request headers</span></span>
|<span data-ttu-id="3da43-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3da43-119">Header</span></span>|<span data-ttu-id="3da43-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3da43-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3da43-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3da43-121">Authorization</span></span>|<span data-ttu-id="3da43-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3da43-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3da43-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3da43-123">Accept</span></span>|<span data-ttu-id="3da43-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3da43-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3da43-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3da43-125">Request body</span></span>
<span data-ttu-id="3da43-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3da43-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3da43-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3da43-127">Response</span></span>
<span data-ttu-id="3da43-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3da43-128">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3da43-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3da43-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="3da43-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3da43-130">Request</span></span>
<span data-ttu-id="3da43-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3da43-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3da43-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3da43-132">Response</span></span>
<span data-ttu-id="3da43-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3da43-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



