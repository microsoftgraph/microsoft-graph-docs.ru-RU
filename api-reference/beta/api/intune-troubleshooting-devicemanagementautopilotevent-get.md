---
title: Получение Девицеманажементаутопилотевент
description: Чтение свойств и связей объекта Девицеманажементаутопилотевент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6fecd5746417e0907feb39a7fa231528153a3f6a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939031"
---
# <a name="get-devicemanagementautopilotevent"></a><span data-ttu-id="82497-103">Получение Девицеманажементаутопилотевент</span><span class="sxs-lookup"><span data-stu-id="82497-103">Get deviceManagementAutopilotEvent</span></span>

> <span data-ttu-id="82497-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82497-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82497-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82497-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82497-106">Чтение свойств и связей объекта [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="82497-106">Read properties and relationships of the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82497-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="82497-107">Prerequisites</span></span>
<span data-ttu-id="82497-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82497-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82497-110">Permission type</span></span>|<span data-ttu-id="82497-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82497-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82497-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82497-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82497-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="82497-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="82497-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82497-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82497-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82497-115">Not supported.</span></span>|
|<span data-ttu-id="82497-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82497-116">Application</span></span>|<span data-ttu-id="82497-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="82497-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82497-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82497-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82497-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="82497-119">Optional query parameters</span></span>
<span data-ttu-id="82497-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="82497-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82497-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82497-121">Request headers</span></span>
|<span data-ttu-id="82497-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82497-122">Header</span></span>|<span data-ttu-id="82497-123">Значение</span><span class="sxs-lookup"><span data-stu-id="82497-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82497-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82497-124">Authorization</span></span>|<span data-ttu-id="82497-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82497-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82497-126">Accept</span><span class="sxs-lookup"><span data-stu-id="82497-126">Accept</span></span>|<span data-ttu-id="82497-127">application/json</span><span class="sxs-lookup"><span data-stu-id="82497-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82497-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82497-128">Request body</span></span>
<span data-ttu-id="82497-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82497-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82497-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="82497-130">Response</span></span>
<span data-ttu-id="82497-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82497-131">If successful, this method returns a `200 OK` response code and [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82497-132">Пример</span><span class="sxs-lookup"><span data-stu-id="82497-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="82497-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="82497-133">Request</span></span>
<span data-ttu-id="82497-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82497-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

### <a name="response"></a><span data-ttu-id="82497-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="82497-135">Response</span></span>
<span data-ttu-id="82497-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82497-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1439

{
  "value": {
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
}
```





