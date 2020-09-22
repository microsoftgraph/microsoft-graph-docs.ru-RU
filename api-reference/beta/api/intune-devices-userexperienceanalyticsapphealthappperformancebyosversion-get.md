---
title: Получение Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион
description: Чтение свойств и связей объекта Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9476fc0dd48f8f49922a1a3f342ac784f4b82c34
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992721"
---
# <a name="get-userexperienceanalyticsapphealthappperformancebyosversion"></a><span data-ttu-id="5ebde-103">Получение Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион</span><span class="sxs-lookup"><span data-stu-id="5ebde-103">Get userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span></span>

<span data-ttu-id="5ebde-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ebde-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ebde-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ebde-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ebde-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ebde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ebde-107">Чтение свойств и связей объекта [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) .</span><span class="sxs-lookup"><span data-stu-id="5ebde-107">Read properties and relationships of the [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ebde-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5ebde-108">Prerequisites</span></span>
<span data-ttu-id="5ebde-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ebde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ebde-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ebde-111">Permission type</span></span>|<span data-ttu-id="5ebde-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ebde-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ebde-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ebde-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ebde-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ebde-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5ebde-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ebde-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ebde-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ebde-116">Not supported.</span></span>|
|<span data-ttu-id="5ebde-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ebde-117">Application</span></span>|<span data-ttu-id="5ebde-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ebde-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ebde-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ebde-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion/{userExperienceAnalyticsAppHealthAppPerformanceByOSVersionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ebde-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="5ebde-120">Optional query parameters</span></span>
<span data-ttu-id="5ebde-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5ebde-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ebde-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ebde-122">Request headers</span></span>
|<span data-ttu-id="5ebde-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ebde-123">Header</span></span>|<span data-ttu-id="5ebde-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5ebde-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ebde-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ebde-125">Authorization</span></span>|<span data-ttu-id="5ebde-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ebde-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ebde-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5ebde-127">Accept</span></span>|<span data-ttu-id="5ebde-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5ebde-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ebde-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5ebde-129">Request body</span></span>
<span data-ttu-id="5ebde-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ebde-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ebde-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ebde-131">Response</span></span>
<span data-ttu-id="5ebde-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5ebde-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ebde-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5ebde-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ebde-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ebde-134">Request</span></span>
<span data-ttu-id="5ebde-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ebde-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion/{userExperienceAnalyticsAppHealthAppPerformanceByOSVersionId}
```

### <a name="response"></a><span data-ttu-id="5ebde-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ebde-136">Response</span></span>
<span data-ttu-id="5ebde-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ebde-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 505

{
  "value": {
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
}
```






