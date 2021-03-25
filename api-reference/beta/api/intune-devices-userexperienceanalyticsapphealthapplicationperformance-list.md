---
title: Список userExperienceAnalyticsAppHealthApplicationPerformances
description: Список свойств и связей объектов userExperienceAnalyticsAppHealthApplicationPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 85d5827ec0b584c72510de4df71436be5db64b57
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158110"
---
# <a name="list-userexperienceanalyticsapphealthapplicationperformances"></a><span data-ttu-id="28531-103">Список userExperienceAnalyticsAppHealthApplicationPerformances</span><span class="sxs-lookup"><span data-stu-id="28531-103">List userExperienceAnalyticsAppHealthApplicationPerformances</span></span>

<span data-ttu-id="28531-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28531-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28531-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28531-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28531-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28531-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28531-107">Список свойств и связей [объектов userExperienceAnalyticsAppHealthApplicationPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)</span><span class="sxs-lookup"><span data-stu-id="28531-107">List properties and relationships of the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28531-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="28531-108">Prerequisites</span></span>
<span data-ttu-id="28531-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28531-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28531-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28531-111">Permission type</span></span>|<span data-ttu-id="28531-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28531-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28531-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28531-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28531-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28531-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="28531-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28531-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28531-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28531-116">Not supported.</span></span>|
|<span data-ttu-id="28531-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="28531-117">Application</span></span>|<span data-ttu-id="28531-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28531-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28531-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28531-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
```

## <a name="request-headers"></a><span data-ttu-id="28531-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="28531-120">Request headers</span></span>
|<span data-ttu-id="28531-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28531-121">Header</span></span>|<span data-ttu-id="28531-122">Значение</span><span class="sxs-lookup"><span data-stu-id="28531-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28531-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="28531-123">Authorization</span></span>|<span data-ttu-id="28531-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28531-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28531-125">Accept</span><span class="sxs-lookup"><span data-stu-id="28531-125">Accept</span></span>|<span data-ttu-id="28531-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28531-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28531-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28531-127">Request body</span></span>
<span data-ttu-id="28531-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28531-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28531-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="28531-129">Response</span></span>
<span data-ttu-id="28531-130">В случае успеха этот метод возвращает код ответа и коллекцию объектов `200 OK` [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="28531-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28531-131">Пример</span><span class="sxs-lookup"><span data-stu-id="28531-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="28531-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="28531-132">Request</span></span>
<span data-ttu-id="28531-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28531-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
```

### <a name="response"></a><span data-ttu-id="28531-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="28531-134">Response</span></span>
<span data-ttu-id="28531-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28531-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 607

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
      "id": "c7962a87-2a87-c796-872a-96c7872a96c7",
      "appHangCount": 12,
      "appHealthScore": 4.666666666666667,
      "appHealthStatus": "App Health Status value",
      "allOrgsHealthScore": 6.0,
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




