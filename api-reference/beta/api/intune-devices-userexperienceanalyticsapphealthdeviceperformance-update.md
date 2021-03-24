---
title: Обновление userExperienceAnalyticsAppHealthDevicePerformance
description: Обновление свойств объекта userExperienceAnalyticsAppHealthDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a4c5a2b034c6a0e4870943c7054c47921eacd41
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136099"
---
# <a name="update-userexperienceanalyticsapphealthdeviceperformance"></a><span data-ttu-id="5249e-103">Обновление userExperienceAnalyticsAppHealthDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="5249e-103">Update userExperienceAnalyticsAppHealthDevicePerformance</span></span>

<span data-ttu-id="5249e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5249e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5249e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5249e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5249e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5249e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5249e-107">Обновление свойств объекта [userExperienceAnalyticsAppHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="5249e-107">Update the properties of a [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5249e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5249e-108">Prerequisites</span></span>
<span data-ttu-id="5249e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5249e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5249e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5249e-111">Permission type</span></span>|<span data-ttu-id="5249e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5249e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5249e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5249e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5249e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5249e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5249e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5249e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5249e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5249e-116">Not supported.</span></span>|
|<span data-ttu-id="5249e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5249e-117">Application</span></span>|<span data-ttu-id="5249e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5249e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5249e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5249e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance/{userExperienceAnalyticsAppHealthDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="5249e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5249e-120">Request headers</span></span>
|<span data-ttu-id="5249e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5249e-121">Header</span></span>|<span data-ttu-id="5249e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5249e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5249e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5249e-123">Authorization</span></span>|<span data-ttu-id="5249e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5249e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5249e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5249e-125">Accept</span></span>|<span data-ttu-id="5249e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5249e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5249e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5249e-127">Request body</span></span>
<span data-ttu-id="5249e-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsAppHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="5249e-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object.</span></span>

<span data-ttu-id="5249e-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsAppHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="5249e-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md).</span></span>

|<span data-ttu-id="5249e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5249e-130">Property</span></span>|<span data-ttu-id="5249e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5249e-131">Type</span></span>|<span data-ttu-id="5249e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5249e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5249e-133">id</span><span class="sxs-lookup"><span data-stu-id="5249e-133">id</span></span>|<span data-ttu-id="5249e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5249e-134">String</span></span>|<span data-ttu-id="5249e-135">Уникальный идентификатор объекта производительности устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="5249e-135">The unique identifier of the user experience analytics device performance object.</span></span>|
|<span data-ttu-id="5249e-136">deviceModel</span><span class="sxs-lookup"><span data-stu-id="5249e-136">deviceModel</span></span>|<span data-ttu-id="5249e-137">String</span><span class="sxs-lookup"><span data-stu-id="5249e-137">String</span></span>|<span data-ttu-id="5249e-138">Имя модели устройства.</span><span class="sxs-lookup"><span data-stu-id="5249e-138">The model name of the device.</span></span>|
|<span data-ttu-id="5249e-139">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="5249e-139">deviceManufacturer</span></span>|<span data-ttu-id="5249e-140">Строка</span><span class="sxs-lookup"><span data-stu-id="5249e-140">String</span></span>|<span data-ttu-id="5249e-141">Имя производителя устройства.</span><span class="sxs-lookup"><span data-stu-id="5249e-141">The manufacturer name of the device.</span></span>|
|<span data-ttu-id="5249e-142">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="5249e-142">appCrashCount</span></span>|<span data-ttu-id="5249e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5249e-143">Int32</span></span>|<span data-ttu-id="5249e-144">Количество сбоей приложения для устройства.</span><span class="sxs-lookup"><span data-stu-id="5249e-144">The number of app crashes for the device.</span></span> <span data-ttu-id="5249e-145">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="5249e-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="5249e-146">crashedAppCount</span><span class="sxs-lookup"><span data-stu-id="5249e-146">crashedAppCount</span></span>|<span data-ttu-id="5249e-147">Int32</span><span class="sxs-lookup"><span data-stu-id="5249e-147">Int32</span></span>|<span data-ttu-id="5249e-148">Количество различных сбоей приложения для устройства.</span><span class="sxs-lookup"><span data-stu-id="5249e-148">The number of distinct app crashes for the device.</span></span> <span data-ttu-id="5249e-149">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="5249e-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="5249e-150">appHangCount</span><span class="sxs-lookup"><span data-stu-id="5249e-150">appHangCount</span></span>|<span data-ttu-id="5249e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="5249e-151">Int32</span></span>|<span data-ttu-id="5249e-152">Для устройства зависает число приложений.</span><span class="sxs-lookup"><span data-stu-id="5249e-152">The number of app hangs for the device.</span></span> <span data-ttu-id="5249e-153">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="5249e-153">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="5249e-154">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="5249e-154">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="5249e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="5249e-155">Int32</span></span>|<span data-ttu-id="5249e-156">Время сбоя устройства в минутах.</span><span class="sxs-lookup"><span data-stu-id="5249e-156">The mean time to failure for the device in minutes.</span></span> <span data-ttu-id="5249e-157">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="5249e-157">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="5249e-158">deviceAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="5249e-158">deviceAppHealthScore</span></span>|<span data-ttu-id="5249e-159">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="5249e-159">Double</span></span>|<span data-ttu-id="5249e-160">Оценка состояния приложения устройства.</span><span class="sxs-lookup"><span data-stu-id="5249e-160">The app health score of the device.</span></span> <span data-ttu-id="5249e-161">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="5249e-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="5249e-162">deviceAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="5249e-162">deviceAppHealthStatus</span></span>|<span data-ttu-id="5249e-163">Строка</span><span class="sxs-lookup"><span data-stu-id="5249e-163">String</span></span>|<span data-ttu-id="5249e-164">Общее состояние состояния здоровья приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="5249e-164">The overall app health status of the device.</span></span>|
|<span data-ttu-id="5249e-165">deviceId</span><span class="sxs-lookup"><span data-stu-id="5249e-165">deviceId</span></span>|<span data-ttu-id="5249e-166">String</span><span class="sxs-lookup"><span data-stu-id="5249e-166">String</span></span>|<span data-ttu-id="5249e-167">ID устройства.</span><span class="sxs-lookup"><span data-stu-id="5249e-167">The id of the device.</span></span>|
|<span data-ttu-id="5249e-168">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="5249e-168">deviceDisplayName</span></span>|<span data-ttu-id="5249e-169">String</span><span class="sxs-lookup"><span data-stu-id="5249e-169">String</span></span>|<span data-ttu-id="5249e-170">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="5249e-170">The name of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="5249e-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="5249e-171">Response</span></span>
<span data-ttu-id="5249e-172">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5249e-172">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5249e-173">Пример</span><span class="sxs-lookup"><span data-stu-id="5249e-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="5249e-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="5249e-174">Request</span></span>
<span data-ttu-id="5249e-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5249e-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance/{userExperienceAnalyticsAppHealthDevicePerformanceId}
Content-type: application/json
Content-length: 490

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "appCrashCount": 13,
  "crashedAppCount": 15,
  "appHangCount": 12,
  "meanTimeToFailureInMinutes": 10,
  "deviceAppHealthScore": 6.666666666666667,
  "deviceAppHealthStatus": "Device App Health Status value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="5249e-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="5249e-176">Response</span></span>
<span data-ttu-id="5249e-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5249e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "id": "2c651499-1499-2c65-9914-652c9914652c",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "appCrashCount": 13,
  "crashedAppCount": 15,
  "appHangCount": 12,
  "meanTimeToFailureInMinutes": 10,
  "deviceAppHealthScore": 6.666666666666667,
  "deviceAppHealthStatus": "Device App Health Status value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```




