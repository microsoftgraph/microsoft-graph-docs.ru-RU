---
title: Создание Усерекспериенцеаналитиксдевицеперформанце
description: Создание нового объекта Усерекспериенцеаналитиксдевицеперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f76f62ff69701fd57a41080b344c5f5fd2366227
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050663"
---
# <a name="create-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="f1a1a-103">Создание Усерекспериенцеаналитиксдевицеперформанце</span><span class="sxs-lookup"><span data-stu-id="f1a1a-103">Create userExperienceAnalyticsDevicePerformance</span></span>

<span data-ttu-id="f1a1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1a1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1a1a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1a1a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1a1a-107">Создание нового объекта [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="f1a1a-107">Create a new [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1a1a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1a1a-108">Prerequisites</span></span>
<span data-ttu-id="f1a1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1a1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1a1a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1a1a-111">Permission type</span></span>|<span data-ttu-id="f1a1a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1a1a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1a1a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1a1a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1a1a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1a1a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f1a1a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1a1a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1a1a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-116">Not supported.</span></span>|
|<span data-ttu-id="f1a1a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1a1a-117">Application</span></span>|<span data-ttu-id="f1a1a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1a1a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1a1a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1a1a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="f1a1a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f1a1a-120">Request headers</span></span>
|<span data-ttu-id="f1a1a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1a1a-121">Header</span></span>|<span data-ttu-id="f1a1a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f1a1a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1a1a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1a1a-123">Authorization</span></span>|<span data-ttu-id="f1a1a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1a1a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f1a1a-125">Accept</span></span>|<span data-ttu-id="f1a1a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1a1a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1a1a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1a1a-127">Request body</span></span>
<span data-ttu-id="f1a1a-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксдевицеперформанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDevicePerformance object.</span></span>

<span data-ttu-id="f1a1a-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксдевицеперформанце.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDevicePerformance.</span></span>

|<span data-ttu-id="f1a1a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1a1a-130">Property</span></span>|<span data-ttu-id="f1a1a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f1a1a-131">Type</span></span>|<span data-ttu-id="f1a1a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f1a1a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1a1a-133">id</span><span class="sxs-lookup"><span data-stu-id="f1a1a-133">id</span></span>|<span data-ttu-id="f1a1a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f1a1a-134">String</span></span>|<span data-ttu-id="f1a1a-135">Уникальный идентификатор устройства для загрузки устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-135">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="f1a1a-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="f1a1a-136">deviceName</span></span>|<span data-ttu-id="f1a1a-137">String</span><span class="sxs-lookup"><span data-stu-id="f1a1a-137">String</span></span>|<span data-ttu-id="f1a1a-138">Имя устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="f1a1a-139">model</span><span class="sxs-lookup"><span data-stu-id="f1a1a-139">model</span></span>|<span data-ttu-id="f1a1a-140">String</span><span class="sxs-lookup"><span data-stu-id="f1a1a-140">String</span></span>|<span data-ttu-id="f1a1a-141">Модель устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="f1a1a-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="f1a1a-142">manufacturer</span></span>|<span data-ttu-id="f1a1a-143">String</span><span class="sxs-lookup"><span data-stu-id="f1a1a-143">String</span></span>|<span data-ttu-id="f1a1a-144">Производитель устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="f1a1a-145">diskType</span><span class="sxs-lookup"><span data-stu-id="f1a1a-145">diskType</span></span>|[<span data-ttu-id="f1a1a-146">diskType</span><span class="sxs-lookup"><span data-stu-id="f1a1a-146">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="f1a1a-147">Тип диска устройства анализа взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-147">The user experience analytics device disk type.</span></span> <span data-ttu-id="f1a1a-148">Возможные значения: `unkown`, `hdd`, `ssd`.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-148">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="f1a1a-149">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="f1a1a-149">operatingSystemVersion</span></span>|<span data-ttu-id="f1a1a-150">String</span><span class="sxs-lookup"><span data-stu-id="f1a1a-150">String</span></span>|<span data-ttu-id="f1a1a-151">Версия операционной системы устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-151">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="f1a1a-152">бутскоре</span><span class="sxs-lookup"><span data-stu-id="f1a1a-152">bootScore</span></span>|<span data-ttu-id="f1a1a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a1a-153">Int32</span></span>|<span data-ttu-id="f1a1a-154">Оценка загрузки устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-154">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="f1a1a-155">коребуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="f1a1a-155">coreBootTimeInMs</span></span>|<span data-ttu-id="f1a1a-156">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a1a-156">Int32</span></span>|<span data-ttu-id="f1a1a-157">Время загрузки ядра устройства аналитики для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="f1a1a-157">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="f1a1a-158">граупполицибуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="f1a1a-158">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="f1a1a-159">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a1a-159">Int32</span></span>|<span data-ttu-id="f1a1a-160">Время загрузки групповой политики устройства Analytics для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="f1a1a-160">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="f1a1a-161">хеалсстатус</span><span class="sxs-lookup"><span data-stu-id="f1a1a-161">healthStatus</span></span>|[<span data-ttu-id="f1a1a-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="f1a1a-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="f1a1a-163">Состояние работоспособности устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-163">The health state of the user experience analytics device.</span></span> <span data-ttu-id="f1a1a-164">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="f1a1a-165">логинскоре</span><span class="sxs-lookup"><span data-stu-id="f1a1a-165">loginScore</span></span>|<span data-ttu-id="f1a1a-166">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a1a-166">Int32</span></span>|<span data-ttu-id="f1a1a-167">Оценка имени для входа на устройство аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-167">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="f1a1a-168">корелогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="f1a1a-168">coreLoginTimeInMs</span></span>|<span data-ttu-id="f1a1a-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a1a-169">Int32</span></span>|<span data-ttu-id="f1a1a-170">Время входа в ядро устройства аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="f1a1a-170">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="f1a1a-171">граупполицилогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="f1a1a-171">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="f1a1a-172">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a1a-172">Int32</span></span>|<span data-ttu-id="f1a1a-173">Время входа в групповую политику устройства Analytics User Experience (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="f1a1a-173">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="f1a1a-174">deviceCount</span><span class="sxs-lookup"><span data-stu-id="f1a1a-174">deviceCount</span></span>|<span data-ttu-id="f1a1a-175">Int64</span><span class="sxs-lookup"><span data-stu-id="f1a1a-175">Int64</span></span>|<span data-ttu-id="f1a1a-176">Число устройств для аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-176">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="f1a1a-177">респонсиведесктоптимеинмс</span><span class="sxs-lookup"><span data-stu-id="f1a1a-177">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="f1a1a-178">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a1a-178">Int32</span></span>|<span data-ttu-id="f1a1a-179">Время, в течение которого выполняется анализ пользовательского интерфейса на рабочем столе в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-179">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="f1a1a-180">блуескринкаунт</span><span class="sxs-lookup"><span data-stu-id="f1a1a-180">blueScreenCount</span></span>|<span data-ttu-id="f1a1a-181">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a1a-181">Int32</span></span>|<span data-ttu-id="f1a1a-182">Число синих экранов за последние 14 дней.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-182">Number of Blue Screens in the last 14 days.</span></span> <span data-ttu-id="f1a1a-183">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="f1a1a-183">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="f1a1a-184">restartCount</span><span class="sxs-lookup"><span data-stu-id="f1a1a-184">restartCount</span></span>|<span data-ttu-id="f1a1a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a1a-185">Int32</span></span>|<span data-ttu-id="f1a1a-186">Количество перезапусков за последние 14 дней.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-186">Number of Restarts in the last 14 days.</span></span> <span data-ttu-id="f1a1a-187">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="f1a1a-187">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="f1a1a-188">аверажеблуескринс</span><span class="sxs-lookup"><span data-stu-id="f1a1a-188">averageBlueScreens</span></span>|<span data-ttu-id="f1a1a-189">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="f1a1a-189">Double</span></span>|<span data-ttu-id="f1a1a-190">Среднее (среднее) количество синих экранов на устройство за последние 14 дней.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-190">Average (mean) number of Blue Screens per device in the last 14 days.</span></span> <span data-ttu-id="f1a1a-191">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="f1a1a-191">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="f1a1a-192">аверажерестартс</span><span class="sxs-lookup"><span data-stu-id="f1a1a-192">averageRestarts</span></span>|<span data-ttu-id="f1a1a-193">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="f1a1a-193">Double</span></span>|<span data-ttu-id="f1a1a-194">Средняя (среднее) Количество перезапусков на устройство за последние 14 дней.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-194">Average (mean) number of Restarts per device in the last 14 days.</span></span> <span data-ttu-id="f1a1a-195">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="f1a1a-195">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="f1a1a-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1a1a-196">Response</span></span>
<span data-ttu-id="f1a1a-197">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-197">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1a1a-198">Пример</span><span class="sxs-lookup"><span data-stu-id="f1a1a-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1a1a-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1a1a-199">Request</span></span>
<span data-ttu-id="f1a1a-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance
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

### <a name="response"></a><span data-ttu-id="f1a1a-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1a1a-201">Response</span></span>
<span data-ttu-id="f1a1a-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1a1a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






