---
title: Создание Усерекспериенцеаналитиксдевицеперформанце
description: Создание нового объекта Усерекспериенцеаналитиксдевицеперформанце.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ff3b8a6fa39038b2115720647b776dc30c7d1962
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43322578"
---
# <a name="create-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="8d898-103">Создание Усерекспериенцеаналитиксдевицеперформанце</span><span class="sxs-lookup"><span data-stu-id="8d898-103">Create userExperienceAnalyticsDevicePerformance</span></span>

<span data-ttu-id="8d898-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d898-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d898-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d898-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d898-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d898-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d898-107">Создание нового объекта [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="8d898-107">Create a new [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d898-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8d898-108">Prerequisites</span></span>
<span data-ttu-id="8d898-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d898-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d898-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d898-111">Permission type</span></span>|<span data-ttu-id="8d898-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d898-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d898-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d898-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d898-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d898-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8d898-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d898-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d898-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d898-116">Not supported.</span></span>|
|<span data-ttu-id="8d898-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d898-117">Application</span></span>|<span data-ttu-id="8d898-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d898-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d898-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d898-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="8d898-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8d898-120">Request headers</span></span>
|<span data-ttu-id="8d898-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d898-121">Header</span></span>|<span data-ttu-id="8d898-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8d898-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d898-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d898-123">Authorization</span></span>|<span data-ttu-id="8d898-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d898-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d898-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8d898-125">Accept</span></span>|<span data-ttu-id="8d898-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d898-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d898-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d898-127">Request body</span></span>
<span data-ttu-id="8d898-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксдевицеперформанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d898-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDevicePerformance object.</span></span>

<span data-ttu-id="8d898-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксдевицеперформанце.</span><span class="sxs-lookup"><span data-stu-id="8d898-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDevicePerformance.</span></span>

|<span data-ttu-id="8d898-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d898-130">Property</span></span>|<span data-ttu-id="8d898-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8d898-131">Type</span></span>|<span data-ttu-id="8d898-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8d898-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d898-133">id</span><span class="sxs-lookup"><span data-stu-id="8d898-133">id</span></span>|<span data-ttu-id="8d898-134">String</span><span class="sxs-lookup"><span data-stu-id="8d898-134">String</span></span>|<span data-ttu-id="8d898-135">Уникальный идентификатор устройства для загрузки устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="8d898-135">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="8d898-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="8d898-136">deviceName</span></span>|<span data-ttu-id="8d898-137">String</span><span class="sxs-lookup"><span data-stu-id="8d898-137">String</span></span>|<span data-ttu-id="8d898-138">Имя устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="8d898-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="8d898-139">model</span><span class="sxs-lookup"><span data-stu-id="8d898-139">model</span></span>|<span data-ttu-id="8d898-140">String</span><span class="sxs-lookup"><span data-stu-id="8d898-140">String</span></span>|<span data-ttu-id="8d898-141">Модель устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="8d898-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="8d898-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="8d898-142">manufacturer</span></span>|<span data-ttu-id="8d898-143">String</span><span class="sxs-lookup"><span data-stu-id="8d898-143">String</span></span>|<span data-ttu-id="8d898-144">Производитель устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="8d898-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="8d898-145">diskType</span><span class="sxs-lookup"><span data-stu-id="8d898-145">diskType</span></span>|[<span data-ttu-id="8d898-146">diskType</span><span class="sxs-lookup"><span data-stu-id="8d898-146">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="8d898-147">Тип диска устройства анализа взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="8d898-147">The user experience analytics device disk type.</span></span> <span data-ttu-id="8d898-148">Возможные значения: `unkown`, `hdd`, `ssd`.</span><span class="sxs-lookup"><span data-stu-id="8d898-148">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="8d898-149">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="8d898-149">operatingSystemVersion</span></span>|<span data-ttu-id="8d898-150">String</span><span class="sxs-lookup"><span data-stu-id="8d898-150">String</span></span>|<span data-ttu-id="8d898-151">Версия операционной системы устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="8d898-151">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="8d898-152">бутскоре</span><span class="sxs-lookup"><span data-stu-id="8d898-152">bootScore</span></span>|<span data-ttu-id="8d898-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8d898-153">Int32</span></span>|<span data-ttu-id="8d898-154">Оценка загрузки устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="8d898-154">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="8d898-155">коребуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="8d898-155">coreBootTimeInMs</span></span>|<span data-ttu-id="8d898-156">Int32</span><span class="sxs-lookup"><span data-stu-id="8d898-156">Int32</span></span>|<span data-ttu-id="8d898-157">Время загрузки ядра устройства аналитики для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="8d898-157">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="8d898-158">граупполицибуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="8d898-158">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="8d898-159">Int32</span><span class="sxs-lookup"><span data-stu-id="8d898-159">Int32</span></span>|<span data-ttu-id="8d898-160">Время загрузки групповой политики устройства Analytics для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="8d898-160">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="8d898-161">хеалсстатус</span><span class="sxs-lookup"><span data-stu-id="8d898-161">healthStatus</span></span>|[<span data-ttu-id="8d898-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="8d898-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="8d898-163">Состояние работоспособности устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="8d898-163">The health state of the user experience analytics device.</span></span> <span data-ttu-id="8d898-164">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="8d898-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="8d898-165">логинскоре</span><span class="sxs-lookup"><span data-stu-id="8d898-165">loginScore</span></span>|<span data-ttu-id="8d898-166">Int32</span><span class="sxs-lookup"><span data-stu-id="8d898-166">Int32</span></span>|<span data-ttu-id="8d898-167">Оценка имени для входа на устройство аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="8d898-167">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="8d898-168">корелогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="8d898-168">coreLoginTimeInMs</span></span>|<span data-ttu-id="8d898-169">Int32</span><span class="sxs-lookup"><span data-stu-id="8d898-169">Int32</span></span>|<span data-ttu-id="8d898-170">Время входа в ядро устройства аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="8d898-170">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="8d898-171">граупполицилогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="8d898-171">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="8d898-172">Int32</span><span class="sxs-lookup"><span data-stu-id="8d898-172">Int32</span></span>|<span data-ttu-id="8d898-173">Время входа в групповую политику устройства Analytics User Experience (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="8d898-173">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="8d898-174">deviceCount</span><span class="sxs-lookup"><span data-stu-id="8d898-174">deviceCount</span></span>|<span data-ttu-id="8d898-175">Int64</span><span class="sxs-lookup"><span data-stu-id="8d898-175">Int64</span></span>|<span data-ttu-id="8d898-176">Число устройств для аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="8d898-176">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="8d898-177">респонсиведесктоптимеинмс</span><span class="sxs-lookup"><span data-stu-id="8d898-177">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="8d898-178">Int32</span><span class="sxs-lookup"><span data-stu-id="8d898-178">Int32</span></span>|<span data-ttu-id="8d898-179">Время, в течение которого выполняется анализ пользовательского интерфейса на рабочем столе в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="8d898-179">The user experience analytics responsive desktop time in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="8d898-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d898-180">Response</span></span>
<span data-ttu-id="8d898-181">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d898-181">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d898-182">Пример</span><span class="sxs-lookup"><span data-stu-id="8d898-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d898-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d898-183">Request</span></span>
<span data-ttu-id="8d898-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d898-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance
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

### <a name="response"></a><span data-ttu-id="8d898-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d898-185">Response</span></span>
<span data-ttu-id="8d898-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d898-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



