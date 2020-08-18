---
title: Создание Усерекспериенцеаналитиксдевицестартуфистори
description: Создание нового объекта Усерекспериенцеаналитиксдевицестартуфистори.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f5b91043417fb0e33dd7f7781c82503525b5d185
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791353"
---
# <a name="create-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="53974-103">Создание Усерекспериенцеаналитиксдевицестартуфистори</span><span class="sxs-lookup"><span data-stu-id="53974-103">Create userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="53974-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53974-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53974-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53974-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53974-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53974-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53974-107">Создание нового объекта [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .</span><span class="sxs-lookup"><span data-stu-id="53974-107">Create a new [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53974-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="53974-108">Prerequisites</span></span>
<span data-ttu-id="53974-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53974-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53974-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53974-111">Permission type</span></span>|<span data-ttu-id="53974-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53974-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53974-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53974-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53974-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53974-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="53974-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53974-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53974-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53974-116">Not supported.</span></span>|
|<span data-ttu-id="53974-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="53974-117">Application</span></span>|<span data-ttu-id="53974-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53974-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53974-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53974-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a><span data-ttu-id="53974-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="53974-120">Request headers</span></span>
|<span data-ttu-id="53974-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53974-121">Header</span></span>|<span data-ttu-id="53974-122">Значение</span><span class="sxs-lookup"><span data-stu-id="53974-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53974-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53974-123">Authorization</span></span>|<span data-ttu-id="53974-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53974-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53974-125">Accept</span><span class="sxs-lookup"><span data-stu-id="53974-125">Accept</span></span>|<span data-ttu-id="53974-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53974-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53974-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53974-127">Request body</span></span>
<span data-ttu-id="53974-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксдевицестартуфистори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53974-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupHistory object.</span></span>

<span data-ttu-id="53974-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксдевицестартуфистори.</span><span class="sxs-lookup"><span data-stu-id="53974-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupHistory.</span></span>

