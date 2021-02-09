---
title: Список userExperienceAnalyticsResourcePerformances
description: Список свойств и связей объектов userExperienceAnalyticsResourcePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9d06e48ed7533ec351305e075b6eb38f44504f7e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162507"
---
# <a name="list-userexperienceanalyticsresourceperformances"></a><span data-ttu-id="cdabe-103">Список userExperienceAnalyticsResourcePerformances</span><span class="sxs-lookup"><span data-stu-id="cdabe-103">List userExperienceAnalyticsResourcePerformances</span></span>

<span data-ttu-id="cdabe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdabe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdabe-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdabe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdabe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cdabe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdabe-107">Список свойств и связей [объектов userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="cdabe-107">List properties and relationships of the [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdabe-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cdabe-108">Prerequisites</span></span>
<span data-ttu-id="cdabe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdabe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdabe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdabe-111">Permission type</span></span>|<span data-ttu-id="cdabe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdabe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdabe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdabe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cdabe-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdabe-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="cdabe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdabe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdabe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdabe-116">Not supported.</span></span>|
|<span data-ttu-id="cdabe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdabe-117">Application</span></span>|<span data-ttu-id="cdabe-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdabe-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdabe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdabe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsResourcePerformance
```

## <a name="request-headers"></a><span data-ttu-id="cdabe-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cdabe-120">Request headers</span></span>
|<span data-ttu-id="cdabe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdabe-121">Header</span></span>|<span data-ttu-id="cdabe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cdabe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdabe-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdabe-123">Authorization</span></span>|<span data-ttu-id="cdabe-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdabe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdabe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cdabe-125">Accept</span></span>|<span data-ttu-id="cdabe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cdabe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdabe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdabe-127">Request body</span></span>
<span data-ttu-id="cdabe-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cdabe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdabe-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdabe-129">Response</span></span>
<span data-ttu-id="cdabe-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cdabe-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdabe-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cdabe-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdabe-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdabe-132">Request</span></span>
<span data-ttu-id="cdabe-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdabe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsResourcePerformance
```

### <a name="response"></a><span data-ttu-id="cdabe-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdabe-134">Response</span></span>
<span data-ttu-id="cdabe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cdabe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




