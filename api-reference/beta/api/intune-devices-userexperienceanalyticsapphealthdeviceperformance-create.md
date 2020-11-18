---
title: Создание Усерекспериенцеаналитиксапфеалсдевицеперформанце
description: Создание нового объекта Усерекспериенцеаналитиксапфеалсдевицеперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ef02600ac660ab328e79df1da68be17c4f1776ed
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202852"
---
# <a name="create-userexperienceanalyticsapphealthdeviceperformance"></a><span data-ttu-id="87372-103">Создание Усерекспериенцеаналитиксапфеалсдевицеперформанце</span><span class="sxs-lookup"><span data-stu-id="87372-103">Create userExperienceAnalyticsAppHealthDevicePerformance</span></span>

<span data-ttu-id="87372-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87372-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87372-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87372-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87372-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87372-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87372-107">Создание нового объекта [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="87372-107">Create a new [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87372-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="87372-108">Prerequisites</span></span>
<span data-ttu-id="87372-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87372-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87372-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87372-111">Permission type</span></span>|<span data-ttu-id="87372-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87372-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87372-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87372-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87372-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87372-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="87372-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87372-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87372-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87372-116">Not supported.</span></span>|
|<span data-ttu-id="87372-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="87372-117">Application</span></span>|<span data-ttu-id="87372-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87372-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87372-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87372-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="87372-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="87372-120">Request headers</span></span>
|<span data-ttu-id="87372-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87372-121">Header</span></span>|<span data-ttu-id="87372-122">Значение</span><span class="sxs-lookup"><span data-stu-id="87372-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87372-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87372-123">Authorization</span></span>|<span data-ttu-id="87372-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87372-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87372-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87372-125">Accept</span></span>|<span data-ttu-id="87372-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87372-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87372-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87372-127">Request body</span></span>
<span data-ttu-id="87372-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксапфеалсдевицеперформанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87372-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthDevicePerformance object.</span></span>

<span data-ttu-id="87372-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксапфеалсдевицеперформанце.</span><span class="sxs-lookup"><span data-stu-id="87372-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthDevicePerformance.</span></span>

|<span data-ttu-id="87372-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="87372-130">Property</span></span>|<span data-ttu-id="87372-131">Тип</span><span class="sxs-lookup"><span data-stu-id="87372-131">Type</span></span>|<span data-ttu-id="87372-132">Описание</span><span class="sxs-lookup"><span data-stu-id="87372-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87372-133">id</span><span class="sxs-lookup"><span data-stu-id="87372-133">id</span></span>|<span data-ttu-id="87372-134">String</span><span class="sxs-lookup"><span data-stu-id="87372-134">String</span></span>|<span data-ttu-id="87372-135">Уникальный идентификатор объекта производительности устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="87372-135">The unique identifier of the user experience analytics device performance object.</span></span>|
|<span data-ttu-id="87372-136">deviceModel</span><span class="sxs-lookup"><span data-stu-id="87372-136">deviceModel</span></span>|<span data-ttu-id="87372-137">String</span><span class="sxs-lookup"><span data-stu-id="87372-137">String</span></span>|<span data-ttu-id="87372-138">Имя модели устройства.</span><span class="sxs-lookup"><span data-stu-id="87372-138">The model name of the device.</span></span>|
|<span data-ttu-id="87372-139">девицемануфактурер</span><span class="sxs-lookup"><span data-stu-id="87372-139">deviceManufacturer</span></span>|<span data-ttu-id="87372-140">String</span><span class="sxs-lookup"><span data-stu-id="87372-140">String</span></span>|<span data-ttu-id="87372-141">Название изготовителя устройства.</span><span class="sxs-lookup"><span data-stu-id="87372-141">The manufacturer name of the device.</span></span>|
|<span data-ttu-id="87372-142">аппкрашкаунт</span><span class="sxs-lookup"><span data-stu-id="87372-142">appCrashCount</span></span>|<span data-ttu-id="87372-143">Int32</span><span class="sxs-lookup"><span data-stu-id="87372-143">Int32</span></span>|<span data-ttu-id="87372-144">Количество сбоев приложений для устройства.</span><span class="sxs-lookup"><span data-stu-id="87372-144">The number of app crashes for the device.</span></span> <span data-ttu-id="87372-145">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="87372-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="87372-146">крашедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="87372-146">crashedAppCount</span></span>|<span data-ttu-id="87372-147">Int32</span><span class="sxs-lookup"><span data-stu-id="87372-147">Int32</span></span>|<span data-ttu-id="87372-148">Количество отдельных сбоев приложений для устройства.</span><span class="sxs-lookup"><span data-stu-id="87372-148">The number of distinct app crashes for the device.</span></span> <span data-ttu-id="87372-149">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="87372-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="87372-150">апфангкаунт</span><span class="sxs-lookup"><span data-stu-id="87372-150">appHangCount</span></span>|<span data-ttu-id="87372-151">Int32</span><span class="sxs-lookup"><span data-stu-id="87372-151">Int32</span></span>|<span data-ttu-id="87372-152">Количество зависаний приложения для устройства.</span><span class="sxs-lookup"><span data-stu-id="87372-152">The number of app hangs for the device.</span></span> <span data-ttu-id="87372-153">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="87372-153">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="87372-154">меантиметофаилуреинминутес</span><span class="sxs-lookup"><span data-stu-id="87372-154">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="87372-155">Int32</span><span class="sxs-lookup"><span data-stu-id="87372-155">Int32</span></span>|<span data-ttu-id="87372-156">Среднее время до сбоя устройства в минутах.</span><span class="sxs-lookup"><span data-stu-id="87372-156">The mean time to failure for the device in minutes.</span></span> <span data-ttu-id="87372-157">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="87372-157">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="87372-158">девицеапфеалсскоре</span><span class="sxs-lookup"><span data-stu-id="87372-158">deviceAppHealthScore</span></span>|<span data-ttu-id="87372-159">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="87372-159">Double</span></span>|<span data-ttu-id="87372-160">Показатель работоспособности приложения для устройства.</span><span class="sxs-lookup"><span data-stu-id="87372-160">The app health score of the device.</span></span> <span data-ttu-id="87372-161">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="87372-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="87372-162">девицеапфеалсстатус</span><span class="sxs-lookup"><span data-stu-id="87372-162">deviceAppHealthStatus</span></span>|<span data-ttu-id="87372-163">String</span><span class="sxs-lookup"><span data-stu-id="87372-163">String</span></span>|<span data-ttu-id="87372-164">Общее состояние работоспособности приложений для устройства.</span><span class="sxs-lookup"><span data-stu-id="87372-164">The overall app health status of the device.</span></span>|
|<span data-ttu-id="87372-165">deviceId</span><span class="sxs-lookup"><span data-stu-id="87372-165">deviceId</span></span>|<span data-ttu-id="87372-166">String</span><span class="sxs-lookup"><span data-stu-id="87372-166">String</span></span>|<span data-ttu-id="87372-167">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="87372-167">The id of the device.</span></span>|
|<span data-ttu-id="87372-168">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="87372-168">deviceDisplayName</span></span>|<span data-ttu-id="87372-169">String</span><span class="sxs-lookup"><span data-stu-id="87372-169">String</span></span>|<span data-ttu-id="87372-170">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="87372-170">The name of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="87372-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="87372-171">Response</span></span>
<span data-ttu-id="87372-172">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="87372-172">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87372-173">Пример</span><span class="sxs-lookup"><span data-stu-id="87372-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="87372-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="87372-174">Request</span></span>
<span data-ttu-id="87372-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87372-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
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

### <a name="response"></a><span data-ttu-id="87372-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="87372-176">Response</span></span>
<span data-ttu-id="87372-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="87372-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




