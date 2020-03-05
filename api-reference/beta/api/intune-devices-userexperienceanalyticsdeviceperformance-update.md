---
title: Обновление Усерекспериенцеаналитиксдевицеперформанце
description: Обновление свойств объекта Усерекспериенцеаналитиксдевицеперформанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3d116950d788c57c19ce153605d1dd88909e5be9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468392"
---
# <a name="update-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="1de1d-103">Обновление Усерекспериенцеаналитиксдевицеперформанце</span><span class="sxs-lookup"><span data-stu-id="1de1d-103">Update userExperienceAnalyticsDevicePerformance</span></span>

<span data-ttu-id="1de1d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1de1d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1de1d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1de1d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1de1d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1de1d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1de1d-107">Обновление свойств объекта [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="1de1d-107">Update the properties of a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1de1d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1de1d-108">Prerequisites</span></span>
<span data-ttu-id="1de1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1de1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1de1d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1de1d-111">Permission type</span></span>|<span data-ttu-id="1de1d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1de1d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1de1d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1de1d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1de1d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1de1d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1de1d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1de1d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1de1d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1de1d-116">Not supported.</span></span>|
|<span data-ttu-id="1de1d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1de1d-117">Application</span></span>|<span data-ttu-id="1de1d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1de1d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1de1d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1de1d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="1de1d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1de1d-120">Request headers</span></span>
|<span data-ttu-id="1de1d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1de1d-121">Header</span></span>|<span data-ttu-id="1de1d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1de1d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1de1d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1de1d-123">Authorization</span></span>|<span data-ttu-id="1de1d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1de1d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1de1d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1de1d-125">Accept</span></span>|<span data-ttu-id="1de1d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1de1d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1de1d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1de1d-127">Request body</span></span>
<span data-ttu-id="1de1d-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1de1d-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

<span data-ttu-id="1de1d-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span><span class="sxs-lookup"><span data-stu-id="1de1d-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span></span>

|<span data-ttu-id="1de1d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1de1d-130">Property</span></span>|<span data-ttu-id="1de1d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1de1d-131">Type</span></span>|<span data-ttu-id="1de1d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1de1d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1de1d-133">id</span><span class="sxs-lookup"><span data-stu-id="1de1d-133">id</span></span>|<span data-ttu-id="1de1d-134">String</span><span class="sxs-lookup"><span data-stu-id="1de1d-134">String</span></span>|<span data-ttu-id="1de1d-135">Уникальный идентификатор устройства для загрузки устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="1de1d-135">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="1de1d-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="1de1d-136">deviceName</span></span>|<span data-ttu-id="1de1d-137">String</span><span class="sxs-lookup"><span data-stu-id="1de1d-137">String</span></span>|<span data-ttu-id="1de1d-138">Имя устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="1de1d-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="1de1d-139">model</span><span class="sxs-lookup"><span data-stu-id="1de1d-139">model</span></span>|<span data-ttu-id="1de1d-140">String</span><span class="sxs-lookup"><span data-stu-id="1de1d-140">String</span></span>|<span data-ttu-id="1de1d-141">Модель устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="1de1d-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="1de1d-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="1de1d-142">manufacturer</span></span>|<span data-ttu-id="1de1d-143">String</span><span class="sxs-lookup"><span data-stu-id="1de1d-143">String</span></span>|<span data-ttu-id="1de1d-144">Производитель устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="1de1d-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="1de1d-145">diskType</span><span class="sxs-lookup"><span data-stu-id="1de1d-145">diskType</span></span>|[<span data-ttu-id="1de1d-146">diskType</span><span class="sxs-lookup"><span data-stu-id="1de1d-146">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="1de1d-147">Тип диска устройства анализа взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="1de1d-147">The user experience analytics device disk type.</span></span> <span data-ttu-id="1de1d-148">Возможные значения: `unkown`, `hdd`, `ssd`.</span><span class="sxs-lookup"><span data-stu-id="1de1d-148">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="1de1d-149">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="1de1d-149">operatingSystemVersion</span></span>|<span data-ttu-id="1de1d-150">String</span><span class="sxs-lookup"><span data-stu-id="1de1d-150">String</span></span>|<span data-ttu-id="1de1d-151">Версия операционной системы устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="1de1d-151">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="1de1d-152">бутскоре</span><span class="sxs-lookup"><span data-stu-id="1de1d-152">bootScore</span></span>|<span data-ttu-id="1de1d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="1de1d-153">Int32</span></span>|<span data-ttu-id="1de1d-154">Оценка загрузки устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="1de1d-154">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="1de1d-155">коребуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="1de1d-155">coreBootTimeInMs</span></span>|<span data-ttu-id="1de1d-156">Int32</span><span class="sxs-lookup"><span data-stu-id="1de1d-156">Int32</span></span>|<span data-ttu-id="1de1d-157">Время загрузки ядра устройства аналитики для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="1de1d-157">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="1de1d-158">граупполицибуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="1de1d-158">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="1de1d-159">Int32</span><span class="sxs-lookup"><span data-stu-id="1de1d-159">Int32</span></span>|<span data-ttu-id="1de1d-160">Время загрузки групповой политики устройства Analytics для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="1de1d-160">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="1de1d-161">хеалсстатус</span><span class="sxs-lookup"><span data-stu-id="1de1d-161">healthStatus</span></span>|[<span data-ttu-id="1de1d-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="1de1d-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="1de1d-163">Состояние работоспособности устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="1de1d-163">The health state of the user experience analytics device.</span></span> <span data-ttu-id="1de1d-164">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="1de1d-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="1de1d-165">логинскоре</span><span class="sxs-lookup"><span data-stu-id="1de1d-165">loginScore</span></span>|<span data-ttu-id="1de1d-166">Int32</span><span class="sxs-lookup"><span data-stu-id="1de1d-166">Int32</span></span>|<span data-ttu-id="1de1d-167">Оценка имени для входа на устройство аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="1de1d-167">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="1de1d-168">корелогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="1de1d-168">coreLoginTimeInMs</span></span>|<span data-ttu-id="1de1d-169">Int32</span><span class="sxs-lookup"><span data-stu-id="1de1d-169">Int32</span></span>|<span data-ttu-id="1de1d-170">Время входа в ядро устройства аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="1de1d-170">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="1de1d-171">граупполицилогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="1de1d-171">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="1de1d-172">Int32</span><span class="sxs-lookup"><span data-stu-id="1de1d-172">Int32</span></span>|<span data-ttu-id="1de1d-173">Время входа в групповую политику устройства Analytics User Experience (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="1de1d-173">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="1de1d-174">deviceCount</span><span class="sxs-lookup"><span data-stu-id="1de1d-174">deviceCount</span></span>|<span data-ttu-id="1de1d-175">Int64</span><span class="sxs-lookup"><span data-stu-id="1de1d-175">Int64</span></span>|<span data-ttu-id="1de1d-176">Число устройств для аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="1de1d-176">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="1de1d-177">респонсиведесктоптимеинмс</span><span class="sxs-lookup"><span data-stu-id="1de1d-177">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="1de1d-178">Int32</span><span class="sxs-lookup"><span data-stu-id="1de1d-178">Int32</span></span>|<span data-ttu-id="1de1d-179">Время, в течение которого выполняется анализ пользовательского интерфейса на рабочем столе в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="1de1d-179">The user experience analytics responsive desktop time in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="1de1d-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="1de1d-180">Response</span></span>
<span data-ttu-id="1de1d-181">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1de1d-181">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1de1d-182">Пример</span><span class="sxs-lookup"><span data-stu-id="1de1d-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="1de1d-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="1de1d-183">Request</span></span>
<span data-ttu-id="1de1d-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1de1d-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1de1d-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="1de1d-185">Response</span></span>
<span data-ttu-id="1de1d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1de1d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





