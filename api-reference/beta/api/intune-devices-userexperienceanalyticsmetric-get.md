---
title: Получение Усерекспериенцеаналитиксметрик
description: Чтение свойств и связей объекта Усерекспериенцеаналитиксметрик.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eebcbeb2d6793dc980b4594b1ff54def242d0329
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970140"
---
# <a name="get-userexperienceanalyticsmetric"></a><span data-ttu-id="1fb33-103">Получение Усерекспериенцеаналитиксметрик</span><span class="sxs-lookup"><span data-stu-id="1fb33-103">Get userExperienceAnalyticsMetric</span></span>

<span data-ttu-id="1fb33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fb33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1fb33-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fb33-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fb33-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1fb33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fb33-107">Чтение свойств и связей объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="1fb33-107">Read properties and relationships of the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fb33-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1fb33-108">Prerequisites</span></span>
<span data-ttu-id="1fb33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fb33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fb33-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fb33-111">Permission type</span></span>|<span data-ttu-id="1fb33-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fb33-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fb33-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fb33-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1fb33-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fb33-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1fb33-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fb33-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fb33-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fb33-116">Not supported.</span></span>|
|<span data-ttu-id="1fb33-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1fb33-117">Application</span></span>|<span data-ttu-id="1fb33-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fb33-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fb33-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fb33-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression/{userExperienceAnalyticsMetricId}
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression/{userExperienceAnalyticsMetricId}
GET /deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}/userExperienceAnalyticsMetric
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues/{userExperienceAnalyticsMetricId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1fb33-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="1fb33-120">Optional query parameters</span></span>
<span data-ttu-id="1fb33-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1fb33-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1fb33-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1fb33-122">Request headers</span></span>
|<span data-ttu-id="1fb33-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1fb33-123">Header</span></span>|<span data-ttu-id="1fb33-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1fb33-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fb33-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fb33-125">Authorization</span></span>|<span data-ttu-id="1fb33-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fb33-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fb33-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1fb33-127">Accept</span></span>|<span data-ttu-id="1fb33-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1fb33-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fb33-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1fb33-129">Request body</span></span>
<span data-ttu-id="1fb33-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1fb33-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fb33-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fb33-131">Response</span></span>
<span data-ttu-id="1fb33-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1fb33-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fb33-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1fb33-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fb33-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fb33-134">Request</span></span>
<span data-ttu-id="1fb33-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fb33-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
```

### <a name="response"></a><span data-ttu-id="1fb33-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fb33-136">Response</span></span>
<span data-ttu-id="1fb33-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1fb33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 204

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
    "id": "1371822e-822e-1371-2e82-71132e827113",
    "value": 1.6666666666666667,
    "unit": "Unit value"
  }
}
```






