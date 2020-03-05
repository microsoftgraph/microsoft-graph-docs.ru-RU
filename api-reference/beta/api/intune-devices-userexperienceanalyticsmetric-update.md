---
title: Обновление Усерекспериенцеаналитиксметрик
description: Обновление свойств объекта Усерекспериенцеаналитиксметрик.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1a52039aa25a681d07d0f6c13594e90e96896eec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468175"
---
# <a name="update-userexperienceanalyticsmetric"></a><span data-ttu-id="be978-103">Обновление Усерекспериенцеаналитиксметрик</span><span class="sxs-lookup"><span data-stu-id="be978-103">Update userExperienceAnalyticsMetric</span></span>

<span data-ttu-id="be978-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="be978-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be978-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be978-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be978-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be978-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be978-107">Обновление свойств объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="be978-107">Update the properties of a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be978-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be978-108">Prerequisites</span></span>
<span data-ttu-id="be978-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be978-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be978-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be978-111">Permission type</span></span>|<span data-ttu-id="be978-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be978-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be978-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be978-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be978-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be978-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="be978-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be978-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be978-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be978-116">Not supported.</span></span>|
|<span data-ttu-id="be978-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be978-117">Application</span></span>|<span data-ttu-id="be978-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be978-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be978-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be978-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues/{userExperienceAnalyticsMetricId}
```

## <a name="request-headers"></a><span data-ttu-id="be978-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="be978-120">Request headers</span></span>
|<span data-ttu-id="be978-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be978-121">Header</span></span>|<span data-ttu-id="be978-122">Значение</span><span class="sxs-lookup"><span data-stu-id="be978-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be978-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="be978-123">Authorization</span></span>|<span data-ttu-id="be978-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be978-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be978-125">Accept</span><span class="sxs-lookup"><span data-stu-id="be978-125">Accept</span></span>|<span data-ttu-id="be978-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be978-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be978-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be978-127">Request body</span></span>
<span data-ttu-id="be978-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be978-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

<span data-ttu-id="be978-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md).</span><span class="sxs-lookup"><span data-stu-id="be978-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md).</span></span>

|<span data-ttu-id="be978-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="be978-130">Property</span></span>|<span data-ttu-id="be978-131">Тип</span><span class="sxs-lookup"><span data-stu-id="be978-131">Type</span></span>|<span data-ttu-id="be978-132">Описание</span><span class="sxs-lookup"><span data-stu-id="be978-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be978-133">id</span><span class="sxs-lookup"><span data-stu-id="be978-133">id</span></span>|<span data-ttu-id="be978-134">String</span><span class="sxs-lookup"><span data-stu-id="be978-134">String</span></span>|<span data-ttu-id="be978-135">Уникальный идентификатор метрики аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="be978-135">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="be978-136">значение</span><span class="sxs-lookup"><span data-stu-id="be978-136">value</span></span>|<span data-ttu-id="be978-137">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="be978-137">Double</span></span>|<span data-ttu-id="be978-138">Значение метрики аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="be978-138">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="be978-139">устройств</span><span class="sxs-lookup"><span data-stu-id="be978-139">unit</span></span>|<span data-ttu-id="be978-140">String</span><span class="sxs-lookup"><span data-stu-id="be978-140">String</span></span>|<span data-ttu-id="be978-141">Единица измерения показателя взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="be978-141">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="be978-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="be978-142">Response</span></span>
<span data-ttu-id="be978-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be978-143">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be978-144">Пример</span><span class="sxs-lookup"><span data-stu-id="be978-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="be978-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="be978-145">Request</span></span>
<span data-ttu-id="be978-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be978-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
Content-type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```

### <a name="response"></a><span data-ttu-id="be978-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="be978-147">Response</span></span>
<span data-ttu-id="be978-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be978-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 196

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "1371822e-822e-1371-2e82-71132e827113",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```





