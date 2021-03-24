---
title: Создание userExperienceAnalyticsAppHealthDevicePerformance
description: Создание нового объекта userExperienceAnalyticsAppHealthDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b10beeca6d79b8dc596cfa509a5a1a817af9a346
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136134"
---
# <a name="create-userexperienceanalyticsapphealthdeviceperformance"></a><span data-ttu-id="6dd04-103">Создание userExperienceAnalyticsAppHealthDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="6dd04-103">Create userExperienceAnalyticsAppHealthDevicePerformance</span></span>

<span data-ttu-id="6dd04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dd04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6dd04-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dd04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dd04-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6dd04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dd04-107">Создание нового [объекта userExperienceAnalyticsAppHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="6dd04-107">Create a new [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dd04-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6dd04-108">Prerequisites</span></span>
<span data-ttu-id="6dd04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dd04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dd04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dd04-111">Permission type</span></span>|<span data-ttu-id="6dd04-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dd04-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dd04-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dd04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6dd04-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dd04-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6dd04-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dd04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dd04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dd04-116">Not supported.</span></span>|
|<span data-ttu-id="6dd04-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6dd04-117">Application</span></span>|<span data-ttu-id="6dd04-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dd04-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dd04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dd04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="6dd04-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6dd04-120">Request headers</span></span>
|<span data-ttu-id="6dd04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6dd04-121">Header</span></span>|<span data-ttu-id="6dd04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6dd04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dd04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dd04-123">Authorization</span></span>|<span data-ttu-id="6dd04-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6dd04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dd04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6dd04-125">Accept</span></span>|<span data-ttu-id="6dd04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6dd04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dd04-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6dd04-127">Request body</span></span>
<span data-ttu-id="6dd04-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsAppHealthDevicePerformance.</span><span class="sxs-lookup"><span data-stu-id="6dd04-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthDevicePerformance object.</span></span>

<span data-ttu-id="6dd04-129">В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsAppHealthDevicePerformance.</span><span class="sxs-lookup"><span data-stu-id="6dd04-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthDevicePerformance.</span></span>

|<span data-ttu-id="6dd04-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6dd04-130">Property</span></span>|<span data-ttu-id="6dd04-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6dd04-131">Type</span></span>|<span data-ttu-id="6dd04-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6dd04-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dd04-133">id</span><span class="sxs-lookup"><span data-stu-id="6dd04-133">id</span></span>|<span data-ttu-id="6dd04-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6dd04-134">String</span></span>|<span data-ttu-id="6dd04-135">Уникальный идентификатор объекта производительности устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="6dd04-135">The unique identifier of the user experience analytics device performance object.</span></span>|
|<span data-ttu-id="6dd04-136">deviceModel</span><span class="sxs-lookup"><span data-stu-id="6dd04-136">deviceModel</span></span>|<span data-ttu-id="6dd04-137">String</span><span class="sxs-lookup"><span data-stu-id="6dd04-137">String</span></span>|<span data-ttu-id="6dd04-138">Имя модели устройства.</span><span class="sxs-lookup"><span data-stu-id="6dd04-138">The model name of the device.</span></span>|
|<span data-ttu-id="6dd04-139">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="6dd04-139">deviceManufacturer</span></span>|<span data-ttu-id="6dd04-140">Строка</span><span class="sxs-lookup"><span data-stu-id="6dd04-140">String</span></span>|<span data-ttu-id="6dd04-141">Имя производителя устройства.</span><span class="sxs-lookup"><span data-stu-id="6dd04-141">The manufacturer name of the device.</span></span>|
|<span data-ttu-id="6dd04-142">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="6dd04-142">appCrashCount</span></span>|<span data-ttu-id="6dd04-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6dd04-143">Int32</span></span>|<span data-ttu-id="6dd04-144">Количество сбоей приложения для устройства.</span><span class="sxs-lookup"><span data-stu-id="6dd04-144">The number of app crashes for the device.</span></span> <span data-ttu-id="6dd04-145">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="6dd04-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="6dd04-146">crashedAppCount</span><span class="sxs-lookup"><span data-stu-id="6dd04-146">crashedAppCount</span></span>|<span data-ttu-id="6dd04-147">Int32</span><span class="sxs-lookup"><span data-stu-id="6dd04-147">Int32</span></span>|<span data-ttu-id="6dd04-148">Количество различных сбоей приложения для устройства.</span><span class="sxs-lookup"><span data-stu-id="6dd04-148">The number of distinct app crashes for the device.</span></span> <span data-ttu-id="6dd04-149">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="6dd04-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="6dd04-150">appHangCount</span><span class="sxs-lookup"><span data-stu-id="6dd04-150">appHangCount</span></span>|<span data-ttu-id="6dd04-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6dd04-151">Int32</span></span>|<span data-ttu-id="6dd04-152">Для устройства зависает число приложений.</span><span class="sxs-lookup"><span data-stu-id="6dd04-152">The number of app hangs for the device.</span></span> <span data-ttu-id="6dd04-153">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="6dd04-153">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="6dd04-154">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="6dd04-154">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="6dd04-155">Int32</span><span class="sxs-lookup"><span data-stu-id="6dd04-155">Int32</span></span>|<span data-ttu-id="6dd04-156">Время сбоя устройства в минутах.</span><span class="sxs-lookup"><span data-stu-id="6dd04-156">The mean time to failure for the device in minutes.</span></span> <span data-ttu-id="6dd04-157">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="6dd04-157">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="6dd04-158">deviceAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="6dd04-158">deviceAppHealthScore</span></span>|<span data-ttu-id="6dd04-159">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="6dd04-159">Double</span></span>|<span data-ttu-id="6dd04-160">Оценка состояния приложения устройства.</span><span class="sxs-lookup"><span data-stu-id="6dd04-160">The app health score of the device.</span></span> <span data-ttu-id="6dd04-161">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="6dd04-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="6dd04-162">deviceAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="6dd04-162">deviceAppHealthStatus</span></span>|<span data-ttu-id="6dd04-163">Строка</span><span class="sxs-lookup"><span data-stu-id="6dd04-163">String</span></span>|<span data-ttu-id="6dd04-164">Общее состояние состояния здоровья приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6dd04-164">The overall app health status of the device.</span></span>|
|<span data-ttu-id="6dd04-165">deviceId</span><span class="sxs-lookup"><span data-stu-id="6dd04-165">deviceId</span></span>|<span data-ttu-id="6dd04-166">String</span><span class="sxs-lookup"><span data-stu-id="6dd04-166">String</span></span>|<span data-ttu-id="6dd04-167">ID устройства.</span><span class="sxs-lookup"><span data-stu-id="6dd04-167">The id of the device.</span></span>|
|<span data-ttu-id="6dd04-168">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6dd04-168">deviceDisplayName</span></span>|<span data-ttu-id="6dd04-169">String</span><span class="sxs-lookup"><span data-stu-id="6dd04-169">String</span></span>|<span data-ttu-id="6dd04-170">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="6dd04-170">The name of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="6dd04-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dd04-171">Response</span></span>
<span data-ttu-id="6dd04-172">В случае успеха этот метод возвращает код ответа и `201 Created` [объект userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6dd04-172">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dd04-173">Пример</span><span class="sxs-lookup"><span data-stu-id="6dd04-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dd04-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dd04-174">Request</span></span>
<span data-ttu-id="6dd04-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6dd04-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6dd04-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dd04-176">Response</span></span>
<span data-ttu-id="6dd04-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6dd04-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




