---
title: Обновление userExperienceAnalyticsDevicePerformance
description: Обновление свойств объекта userExperienceAnalyticsDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b9ddba61608e2b215d419c341a0240667fca4840
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154156"
---
# <a name="update-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="d2d35-103">Обновление userExperienceAnalyticsDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="d2d35-103">Update userExperienceAnalyticsDevicePerformance</span></span>

<span data-ttu-id="d2d35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2d35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2d35-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2d35-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2d35-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2d35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2d35-107">Обновление свойств объекта [userExperienceAnalyticsDevicePerformance.](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="d2d35-107">Update the properties of a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2d35-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d2d35-108">Prerequisites</span></span>
<span data-ttu-id="d2d35-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2d35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2d35-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2d35-111">Permission type</span></span>|<span data-ttu-id="d2d35-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2d35-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2d35-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2d35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2d35-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d35-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d2d35-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2d35-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2d35-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2d35-116">Not supported.</span></span>|
|<span data-ttu-id="d2d35-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d2d35-117">Application</span></span>|<span data-ttu-id="d2d35-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d35-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2d35-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2d35-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="d2d35-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d2d35-120">Request headers</span></span>
|<span data-ttu-id="d2d35-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2d35-121">Header</span></span>|<span data-ttu-id="d2d35-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d2d35-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2d35-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2d35-123">Authorization</span></span>|<span data-ttu-id="d2d35-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2d35-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2d35-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d2d35-125">Accept</span></span>|<span data-ttu-id="d2d35-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2d35-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2d35-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2d35-127">Request body</span></span>
<span data-ttu-id="d2d35-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsDevicePerformance.](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="d2d35-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

<span data-ttu-id="d2d35-129">В следующей таблице показаны свойства, необходимые при создании [пользователяExperienceAnalyticsDevicePerformance.](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="d2d35-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span></span>

|<span data-ttu-id="d2d35-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2d35-130">Property</span></span>|<span data-ttu-id="d2d35-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d2d35-131">Type</span></span>|<span data-ttu-id="d2d35-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d2d35-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2d35-133">id</span><span class="sxs-lookup"><span data-stu-id="d2d35-133">id</span></span>|<span data-ttu-id="d2d35-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d2d35-134">String</span></span>|<span data-ttu-id="d2d35-135">Уникальный идентификатор устройства загрузки загрузочного устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="d2d35-135">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="d2d35-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="d2d35-136">deviceName</span></span>|<span data-ttu-id="d2d35-137">String</span><span class="sxs-lookup"><span data-stu-id="d2d35-137">String</span></span>|<span data-ttu-id="d2d35-138">Имя устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="d2d35-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="d2d35-139">model</span><span class="sxs-lookup"><span data-stu-id="d2d35-139">model</span></span>|<span data-ttu-id="d2d35-140">String</span><span class="sxs-lookup"><span data-stu-id="d2d35-140">String</span></span>|<span data-ttu-id="d2d35-141">Модель устройства аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="d2d35-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="d2d35-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="d2d35-142">manufacturer</span></span>|<span data-ttu-id="d2d35-143">String</span><span class="sxs-lookup"><span data-stu-id="d2d35-143">String</span></span>|<span data-ttu-id="d2d35-144">Производитель устройств аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="d2d35-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="d2d35-145">diskType</span><span class="sxs-lookup"><span data-stu-id="d2d35-145">diskType</span></span>|[<span data-ttu-id="d2d35-146">diskType</span><span class="sxs-lookup"><span data-stu-id="d2d35-146">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="d2d35-147">Тип диска для аналитики пользовательского интерфейса устройства.</span><span class="sxs-lookup"><span data-stu-id="d2d35-147">The user experience analytics device disk type.</span></span> <span data-ttu-id="d2d35-148">Возможные значения: `unkown`, `hdd`, `ssd`.</span><span class="sxs-lookup"><span data-stu-id="d2d35-148">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="d2d35-149">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="d2d35-149">operatingSystemVersion</span></span>|<span data-ttu-id="d2d35-150">String</span><span class="sxs-lookup"><span data-stu-id="d2d35-150">String</span></span>|<span data-ttu-id="d2d35-151">Версия операционной системы для аналитики пользовательского интерфейса устройства.</span><span class="sxs-lookup"><span data-stu-id="d2d35-151">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="d2d35-152">bootScore</span><span class="sxs-lookup"><span data-stu-id="d2d35-152">bootScore</span></span>|<span data-ttu-id="d2d35-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d2d35-153">Int32</span></span>|<span data-ttu-id="d2d35-154">Оценка загрузки устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="d2d35-154">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="d2d35-155">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="d2d35-155">coreBootTimeInMs</span></span>|<span data-ttu-id="d2d35-156">Int32</span><span class="sxs-lookup"><span data-stu-id="d2d35-156">Int32</span></span>|<span data-ttu-id="d2d35-157">Основное время загрузки устройства для аналитики пользовательского интерфейса в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="d2d35-157">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="d2d35-158">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="d2d35-158">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="d2d35-159">Int32</span><span class="sxs-lookup"><span data-stu-id="d2d35-159">Int32</span></span>|<span data-ttu-id="d2d35-160">Время загрузки групповой политики устройств для пользовательского интерфейса в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="d2d35-160">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="d2d35-161">healthStatus</span><span class="sxs-lookup"><span data-stu-id="d2d35-161">healthStatus</span></span>|[<span data-ttu-id="d2d35-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="d2d35-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="d2d35-163">Состояние здоровья устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="d2d35-163">The health state of the user experience analytics device.</span></span> <span data-ttu-id="d2d35-164">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="d2d35-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="d2d35-165">loginScore</span><span class="sxs-lookup"><span data-stu-id="d2d35-165">loginScore</span></span>|<span data-ttu-id="d2d35-166">Int32</span><span class="sxs-lookup"><span data-stu-id="d2d35-166">Int32</span></span>|<span data-ttu-id="d2d35-167">Оценка входа устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="d2d35-167">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="d2d35-168">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="d2d35-168">coreLoginTimeInMs</span></span>|<span data-ttu-id="d2d35-169">Int32</span><span class="sxs-lookup"><span data-stu-id="d2d35-169">Int32</span></span>|<span data-ttu-id="d2d35-170">Время входа основного устройства для аналитики пользовательского интерфейса в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="d2d35-170">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="d2d35-171">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="d2d35-171">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="d2d35-172">Int32</span><span class="sxs-lookup"><span data-stu-id="d2d35-172">Int32</span></span>|<span data-ttu-id="d2d35-173">Время входа в группу политик пользовательского интерфейса для аналитики устройств в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="d2d35-173">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="d2d35-174">deviceCount</span><span class="sxs-lookup"><span data-stu-id="d2d35-174">deviceCount</span></span>|<span data-ttu-id="d2d35-175">Int64</span><span class="sxs-lookup"><span data-stu-id="d2d35-175">Int64</span></span>|<span data-ttu-id="d2d35-176">Аналитика пользовательских интерфейсов суммирует количество устройств.</span><span class="sxs-lookup"><span data-stu-id="d2d35-176">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="d2d35-177">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="d2d35-177">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="d2d35-178">Int32</span><span class="sxs-lookup"><span data-stu-id="d2d35-178">Int32</span></span>|<span data-ttu-id="d2d35-179">Аналитика пользовательского интерфейса реагирует на время рабочего стола в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="d2d35-179">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="d2d35-180">blueScreenCount</span><span class="sxs-lookup"><span data-stu-id="d2d35-180">blueScreenCount</span></span>|<span data-ttu-id="d2d35-181">Int32</span><span class="sxs-lookup"><span data-stu-id="d2d35-181">Int32</span></span>|<span data-ttu-id="d2d35-182">Количество синих экранов за последние 14 дней.</span><span class="sxs-lookup"><span data-stu-id="d2d35-182">Number of Blue Screens in the last 14 days.</span></span> <span data-ttu-id="d2d35-183">Допустимые значения от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="d2d35-183">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="d2d35-184">restartCount</span><span class="sxs-lookup"><span data-stu-id="d2d35-184">restartCount</span></span>|<span data-ttu-id="d2d35-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d2d35-185">Int32</span></span>|<span data-ttu-id="d2d35-186">Количество перезапусков за последние 14 дней.</span><span class="sxs-lookup"><span data-stu-id="d2d35-186">Number of Restarts in the last 14 days.</span></span> <span data-ttu-id="d2d35-187">Допустимые значения от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="d2d35-187">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="d2d35-188">averageBlueScreens</span><span class="sxs-lookup"><span data-stu-id="d2d35-188">averageBlueScreens</span></span>|<span data-ttu-id="d2d35-189">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="d2d35-189">Double</span></span>|<span data-ttu-id="d2d35-190">Среднее (среднее) число синих экранов на устройство за последние 14 дней.</span><span class="sxs-lookup"><span data-stu-id="d2d35-190">Average (mean) number of Blue Screens per device in the last 14 days.</span></span> <span data-ttu-id="d2d35-191">Допустимые значения от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="d2d35-191">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="d2d35-192">averageRestarts</span><span class="sxs-lookup"><span data-stu-id="d2d35-192">averageRestarts</span></span>|<span data-ttu-id="d2d35-193">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="d2d35-193">Double</span></span>|<span data-ttu-id="d2d35-194">Среднее (среднее) число перезапусков на устройство за последние 14 дней.</span><span class="sxs-lookup"><span data-stu-id="d2d35-194">Average (mean) number of Restarts per device in the last 14 days.</span></span> <span data-ttu-id="d2d35-195">Допустимые значения от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="d2d35-195">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="d2d35-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2d35-196">Response</span></span>
<span data-ttu-id="d2d35-197">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d2d35-197">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2d35-198">Пример</span><span class="sxs-lookup"><span data-stu-id="d2d35-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2d35-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2d35-199">Request</span></span>
<span data-ttu-id="d2d35-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2d35-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
Content-type: application/json
Content-length: 635

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "diskType": "hdd",
  "operatingSystemVersion": "Operating System Version value",
  "bootScore": 9,
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "healthStatus": "insufficientData",
  "loginScore": 10,
  "coreLoginTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "deviceCount": 11,
  "responsiveDesktopTimeInMs": 9,
  "blueScreenCount": 15,
  "restartCount": 12,
  "averageBlueScreens": 6.0,
  "averageRestarts": 5.0
}
```

### <a name="response"></a><span data-ttu-id="d2d35-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2d35-201">Response</span></span>
<span data-ttu-id="d2d35-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2d35-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 684

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "id": "852ae826-e826-852a-26e8-2a8526e82a85",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "diskType": "hdd",
  "operatingSystemVersion": "Operating System Version value",
  "bootScore": 9,
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "healthStatus": "insufficientData",
  "loginScore": 10,
  "coreLoginTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "deviceCount": 11,
  "responsiveDesktopTimeInMs": 9,
  "blueScreenCount": 15,
  "restartCount": 12,
  "averageBlueScreens": 6.0,
  "averageRestarts": 5.0
}
```




