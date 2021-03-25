---
title: Обновление userExperienceAnalyticsMetric
description: Обновление свойств объекта userExperienceAnalyticsMetric.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d2faace9e102011f8f7f0f7b9382e69a03355c27
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159272"
---
# <a name="update-userexperienceanalyticsmetric"></a><span data-ttu-id="13799-103">Обновление userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="13799-103">Update userExperienceAnalyticsMetric</span></span>

<span data-ttu-id="13799-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13799-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13799-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13799-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13799-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13799-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13799-107">Обновление свойств объекта [userExperienceAnalyticsMetric.](../resources/intune-devices-userexperienceanalyticsmetric.md)</span><span class="sxs-lookup"><span data-stu-id="13799-107">Update the properties of a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13799-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="13799-108">Prerequisites</span></span>
<span data-ttu-id="13799-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13799-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13799-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13799-111">Permission type</span></span>|<span data-ttu-id="13799-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13799-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13799-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13799-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13799-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13799-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="13799-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13799-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13799-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13799-116">Not supported.</span></span>|
|<span data-ttu-id="13799-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="13799-117">Application</span></span>|<span data-ttu-id="13799-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13799-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13799-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13799-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}/userExperienceAnalyticsMetric
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues/{userExperienceAnalyticsMetricId}
```

## <a name="request-headers"></a><span data-ttu-id="13799-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="13799-120">Request headers</span></span>
|<span data-ttu-id="13799-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13799-121">Header</span></span>|<span data-ttu-id="13799-122">Значение</span><span class="sxs-lookup"><span data-stu-id="13799-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13799-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13799-123">Authorization</span></span>|<span data-ttu-id="13799-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13799-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13799-125">Accept</span><span class="sxs-lookup"><span data-stu-id="13799-125">Accept</span></span>|<span data-ttu-id="13799-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13799-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13799-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13799-127">Request body</span></span>
<span data-ttu-id="13799-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsMetric.](../resources/intune-devices-userexperienceanalyticsmetric.md)</span><span class="sxs-lookup"><span data-stu-id="13799-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

<span data-ttu-id="13799-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsMetric.](../resources/intune-devices-userexperienceanalyticsmetric.md)</span><span class="sxs-lookup"><span data-stu-id="13799-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md).</span></span>

|<span data-ttu-id="13799-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="13799-130">Property</span></span>|<span data-ttu-id="13799-131">Тип</span><span class="sxs-lookup"><span data-stu-id="13799-131">Type</span></span>|<span data-ttu-id="13799-132">Описание</span><span class="sxs-lookup"><span data-stu-id="13799-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13799-133">id</span><span class="sxs-lookup"><span data-stu-id="13799-133">id</span></span>|<span data-ttu-id="13799-134">Строка</span><span class="sxs-lookup"><span data-stu-id="13799-134">String</span></span>|<span data-ttu-id="13799-135">Уникальный идентификатор метрики аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="13799-135">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="13799-136">значение</span><span class="sxs-lookup"><span data-stu-id="13799-136">value</span></span>|<span data-ttu-id="13799-137">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="13799-137">Double</span></span>|<span data-ttu-id="13799-138">Значение метрики аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="13799-138">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="13799-139">unit</span><span class="sxs-lookup"><span data-stu-id="13799-139">unit</span></span>|<span data-ttu-id="13799-140">Строка</span><span class="sxs-lookup"><span data-stu-id="13799-140">String</span></span>|<span data-ttu-id="13799-141">Единица метрики аналитики пользовательского опыта.</span><span class="sxs-lookup"><span data-stu-id="13799-141">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="13799-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="13799-142">Response</span></span>
<span data-ttu-id="13799-143">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="13799-143">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13799-144">Пример</span><span class="sxs-lookup"><span data-stu-id="13799-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="13799-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="13799-145">Request</span></span>
<span data-ttu-id="13799-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13799-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "value": 1.6666666666666667,
  "unit": "Unit value"
}
```

### <a name="response"></a><span data-ttu-id="13799-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="13799-147">Response</span></span>
<span data-ttu-id="13799-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13799-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 177

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "1371822e-822e-1371-2e82-71132e827113",
  "value": 1.6666666666666667,
  "unit": "Unit value"
}
```




