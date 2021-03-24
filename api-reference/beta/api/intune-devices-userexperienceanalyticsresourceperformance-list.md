---
title: Список userExperienceAnalyticsResourcePerformances
description: Список свойств и связей объектов userExperienceAnalyticsResourcePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0276c93a9e91fdad9e5cad19531887d439c74415
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135931"
---
# <a name="list-userexperienceanalyticsresourceperformances"></a><span data-ttu-id="aa556-103">Список userExperienceAnalyticsResourcePerformances</span><span class="sxs-lookup"><span data-stu-id="aa556-103">List userExperienceAnalyticsResourcePerformances</span></span>

<span data-ttu-id="aa556-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa556-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa556-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa556-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa556-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa556-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa556-107">Список свойств и связей [объектов userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="aa556-107">List properties and relationships of the [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa556-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aa556-108">Prerequisites</span></span>
<span data-ttu-id="aa556-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa556-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa556-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa556-111">Permission type</span></span>|<span data-ttu-id="aa556-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa556-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa556-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa556-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa556-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa556-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="aa556-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa556-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa556-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa556-116">Not supported.</span></span>|
|<span data-ttu-id="aa556-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="aa556-117">Application</span></span>|<span data-ttu-id="aa556-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa556-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa556-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa556-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsResourcePerformance
```

## <a name="request-headers"></a><span data-ttu-id="aa556-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aa556-120">Request headers</span></span>
|<span data-ttu-id="aa556-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aa556-121">Header</span></span>|<span data-ttu-id="aa556-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aa556-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa556-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa556-123">Authorization</span></span>|<span data-ttu-id="aa556-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa556-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa556-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aa556-125">Accept</span></span>|<span data-ttu-id="aa556-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa556-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa556-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa556-127">Request body</span></span>
<span data-ttu-id="aa556-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa556-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa556-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa556-129">Response</span></span>
<span data-ttu-id="aa556-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="aa556-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa556-131">Пример</span><span class="sxs-lookup"><span data-stu-id="aa556-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa556-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa556-132">Request</span></span>
<span data-ttu-id="aa556-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa556-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsResourcePerformance
```

### <a name="response"></a><span data-ttu-id="aa556-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa556-134">Response</span></span>
<span data-ttu-id="aa556-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa556-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 691

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
      "id": "d34d78e8-78e8-d34d-e878-4dd3e8784dd3",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "model": "Model value",
      "deviceCount": 11,
      "manufacturer": "Manufacturer value",
      "cpuSpikeTimePercentage": 7.333333333333333,
      "ramSpikeTimePercentage": 7.333333333333333,
      "cpuSpikeTimeScore": 1,
      "cpuSpikeTimePercentageThreshold": 10.333333333333334,
      "ramSpikeTimeScore": 1,
      "ramSpikeTimePercentageThreshold": 10.333333333333334,
      "deviceResourcePerformanceScore": 14
    }
  ]
}
```




