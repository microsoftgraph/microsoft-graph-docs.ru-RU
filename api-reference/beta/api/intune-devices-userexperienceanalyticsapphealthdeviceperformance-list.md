---
title: Список Усерекспериенцеаналитиксапфеалсдевицеперформанцес
description: Список свойств и связей объектов Усерекспериенцеаналитиксапфеалсдевицеперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10843547afbfb0ab9840cf6af04681054ff8ad00
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202829"
---
# <a name="list-userexperienceanalyticsapphealthdeviceperformances"></a><span data-ttu-id="cd574-103">Список Усерекспериенцеаналитиксапфеалсдевицеперформанцес</span><span class="sxs-lookup"><span data-stu-id="cd574-103">List userExperienceAnalyticsAppHealthDevicePerformances</span></span>

<span data-ttu-id="cd574-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd574-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd574-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd574-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd574-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd574-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd574-107">Список свойств и связей объектов [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="cd574-107">List properties and relationships of the [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd574-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cd574-108">Prerequisites</span></span>
<span data-ttu-id="cd574-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd574-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd574-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd574-111">Permission type</span></span>|<span data-ttu-id="cd574-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd574-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd574-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd574-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cd574-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd574-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="cd574-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd574-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd574-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd574-116">Not supported.</span></span>|
|<span data-ttu-id="cd574-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cd574-117">Application</span></span>|<span data-ttu-id="cd574-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd574-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd574-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd574-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="cd574-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cd574-120">Request headers</span></span>
|<span data-ttu-id="cd574-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd574-121">Header</span></span>|<span data-ttu-id="cd574-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cd574-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd574-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd574-123">Authorization</span></span>|<span data-ttu-id="cd574-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd574-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd574-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cd574-125">Accept</span></span>|<span data-ttu-id="cd574-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cd574-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd574-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd574-127">Request body</span></span>
<span data-ttu-id="cd574-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cd574-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd574-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd574-129">Response</span></span>
<span data-ttu-id="cd574-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cd574-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd574-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cd574-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd574-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd574-132">Request</span></span>
<span data-ttu-id="cd574-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd574-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
```

### <a name="response"></a><span data-ttu-id="cd574-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd574-134">Response</span></span>
<span data-ttu-id="cd574-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd574-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




