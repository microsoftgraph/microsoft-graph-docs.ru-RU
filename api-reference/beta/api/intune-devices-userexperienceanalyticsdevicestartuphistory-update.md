---
title: Обновление Усерекспериенцеаналитиксдевицестартуфистори
description: Обновление свойств объекта Усерекспериенцеаналитиксдевицестартуфистори.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1593fc62a9cc6b185af558bd4f4b5c73edd5630b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813925"
---
# <a name="update-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="228da-103">Обновление Усерекспериенцеаналитиксдевицестартуфистори</span><span class="sxs-lookup"><span data-stu-id="228da-103">Update userExperienceAnalyticsDeviceStartupHistory</span></span>

> <span data-ttu-id="228da-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="228da-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="228da-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="228da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="228da-106">Обновление свойств объекта [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .</span><span class="sxs-lookup"><span data-stu-id="228da-106">Update the properties of a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="228da-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="228da-107">Prerequisites</span></span>
<span data-ttu-id="228da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="228da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="228da-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="228da-110">Permission type</span></span>|<span data-ttu-id="228da-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="228da-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="228da-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="228da-112">Delegated (work or school account)</span></span>|<span data-ttu-id="228da-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="228da-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="228da-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="228da-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="228da-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="228da-115">Not supported.</span></span>|
|<span data-ttu-id="228da-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="228da-116">Application</span></span>|<span data-ttu-id="228da-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="228da-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="228da-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="228da-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="228da-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="228da-119">Request headers</span></span>
|<span data-ttu-id="228da-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="228da-120">Header</span></span>|<span data-ttu-id="228da-121">Значение</span><span class="sxs-lookup"><span data-stu-id="228da-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="228da-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="228da-122">Authorization</span></span>|<span data-ttu-id="228da-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="228da-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="228da-124">Accept</span><span class="sxs-lookup"><span data-stu-id="228da-124">Accept</span></span>|<span data-ttu-id="228da-125">application/json</span><span class="sxs-lookup"><span data-stu-id="228da-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="228da-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="228da-126">Request body</span></span>
<span data-ttu-id="228da-127">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="228da-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

<span data-ttu-id="228da-128">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).</span><span class="sxs-lookup"><span data-stu-id="228da-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).</span></span>

