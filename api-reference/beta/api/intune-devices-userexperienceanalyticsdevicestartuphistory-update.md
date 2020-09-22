---
title: Обновление Усерекспериенцеаналитиксдевицестартуфистори
description: Обновление свойств объекта Усерекспериенцеаналитиксдевицестартуфистори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ff216d06922f50dabc539f046055c73aebca739
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082590"
---
# <a name="update-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="30b04-103">Обновление Усерекспериенцеаналитиксдевицестартуфистори</span><span class="sxs-lookup"><span data-stu-id="30b04-103">Update userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="30b04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30b04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30b04-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30b04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30b04-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30b04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30b04-107">Обновление свойств объекта [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .</span><span class="sxs-lookup"><span data-stu-id="30b04-107">Update the properties of a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30b04-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="30b04-108">Prerequisites</span></span>
<span data-ttu-id="30b04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30b04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30b04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30b04-111">Permission type</span></span>|<span data-ttu-id="30b04-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30b04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30b04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30b04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30b04-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30b04-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="30b04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30b04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30b04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30b04-116">Not supported.</span></span>|
|<span data-ttu-id="30b04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30b04-117">Application</span></span>|<span data-ttu-id="30b04-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30b04-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30b04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30b04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="30b04-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="30b04-120">Request headers</span></span>
|<span data-ttu-id="30b04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30b04-121">Header</span></span>|<span data-ttu-id="30b04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="30b04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30b04-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30b04-123">Authorization</span></span>|<span data-ttu-id="30b04-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30b04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30b04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30b04-125">Accept</span></span>|<span data-ttu-id="30b04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30b04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30b04-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30b04-127">Request body</span></span>
<span data-ttu-id="30b04-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30b04-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

<span data-ttu-id="30b04-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).</span><span class="sxs-lookup"><span data-stu-id="30b04-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).</span></span>

