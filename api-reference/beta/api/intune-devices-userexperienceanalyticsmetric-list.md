---
title: Список Усерекспериенцеаналитиксметрикс
description: Список свойств и связей объектов Усерекспериенцеаналитиксметрик.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0ec8bdea580c3c2cae731f28bb23fa1d417f3b75
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468223"
---
# <a name="list-userexperienceanalyticsmetrics"></a><span data-ttu-id="07e12-103">Список Усерекспериенцеаналитиксметрикс</span><span class="sxs-lookup"><span data-stu-id="07e12-103">List userExperienceAnalyticsMetrics</span></span>

<span data-ttu-id="07e12-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="07e12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07e12-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07e12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07e12-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07e12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07e12-107">Список свойств и связей объектов [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="07e12-107">List properties and relationships of the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07e12-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="07e12-108">Prerequisites</span></span>
<span data-ttu-id="07e12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07e12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07e12-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07e12-111">Permission type</span></span>|<span data-ttu-id="07e12-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="07e12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07e12-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07e12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07e12-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="07e12-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="07e12-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07e12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07e12-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07e12-116">Not supported.</span></span>|
|<span data-ttu-id="07e12-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07e12-117">Application</span></span>|<span data-ttu-id="07e12-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="07e12-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07e12-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07e12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
```

## <a name="request-headers"></a><span data-ttu-id="07e12-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="07e12-120">Request headers</span></span>
|<span data-ttu-id="07e12-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07e12-121">Header</span></span>|<span data-ttu-id="07e12-122">Значение</span><span class="sxs-lookup"><span data-stu-id="07e12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07e12-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07e12-123">Authorization</span></span>|<span data-ttu-id="07e12-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07e12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07e12-125">Accept</span><span class="sxs-lookup"><span data-stu-id="07e12-125">Accept</span></span>|<span data-ttu-id="07e12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07e12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07e12-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07e12-127">Request body</span></span>
<span data-ttu-id="07e12-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07e12-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07e12-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="07e12-129">Response</span></span>
<span data-ttu-id="07e12-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07e12-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07e12-131">Пример</span><span class="sxs-lookup"><span data-stu-id="07e12-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="07e12-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="07e12-132">Request</span></span>
<span data-ttu-id="07e12-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07e12-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
```

### <a name="response"></a><span data-ttu-id="07e12-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="07e12-134">Response</span></span>
<span data-ttu-id="07e12-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07e12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 245

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
      "id": "1371822e-822e-1371-2e82-71132e827113",
      "value": "<Unknown Primitive Type Edm.Double>",
      "unit": "Unit value"
    }
  ]
}
```





