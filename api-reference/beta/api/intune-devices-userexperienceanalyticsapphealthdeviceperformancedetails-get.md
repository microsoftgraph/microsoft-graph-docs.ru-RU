---
title: Получение Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс
description: Чтение свойств и связей объекта Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 50e21c7559b614ab1010956653d48943290ece47
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023570"
---
# <a name="get-userexperienceanalyticsapphealthdeviceperformancedetails"></a><span data-ttu-id="48875-103">Получение Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс</span><span class="sxs-lookup"><span data-stu-id="48875-103">Get userExperienceAnalyticsAppHealthDevicePerformanceDetails</span></span>

<span data-ttu-id="48875-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48875-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48875-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48875-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48875-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48875-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48875-107">Чтение свойств и связей объекта [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .</span><span class="sxs-lookup"><span data-stu-id="48875-107">Read properties and relationships of the [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48875-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="48875-108">Prerequisites</span></span>
<span data-ttu-id="48875-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48875-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48875-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48875-111">Permission type</span></span>|<span data-ttu-id="48875-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48875-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48875-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48875-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48875-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="48875-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="48875-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48875-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48875-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48875-116">Not supported.</span></span>|
|<span data-ttu-id="48875-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48875-117">Application</span></span>|<span data-ttu-id="48875-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="48875-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48875-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48875-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails/{userExperienceAnalyticsAppHealthDevicePerformanceDetailsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48875-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="48875-120">Optional query parameters</span></span>
<span data-ttu-id="48875-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="48875-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48875-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48875-122">Request headers</span></span>
|<span data-ttu-id="48875-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48875-123">Header</span></span>|<span data-ttu-id="48875-124">Значение</span><span class="sxs-lookup"><span data-stu-id="48875-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48875-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="48875-125">Authorization</span></span>|<span data-ttu-id="48875-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48875-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48875-127">Accept</span><span class="sxs-lookup"><span data-stu-id="48875-127">Accept</span></span>|<span data-ttu-id="48875-128">application/json</span><span class="sxs-lookup"><span data-stu-id="48875-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48875-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48875-129">Request body</span></span>
<span data-ttu-id="48875-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48875-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48875-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="48875-131">Response</span></span>
<span data-ttu-id="48875-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48875-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48875-133">Пример</span><span class="sxs-lookup"><span data-stu-id="48875-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="48875-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="48875-134">Request</span></span>
<span data-ttu-id="48875-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48875-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails/{userExperienceAnalyticsAppHealthDevicePerformanceDetailsId}
```

### <a name="response"></a><span data-ttu-id="48875-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="48875-136">Response</span></span>
<span data-ttu-id="48875-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48875-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 407

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
    "id": "bc8c5273-5273-bc8c-7352-8cbc73528cbc",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "eventType": "Event Type value",
    "appDisplayName": "App Display Name value",
    "deviceId": "Device Id value",
    "deviceDisplayName": "Device Display Name value"
  }
}
```






