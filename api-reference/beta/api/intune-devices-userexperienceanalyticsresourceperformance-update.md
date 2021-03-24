---
title: Обновление userExperienceAnalyticsResourcePerformance
description: Обновление свойств объекта userExperienceAnalyticsResourcePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b5ca79e7870893e9748ea93222e96ade36649e6e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135917"
---
# <a name="update-userexperienceanalyticsresourceperformance"></a><span data-ttu-id="ca503-103">Обновление userExperienceAnalyticsResourcePerformance</span><span class="sxs-lookup"><span data-stu-id="ca503-103">Update userExperienceAnalyticsResourcePerformance</span></span>

<span data-ttu-id="ca503-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca503-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca503-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca503-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca503-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca503-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca503-107">Обновление свойств объекта [userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="ca503-107">Update the properties of a [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca503-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ca503-108">Prerequisites</span></span>
<span data-ttu-id="ca503-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca503-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca503-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca503-111">Permission type</span></span>|<span data-ttu-id="ca503-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca503-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca503-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca503-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca503-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca503-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ca503-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca503-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca503-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca503-116">Not supported.</span></span>|
|<span data-ttu-id="ca503-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ca503-117">Application</span></span>|<span data-ttu-id="ca503-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca503-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca503-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca503-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsResourcePerformance/{userExperienceAnalyticsResourcePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="ca503-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ca503-120">Request headers</span></span>
|<span data-ttu-id="ca503-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca503-121">Header</span></span>|<span data-ttu-id="ca503-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ca503-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca503-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca503-123">Authorization</span></span>|<span data-ttu-id="ca503-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca503-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca503-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ca503-125">Accept</span></span>|<span data-ttu-id="ca503-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca503-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca503-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca503-127">Request body</span></span>
<span data-ttu-id="ca503-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="ca503-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) object.</span></span>

<span data-ttu-id="ca503-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="ca503-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md).</span></span>

