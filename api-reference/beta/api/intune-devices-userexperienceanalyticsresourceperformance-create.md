---
title: Создание userExperienceAnalyticsResourcePerformance
description: Создание объекта userExperienceAnalyticsResourcePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b35601c4ad92313d910d4813ac8ace84c4fce9da
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162516"
---
# <a name="create-userexperienceanalyticsresourceperformance"></a><span data-ttu-id="4276e-103">Создание userExperienceAnalyticsResourcePerformance</span><span class="sxs-lookup"><span data-stu-id="4276e-103">Create userExperienceAnalyticsResourcePerformance</span></span>

<span data-ttu-id="4276e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4276e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4276e-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4276e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4276e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4276e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4276e-107">Создание объекта [userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="4276e-107">Create a new [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4276e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4276e-108">Prerequisites</span></span>
<span data-ttu-id="4276e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4276e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4276e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4276e-111">Permission type</span></span>|<span data-ttu-id="4276e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4276e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4276e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4276e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4276e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4276e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4276e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4276e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4276e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4276e-116">Not supported.</span></span>|
|<span data-ttu-id="4276e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4276e-117">Application</span></span>|<span data-ttu-id="4276e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4276e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4276e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4276e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsResourcePerformance
```

## <a name="request-headers"></a><span data-ttu-id="4276e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4276e-120">Request headers</span></span>
|<span data-ttu-id="4276e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4276e-121">Header</span></span>|<span data-ttu-id="4276e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4276e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4276e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4276e-123">Authorization</span></span>|<span data-ttu-id="4276e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4276e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4276e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4276e-125">Accept</span></span>|<span data-ttu-id="4276e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4276e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4276e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4276e-127">Request body</span></span>
<span data-ttu-id="4276e-128">В теле запроса укажу представление объекта userExperienceAnalyticsResourcePerformance в JSON.</span><span class="sxs-lookup"><span data-stu-id="4276e-128">In the request body, supply a JSON representation for the userExperienceAnalyticsResourcePerformance object.</span></span>

<span data-ttu-id="4276e-129">В следующей таблице показаны свойства, необходимые при создании объекта userExperienceAnalyticsResourcePerformance.</span><span class="sxs-lookup"><span data-stu-id="4276e-129">The following table shows the properties that are required when you create the userExperienceAnalyticsResourcePerformance.</span></span>

|<span data-ttu-id="4276e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4276e-130">Property</span></span>|<span data-ttu-id="4276e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4276e-131">Type</span></span>|<span data-ttu-id="4276e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4276e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4276e-133">id</span><span class="sxs-lookup"><span data-stu-id="4276e-133">id</span></span>|<span data-ttu-id="4276e-134">String</span><span class="sxs-lookup"><span data-stu-id="4276e-134">String</span></span>|<span data-ttu-id="4276e-135">Уникальный идентификатор сущности производительности ресурсов аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="4276e-135">The unique identifier of the user experience analytics resource performance entity.</span></span>|
|<span data-ttu-id="4276e-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="4276e-136">deviceId</span></span>|<span data-ttu-id="4276e-137">String</span><span class="sxs-lookup"><span data-stu-id="4276e-137">String</span></span>|<span data-ttu-id="4276e-138">ИД устройства.</span><span class="sxs-lookup"><span data-stu-id="4276e-138">The id of the device.</span></span>|
|<span data-ttu-id="4276e-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="4276e-139">deviceName</span></span>|<span data-ttu-id="4276e-140">String</span><span class="sxs-lookup"><span data-stu-id="4276e-140">String</span></span>|<span data-ttu-id="4276e-141">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="4276e-141">The name of the device.</span></span>|
|<span data-ttu-id="4276e-142">model</span><span class="sxs-lookup"><span data-stu-id="4276e-142">model</span></span>|<span data-ttu-id="4276e-143">String</span><span class="sxs-lookup"><span data-stu-id="4276e-143">String</span></span>|<span data-ttu-id="4276e-144">Модель устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="4276e-144">The user experience analytics device model.</span></span>|
|<span data-ttu-id="4276e-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="4276e-145">deviceCount</span></span>|<span data-ttu-id="4276e-146">Int64</span><span class="sxs-lookup"><span data-stu-id="4276e-146">Int64</span></span>|<span data-ttu-id="4276e-147">Аналитика пользовательского интерфейса суммирует количество устройств.</span><span class="sxs-lookup"><span data-stu-id="4276e-147">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="4276e-148">manufacturer</span><span class="sxs-lookup"><span data-stu-id="4276e-148">manufacturer</span></span>|<span data-ttu-id="4276e-149">String</span><span class="sxs-lookup"><span data-stu-id="4276e-149">String</span></span>|<span data-ttu-id="4276e-150">Изготовитель устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="4276e-150">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="4276e-151">cpuSpikeTimePercentage</span><span class="sxs-lookup"><span data-stu-id="4276e-151">cpuSpikeTimePercentage</span></span>|<span data-ttu-id="4276e-152">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4276e-152">Double</span></span>|<span data-ttu-id="4276e-153">Время пика ЦП в процентах.</span><span class="sxs-lookup"><span data-stu-id="4276e-153">CPU spike time in percentage.</span></span> <span data-ttu-id="4276e-154">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="4276e-154">Valid values 0 to 100</span></span>|
|<span data-ttu-id="4276e-155">ramSpikeTimePercentage</span><span class="sxs-lookup"><span data-stu-id="4276e-155">ramSpikeTimePercentage</span></span>|<span data-ttu-id="4276e-156">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4276e-156">Double</span></span>|<span data-ttu-id="4276e-157">Время пика ОЗУ в процентах.</span><span class="sxs-lookup"><span data-stu-id="4276e-157">RAM spike time in percentage.</span></span> <span data-ttu-id="4276e-158">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="4276e-158">Valid values 0 to 100</span></span>|
|<span data-ttu-id="4276e-159">cpuSpikeTimeScore</span><span class="sxs-lookup"><span data-stu-id="4276e-159">cpuSpikeTimeScore</span></span>|<span data-ttu-id="4276e-160">Int32</span><span class="sxs-lookup"><span data-stu-id="4276e-160">Int32</span></span>|<span data-ttu-id="4276e-161">Оценка времени пика пика ЦП устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="4276e-161">The user experience analytics device CPU spike time score.</span></span> <span data-ttu-id="4276e-162">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="4276e-162">Valid values 0 to 100</span></span>|
|<span data-ttu-id="4276e-163">cpuSpikeTimePercentageThreshold</span><span class="sxs-lookup"><span data-stu-id="4276e-163">cpuSpikeTimePercentageThreshold</span></span>|<span data-ttu-id="4276e-164">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4276e-164">Double</span></span>|<span data-ttu-id="4276e-165">Пороговое значение cpuSpikeTimeScore.</span><span class="sxs-lookup"><span data-stu-id="4276e-165">Threshold of cpuSpikeTimeScore.</span></span> <span data-ttu-id="4276e-166">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="4276e-166">Valid values 0 to 100</span></span>|
|<span data-ttu-id="4276e-167">ramSpikeTimeScore</span><span class="sxs-lookup"><span data-stu-id="4276e-167">ramSpikeTimeScore</span></span>|<span data-ttu-id="4276e-168">Int32</span><span class="sxs-lookup"><span data-stu-id="4276e-168">Int32</span></span>|<span data-ttu-id="4276e-169">Показатель времени пика пика ОЗУ устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="4276e-169">The user experience analytics device RAM spike time score.</span></span> <span data-ttu-id="4276e-170">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="4276e-170">Valid values 0 to 100</span></span>|
|<span data-ttu-id="4276e-171">ramSpikeTimePercentageThreshold</span><span class="sxs-lookup"><span data-stu-id="4276e-171">ramSpikeTimePercentageThreshold</span></span>|<span data-ttu-id="4276e-172">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4276e-172">Double</span></span>|<span data-ttu-id="4276e-173">Пороговое значение ramSpikeTimeScore.</span><span class="sxs-lookup"><span data-stu-id="4276e-173">Threshold of ramSpikeTimeScore.</span></span> <span data-ttu-id="4276e-174">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="4276e-174">Valid values 0 to 100</span></span>|
|<span data-ttu-id="4276e-175">deviceResourcePerformanceScore</span><span class="sxs-lookup"><span data-stu-id="4276e-175">deviceResourcePerformanceScore</span></span>|<span data-ttu-id="4276e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4276e-176">Int32</span></span>|<span data-ttu-id="4276e-177">Оценка производительности ресурсов для конкретного устройства.</span><span class="sxs-lookup"><span data-stu-id="4276e-177">Resource performance score of a specific device.</span></span> <span data-ttu-id="4276e-178">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="4276e-178">Valid values 0 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="4276e-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="4276e-179">Response</span></span>
<span data-ttu-id="4276e-180">В случае успеха этот метод возвращает код отклика и объект `201 Created` [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4276e-180">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4276e-181">Пример</span><span class="sxs-lookup"><span data-stu-id="4276e-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="4276e-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="4276e-182">Request</span></span>
<span data-ttu-id="4276e-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4276e-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4276e-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="4276e-184">Response</span></span>
<span data-ttu-id="4276e-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4276e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




