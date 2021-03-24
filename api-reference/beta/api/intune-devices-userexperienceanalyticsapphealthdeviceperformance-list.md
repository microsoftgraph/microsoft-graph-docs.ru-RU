---
title: Список userExperienceAnalyticsAppHealthDevicePerformances
description: Список свойств и связей объектов userExperienceAnalyticsAppHealthDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3ffa44f4f3c66e9c6ad0aad68102d659aa28a6d8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136113"
---
# <a name="list-userexperienceanalyticsapphealthdeviceperformances"></a><span data-ttu-id="24eef-103">Список userExperienceAnalyticsAppHealthDevicePerformances</span><span class="sxs-lookup"><span data-stu-id="24eef-103">List userExperienceAnalyticsAppHealthDevicePerformances</span></span>

<span data-ttu-id="24eef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24eef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24eef-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24eef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24eef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24eef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24eef-107">Список свойств и связей [объектов userExperienceAnalyticsAppHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="24eef-107">List properties and relationships of the [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24eef-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="24eef-108">Prerequisites</span></span>
<span data-ttu-id="24eef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24eef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24eef-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24eef-111">Permission type</span></span>|<span data-ttu-id="24eef-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24eef-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24eef-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24eef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24eef-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24eef-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="24eef-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24eef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24eef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24eef-116">Not supported.</span></span>|
|<span data-ttu-id="24eef-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="24eef-117">Application</span></span>|<span data-ttu-id="24eef-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24eef-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24eef-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24eef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="24eef-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24eef-120">Request headers</span></span>
|<span data-ttu-id="24eef-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24eef-121">Header</span></span>|<span data-ttu-id="24eef-122">Значение</span><span class="sxs-lookup"><span data-stu-id="24eef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24eef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="24eef-123">Authorization</span></span>|<span data-ttu-id="24eef-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24eef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24eef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="24eef-125">Accept</span></span>|<span data-ttu-id="24eef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24eef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24eef-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24eef-127">Request body</span></span>
<span data-ttu-id="24eef-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24eef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24eef-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="24eef-129">Response</span></span>
<span data-ttu-id="24eef-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="24eef-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24eef-131">Пример</span><span class="sxs-lookup"><span data-stu-id="24eef-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="24eef-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="24eef-132">Request</span></span>
<span data-ttu-id="24eef-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24eef-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
```

### <a name="response"></a><span data-ttu-id="24eef-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="24eef-134">Response</span></span>
<span data-ttu-id="24eef-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24eef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 620

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
      "id": "2c651499-1499-2c65-9914-652c9914652c",
      "deviceModel": "Device Model value",
      "deviceManufacturer": "Device Manufacturer value",
      "appCrashCount": 13,
      "crashedAppCount": 15,
      "appHangCount": 12,
      "meanTimeToFailureInMinutes": 10,
      "deviceAppHealthScore": 6.666666666666667,
      "deviceAppHealthStatus": "Device App Health Status value",
      "deviceId": "Device Id value",
      "deviceDisplayName": "Device Display Name value"
    }
  ]
}
```




