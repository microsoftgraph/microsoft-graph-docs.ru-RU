---
title: Список Усерекспериенцеаналитиксдевицеперформанцес
description: Список свойств и связей объектов Усерекспериенцеаналитиксдевицеперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cff6afe7c2857d4e53225b06be5bdec0ca13b3dc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49310141"
---
# <a name="list-userexperienceanalyticsdeviceperformances"></a><span data-ttu-id="3043b-103">Список Усерекспериенцеаналитиксдевицеперформанцес</span><span class="sxs-lookup"><span data-stu-id="3043b-103">List userExperienceAnalyticsDevicePerformances</span></span>

<span data-ttu-id="3043b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3043b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3043b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3043b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3043b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3043b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3043b-107">Список свойств и связей объектов [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="3043b-107">List properties and relationships of the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3043b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3043b-108">Prerequisites</span></span>
<span data-ttu-id="3043b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3043b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3043b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3043b-111">Permission type</span></span>|<span data-ttu-id="3043b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3043b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3043b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3043b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3043b-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3043b-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3043b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3043b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3043b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3043b-116">Not supported.</span></span>|
|<span data-ttu-id="3043b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3043b-117">Application</span></span>|<span data-ttu-id="3043b-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3043b-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3043b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3043b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="3043b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3043b-120">Request headers</span></span>
|<span data-ttu-id="3043b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3043b-121">Header</span></span>|<span data-ttu-id="3043b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3043b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3043b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3043b-123">Authorization</span></span>|<span data-ttu-id="3043b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3043b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3043b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3043b-125">Accept</span></span>|<span data-ttu-id="3043b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3043b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3043b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3043b-127">Request body</span></span>
<span data-ttu-id="3043b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3043b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3043b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3043b-129">Response</span></span>
<span data-ttu-id="3043b-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3043b-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3043b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3043b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3043b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3043b-132">Request</span></span>
<span data-ttu-id="3043b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3043b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance
```

### <a name="response"></a><span data-ttu-id="3043b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3043b-134">Response</span></span>
<span data-ttu-id="3043b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3043b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 797

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
      "id": "852ae826-e826-852a-26e8-2a8526e82a85",
      "deviceName": "Device Name value",
      "model": "Model value",
      "manufacturer": "Manufacturer value",
      "diskType": "hdd",
      "operatingSystemVersion": "Operating System Version value",
      "bootScore": 9,
      "coreBootTimeInMs": 0,
      "groupPolicyBootTimeInMs": 7,
      "healthStatus": "insufficientData",
      "loginScore": 10,
      "coreLoginTimeInMs": 1,
      "groupPolicyLoginTimeInMs": 8,
      "deviceCount": 11,
      "responsiveDesktopTimeInMs": 9,
      "blueScreenCount": 15,
      "restartCount": 12,
      "averageBlueScreens": 6.0,
      "averageRestarts": 5.0
    }
  ]
}
```




