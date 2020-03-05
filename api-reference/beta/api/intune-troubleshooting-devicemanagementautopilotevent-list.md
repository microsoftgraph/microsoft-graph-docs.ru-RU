---
title: Список Девицеманажементаутопилотевентс
description: Список свойств и связей объектов Девицеманажементаутопилотевент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f21f7ea7359e9503d1f2f03863536ffcb19b92f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457708"
---
# <a name="list-devicemanagementautopilotevents"></a><span data-ttu-id="328b9-103">Список Девицеманажементаутопилотевентс</span><span class="sxs-lookup"><span data-stu-id="328b9-103">List deviceManagementAutopilotEvents</span></span>

<span data-ttu-id="328b9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="328b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="328b9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="328b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="328b9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="328b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="328b9-107">Список свойств и связей объектов [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="328b9-107">List properties and relationships of the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="328b9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="328b9-108">Prerequisites</span></span>
<span data-ttu-id="328b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="328b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="328b9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="328b9-111">Permission type</span></span>|<span data-ttu-id="328b9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="328b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="328b9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="328b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="328b9-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="328b9-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="328b9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="328b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="328b9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="328b9-116">Not supported.</span></span>|
|<span data-ttu-id="328b9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="328b9-117">Application</span></span>|<span data-ttu-id="328b9-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="328b9-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="328b9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="328b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="328b9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="328b9-120">Request headers</span></span>
|<span data-ttu-id="328b9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="328b9-121">Header</span></span>|<span data-ttu-id="328b9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="328b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="328b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="328b9-123">Authorization</span></span>|<span data-ttu-id="328b9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="328b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="328b9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="328b9-125">Accept</span></span>|<span data-ttu-id="328b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="328b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="328b9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="328b9-127">Request body</span></span>
<span data-ttu-id="328b9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="328b9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="328b9-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="328b9-129">Response</span></span>
<span data-ttu-id="328b9-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="328b9-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="328b9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="328b9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="328b9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="328b9-132">Request</span></span>
<span data-ttu-id="328b9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="328b9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
```

### <a name="response"></a><span data-ttu-id="328b9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="328b9-134">Response</span></span>
<span data-ttu-id="328b9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="328b9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1501

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
      "id": "3e455cab-5cab-3e45-ab5c-453eab5c453e",
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
      "deploymentState": "success",
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





