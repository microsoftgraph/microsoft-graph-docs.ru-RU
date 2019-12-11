---
title: Обновление Усерекспериенцеаналитиксметрик
description: Обновление свойств объекта Усерекспериенцеаналитиксметрик.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 88fc0a60be39baf4be9c624bc4e37a1d23ad3d3d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944409"
---
# <a name="update-userexperienceanalyticsmetric"></a><span data-ttu-id="74f32-103">Обновление Усерекспериенцеаналитиксметрик</span><span class="sxs-lookup"><span data-stu-id="74f32-103">Update userExperienceAnalyticsMetric</span></span>

> <span data-ttu-id="74f32-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74f32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74f32-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74f32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74f32-106">Обновление свойств объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="74f32-106">Update the properties of a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74f32-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="74f32-107">Prerequisites</span></span>
<span data-ttu-id="74f32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74f32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74f32-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74f32-110">Permission type</span></span>|<span data-ttu-id="74f32-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="74f32-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74f32-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74f32-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74f32-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74f32-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="74f32-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74f32-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74f32-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74f32-115">Not supported.</span></span>|
|<span data-ttu-id="74f32-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74f32-116">Application</span></span>|<span data-ttu-id="74f32-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74f32-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74f32-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74f32-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="74f32-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="74f32-119">Request headers</span></span>
|<span data-ttu-id="74f32-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74f32-120">Header</span></span>|<span data-ttu-id="74f32-121">Значение</span><span class="sxs-lookup"><span data-stu-id="74f32-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74f32-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74f32-122">Authorization</span></span>|<span data-ttu-id="74f32-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74f32-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74f32-124">Accept</span><span class="sxs-lookup"><span data-stu-id="74f32-124">Accept</span></span>|<span data-ttu-id="74f32-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74f32-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74f32-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74f32-126">Request body</span></span>
<span data-ttu-id="74f32-127">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74f32-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

<span data-ttu-id="74f32-128">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md).</span><span class="sxs-lookup"><span data-stu-id="74f32-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md).</span></span>

|<span data-ttu-id="74f32-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="74f32-129">Property</span></span>|<span data-ttu-id="74f32-130">Тип</span><span class="sxs-lookup"><span data-stu-id="74f32-130">Type</span></span>|<span data-ttu-id="74f32-131">Описание</span><span class="sxs-lookup"><span data-stu-id="74f32-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74f32-132">id</span><span class="sxs-lookup"><span data-stu-id="74f32-132">id</span></span>|<span data-ttu-id="74f32-133">Строка</span><span class="sxs-lookup"><span data-stu-id="74f32-133">String</span></span>|<span data-ttu-id="74f32-134">Уникальный идентификатор метрики аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="74f32-134">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="74f32-135">значение</span><span class="sxs-lookup"><span data-stu-id="74f32-135">value</span></span>|<span data-ttu-id="74f32-136">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="74f32-136">Double</span></span>|<span data-ttu-id="74f32-137">Значение метрики аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="74f32-137">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="74f32-138">устройств</span><span class="sxs-lookup"><span data-stu-id="74f32-138">unit</span></span>|<span data-ttu-id="74f32-139">Строка</span><span class="sxs-lookup"><span data-stu-id="74f32-139">String</span></span>|<span data-ttu-id="74f32-140">Единица измерения показателя взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="74f32-140">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="74f32-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="74f32-141">Response</span></span>
<span data-ttu-id="74f32-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="74f32-142">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74f32-143">Пример</span><span class="sxs-lookup"><span data-stu-id="74f32-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="74f32-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="74f32-144">Request</span></span>
<span data-ttu-id="74f32-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74f32-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="74f32-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="74f32-146">Response</span></span>
<span data-ttu-id="74f32-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74f32-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





