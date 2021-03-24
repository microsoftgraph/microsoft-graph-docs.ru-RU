---
title: List deviceManagementAutopilotEvents
description: Список свойств и связей объектов deviceManagementAutopilotEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f138f09e8cb913023e60cec5ef30d24a4d2a26e3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148269"
---
# <a name="list-devicemanagementautopilotevents"></a><span data-ttu-id="190c1-103">List deviceManagementAutopilotEvents</span><span class="sxs-lookup"><span data-stu-id="190c1-103">List deviceManagementAutopilotEvents</span></span>

<span data-ttu-id="190c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="190c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="190c1-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="190c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="190c1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="190c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="190c1-107">Список свойств и связей [объектов deviceManagementAutopilotEvent.](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)</span><span class="sxs-lookup"><span data-stu-id="190c1-107">List properties and relationships of the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="190c1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="190c1-108">Prerequisites</span></span>
<span data-ttu-id="190c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="190c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="190c1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="190c1-111">Permission type</span></span>|<span data-ttu-id="190c1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="190c1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="190c1-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="190c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="190c1-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="190c1-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="190c1-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="190c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="190c1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="190c1-116">Not supported.</span></span>|
|<span data-ttu-id="190c1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="190c1-117">Application</span></span>|<span data-ttu-id="190c1-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="190c1-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="190c1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="190c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="190c1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="190c1-120">Request headers</span></span>
|<span data-ttu-id="190c1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="190c1-121">Header</span></span>|<span data-ttu-id="190c1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="190c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="190c1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="190c1-123">Authorization</span></span>|<span data-ttu-id="190c1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="190c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="190c1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="190c1-125">Accept</span></span>|<span data-ttu-id="190c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="190c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="190c1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="190c1-127">Request body</span></span>
<span data-ttu-id="190c1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="190c1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="190c1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="190c1-129">Response</span></span>
<span data-ttu-id="190c1-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="190c1-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="190c1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="190c1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="190c1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="190c1-132">Request</span></span>
<span data-ttu-id="190c1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="190c1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
```

### <a name="response"></a><span data-ttu-id="190c1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="190c1-134">Response</span></span>
<span data-ttu-id="190c1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="190c1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1739

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
      "id": "3e455cab-5cab-3e45-ab5c-453eab5c453e",
      "deviceId": "Device Id value",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "deviceRegisteredDateTime": "2017-01-01T00:02:48.7185581-08:00",
      "enrollmentStartDateTime": "2017-01-01T00:00:19.6280481-08:00",
      "enrollmentType": "azureADJoinedWithAutopilotProfile",
      "deviceSerialNumber": "Device Serial Number value",
      "managedDeviceName": "Managed Device Name value",
      "userPrincipalName": "User Principal Name value",
      "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
      "enrollmentState": "enrolled",
      "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
      "windows10EnrollmentCompletionPageConfigurationId": "Windows10Enrollment Completion Page Configuration Id value",
      "deploymentState": "success",
      "deviceSetupStatus": "success",
      "accountSetupStatus": "success",
      "osVersion": "Os Version value",
      "deploymentDuration": "PT3M21.5549443S",
      "deploymentTotalDuration": "PT1M43.5284261S",
      "devicePreparationDuration": "-PT1M32.1347897S",
      "deviceSetupDuration": "-PT2M57.2190107S",
      "accountSetupDuration": "-PT2M32.0507894S",
      "deploymentStartDateTime": "2016-12-31T23:59:37.257201-08:00",
      "deploymentEndDateTime": "2017-01-01T00:00:46.5128291-08:00",
      "targetedAppCount": 0,
      "targetedPolicyCount": 3,
      "enrollmentFailureDetails": "Enrollment Failure Details value"
    }
  ]
}
```




