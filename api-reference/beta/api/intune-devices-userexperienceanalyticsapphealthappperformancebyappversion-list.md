---
title: Список Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсионс
description: Список свойств и связей объектов Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3e44eca3b028babf8ffaf0cb00ec5f1d71bf1f4c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706704"
---
# <a name="list-userexperienceanalyticsapphealthappperformancebyappversions"></a><span data-ttu-id="051d9-103">Список Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсионс</span><span class="sxs-lookup"><span data-stu-id="051d9-103">List userExperienceAnalyticsAppHealthAppPerformanceByAppVersions</span></span>

<span data-ttu-id="051d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="051d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="051d9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="051d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="051d9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="051d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="051d9-107">Список свойств и связей объектов [усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) .</span><span class="sxs-lookup"><span data-stu-id="051d9-107">List properties and relationships of the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="051d9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="051d9-108">Prerequisites</span></span>
<span data-ttu-id="051d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="051d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="051d9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="051d9-111">Permission type</span></span>|<span data-ttu-id="051d9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="051d9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="051d9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="051d9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="051d9-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="051d9-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="051d9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="051d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="051d9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="051d9-116">Not supported.</span></span>|
|<span data-ttu-id="051d9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="051d9-117">Application</span></span>|<span data-ttu-id="051d9-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="051d9-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="051d9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="051d9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion
```

## <a name="request-headers"></a><span data-ttu-id="051d9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="051d9-120">Request headers</span></span>
|<span data-ttu-id="051d9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="051d9-121">Header</span></span>|<span data-ttu-id="051d9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="051d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="051d9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="051d9-123">Authorization</span></span>|<span data-ttu-id="051d9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="051d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="051d9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="051d9-125">Accept</span></span>|<span data-ttu-id="051d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="051d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="051d9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="051d9-127">Request body</span></span>
<span data-ttu-id="051d9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="051d9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="051d9-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="051d9-129">Response</span></span>
<span data-ttu-id="051d9-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="051d9-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="051d9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="051d9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="051d9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="051d9-132">Request</span></span>
<span data-ttu-id="051d9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="051d9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion
```

### <a name="response"></a><span data-ttu-id="051d9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="051d9-134">Response</span></span>
<span data-ttu-id="051d9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="051d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 464

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersion",
      "id": "257804c8-04c8-2578-c804-7825c8047825",
      "appVersion": "App Version value",
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





