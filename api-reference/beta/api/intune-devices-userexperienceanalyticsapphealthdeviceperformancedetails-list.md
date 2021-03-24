---
title: Список userExperienceAnalyticsAppHealthDevicePerformanceDetailses
description: Список свойств и связей объектов userExperienceAnalyticsAppHealthDevicePerformanceDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 07349e21ec1fef789f98b2401020b4488b370a1a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136050"
---
# <a name="list-userexperienceanalyticsapphealthdeviceperformancedetailses"></a><span data-ttu-id="69f84-103">Список userExperienceAnalyticsAppHealthDevicePerformanceDetailses</span><span class="sxs-lookup"><span data-stu-id="69f84-103">List userExperienceAnalyticsAppHealthDevicePerformanceDetailses</span></span>

<span data-ttu-id="69f84-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69f84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69f84-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f84-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69f84-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69f84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69f84-107">Список свойств и связей [объектов userExperienceAnalyticsAppHealthDevicePerformanceDetails.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)</span><span class="sxs-lookup"><span data-stu-id="69f84-107">List properties and relationships of the [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69f84-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="69f84-108">Prerequisites</span></span>
<span data-ttu-id="69f84-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69f84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f84-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69f84-111">Permission type</span></span>|<span data-ttu-id="69f84-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69f84-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69f84-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69f84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69f84-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f84-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="69f84-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69f84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69f84-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f84-116">Not supported.</span></span>|
|<span data-ttu-id="69f84-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="69f84-117">Application</span></span>|<span data-ttu-id="69f84-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f84-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69f84-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69f84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
```

## <a name="request-headers"></a><span data-ttu-id="69f84-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="69f84-120">Request headers</span></span>
|<span data-ttu-id="69f84-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69f84-121">Header</span></span>|<span data-ttu-id="69f84-122">Значение</span><span class="sxs-lookup"><span data-stu-id="69f84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69f84-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69f84-123">Authorization</span></span>|<span data-ttu-id="69f84-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69f84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69f84-125">Accept</span><span class="sxs-lookup"><span data-stu-id="69f84-125">Accept</span></span>|<span data-ttu-id="69f84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69f84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f84-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69f84-127">Request body</span></span>
<span data-ttu-id="69f84-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69f84-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69f84-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="69f84-129">Response</span></span>
<span data-ttu-id="69f84-130">В случае успеха этот метод возвращает код ответа и коллекцию объектов `200 OK` [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="69f84-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69f84-131">Пример</span><span class="sxs-lookup"><span data-stu-id="69f84-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="69f84-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="69f84-132">Request</span></span>
<span data-ttu-id="69f84-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69f84-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
```

### <a name="response"></a><span data-ttu-id="69f84-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="69f84-134">Response</span></span>
<span data-ttu-id="69f84-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69f84-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 435

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
      "id": "bc8c5273-5273-bc8c-7352-8cbc73528cbc",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "eventType": "Event Type value",
      "appDisplayName": "App Display Name value",
      "deviceId": "Device Id value",
      "deviceDisplayName": "Device Display Name value"
    }
  ]
}
```




