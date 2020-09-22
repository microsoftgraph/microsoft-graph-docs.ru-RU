---
title: Список Усерекспериенцеаналитиксдевицестартуфисториес
description: Список свойств и связей объектов Усерекспериенцеаналитиксдевицестартуфистори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2b5563bcdfcdf78f16f931ddec99c20037c45d23
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082597"
---
# <a name="list-userexperienceanalyticsdevicestartuphistories"></a><span data-ttu-id="7b5ce-103">Список Усерекспериенцеаналитиксдевицестартуфисториес</span><span class="sxs-lookup"><span data-stu-id="7b5ce-103">List userExperienceAnalyticsDeviceStartupHistories</span></span>

<span data-ttu-id="7b5ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b5ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b5ce-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b5ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b5ce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b5ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b5ce-107">Список свойств и связей объектов [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .</span><span class="sxs-lookup"><span data-stu-id="7b5ce-107">List properties and relationships of the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b5ce-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7b5ce-108">Prerequisites</span></span>
<span data-ttu-id="7b5ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b5ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b5ce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b5ce-111">Permission type</span></span>|<span data-ttu-id="7b5ce-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b5ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b5ce-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b5ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b5ce-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b5ce-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7b5ce-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b5ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b5ce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b5ce-116">Not supported.</span></span>|
|<span data-ttu-id="7b5ce-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b5ce-117">Application</span></span>|<span data-ttu-id="7b5ce-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b5ce-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b5ce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b5ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a><span data-ttu-id="7b5ce-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7b5ce-120">Request headers</span></span>
|<span data-ttu-id="7b5ce-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b5ce-121">Header</span></span>|<span data-ttu-id="7b5ce-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7b5ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b5ce-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b5ce-123">Authorization</span></span>|<span data-ttu-id="7b5ce-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b5ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b5ce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7b5ce-125">Accept</span></span>|<span data-ttu-id="7b5ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b5ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b5ce-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b5ce-127">Request body</span></span>
<span data-ttu-id="7b5ce-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b5ce-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b5ce-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b5ce-129">Response</span></span>
<span data-ttu-id="7b5ce-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7b5ce-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b5ce-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7b5ce-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b5ce-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b5ce-132">Request</span></span>
<span data-ttu-id="7b5ce-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b5ce-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

### <a name="response"></a><span data-ttu-id="7b5ce-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b5ce-134">Response</span></span>
<span data-ttu-id="7b5ce-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b5ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 834

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
      "id": "13357123-7123-1335-2371-351323713513",
      "deviceId": "Device Id value",
      "startTime": "2017-01-01T00:03:29.2730865-08:00",
      "coreBootTimeInMs": 0,
      "groupPolicyBootTimeInMs": 7,
      "featureUpdateBootTimeInMs": 9,
      "totalBootTimeInMs": 1,
      "groupPolicyLoginTimeInMs": 8,
      "coreLoginTimeInMs": 1,
      "responsiveDesktopTimeInMs": 9,
      "totalLoginTimeInMs": 2,
      "isFirstLogin": true,
      "isFeatureUpdate": true,
      "operatingSystemVersion": "Operating System Version value",
      "restartCategory": "restartWithUpdate",
      "restartStopCode": "Restart Stop Code value",
      "restartFaultBucket": "Restart Fault Bucket value"
    }
  ]
}
```






