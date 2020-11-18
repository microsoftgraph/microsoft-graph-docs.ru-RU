---
title: Обновление Усерекспериенцеаналитиксапфеалсдевицеперформанце
description: Обновление свойств объекта Усерекспериенцеаналитиксапфеалсдевицеперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c14e2b4b2955dc028ab45aab5db87710e6780acc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202825"
---
# <a name="update-userexperienceanalyticsapphealthdeviceperformance"></a><span data-ttu-id="1c02f-103">Обновление Усерекспериенцеаналитиксапфеалсдевицеперформанце</span><span class="sxs-lookup"><span data-stu-id="1c02f-103">Update userExperienceAnalyticsAppHealthDevicePerformance</span></span>

<span data-ttu-id="1c02f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c02f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c02f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c02f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c02f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c02f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c02f-107">Обновление свойств объекта [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="1c02f-107">Update the properties of a [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c02f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1c02f-108">Prerequisites</span></span>
<span data-ttu-id="1c02f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c02f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c02f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c02f-111">Permission type</span></span>|<span data-ttu-id="1c02f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c02f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c02f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c02f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c02f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c02f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1c02f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c02f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c02f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c02f-116">Not supported.</span></span>|
|<span data-ttu-id="1c02f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1c02f-117">Application</span></span>|<span data-ttu-id="1c02f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c02f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c02f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c02f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance/{userExperienceAnalyticsAppHealthDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="1c02f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1c02f-120">Request headers</span></span>
|<span data-ttu-id="1c02f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c02f-121">Header</span></span>|<span data-ttu-id="1c02f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1c02f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c02f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c02f-123">Authorization</span></span>|<span data-ttu-id="1c02f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c02f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c02f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1c02f-125">Accept</span></span>|<span data-ttu-id="1c02f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c02f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c02f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c02f-127">Request body</span></span>
<span data-ttu-id="1c02f-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c02f-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object.</span></span>

<span data-ttu-id="1c02f-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md).</span><span class="sxs-lookup"><span data-stu-id="1c02f-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md).</span></span>

|<span data-ttu-id="1c02f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c02f-130">Property</span></span>|<span data-ttu-id="1c02f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1c02f-131">Type</span></span>|<span data-ttu-id="1c02f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1c02f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c02f-133">id</span><span class="sxs-lookup"><span data-stu-id="1c02f-133">id</span></span>|<span data-ttu-id="1c02f-134">String</span><span class="sxs-lookup"><span data-stu-id="1c02f-134">String</span></span>|<span data-ttu-id="1c02f-135">Уникальный идентификатор объекта производительности устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="1c02f-135">The unique identifier of the user experience analytics device performance object.</span></span>|
|<span data-ttu-id="1c02f-136">deviceModel</span><span class="sxs-lookup"><span data-stu-id="1c02f-136">deviceModel</span></span>|<span data-ttu-id="1c02f-137">String</span><span class="sxs-lookup"><span data-stu-id="1c02f-137">String</span></span>|<span data-ttu-id="1c02f-138">Имя модели устройства.</span><span class="sxs-lookup"><span data-stu-id="1c02f-138">The model name of the device.</span></span>|
|<span data-ttu-id="1c02f-139">девицемануфактурер</span><span class="sxs-lookup"><span data-stu-id="1c02f-139">deviceManufacturer</span></span>|<span data-ttu-id="1c02f-140">String</span><span class="sxs-lookup"><span data-stu-id="1c02f-140">String</span></span>|<span data-ttu-id="1c02f-141">Название изготовителя устройства.</span><span class="sxs-lookup"><span data-stu-id="1c02f-141">The manufacturer name of the device.</span></span>|
|<span data-ttu-id="1c02f-142">аппкрашкаунт</span><span class="sxs-lookup"><span data-stu-id="1c02f-142">appCrashCount</span></span>|<span data-ttu-id="1c02f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1c02f-143">Int32</span></span>|<span data-ttu-id="1c02f-144">Количество сбоев приложений для устройства.</span><span class="sxs-lookup"><span data-stu-id="1c02f-144">The number of app crashes for the device.</span></span> <span data-ttu-id="1c02f-145">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="1c02f-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="1c02f-146">крашедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="1c02f-146">crashedAppCount</span></span>|<span data-ttu-id="1c02f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="1c02f-147">Int32</span></span>|<span data-ttu-id="1c02f-148">Количество отдельных сбоев приложений для устройства.</span><span class="sxs-lookup"><span data-stu-id="1c02f-148">The number of distinct app crashes for the device.</span></span> <span data-ttu-id="1c02f-149">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="1c02f-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="1c02f-150">апфангкаунт</span><span class="sxs-lookup"><span data-stu-id="1c02f-150">appHangCount</span></span>|<span data-ttu-id="1c02f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1c02f-151">Int32</span></span>|<span data-ttu-id="1c02f-152">Количество зависаний приложения для устройства.</span><span class="sxs-lookup"><span data-stu-id="1c02f-152">The number of app hangs for the device.</span></span> <span data-ttu-id="1c02f-153">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="1c02f-153">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="1c02f-154">меантиметофаилуреинминутес</span><span class="sxs-lookup"><span data-stu-id="1c02f-154">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="1c02f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="1c02f-155">Int32</span></span>|<span data-ttu-id="1c02f-156">Среднее время до сбоя устройства в минутах.</span><span class="sxs-lookup"><span data-stu-id="1c02f-156">The mean time to failure for the device in minutes.</span></span> <span data-ttu-id="1c02f-157">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="1c02f-157">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="1c02f-158">девицеапфеалсскоре</span><span class="sxs-lookup"><span data-stu-id="1c02f-158">deviceAppHealthScore</span></span>|<span data-ttu-id="1c02f-159">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="1c02f-159">Double</span></span>|<span data-ttu-id="1c02f-160">Показатель работоспособности приложения для устройства.</span><span class="sxs-lookup"><span data-stu-id="1c02f-160">The app health score of the device.</span></span> <span data-ttu-id="1c02f-161">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="1c02f-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="1c02f-162">девицеапфеалсстатус</span><span class="sxs-lookup"><span data-stu-id="1c02f-162">deviceAppHealthStatus</span></span>|<span data-ttu-id="1c02f-163">String</span><span class="sxs-lookup"><span data-stu-id="1c02f-163">String</span></span>|<span data-ttu-id="1c02f-164">Общее состояние работоспособности приложений для устройства.</span><span class="sxs-lookup"><span data-stu-id="1c02f-164">The overall app health status of the device.</span></span>|
|<span data-ttu-id="1c02f-165">deviceId</span><span class="sxs-lookup"><span data-stu-id="1c02f-165">deviceId</span></span>|<span data-ttu-id="1c02f-166">String</span><span class="sxs-lookup"><span data-stu-id="1c02f-166">String</span></span>|<span data-ttu-id="1c02f-167">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="1c02f-167">The id of the device.</span></span>|
|<span data-ttu-id="1c02f-168">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="1c02f-168">deviceDisplayName</span></span>|<span data-ttu-id="1c02f-169">String</span><span class="sxs-lookup"><span data-stu-id="1c02f-169">String</span></span>|<span data-ttu-id="1c02f-170">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="1c02f-170">The name of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="1c02f-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c02f-171">Response</span></span>
<span data-ttu-id="1c02f-172">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c02f-172">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c02f-173">Пример</span><span class="sxs-lookup"><span data-stu-id="1c02f-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c02f-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c02f-174">Request</span></span>
<span data-ttu-id="1c02f-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c02f-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1c02f-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c02f-176">Response</span></span>
<span data-ttu-id="1c02f-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c02f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




