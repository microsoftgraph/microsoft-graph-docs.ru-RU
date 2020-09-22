---
title: Получение Усерекспериенцеаналитиксапфеалсдевицеперформанце
description: Чтение свойств и связей объекта Усерекспериенцеаналитиксапфеалсдевицеперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 30bd56ff453776ebd8f4fedf3d03f280c0424467
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992673"
---
# <a name="get-userexperienceanalyticsapphealthdeviceperformance"></a><span data-ttu-id="8dcc5-103">Получение Усерекспериенцеаналитиксапфеалсдевицеперформанце</span><span class="sxs-lookup"><span data-stu-id="8dcc5-103">Get userExperienceAnalyticsAppHealthDevicePerformance</span></span>

<span data-ttu-id="8dcc5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dcc5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8dcc5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dcc5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8dcc5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8dcc5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dcc5-107">Чтение свойств и связей объекта [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="8dcc5-107">Read properties and relationships of the [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8dcc5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8dcc5-108">Prerequisites</span></span>
<span data-ttu-id="8dcc5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dcc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dcc5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8dcc5-111">Permission type</span></span>|<span data-ttu-id="8dcc5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8dcc5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8dcc5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8dcc5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8dcc5-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8dcc5-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="8dcc5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8dcc5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8dcc5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dcc5-116">Not supported.</span></span>|
|<span data-ttu-id="8dcc5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8dcc5-117">Application</span></span>|<span data-ttu-id="8dcc5-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8dcc5-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8dcc5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8dcc5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance/{userExperienceAnalyticsAppHealthDevicePerformanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8dcc5-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="8dcc5-120">Optional query parameters</span></span>
<span data-ttu-id="8dcc5-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8dcc5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8dcc5-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8dcc5-122">Request headers</span></span>
|<span data-ttu-id="8dcc5-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8dcc5-123">Header</span></span>|<span data-ttu-id="8dcc5-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8dcc5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8dcc5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8dcc5-125">Authorization</span></span>|<span data-ttu-id="8dcc5-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dcc5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8dcc5-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8dcc5-127">Accept</span></span>|<span data-ttu-id="8dcc5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8dcc5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dcc5-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8dcc5-129">Request body</span></span>
<span data-ttu-id="8dcc5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8dcc5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dcc5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dcc5-131">Response</span></span>
<span data-ttu-id="8dcc5-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8dcc5-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dcc5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8dcc5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8dcc5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dcc5-134">Request</span></span>
<span data-ttu-id="8dcc5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dcc5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance/{userExperienceAnalyticsAppHealthDevicePerformanceId}
```

### <a name="response"></a><span data-ttu-id="8dcc5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dcc5-136">Response</span></span>
<span data-ttu-id="8dcc5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8dcc5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

{
  "value": {
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
}
```