|<span data-ttu-id="ca503-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca503-130">Property</span></span>|<span data-ttu-id="ca503-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ca503-131">Type</span></span>|<span data-ttu-id="ca503-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ca503-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca503-133">id</span><span class="sxs-lookup"><span data-stu-id="ca503-133">id</span></span>|<span data-ttu-id="ca503-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ca503-134">String</span></span>|<span data-ttu-id="ca503-135">Уникальный идентификатор сущности производительности ресурсов аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="ca503-135">The unique identifier of the user experience analytics resource performance entity.</span></span>|
|<span data-ttu-id="ca503-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="ca503-136">deviceId</span></span>|<span data-ttu-id="ca503-137">String</span><span class="sxs-lookup"><span data-stu-id="ca503-137">String</span></span>|<span data-ttu-id="ca503-138">ID устройства.</span><span class="sxs-lookup"><span data-stu-id="ca503-138">The id of the device.</span></span>|
|<span data-ttu-id="ca503-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="ca503-139">deviceName</span></span>|<span data-ttu-id="ca503-140">String</span><span class="sxs-lookup"><span data-stu-id="ca503-140">String</span></span>|<span data-ttu-id="ca503-141">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="ca503-141">The name of the device.</span></span>|
|<span data-ttu-id="ca503-142">model</span><span class="sxs-lookup"><span data-stu-id="ca503-142">model</span></span>|<span data-ttu-id="ca503-143">String</span><span class="sxs-lookup"><span data-stu-id="ca503-143">String</span></span>|<span data-ttu-id="ca503-144">Модель устройства аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="ca503-144">The user experience analytics device model.</span></span>|
|<span data-ttu-id="ca503-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="ca503-145">deviceCount</span></span>|<span data-ttu-id="ca503-146">Int64</span><span class="sxs-lookup"><span data-stu-id="ca503-146">Int64</span></span>|<span data-ttu-id="ca503-147">Аналитика пользовательских интерфейсов суммирует количество устройств.</span><span class="sxs-lookup"><span data-stu-id="ca503-147">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="ca503-148">manufacturer</span><span class="sxs-lookup"><span data-stu-id="ca503-148">manufacturer</span></span>|<span data-ttu-id="ca503-149">String</span><span class="sxs-lookup"><span data-stu-id="ca503-149">String</span></span>|<span data-ttu-id="ca503-150">Производитель устройств аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="ca503-150">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="ca503-151">cpuSpikeTimePercentage</span><span class="sxs-lookup"><span data-stu-id="ca503-151">cpuSpikeTimePercentage</span></span>|<span data-ttu-id="ca503-152">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="ca503-152">Double</span></span>|<span data-ttu-id="ca503-153">Время пика ЦП в процентах.</span><span class="sxs-lookup"><span data-stu-id="ca503-153">CPU spike time in percentage.</span></span> <span data-ttu-id="ca503-154">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="ca503-154">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ca503-155">ramSpikeTimePercentage</span><span class="sxs-lookup"><span data-stu-id="ca503-155">ramSpikeTimePercentage</span></span>|<span data-ttu-id="ca503-156">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="ca503-156">Double</span></span>|<span data-ttu-id="ca503-157">Время пика оперативной памяти в процентах.</span><span class="sxs-lookup"><span data-stu-id="ca503-157">RAM spike time in percentage.</span></span> <span data-ttu-id="ca503-158">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="ca503-158">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ca503-159">cpuSpikeTimeScore</span><span class="sxs-lookup"><span data-stu-id="ca503-159">cpuSpikeTimeScore</span></span>|<span data-ttu-id="ca503-160">Int32</span><span class="sxs-lookup"><span data-stu-id="ca503-160">Int32</span></span>|<span data-ttu-id="ca503-161">Оценка времени пика пика ЦП для пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="ca503-161">The user experience analytics device CPU spike time score.</span></span> <span data-ttu-id="ca503-162">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="ca503-162">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ca503-163">cpuSpikeTimePercentageThreshold</span><span class="sxs-lookup"><span data-stu-id="ca503-163">cpuSpikeTimePercentageThreshold</span></span>|<span data-ttu-id="ca503-164">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="ca503-164">Double</span></span>|<span data-ttu-id="ca503-165">Порог cpuSpikeTimeScore.</span><span class="sxs-lookup"><span data-stu-id="ca503-165">Threshold of cpuSpikeTimeScore.</span></span> <span data-ttu-id="ca503-166">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="ca503-166">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ca503-167">ramSpikeTimeScore</span><span class="sxs-lookup"><span data-stu-id="ca503-167">ramSpikeTimeScore</span></span>|<span data-ttu-id="ca503-168">Int32</span><span class="sxs-lookup"><span data-stu-id="ca503-168">Int32</span></span>|<span data-ttu-id="ca503-169">Оценка времени пика пика оперативной памяти устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="ca503-169">The user experience analytics device RAM spike time score.</span></span> <span data-ttu-id="ca503-170">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="ca503-170">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ca503-171">ramSpikeTimePercentageThreshold</span><span class="sxs-lookup"><span data-stu-id="ca503-171">ramSpikeTimePercentageThreshold</span></span>|<span data-ttu-id="ca503-172">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="ca503-172">Double</span></span>|<span data-ttu-id="ca503-173">Порог ramSpikeTimeScore.</span><span class="sxs-lookup"><span data-stu-id="ca503-173">Threshold of ramSpikeTimeScore.</span></span> <span data-ttu-id="ca503-174">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="ca503-174">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ca503-175">deviceResourcePerformanceScore</span><span class="sxs-lookup"><span data-stu-id="ca503-175">deviceResourcePerformanceScore</span></span>|<span data-ttu-id="ca503-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ca503-176">Int32</span></span>|<span data-ttu-id="ca503-177">Оценка производительности ресурсов определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="ca503-177">Resource performance score of a specific device.</span></span> <span data-ttu-id="ca503-178">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="ca503-178">Valid values 0 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="ca503-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca503-179">Response</span></span>
<span data-ttu-id="ca503-180">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ca503-180">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca503-181">Пример</span><span class="sxs-lookup"><span data-stu-id="ca503-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca503-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca503-182">Request</span></span>
<span data-ttu-id="ca503-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca503-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsResourcePerformance/{userExperienceAnalyticsResourcePerformanceId}
Content-type: application/json
Content-length: 553

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "deviceCount": 11,
  "manufacturer": "Manufacturer value",
  "cpuSpikeTimePercentage": 7.333333333333333,
  "ramSpikeTimePercentage": 7.333333333333333,
  "cpuSpikeTimeScore": 1,
  "cpuSpikeTimePercentageThreshold": 10.333333333333334,
  "ramSpikeTimeScore": 1,
  "ramSpikeTimePercentageThreshold": 10.333333333333334,
  "deviceResourcePerformanceScore": 14
}
```

### <a name="response"></a><span data-ttu-id="ca503-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca503-184">Response</span></span>
<span data-ttu-id="ca503-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca503-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 602

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
  "id": "d34d78e8-78e8-d34d-e878-4dd3e8784dd3",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "deviceCount": 11,
  "manufacturer": "Manufacturer value",
  "cpuSpikeTimePercentage": 7.333333333333333,
  "ramSpikeTimePercentage": 7.333333333333333,
  "cpuSpikeTimeScore": 1,
  "cpuSpikeTimePercentageThreshold": 10.333333333333334,
  "ramSpikeTimeScore": 1,
  "ramSpikeTimePercentageThreshold": 10.333333333333334,
  "deviceResourcePerformanceScore": 14
}
```