|<span data-ttu-id="30b04-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="30b04-130">Property</span></span>|<span data-ttu-id="30b04-131">Тип</span><span class="sxs-lookup"><span data-stu-id="30b04-131">Type</span></span>|<span data-ttu-id="30b04-132">Описание</span><span class="sxs-lookup"><span data-stu-id="30b04-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30b04-133">id</span><span class="sxs-lookup"><span data-stu-id="30b04-133">id</span></span>|<span data-ttu-id="30b04-134">Строка</span><span class="sxs-lookup"><span data-stu-id="30b04-134">String</span></span>|<span data-ttu-id="30b04-135">Уникальный идентификатор журнала запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="30b04-135">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="30b04-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="30b04-136">deviceId</span></span>|<span data-ttu-id="30b04-137">String</span><span class="sxs-lookup"><span data-stu-id="30b04-137">String</span></span>|<span data-ttu-id="30b04-138">Идентификатор устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="30b04-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="30b04-139">startTime</span><span class="sxs-lookup"><span data-stu-id="30b04-139">startTime</span></span>|<span data-ttu-id="30b04-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30b04-140">DateTimeOffset</span></span>|<span data-ttu-id="30b04-141">Время начала загрузки устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="30b04-141">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="30b04-142">коребуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="30b04-142">coreBootTimeInMs</span></span>|<span data-ttu-id="30b04-143">Int32</span><span class="sxs-lookup"><span data-stu-id="30b04-143">Int32</span></span>|<span data-ttu-id="30b04-144">Время загрузки ядра устройства аналитики для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="30b04-144">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="30b04-145">граупполицибуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="30b04-145">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="30b04-146">Int32</span><span class="sxs-lookup"><span data-stu-id="30b04-146">Int32</span></span>|<span data-ttu-id="30b04-147">Время загрузки групповой политики устройства Analytics для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="30b04-147">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="30b04-148">феатуреупдатебуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="30b04-148">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="30b04-149">Int32</span><span class="sxs-lookup"><span data-stu-id="30b04-149">Int32</span></span>|<span data-ttu-id="30b04-150">Время обновления компонента службы аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="30b04-150">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="30b04-151">тоталбуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="30b04-151">totalBootTimeInMs</span></span>|<span data-ttu-id="30b04-152">Int32</span><span class="sxs-lookup"><span data-stu-id="30b04-152">Int32</span></span>|<span data-ttu-id="30b04-153">Общее время загрузки устройства Analytics User Experience (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="30b04-153">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="30b04-154">граупполицилогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="30b04-154">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="30b04-155">Int32</span><span class="sxs-lookup"><span data-stu-id="30b04-155">Int32</span></span>|<span data-ttu-id="30b04-156">Время входа в групповую политику устройства Analytics User Experience (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="30b04-156">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="30b04-157">корелогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="30b04-157">coreLoginTimeInMs</span></span>|<span data-ttu-id="30b04-158">Int32</span><span class="sxs-lookup"><span data-stu-id="30b04-158">Int32</span></span>|<span data-ttu-id="30b04-159">Время входа в ядро устройства аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="30b04-159">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="30b04-160">респонсиведесктоптимеинмс</span><span class="sxs-lookup"><span data-stu-id="30b04-160">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="30b04-161">Int32</span><span class="sxs-lookup"><span data-stu-id="30b04-161">Int32</span></span>|<span data-ttu-id="30b04-162">Время, в течение которого выполняется анализ пользовательского интерфейса на рабочем столе в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="30b04-162">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="30b04-163">тоталлогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="30b04-163">totalLoginTimeInMs</span></span>|<span data-ttu-id="30b04-164">Int32</span><span class="sxs-lookup"><span data-stu-id="30b04-164">Int32</span></span>|<span data-ttu-id="30b04-165">Общее время входа в систему для устройства аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="30b04-165">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="30b04-166">исфирстлогин</span><span class="sxs-lookup"><span data-stu-id="30b04-166">isFirstLogin</span></span>|<span data-ttu-id="30b04-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="30b04-167">Boolean</span></span>|<span data-ttu-id="30b04-168">Первое имя входа устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="30b04-168">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="30b04-169">исфеатуреупдате</span><span class="sxs-lookup"><span data-stu-id="30b04-169">isFeatureUpdate</span></span>|<span data-ttu-id="30b04-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="30b04-170">Boolean</span></span>|<span data-ttu-id="30b04-171">Загрузочная запись устройства аналитики взаимодействия с пользователем — это обновление компонентов.</span><span class="sxs-lookup"><span data-stu-id="30b04-171">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="30b04-172">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="30b04-172">operatingSystemVersion</span></span>|<span data-ttu-id="30b04-173">String</span><span class="sxs-lookup"><span data-stu-id="30b04-173">String</span></span>|<span data-ttu-id="30b04-174">Версия операционной системы для записи загрузки устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="30b04-174">The user experience analytics device boot record's operating system version.</span></span>|
|<span data-ttu-id="30b04-175">рестарткатегори</span><span class="sxs-lookup"><span data-stu-id="30b04-175">restartCategory</span></span>|[<span data-ttu-id="30b04-176">userExperienceAnalyticsOperatingSystemRestartCategory</span><span class="sxs-lookup"><span data-stu-id="30b04-176">userExperienceAnalyticsOperatingSystemRestartCategory</span></span>](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|<span data-ttu-id="30b04-177">Категория перезагрузки ОС.</span><span class="sxs-lookup"><span data-stu-id="30b04-177">OS restart category.</span></span> <span data-ttu-id="30b04-178">Возможные значения: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`.</span><span class="sxs-lookup"><span data-stu-id="30b04-178">Possible values are: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`.</span></span>|
|<span data-ttu-id="30b04-179">рестартстопкоде</span><span class="sxs-lookup"><span data-stu-id="30b04-179">restartStopCode</span></span>|<span data-ttu-id="30b04-180">Строка</span><span class="sxs-lookup"><span data-stu-id="30b04-180">String</span></span>|<span data-ttu-id="30b04-181">Код остановки перезапуска ОС.</span><span class="sxs-lookup"><span data-stu-id="30b04-181">OS restart stop code.</span></span> <span data-ttu-id="30b04-182">Здесь показан код проверки ошибки, который можно использовать для поиска причины синего экрана.</span><span class="sxs-lookup"><span data-stu-id="30b04-182">This shows the bug check code which can be used to look up the blue screen reason.</span></span>|
|<span data-ttu-id="30b04-183">рестартфаултбуккет</span><span class="sxs-lookup"><span data-stu-id="30b04-183">restartFaultBucket</span></span>|<span data-ttu-id="30b04-184">Строка</span><span class="sxs-lookup"><span data-stu-id="30b04-184">String</span></span>|<span data-ttu-id="30b04-185">Сегмент сбоя при перезапуске ОС.</span><span class="sxs-lookup"><span data-stu-id="30b04-185">OS restart fault bucket.</span></span> <span data-ttu-id="30b04-186">Блок сбоя используется для поиска дополнительных сведений о сбое системы.</span><span class="sxs-lookup"><span data-stu-id="30b04-186">The fault bucket is used to find additional information about a system crash.</span></span>|



## <a name="response"></a><span data-ttu-id="30b04-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="30b04-187">Response</span></span>
<span data-ttu-id="30b04-188">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30b04-188">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30b04-189">Пример</span><span class="sxs-lookup"><span data-stu-id="30b04-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="30b04-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="30b04-190">Request</span></span>
<span data-ttu-id="30b04-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30b04-191">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
Content-type: application/json
Content-length: 680

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "responsiveDesktopTimeInMs": 9,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value",
  "restartCategory": "restartWithUpdate",
  "restartStopCode": "Restart Stop Code value",
  "restartFaultBucket": "Restart Fault Bucket value"
}
```

### <a name="response"></a><span data-ttu-id="30b04-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="30b04-192">Response</span></span>
<span data-ttu-id="30b04-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30b04-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 729

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "id": "13357123-7123-1335-2371-351323713513",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "responsiveDesktopTimeInMs": 9,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value",
  "restartCategory": "restartWithUpdate",
  "restartStopCode": "Restart Stop Code value",
  "restartFaultBucket": "Restart Fault Bucket value"
}
```