|<span data-ttu-id="228da-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="228da-129">Property</span></span>|<span data-ttu-id="228da-130">Тип</span><span class="sxs-lookup"><span data-stu-id="228da-130">Type</span></span>|<span data-ttu-id="228da-131">Описание</span><span class="sxs-lookup"><span data-stu-id="228da-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="228da-132">id</span><span class="sxs-lookup"><span data-stu-id="228da-132">id</span></span>|<span data-ttu-id="228da-133">String</span><span class="sxs-lookup"><span data-stu-id="228da-133">String</span></span>|<span data-ttu-id="228da-134">Уникальный идентификатор журнала запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="228da-134">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="228da-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="228da-135">deviceId</span></span>|<span data-ttu-id="228da-136">String</span><span class="sxs-lookup"><span data-stu-id="228da-136">String</span></span>|<span data-ttu-id="228da-137">Идентификатор устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="228da-137">The user experience analytics device id.</span></span>|
|<span data-ttu-id="228da-138">startTime</span><span class="sxs-lookup"><span data-stu-id="228da-138">startTime</span></span>|<span data-ttu-id="228da-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="228da-139">DateTimeOffset</span></span>|<span data-ttu-id="228da-140">Время начала загрузки устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="228da-140">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="228da-141">коребуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="228da-141">coreBootTimeInMs</span></span>|<span data-ttu-id="228da-142">Int32</span><span class="sxs-lookup"><span data-stu-id="228da-142">Int32</span></span>|<span data-ttu-id="228da-143">Время загрузки ядра устройства аналитики для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="228da-143">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="228da-144">граупполицибуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="228da-144">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="228da-145">Int32</span><span class="sxs-lookup"><span data-stu-id="228da-145">Int32</span></span>|<span data-ttu-id="228da-146">Время загрузки групповой политики устройства Analytics для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="228da-146">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="228da-147">феатуреупдатебуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="228da-147">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="228da-148">Int32</span><span class="sxs-lookup"><span data-stu-id="228da-148">Int32</span></span>|<span data-ttu-id="228da-149">Время обновления компонента службы аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="228da-149">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="228da-150">тоталбуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="228da-150">totalBootTimeInMs</span></span>|<span data-ttu-id="228da-151">Int32</span><span class="sxs-lookup"><span data-stu-id="228da-151">Int32</span></span>|<span data-ttu-id="228da-152">Общее время загрузки устройства Analytics User Experience (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="228da-152">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="228da-153">граупполицилогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="228da-153">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="228da-154">Int32</span><span class="sxs-lookup"><span data-stu-id="228da-154">Int32</span></span>|<span data-ttu-id="228da-155">Время входа в групповую политику устройства Analytics User Experience (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="228da-155">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="228da-156">корелогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="228da-156">coreLoginTimeInMs</span></span>|<span data-ttu-id="228da-157">Int32</span><span class="sxs-lookup"><span data-stu-id="228da-157">Int32</span></span>|<span data-ttu-id="228da-158">Время входа в ядро устройства аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="228da-158">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="228da-159">респонсиведесктоптимеинмс</span><span class="sxs-lookup"><span data-stu-id="228da-159">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="228da-160">Int32</span><span class="sxs-lookup"><span data-stu-id="228da-160">Int32</span></span>|<span data-ttu-id="228da-161">Время, в течение которого выполняется анализ пользовательского интерфейса на рабочем столе в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="228da-161">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="228da-162">тоталлогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="228da-162">totalLoginTimeInMs</span></span>|<span data-ttu-id="228da-163">Int32</span><span class="sxs-lookup"><span data-stu-id="228da-163">Int32</span></span>|<span data-ttu-id="228da-164">Общее время входа в систему для устройства аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="228da-164">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="228da-165">исфирстлогин</span><span class="sxs-lookup"><span data-stu-id="228da-165">isFirstLogin</span></span>|<span data-ttu-id="228da-166">Логический</span><span class="sxs-lookup"><span data-stu-id="228da-166">Boolean</span></span>|<span data-ttu-id="228da-167">Первое имя входа устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="228da-167">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="228da-168">исфеатуреупдате</span><span class="sxs-lookup"><span data-stu-id="228da-168">isFeatureUpdate</span></span>|<span data-ttu-id="228da-169">Логический</span><span class="sxs-lookup"><span data-stu-id="228da-169">Boolean</span></span>|<span data-ttu-id="228da-170">Загрузочная запись устройства аналитики взаимодействия с пользователем — это обновление компонентов.</span><span class="sxs-lookup"><span data-stu-id="228da-170">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="228da-171">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="228da-171">operatingSystemVersion</span></span>|<span data-ttu-id="228da-172">String</span><span class="sxs-lookup"><span data-stu-id="228da-172">String</span></span>|<span data-ttu-id="228da-173">Версия операционной системы для записи загрузки устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="228da-173">The user experience analytics device boot record's operating system version.</span></span>|



## <a name="response"></a><span data-ttu-id="228da-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="228da-174">Response</span></span>
<span data-ttu-id="228da-175">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="228da-175">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="228da-176">Пример</span><span class="sxs-lookup"><span data-stu-id="228da-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="228da-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="228da-177">Request</span></span>
<span data-ttu-id="228da-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="228da-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
Content-type: application/json
Content-length: 533

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
  "operatingSystemVersion": "Operating System Version value"
}
```

### <a name="response"></a><span data-ttu-id="228da-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="228da-179">Response</span></span>
<span data-ttu-id="228da-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="228da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

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
  "operatingSystemVersion": "Operating System Version value"
}
```




