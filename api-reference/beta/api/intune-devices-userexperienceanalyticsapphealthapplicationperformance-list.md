---
title: Список Усерекспериенцеаналитиксапфеалсаппликатионперформанцес
description: Список свойств и связей объектов Усерекспериенцеаналитиксапфеалсаппликатионперформанце.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5eee707d9d21b7f872f05d6ab91fbbfab175097a
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790299"
---
# <a name="list-userexperienceanalyticsapphealthapplicationperformances"></a><span data-ttu-id="d6281-103">Список Усерекспериенцеаналитиксапфеалсаппликатионперформанцес</span><span class="sxs-lookup"><span data-stu-id="d6281-103">List userExperienceAnalyticsAppHealthApplicationPerformances</span></span>

<span data-ttu-id="d6281-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6281-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6281-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6281-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6281-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6281-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6281-107">Список свойств и связей объектов [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="d6281-107">List properties and relationships of the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6281-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d6281-108">Prerequisites</span></span>
<span data-ttu-id="d6281-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6281-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6281-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6281-111">Permission type</span></span>|<span data-ttu-id="d6281-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6281-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6281-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6281-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6281-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6281-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d6281-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6281-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6281-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6281-116">Not supported.</span></span>|
|<span data-ttu-id="d6281-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d6281-117">Application</span></span>|<span data-ttu-id="d6281-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6281-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6281-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6281-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
```

## <a name="request-headers"></a><span data-ttu-id="d6281-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6281-120">Request headers</span></span>
|<span data-ttu-id="d6281-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6281-121">Header</span></span>|<span data-ttu-id="d6281-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d6281-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6281-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6281-123">Authorization</span></span>|<span data-ttu-id="d6281-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6281-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6281-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d6281-125">Accept</span></span>|<span data-ttu-id="d6281-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6281-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6281-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6281-127">Request body</span></span>
<span data-ttu-id="d6281-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6281-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6281-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6281-129">Response</span></span>
<span data-ttu-id="d6281-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6281-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6281-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d6281-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6281-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6281-132">Request</span></span>
<span data-ttu-id="d6281-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6281-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
```

### <a name="response"></a><span data-ttu-id="d6281-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6281-134">Response</span></span>
<span data-ttu-id="d6281-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6281-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 737

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
      "id": "c7962a87-2a87-c796-872a-96c7872a96c7",
      "appName": "App Name value",
      "appFriendlyName": "App Friendly Name value",
      "appPublisher": "App Publisher value",
      "activeDevices": 13,
      "totalAppUsageDuration": 5,
      "totalAppCrashes": 15,
      "totalAppHangs": 13,
      "meanTimeToFailure": 1,
      "appHealthScore": 4.666666666666667,
      "appHealthStatus": "App Health Status value",
      "allOrgsHealthScore": 6.0,
      "allOrgsMeanTimeToFailure": 8,
      "tenantId": "Tenant Id value",
      "memaTimeGenerated": "Mema Time Generated value"
    }
  ]
}
```



