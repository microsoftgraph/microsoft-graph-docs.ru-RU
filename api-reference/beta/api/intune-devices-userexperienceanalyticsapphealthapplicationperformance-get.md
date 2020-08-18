---
title: Получение Усерекспериенцеаналитиксапфеалсаппликатионперформанце
description: Чтение свойств и связей объекта Усерекспериенцеаналитиксапфеалсаппликатионперформанце.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b565e811103e21b5f70884107e71d11b28f7a45e
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790301"
---
# <a name="get-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="5e060-103">Получение Усерекспериенцеаналитиксапфеалсаппликатионперформанце</span><span class="sxs-lookup"><span data-stu-id="5e060-103">Get userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="5e060-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e060-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e060-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e060-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e060-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e060-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e060-107">Чтение свойств и связей объекта [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="5e060-107">Read properties and relationships of the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e060-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5e060-108">Prerequisites</span></span>
<span data-ttu-id="5e060-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e060-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e060-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e060-111">Permission type</span></span>|<span data-ttu-id="5e060-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e060-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e060-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e060-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e060-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e060-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5e060-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e060-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e060-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e060-116">Not supported.</span></span>|
|<span data-ttu-id="5e060-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5e060-117">Application</span></span>|<span data-ttu-id="5e060-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e060-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e060-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e060-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5e060-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5e060-120">Optional query parameters</span></span>
<span data-ttu-id="5e060-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5e060-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e060-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e060-122">Request headers</span></span>
|<span data-ttu-id="5e060-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e060-123">Header</span></span>|<span data-ttu-id="5e060-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5e060-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e060-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e060-125">Authorization</span></span>|<span data-ttu-id="5e060-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e060-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e060-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5e060-127">Accept</span></span>|<span data-ttu-id="5e060-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5e060-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e060-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e060-129">Request body</span></span>
<span data-ttu-id="5e060-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e060-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e060-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e060-131">Response</span></span>
<span data-ttu-id="5e060-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e060-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e060-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5e060-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e060-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e060-134">Request</span></span>
<span data-ttu-id="5e060-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e060-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
```

### <a name="response"></a><span data-ttu-id="5e060-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e060-136">Response</span></span>
<span data-ttu-id="5e060-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e060-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 691

{
  "value": {
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
}
```



