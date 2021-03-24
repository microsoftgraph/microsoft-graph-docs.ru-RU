---
title: Список userExperienceAnalyticsAppHealthOSVersionPerformances
description: Список свойств и связей объектов userExperienceAnalyticsAppHealthOSVersionPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9116d8f8e77495115c65dd18561b41ff1a7f42b3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126439"
---
# <a name="list-userexperienceanalyticsapphealthosversionperformances"></a><span data-ttu-id="5e744-103">Список userExperienceAnalyticsAppHealthOSVersionPerformances</span><span class="sxs-lookup"><span data-stu-id="5e744-103">List userExperienceAnalyticsAppHealthOSVersionPerformances</span></span>

<span data-ttu-id="5e744-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e744-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e744-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e744-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e744-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e744-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e744-107">Список свойств и связей [объектов userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)</span><span class="sxs-lookup"><span data-stu-id="5e744-107">List properties and relationships of the [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e744-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5e744-108">Prerequisites</span></span>
<span data-ttu-id="5e744-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e744-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e744-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e744-111">Permission type</span></span>|<span data-ttu-id="5e744-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e744-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e744-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e744-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e744-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e744-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5e744-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e744-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e744-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e744-116">Not supported.</span></span>|
|<span data-ttu-id="5e744-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5e744-117">Application</span></span>|<span data-ttu-id="5e744-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e744-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e744-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e744-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance
```

## <a name="request-headers"></a><span data-ttu-id="5e744-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5e744-120">Request headers</span></span>
|<span data-ttu-id="5e744-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e744-121">Header</span></span>|<span data-ttu-id="5e744-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5e744-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e744-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e744-123">Authorization</span></span>|<span data-ttu-id="5e744-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e744-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e744-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5e744-125">Accept</span></span>|<span data-ttu-id="5e744-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e744-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e744-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e744-127">Request body</span></span>
<span data-ttu-id="5e744-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e744-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e744-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e744-129">Response</span></span>
<span data-ttu-id="5e744-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5e744-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e744-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5e744-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e744-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e744-132">Request</span></span>
<span data-ttu-id="5e744-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e744-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance
```

### <a name="response"></a><span data-ttu-id="5e744-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e744-134">Response</span></span>
<span data-ttu-id="5e744-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e744-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
      "id": "7c28e16b-e16b-7c28-6be1-287c6be1287c",
      "osVersion": "Os Version value",
      "osBuildNumber": "Os Build Number value",
      "activeDeviceCount": 1,
      "meanTimeToFailureInMinutes": 10,
      "osVersionAppHealthScore": 7.666666666666667,
      "osVersionAppHealthStatus": "Os Version App Health Status value"
    }
  ]
}
```




