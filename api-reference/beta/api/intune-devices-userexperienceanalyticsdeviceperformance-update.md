---
title: Обновление Усерекспериенцеаналитиксдевицеперформанце
description: Обновление свойств объекта Усерекспериенцеаналитиксдевицеперформанце.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75719a81a38e70cfbfc487710358a9f75e866690
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43379646"
---
# <a name="update-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="d8f0b-103">Обновление Усерекспериенцеаналитиксдевицеперформанце</span><span class="sxs-lookup"><span data-stu-id="d8f0b-103">Update userExperienceAnalyticsDevicePerformance</span></span>

<span data-ttu-id="d8f0b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8f0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8f0b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8f0b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8f0b-107">Обновление свойств объекта [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="d8f0b-107">Update the properties of a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8f0b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d8f0b-108">Prerequisites</span></span>
<span data-ttu-id="d8f0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8f0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8f0b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8f0b-111">Permission type</span></span>|<span data-ttu-id="d8f0b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8f0b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8f0b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8f0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8f0b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8f0b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d8f0b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8f0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8f0b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-116">Not supported.</span></span>|
|<span data-ttu-id="d8f0b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8f0b-117">Application</span></span>|<span data-ttu-id="d8f0b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8f0b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8f0b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8f0b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="d8f0b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d8f0b-120">Request headers</span></span>
|<span data-ttu-id="d8f0b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8f0b-121">Header</span></span>|<span data-ttu-id="d8f0b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d8f0b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8f0b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8f0b-123">Authorization</span></span>|<span data-ttu-id="d8f0b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8f0b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d8f0b-125">Accept</span></span>|<span data-ttu-id="d8f0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8f0b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8f0b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d8f0b-127">Request body</span></span>
<span data-ttu-id="d8f0b-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

<span data-ttu-id="d8f0b-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span><span class="sxs-lookup"><span data-stu-id="d8f0b-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span></span>

|<span data-ttu-id="d8f0b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8f0b-130">Property</span></span>|<span data-ttu-id="d8f0b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d8f0b-131">Type</span></span>|<span data-ttu-id="d8f0b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d8f0b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8f0b-133">id</span><span class="sxs-lookup"><span data-stu-id="d8f0b-133">id</span></span>|<span data-ttu-id="d8f0b-134">String</span><span class="sxs-lookup"><span data-stu-id="d8f0b-134">String</span></span>|<span data-ttu-id="d8f0b-135">Уникальный идентификатор устройства для загрузки устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-135">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="d8f0b-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="d8f0b-136">deviceName</span></span>|<span data-ttu-id="d8f0b-137">String</span><span class="sxs-lookup"><span data-stu-id="d8f0b-137">String</span></span>|<span data-ttu-id="d8f0b-138">Имя устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="d8f0b-139">model</span><span class="sxs-lookup"><span data-stu-id="d8f0b-139">model</span></span>|<span data-ttu-id="d8f0b-140">String</span><span class="sxs-lookup"><span data-stu-id="d8f0b-140">String</span></span>|<span data-ttu-id="d8f0b-141">Модель устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="d8f0b-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="d8f0b-142">manufacturer</span></span>|<span data-ttu-id="d8f0b-143">String</span><span class="sxs-lookup"><span data-stu-id="d8f0b-143">String</span></span>|<span data-ttu-id="d8f0b-144">Производитель устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="d8f0b-145">diskType</span><span class="sxs-lookup"><span data-stu-id="d8f0b-145">diskType</span></span>|[<span data-ttu-id="d8f0b-146">diskType</span><span class="sxs-lookup"><span data-stu-id="d8f0b-146">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="d8f0b-147">Тип диска устройства анализа взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-147">The user experience analytics device disk type.</span></span> <span data-ttu-id="d8f0b-148">Возможные значения: `unkown`, `hdd`, `ssd`.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-148">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="d8f0b-149">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="d8f0b-149">operatingSystemVersion</span></span>|<span data-ttu-id="d8f0b-150">String</span><span class="sxs-lookup"><span data-stu-id="d8f0b-150">String</span></span>|<span data-ttu-id="d8f0b-151">Версия операционной системы устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-151">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="d8f0b-152">бутскоре</span><span class="sxs-lookup"><span data-stu-id="d8f0b-152">bootScore</span></span>|<span data-ttu-id="d8f0b-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d8f0b-153">Int32</span></span>|<span data-ttu-id="d8f0b-154">Оценка загрузки устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-154">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="d8f0b-155">коребуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="d8f0b-155">coreBootTimeInMs</span></span>|<span data-ttu-id="d8f0b-156">Int32</span><span class="sxs-lookup"><span data-stu-id="d8f0b-156">Int32</span></span>|<span data-ttu-id="d8f0b-157">Время загрузки ядра устройства аналитики для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="d8f0b-157">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="d8f0b-158">граупполицибуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="d8f0b-158">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="d8f0b-159">Int32</span><span class="sxs-lookup"><span data-stu-id="d8f0b-159">Int32</span></span>|<span data-ttu-id="d8f0b-160">Время загрузки групповой политики устройства Analytics для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="d8f0b-160">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="d8f0b-161">хеалсстатус</span><span class="sxs-lookup"><span data-stu-id="d8f0b-161">healthStatus</span></span>|[<span data-ttu-id="d8f0b-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="d8f0b-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="d8f0b-163">Состояние работоспособности устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-163">The health state of the user experience analytics device.</span></span> <span data-ttu-id="d8f0b-164">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="d8f0b-165">логинскоре</span><span class="sxs-lookup"><span data-stu-id="d8f0b-165">loginScore</span></span>|<span data-ttu-id="d8f0b-166">Int32</span><span class="sxs-lookup"><span data-stu-id="d8f0b-166">Int32</span></span>|<span data-ttu-id="d8f0b-167">Оценка имени для входа на устройство аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-167">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="d8f0b-168">корелогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="d8f0b-168">coreLoginTimeInMs</span></span>|<span data-ttu-id="d8f0b-169">Int32</span><span class="sxs-lookup"><span data-stu-id="d8f0b-169">Int32</span></span>|<span data-ttu-id="d8f0b-170">Время входа в ядро устройства аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="d8f0b-170">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="d8f0b-171">граупполицилогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="d8f0b-171">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="d8f0b-172">Int32</span><span class="sxs-lookup"><span data-stu-id="d8f0b-172">Int32</span></span>|<span data-ttu-id="d8f0b-173">Время входа в групповую политику устройства Analytics User Experience (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="d8f0b-173">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="d8f0b-174">deviceCount</span><span class="sxs-lookup"><span data-stu-id="d8f0b-174">deviceCount</span></span>|<span data-ttu-id="d8f0b-175">Int64</span><span class="sxs-lookup"><span data-stu-id="d8f0b-175">Int64</span></span>|<span data-ttu-id="d8f0b-176">Число устройств для аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-176">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="d8f0b-177">респонсиведесктоптимеинмс</span><span class="sxs-lookup"><span data-stu-id="d8f0b-177">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="d8f0b-178">Int32</span><span class="sxs-lookup"><span data-stu-id="d8f0b-178">Int32</span></span>|<span data-ttu-id="d8f0b-179">Время, в течение которого выполняется анализ пользовательского интерфейса на рабочем столе в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-179">The user experience analytics responsive desktop time in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="d8f0b-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8f0b-180">Response</span></span>
<span data-ttu-id="d8f0b-181">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-181">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8f0b-182">Пример</span><span class="sxs-lookup"><span data-stu-id="d8f0b-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8f0b-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8f0b-183">Request</span></span>
<span data-ttu-id="d8f0b-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
Content-type: application/json
Content-length: 529

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
  "responsiveDesktopTimeInMs": 9
}
```

### <a name="response"></a><span data-ttu-id="d8f0b-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8f0b-185">Response</span></span>
<span data-ttu-id="d8f0b-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8f0b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 578

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
  "responsiveDesktopTimeInMs": 9
}
```



