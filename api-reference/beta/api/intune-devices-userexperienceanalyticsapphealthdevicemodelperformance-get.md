---
title: Получение Усерекспериенцеаналитиксапфеалсдевицемоделперформанце
description: Чтение свойств и связей объекта Усерекспериенцеаналитиксапфеалсдевицемоделперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a28b1ab458139b1ecd542991ef1de0e189b202f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992708"
---
# <a name="get-userexperienceanalyticsapphealthdevicemodelperformance"></a><span data-ttu-id="aeac4-103">Получение Усерекспериенцеаналитиксапфеалсдевицемоделперформанце</span><span class="sxs-lookup"><span data-stu-id="aeac4-103">Get userExperienceAnalyticsAppHealthDeviceModelPerformance</span></span>

<span data-ttu-id="aeac4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aeac4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aeac4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aeac4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aeac4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aeac4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aeac4-107">Чтение свойств и связей объекта [усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="aeac4-107">Read properties and relationships of the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aeac4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aeac4-108">Prerequisites</span></span>
<span data-ttu-id="aeac4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aeac4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aeac4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aeac4-111">Permission type</span></span>|<span data-ttu-id="aeac4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aeac4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aeac4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aeac4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aeac4-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="aeac4-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="aeac4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aeac4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aeac4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aeac4-116">Not supported.</span></span>|
|<span data-ttu-id="aeac4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aeac4-117">Application</span></span>|<span data-ttu-id="aeac4-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="aeac4-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aeac4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aeac4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aeac4-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="aeac4-120">Optional query parameters</span></span>
<span data-ttu-id="aeac4-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aeac4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aeac4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aeac4-122">Request headers</span></span>
|<span data-ttu-id="aeac4-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aeac4-123">Header</span></span>|<span data-ttu-id="aeac4-124">Значение</span><span class="sxs-lookup"><span data-stu-id="aeac4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aeac4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aeac4-125">Authorization</span></span>|<span data-ttu-id="aeac4-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aeac4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aeac4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="aeac4-127">Accept</span></span>|<span data-ttu-id="aeac4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="aeac4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aeac4-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aeac4-129">Request body</span></span>
<span data-ttu-id="aeac4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aeac4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aeac4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="aeac4-131">Response</span></span>
<span data-ttu-id="aeac4-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aeac4-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aeac4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="aeac4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="aeac4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="aeac4-134">Request</span></span>
<span data-ttu-id="aeac4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aeac4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
```

### <a name="response"></a><span data-ttu-id="aeac4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="aeac4-136">Response</span></span>
<span data-ttu-id="aeac4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aeac4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance",
    "id": "4daddc60-dc60-4dad-60dc-ad4d60dcad4d",
    "deviceModel": "Device Model value",
    "deviceManufacturer": "Device Manufacturer value",
    "activeDeviceCount": 1,
    "meanTimeToFailureInMinutes": 10,
    "modelAppHealthScore": 6.333333333333333,
    "modelAppHealthStatus": "Model App Health Status value"
  }
}
```