|<span data-ttu-id="53974-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="53974-130">Property</span></span>|<span data-ttu-id="53974-131">Тип</span><span class="sxs-lookup"><span data-stu-id="53974-131">Type</span></span>|<span data-ttu-id="53974-132">Описание</span><span class="sxs-lookup"><span data-stu-id="53974-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53974-133">id</span><span class="sxs-lookup"><span data-stu-id="53974-133">id</span></span>|<span data-ttu-id="53974-134">String</span><span class="sxs-lookup"><span data-stu-id="53974-134">String</span></span>|<span data-ttu-id="53974-135">Уникальный идентификатор журнала запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="53974-135">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="53974-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="53974-136">deviceId</span></span>|<span data-ttu-id="53974-137">String</span><span class="sxs-lookup"><span data-stu-id="53974-137">String</span></span>|<span data-ttu-id="53974-138">Идентификатор устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="53974-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="53974-139">startTime</span><span class="sxs-lookup"><span data-stu-id="53974-139">startTime</span></span>|<span data-ttu-id="53974-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53974-140">DateTimeOffset</span></span>|<span data-ttu-id="53974-141">Время начала загрузки устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="53974-141">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="53974-142">коребуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="53974-142">coreBootTimeInMs</span></span>|<span data-ttu-id="53974-143">Int32</span><span class="sxs-lookup"><span data-stu-id="53974-143">Int32</span></span>|<span data-ttu-id="53974-144">Время загрузки ядра устройства аналитики для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="53974-144">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="53974-145">граупполицибуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="53974-145">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="53974-146">Int32</span><span class="sxs-lookup"><span data-stu-id="53974-146">Int32</span></span>|<span data-ttu-id="53974-147">Время загрузки групповой политики устройства Analytics для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="53974-147">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="53974-148">феатуреупдатебуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="53974-148">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="53974-149">Int32</span><span class="sxs-lookup"><span data-stu-id="53974-149">Int32</span></span>|<span data-ttu-id="53974-150">Время обновления компонента службы аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="53974-150">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="53974-151">тоталбуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="53974-151">totalBootTimeInMs</span></span>|<span data-ttu-id="53974-152">Int32</span><span class="sxs-lookup"><span data-stu-id="53974-152">Int32</span></span>|<span data-ttu-id="53974-153">Общее время загрузки устройства Analytics User Experience (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="53974-153">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="53974-154">граупполицилогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="53974-154">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="53974-155">Int32</span><span class="sxs-lookup"><span data-stu-id="53974-155">Int32</span></span>|<span data-ttu-id="53974-156">Время входа в групповую политику устройства Analytics User Experience (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="53974-156">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="53974-157">корелогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="53974-157">coreLoginTimeInMs</span></span>|<span data-ttu-id="53974-158">Int32</span><span class="sxs-lookup"><span data-stu-id="53974-158">Int32</span></span>|<span data-ttu-id="53974-159">Время входа в ядро устройства аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="53974-159">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="53974-160">респонсиведесктоптимеинмс</span><span class="sxs-lookup"><span data-stu-id="53974-160">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="53974-161">Int32</span><span class="sxs-lookup"><span data-stu-id="53974-161">Int32</span></span>|<span data-ttu-id="53974-162">Время, в течение которого выполняется анализ пользовательского интерфейса на рабочем столе в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="53974-162">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="53974-163">тоталлогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="53974-163">totalLoginTimeInMs</span></span>|<span data-ttu-id="53974-164">Int32</span><span class="sxs-lookup"><span data-stu-id="53974-164">Int32</span></span>|<span data-ttu-id="53974-165">Общее время входа в систему для устройства аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="53974-165">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="53974-166">исфирстлогин</span><span class="sxs-lookup"><span data-stu-id="53974-166">isFirstLogin</span></span>|<span data-ttu-id="53974-167">Логический</span><span class="sxs-lookup"><span data-stu-id="53974-167">Boolean</span></span>|<span data-ttu-id="53974-168">Первое имя входа устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="53974-168">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="53974-169">исфеатуреупдате</span><span class="sxs-lookup"><span data-stu-id="53974-169">isFeatureUpdate</span></span>|<span data-ttu-id="53974-170">Логический</span><span class="sxs-lookup"><span data-stu-id="53974-170">Boolean</span></span>|<span data-ttu-id="53974-171">Загрузочная запись устройства аналитики взаимодействия с пользователем — это обновление компонентов.</span><span class="sxs-lookup"><span data-stu-id="53974-171">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="53974-172">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="53974-172">operatingSystemVersion</span></span>|<span data-ttu-id="53974-173">String</span><span class="sxs-lookup"><span data-stu-id="53974-173">String</span></span>|<span data-ttu-id="53974-174">Версия операционной системы для записи загрузки устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="53974-174">The user experience analytics device boot record's operating system version.</span></span>|
|<span data-ttu-id="53974-175">рестарткатегори</span><span class="sxs-lookup"><span data-stu-id="53974-175">restartCategory</span></span>|[<span data-ttu-id="53974-176">усерекспериенцеаналитиксоператингсистемрестарткатегори</span><span class="sxs-lookup"><span data-stu-id="53974-176">userExperienceAnalyticsOperatingSystemRestartCategory</span></span>](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|<span data-ttu-id="53974-177">Категория перезагрузки ОС.</span><span class="sxs-lookup"><span data-stu-id="53974-177">OS restart category.</span></span> <span data-ttu-id="53974-178">Возможные значения: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`.</span><span class="sxs-lookup"><span data-stu-id="53974-178">Possible values are: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`.</span></span>|



## <a name="response"></a><span data-ttu-id="53974-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="53974-179">Response</span></span>
<span data-ttu-id="53974-180">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53974-180">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53974-181">Пример</span><span class="sxs-lookup"><span data-stu-id="53974-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="53974-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="53974-182">Request</span></span>
<span data-ttu-id="53974-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53974-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
Content-type: application/json
Content-length: 576

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
  "restartCategory": "restartWithUpdate"
}
```

### <a name="response"></a><span data-ttu-id="53974-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="53974-184">Response</span></span>
<span data-ttu-id="53974-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53974-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 625

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
  "restartCategory": "restartWithUpdate"
}
```



