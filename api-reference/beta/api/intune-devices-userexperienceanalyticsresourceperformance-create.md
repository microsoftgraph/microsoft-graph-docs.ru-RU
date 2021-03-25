---
title: Создание userExperienceAnalyticsResourcePerformance
description: Создание нового объекта userExperienceAnalyticsResourcePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 400f21285e0f379cc59c9ab2c3497dad04ddbeab
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157809"
---
# <a name="create-userexperienceanalyticsresourceperformance"></a><span data-ttu-id="8b0fd-103">Создание userExperienceAnalyticsResourcePerformance</span><span class="sxs-lookup"><span data-stu-id="8b0fd-103">Create userExperienceAnalyticsResourcePerformance</span></span>

<span data-ttu-id="8b0fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b0fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b0fd-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b0fd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b0fd-107">Создание нового [объекта userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="8b0fd-107">Create a new [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b0fd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8b0fd-108">Prerequisites</span></span>
<span data-ttu-id="8b0fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b0fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b0fd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b0fd-111">Permission type</span></span>|<span data-ttu-id="8b0fd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b0fd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b0fd-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b0fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b0fd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b0fd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8b0fd-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b0fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b0fd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-116">Not supported.</span></span>|
|<span data-ttu-id="8b0fd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8b0fd-117">Application</span></span>|<span data-ttu-id="8b0fd-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b0fd-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b0fd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b0fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsResourcePerformance
```

## <a name="request-headers"></a><span data-ttu-id="8b0fd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8b0fd-120">Request headers</span></span>
|<span data-ttu-id="8b0fd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b0fd-121">Header</span></span>|<span data-ttu-id="8b0fd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8b0fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b0fd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b0fd-123">Authorization</span></span>|<span data-ttu-id="8b0fd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b0fd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8b0fd-125">Accept</span></span>|<span data-ttu-id="8b0fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b0fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b0fd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b0fd-127">Request body</span></span>
<span data-ttu-id="8b0fd-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsResourcePerformance.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-128">In the request body, supply a JSON representation for the userExperienceAnalyticsResourcePerformance object.</span></span>

<span data-ttu-id="8b0fd-129">В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsResourcePerformance.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-129">The following table shows the properties that are required when you create the userExperienceAnalyticsResourcePerformance.</span></span>

|<span data-ttu-id="8b0fd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b0fd-130">Property</span></span>|<span data-ttu-id="8b0fd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8b0fd-131">Type</span></span>|<span data-ttu-id="8b0fd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8b0fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b0fd-133">id</span><span class="sxs-lookup"><span data-stu-id="8b0fd-133">id</span></span>|<span data-ttu-id="8b0fd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8b0fd-134">String</span></span>|<span data-ttu-id="8b0fd-135">Уникальный идентификатор сущности производительности ресурсов аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-135">The unique identifier of the user experience analytics resource performance entity.</span></span>|
|<span data-ttu-id="8b0fd-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="8b0fd-136">deviceId</span></span>|<span data-ttu-id="8b0fd-137">String</span><span class="sxs-lookup"><span data-stu-id="8b0fd-137">String</span></span>|<span data-ttu-id="8b0fd-138">ID устройства.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-138">The id of the device.</span></span>|
|<span data-ttu-id="8b0fd-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="8b0fd-139">deviceName</span></span>|<span data-ttu-id="8b0fd-140">String</span><span class="sxs-lookup"><span data-stu-id="8b0fd-140">String</span></span>|<span data-ttu-id="8b0fd-141">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-141">The name of the device.</span></span>|
|<span data-ttu-id="8b0fd-142">model</span><span class="sxs-lookup"><span data-stu-id="8b0fd-142">model</span></span>|<span data-ttu-id="8b0fd-143">String</span><span class="sxs-lookup"><span data-stu-id="8b0fd-143">String</span></span>|<span data-ttu-id="8b0fd-144">Модель устройства аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-144">The user experience analytics device model.</span></span>|
|<span data-ttu-id="8b0fd-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="8b0fd-145">deviceCount</span></span>|<span data-ttu-id="8b0fd-146">Int64</span><span class="sxs-lookup"><span data-stu-id="8b0fd-146">Int64</span></span>|<span data-ttu-id="8b0fd-147">Аналитика пользовательских интерфейсов суммирует количество устройств.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-147">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="8b0fd-148">manufacturer</span><span class="sxs-lookup"><span data-stu-id="8b0fd-148">manufacturer</span></span>|<span data-ttu-id="8b0fd-149">String</span><span class="sxs-lookup"><span data-stu-id="8b0fd-149">String</span></span>|<span data-ttu-id="8b0fd-150">Производитель устройств аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-150">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="8b0fd-151">cpuSpikeTimePercentage</span><span class="sxs-lookup"><span data-stu-id="8b0fd-151">cpuSpikeTimePercentage</span></span>|<span data-ttu-id="8b0fd-152">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b0fd-152">Double</span></span>|<span data-ttu-id="8b0fd-153">Время пика ЦП в процентах.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-153">CPU spike time in percentage.</span></span> <span data-ttu-id="8b0fd-154">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="8b0fd-154">Valid values 0 to 100</span></span>|
|<span data-ttu-id="8b0fd-155">ramSpikeTimePercentage</span><span class="sxs-lookup"><span data-stu-id="8b0fd-155">ramSpikeTimePercentage</span></span>|<span data-ttu-id="8b0fd-156">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b0fd-156">Double</span></span>|<span data-ttu-id="8b0fd-157">Время пика оперативной памяти в процентах.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-157">RAM spike time in percentage.</span></span> <span data-ttu-id="8b0fd-158">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="8b0fd-158">Valid values 0 to 100</span></span>|
|<span data-ttu-id="8b0fd-159">cpuSpikeTimeScore</span><span class="sxs-lookup"><span data-stu-id="8b0fd-159">cpuSpikeTimeScore</span></span>|<span data-ttu-id="8b0fd-160">Int32</span><span class="sxs-lookup"><span data-stu-id="8b0fd-160">Int32</span></span>|<span data-ttu-id="8b0fd-161">Оценка времени пика пика ЦП для пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-161">The user experience analytics device CPU spike time score.</span></span> <span data-ttu-id="8b0fd-162">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="8b0fd-162">Valid values 0 to 100</span></span>|
|<span data-ttu-id="8b0fd-163">cpuSpikeTimePercentageThreshold</span><span class="sxs-lookup"><span data-stu-id="8b0fd-163">cpuSpikeTimePercentageThreshold</span></span>|<span data-ttu-id="8b0fd-164">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b0fd-164">Double</span></span>|<span data-ttu-id="8b0fd-165">Порог cpuSpikeTimeScore.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-165">Threshold of cpuSpikeTimeScore.</span></span> <span data-ttu-id="8b0fd-166">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="8b0fd-166">Valid values 0 to 100</span></span>|
|<span data-ttu-id="8b0fd-167">ramSpikeTimeScore</span><span class="sxs-lookup"><span data-stu-id="8b0fd-167">ramSpikeTimeScore</span></span>|<span data-ttu-id="8b0fd-168">Int32</span><span class="sxs-lookup"><span data-stu-id="8b0fd-168">Int32</span></span>|<span data-ttu-id="8b0fd-169">Оценка времени пика пика оперативной памяти устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-169">The user experience analytics device RAM spike time score.</span></span> <span data-ttu-id="8b0fd-170">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="8b0fd-170">Valid values 0 to 100</span></span>|
|<span data-ttu-id="8b0fd-171">ramSpikeTimePercentageThreshold</span><span class="sxs-lookup"><span data-stu-id="8b0fd-171">ramSpikeTimePercentageThreshold</span></span>|<span data-ttu-id="8b0fd-172">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b0fd-172">Double</span></span>|<span data-ttu-id="8b0fd-173">Порог ramSpikeTimeScore.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-173">Threshold of ramSpikeTimeScore.</span></span> <span data-ttu-id="8b0fd-174">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="8b0fd-174">Valid values 0 to 100</span></span>|
|<span data-ttu-id="8b0fd-175">deviceResourcePerformanceScore</span><span class="sxs-lookup"><span data-stu-id="8b0fd-175">deviceResourcePerformanceScore</span></span>|<span data-ttu-id="8b0fd-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8b0fd-176">Int32</span></span>|<span data-ttu-id="8b0fd-177">Оценка производительности ресурсов определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-177">Resource performance score of a specific device.</span></span> <span data-ttu-id="8b0fd-178">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="8b0fd-178">Valid values 0 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="8b0fd-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b0fd-179">Response</span></span>
<span data-ttu-id="8b0fd-180">В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-180">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b0fd-181">Пример</span><span class="sxs-lookup"><span data-stu-id="8b0fd-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b0fd-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b0fd-182">Request</span></span>
<span data-ttu-id="8b0fd-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsResourcePerformance
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

### <a name="response"></a><span data-ttu-id="8b0fd-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b0fd-184">Response</span></span>
<span data-ttu-id="8b0fd-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b0fd-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




