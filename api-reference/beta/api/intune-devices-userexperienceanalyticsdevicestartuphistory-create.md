---
title: Создание Усерекспериенцеаналитиксдевицестартуфистори
description: Создание нового объекта Усерекспериенцеаналитиксдевицестартуфистори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dec1a8c5848e2646674390ff38ff645e88ec2b6a
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162038"
---
# <a name="create-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="f1530-103">Создание Усерекспериенцеаналитиксдевицестартуфистори</span><span class="sxs-lookup"><span data-stu-id="f1530-103">Create userExperienceAnalyticsDeviceStartupHistory</span></span>

> <span data-ttu-id="f1530-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1530-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1530-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1530-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1530-106">Создание нового объекта [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .</span><span class="sxs-lookup"><span data-stu-id="f1530-106">Create a new [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1530-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1530-107">Prerequisites</span></span>
<span data-ttu-id="f1530-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1530-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1530-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1530-110">Permission type</span></span>|<span data-ttu-id="f1530-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1530-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1530-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1530-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1530-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1530-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f1530-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1530-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1530-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1530-115">Not supported.</span></span>|
|<span data-ttu-id="f1530-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1530-116">Application</span></span>|<span data-ttu-id="f1530-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1530-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1530-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1530-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a><span data-ttu-id="f1530-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f1530-119">Request headers</span></span>
|<span data-ttu-id="f1530-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1530-120">Header</span></span>|<span data-ttu-id="f1530-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f1530-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1530-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1530-122">Authorization</span></span>|<span data-ttu-id="f1530-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1530-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1530-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f1530-124">Accept</span></span>|<span data-ttu-id="f1530-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1530-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1530-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1530-126">Request body</span></span>
<span data-ttu-id="f1530-127">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксдевицестартуфистори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1530-127">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupHistory object.</span></span>

<span data-ttu-id="f1530-128">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксдевицестартуфистори.</span><span class="sxs-lookup"><span data-stu-id="f1530-128">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupHistory.</span></span>

|<span data-ttu-id="f1530-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1530-129">Property</span></span>|<span data-ttu-id="f1530-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f1530-130">Type</span></span>|<span data-ttu-id="f1530-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f1530-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1530-132">id</span><span class="sxs-lookup"><span data-stu-id="f1530-132">id</span></span>|<span data-ttu-id="f1530-133">String</span><span class="sxs-lookup"><span data-stu-id="f1530-133">String</span></span>|<span data-ttu-id="f1530-134">Уникальный идентификатор журнала запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="f1530-134">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="f1530-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="f1530-135">deviceId</span></span>|<span data-ttu-id="f1530-136">String</span><span class="sxs-lookup"><span data-stu-id="f1530-136">String</span></span>|<span data-ttu-id="f1530-137">Идентификатор устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1530-137">The user experience analytics device id.</span></span>|
|<span data-ttu-id="f1530-138">startTime</span><span class="sxs-lookup"><span data-stu-id="f1530-138">startTime</span></span>|<span data-ttu-id="f1530-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1530-139">DateTimeOffset</span></span>|<span data-ttu-id="f1530-140">Время начала загрузки устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="f1530-140">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="f1530-141">коребуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="f1530-141">coreBootTimeInMs</span></span>|<span data-ttu-id="f1530-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f1530-142">Int32</span></span>|<span data-ttu-id="f1530-143">Время загрузки ядра устройства аналитики для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="f1530-143">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="f1530-144">граупполицибуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="f1530-144">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="f1530-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f1530-145">Int32</span></span>|<span data-ttu-id="f1530-146">Время загрузки групповой политики устройства Analytics для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="f1530-146">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="f1530-147">феатуреупдатебуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="f1530-147">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="f1530-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f1530-148">Int32</span></span>|<span data-ttu-id="f1530-149">Время обновления компонента службы аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="f1530-149">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="f1530-150">тоталбуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="f1530-150">totalBootTimeInMs</span></span>|<span data-ttu-id="f1530-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f1530-151">Int32</span></span>|<span data-ttu-id="f1530-152">Общее время загрузки устройства Analytics User Experience (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="f1530-152">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="f1530-153">граупполицилогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="f1530-153">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="f1530-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f1530-154">Int32</span></span>|<span data-ttu-id="f1530-155">Время входа в групповую политику устройства Analytics User Experience (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="f1530-155">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="f1530-156">корелогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="f1530-156">coreLoginTimeInMs</span></span>|<span data-ttu-id="f1530-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f1530-157">Int32</span></span>|<span data-ttu-id="f1530-158">Время входа в ядро устройства аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="f1530-158">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="f1530-159">респонсиведесктоптимеинмс</span><span class="sxs-lookup"><span data-stu-id="f1530-159">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="f1530-160">Int32</span><span class="sxs-lookup"><span data-stu-id="f1530-160">Int32</span></span>|<span data-ttu-id="f1530-161">Время, в течение которого выполняется анализ пользовательского интерфейса на рабочем столе в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="f1530-161">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="f1530-162">тоталлогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="f1530-162">totalLoginTimeInMs</span></span>|<span data-ttu-id="f1530-163">Int32</span><span class="sxs-lookup"><span data-stu-id="f1530-163">Int32</span></span>|<span data-ttu-id="f1530-164">Общее время входа в систему для устройства аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="f1530-164">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="f1530-165">исфирстлогин</span><span class="sxs-lookup"><span data-stu-id="f1530-165">isFirstLogin</span></span>|<span data-ttu-id="f1530-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1530-166">Boolean</span></span>|<span data-ttu-id="f1530-167">Первое имя входа устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="f1530-167">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="f1530-168">исфеатуреупдате</span><span class="sxs-lookup"><span data-stu-id="f1530-168">isFeatureUpdate</span></span>|<span data-ttu-id="f1530-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1530-169">Boolean</span></span>|<span data-ttu-id="f1530-170">Загрузочная запись устройства аналитики взаимодействия с пользователем — это обновление компонентов.</span><span class="sxs-lookup"><span data-stu-id="f1530-170">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="f1530-171">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="f1530-171">operatingSystemVersion</span></span>|<span data-ttu-id="f1530-172">String</span><span class="sxs-lookup"><span data-stu-id="f1530-172">String</span></span>|<span data-ttu-id="f1530-173">Версия операционной системы для записи загрузки устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1530-173">The user experience analytics device boot record's operating system version.</span></span>|



## <a name="response"></a><span data-ttu-id="f1530-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1530-174">Response</span></span>
<span data-ttu-id="f1530-175">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1530-175">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1530-176">Пример</span><span class="sxs-lookup"><span data-stu-id="f1530-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1530-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1530-177">Request</span></span>
<span data-ttu-id="f1530-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1530-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
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

### <a name="response"></a><span data-ttu-id="f1530-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1530-179">Response</span></span>
<span data-ttu-id="f1530-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1530-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





