---
title: Список Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсионс
description: Список свойств и связей объектов Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d950816cf13b69c951b1648c196ffa6eaf1e26d6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49203090"
---
# <a name="list-userexperienceanalyticsapphealthappperformancebyosversions"></a><span data-ttu-id="199ef-103">Список Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсионс</span><span class="sxs-lookup"><span data-stu-id="199ef-103">List userExperienceAnalyticsAppHealthAppPerformanceByOSVersions</span></span>

<span data-ttu-id="199ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="199ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="199ef-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="199ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="199ef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="199ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="199ef-107">Список свойств и связей объектов [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) .</span><span class="sxs-lookup"><span data-stu-id="199ef-107">List properties and relationships of the [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="199ef-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="199ef-108">Prerequisites</span></span>
<span data-ttu-id="199ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="199ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="199ef-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="199ef-111">Permission type</span></span>|<span data-ttu-id="199ef-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="199ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="199ef-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="199ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="199ef-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="199ef-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="199ef-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="199ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="199ef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="199ef-116">Not supported.</span></span>|
|<span data-ttu-id="199ef-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="199ef-117">Application</span></span>|<span data-ttu-id="199ef-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="199ef-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="199ef-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="199ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion
```

## <a name="request-headers"></a><span data-ttu-id="199ef-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="199ef-120">Request headers</span></span>
|<span data-ttu-id="199ef-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="199ef-121">Header</span></span>|<span data-ttu-id="199ef-122">Значение</span><span class="sxs-lookup"><span data-stu-id="199ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="199ef-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="199ef-123">Authorization</span></span>|<span data-ttu-id="199ef-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="199ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="199ef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="199ef-125">Accept</span></span>|<span data-ttu-id="199ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="199ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="199ef-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="199ef-127">Request body</span></span>
<span data-ttu-id="199ef-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="199ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="199ef-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="199ef-129">Response</span></span>
<span data-ttu-id="199ef-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="199ef-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="199ef-131">Пример</span><span class="sxs-lookup"><span data-stu-id="199ef-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="199ef-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="199ef-132">Request</span></span>
<span data-ttu-id="199ef-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="199ef-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion
```

### <a name="response"></a><span data-ttu-id="199ef-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="199ef-134">Response</span></span>
<span data-ttu-id="199ef-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="199ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 541

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByOSVersion",
      "id": "65f9bde9-bde9-65f9-e9bd-f965e9bdf965",
      "osVersion": "Os Version value",
      "osBuildNumber": "Os Build Number value",
      "activeDeviceCount": 1,
      "appName": "App Name value",
      "appDisplayName": "App Display Name value",
      "appPublisher": "App Publisher value",
      "appUsageDuration": 0,
      "appCrashCount": 13,
      "meanTimeToFailureInMinutes": 10
    }
  ]
}
```




