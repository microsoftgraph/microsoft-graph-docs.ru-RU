---
title: Обновление Усерекспериенцеаналитиксдевицеперформанце
description: Обновление свойств объекта Усерекспериенцеаналитиксдевицеперформанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f125ce0beeb76bd8d3a6ef098b8a70e280c6b1a9
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944479"
---
# <a name="update-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="a9b65-103">Обновление Усерекспериенцеаналитиксдевицеперформанце</span><span class="sxs-lookup"><span data-stu-id="a9b65-103">Update userExperienceAnalyticsDevicePerformance</span></span>

> <span data-ttu-id="a9b65-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9b65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9b65-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9b65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9b65-106">Обновление свойств объекта [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="a9b65-106">Update the properties of a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9b65-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a9b65-107">Prerequisites</span></span>
<span data-ttu-id="a9b65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9b65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9b65-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9b65-110">Permission type</span></span>|<span data-ttu-id="a9b65-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9b65-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9b65-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9b65-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9b65-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9b65-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a9b65-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9b65-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9b65-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9b65-115">Not supported.</span></span>|
|<span data-ttu-id="a9b65-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9b65-116">Application</span></span>|<span data-ttu-id="a9b65-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9b65-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9b65-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9b65-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="a9b65-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a9b65-119">Request headers</span></span>
|<span data-ttu-id="a9b65-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9b65-120">Header</span></span>|<span data-ttu-id="a9b65-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a9b65-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9b65-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9b65-122">Authorization</span></span>|<span data-ttu-id="a9b65-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9b65-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9b65-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a9b65-124">Accept</span></span>|<span data-ttu-id="a9b65-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9b65-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9b65-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a9b65-126">Request body</span></span>
<span data-ttu-id="a9b65-127">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9b65-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

<span data-ttu-id="a9b65-128">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span><span class="sxs-lookup"><span data-stu-id="a9b65-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span></span>

|<span data-ttu-id="a9b65-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9b65-129">Property</span></span>|<span data-ttu-id="a9b65-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a9b65-130">Type</span></span>|<span data-ttu-id="a9b65-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a9b65-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9b65-132">id</span><span class="sxs-lookup"><span data-stu-id="a9b65-132">id</span></span>|<span data-ttu-id="a9b65-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a9b65-133">String</span></span>|<span data-ttu-id="a9b65-134">Уникальный идентификатор устройства для загрузки устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="a9b65-134">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="a9b65-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="a9b65-135">deviceName</span></span>|<span data-ttu-id="a9b65-136">Строка</span><span class="sxs-lookup"><span data-stu-id="a9b65-136">String</span></span>|<span data-ttu-id="a9b65-137">Имя устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="a9b65-137">The user experience analytics device name.</span></span>|
|<span data-ttu-id="a9b65-138">model</span><span class="sxs-lookup"><span data-stu-id="a9b65-138">model</span></span>|<span data-ttu-id="a9b65-139">Строка</span><span class="sxs-lookup"><span data-stu-id="a9b65-139">String</span></span>|<span data-ttu-id="a9b65-140">Модель устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="a9b65-140">The user experience analytics device model.</span></span>|
|<span data-ttu-id="a9b65-141">manufacturer</span><span class="sxs-lookup"><span data-stu-id="a9b65-141">manufacturer</span></span>|<span data-ttu-id="a9b65-142">Строка</span><span class="sxs-lookup"><span data-stu-id="a9b65-142">String</span></span>|<span data-ttu-id="a9b65-143">Производитель устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="a9b65-143">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="a9b65-144">diskType</span><span class="sxs-lookup"><span data-stu-id="a9b65-144">diskType</span></span>|[<span data-ttu-id="a9b65-145">diskType</span><span class="sxs-lookup"><span data-stu-id="a9b65-145">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="a9b65-146">Тип диска устройства анализа взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="a9b65-146">The user experience analytics device disk type.</span></span> <span data-ttu-id="a9b65-147">Возможные значения: `unkown`, `hdd`, `ssd`.</span><span class="sxs-lookup"><span data-stu-id="a9b65-147">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="a9b65-148">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="a9b65-148">operatingSystemVersion</span></span>|<span data-ttu-id="a9b65-149">String</span><span class="sxs-lookup"><span data-stu-id="a9b65-149">String</span></span>|<span data-ttu-id="a9b65-150">Версия операционной системы устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="a9b65-150">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="a9b65-151">бутскоре</span><span class="sxs-lookup"><span data-stu-id="a9b65-151">bootScore</span></span>|<span data-ttu-id="a9b65-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a9b65-152">Int32</span></span>|<span data-ttu-id="a9b65-153">Оценка загрузки устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="a9b65-153">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="a9b65-154">коребуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="a9b65-154">coreBootTimeInMs</span></span>|<span data-ttu-id="a9b65-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a9b65-155">Int32</span></span>|<span data-ttu-id="a9b65-156">Время загрузки ядра устройства аналитики для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="a9b65-156">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="a9b65-157">граупполицибуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="a9b65-157">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="a9b65-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a9b65-158">Int32</span></span>|<span data-ttu-id="a9b65-159">Время загрузки групповой политики устройства Analytics для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="a9b65-159">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="a9b65-160">хеалсстатус</span><span class="sxs-lookup"><span data-stu-id="a9b65-160">healthStatus</span></span>|[<span data-ttu-id="a9b65-161">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="a9b65-161">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="a9b65-162">Состояние работоспособности устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="a9b65-162">The health state of the user experience analytics device.</span></span> <span data-ttu-id="a9b65-163">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="a9b65-163">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="a9b65-164">логинскоре</span><span class="sxs-lookup"><span data-stu-id="a9b65-164">loginScore</span></span>|<span data-ttu-id="a9b65-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a9b65-165">Int32</span></span>|<span data-ttu-id="a9b65-166">Оценка имени для входа на устройство аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="a9b65-166">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="a9b65-167">корелогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="a9b65-167">coreLoginTimeInMs</span></span>|<span data-ttu-id="a9b65-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a9b65-168">Int32</span></span>|<span data-ttu-id="a9b65-169">Время входа в ядро устройства аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="a9b65-169">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="a9b65-170">граупполицилогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="a9b65-170">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="a9b65-171">Int32</span><span class="sxs-lookup"><span data-stu-id="a9b65-171">Int32</span></span>|<span data-ttu-id="a9b65-172">Время входа в групповую политику устройства Analytics User Experience (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="a9b65-172">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="a9b65-173">deviceCount</span><span class="sxs-lookup"><span data-stu-id="a9b65-173">deviceCount</span></span>|<span data-ttu-id="a9b65-174">Int64</span><span class="sxs-lookup"><span data-stu-id="a9b65-174">Int64</span></span>|<span data-ttu-id="a9b65-175">Число устройств для аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="a9b65-175">User experience analytics summarized device count.</span></span>|



## <a name="response"></a><span data-ttu-id="a9b65-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9b65-176">Response</span></span>
<span data-ttu-id="a9b65-177">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9b65-177">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9b65-178">Пример</span><span class="sxs-lookup"><span data-stu-id="a9b65-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9b65-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9b65-179">Request</span></span>
<span data-ttu-id="a9b65-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9b65-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
Content-type: application/json
Content-length: 494

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
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="a9b65-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9b65-181">Response</span></span>
<span data-ttu-id="a9b65-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9b65-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

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
  "deviceCount": 11
}
```





