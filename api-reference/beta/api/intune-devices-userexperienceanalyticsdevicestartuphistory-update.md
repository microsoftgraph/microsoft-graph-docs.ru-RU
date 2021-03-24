---
title: Обновление userExperienceAnalyticsDeviceStartupHistory
description: Обновление свойств объекта userExperienceAnalyticsDeviceStartupHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 17eccd604ae452bb169fe4d7eb82f97ed1bc51ab
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146232"
---
# <a name="update-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="f76ca-103">Обновление userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="f76ca-103">Update userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="f76ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f76ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f76ca-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f76ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f76ca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f76ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f76ca-107">Обновление свойств объекта [userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)</span><span class="sxs-lookup"><span data-stu-id="f76ca-107">Update the properties of a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f76ca-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f76ca-108">Prerequisites</span></span>
<span data-ttu-id="f76ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f76ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f76ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f76ca-111">Permission type</span></span>|<span data-ttu-id="f76ca-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f76ca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f76ca-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f76ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f76ca-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f76ca-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f76ca-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f76ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f76ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f76ca-116">Not supported.</span></span>|
|<span data-ttu-id="f76ca-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f76ca-117">Application</span></span>|<span data-ttu-id="f76ca-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f76ca-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f76ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f76ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="f76ca-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f76ca-120">Request headers</span></span>
|<span data-ttu-id="f76ca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f76ca-121">Header</span></span>|<span data-ttu-id="f76ca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f76ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f76ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f76ca-123">Authorization</span></span>|<span data-ttu-id="f76ca-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f76ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f76ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f76ca-125">Accept</span></span>|<span data-ttu-id="f76ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f76ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f76ca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f76ca-127">Request body</span></span>
<span data-ttu-id="f76ca-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)</span><span class="sxs-lookup"><span data-stu-id="f76ca-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

<span data-ttu-id="f76ca-129">В следующей таблице показаны свойства, необходимые при создании [пользователяExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)</span><span class="sxs-lookup"><span data-stu-id="f76ca-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).</span></span>

|<span data-ttu-id="f76ca-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f76ca-130">Property</span></span>|<span data-ttu-id="f76ca-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f76ca-131">Type</span></span>|<span data-ttu-id="f76ca-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f76ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f76ca-133">id</span><span class="sxs-lookup"><span data-stu-id="f76ca-133">id</span></span>|<span data-ttu-id="f76ca-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f76ca-134">String</span></span>|<span data-ttu-id="f76ca-135">Уникальный идентификатор истории запуска устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="f76ca-135">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="f76ca-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="f76ca-136">deviceId</span></span>|<span data-ttu-id="f76ca-137">String</span><span class="sxs-lookup"><span data-stu-id="f76ca-137">String</span></span>|<span data-ttu-id="f76ca-138">ID устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="f76ca-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="f76ca-139">startTime</span><span class="sxs-lookup"><span data-stu-id="f76ca-139">startTime</span></span>|<span data-ttu-id="f76ca-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f76ca-140">DateTimeOffset</span></span>|<span data-ttu-id="f76ca-141">Время запуска загрузки устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="f76ca-141">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="f76ca-142">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f76ca-142">coreBootTimeInMs</span></span>|<span data-ttu-id="f76ca-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f76ca-143">Int32</span></span>|<span data-ttu-id="f76ca-144">Основное время загрузки устройства для аналитики пользовательского интерфейса в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="f76ca-144">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="f76ca-145">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f76ca-145">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="f76ca-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f76ca-146">Int32</span></span>|<span data-ttu-id="f76ca-147">Время загрузки групповой политики пользовательского интерфейса устройства в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="f76ca-147">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="f76ca-148">featureUpdateBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f76ca-148">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="f76ca-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f76ca-149">Int32</span></span>|<span data-ttu-id="f76ca-150">Время обновления устройства аналитики пользовательского интерфейса в миллисекундном периоде.</span><span class="sxs-lookup"><span data-stu-id="f76ca-150">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="f76ca-151">totalBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f76ca-151">totalBootTimeInMs</span></span>|<span data-ttu-id="f76ca-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f76ca-152">Int32</span></span>|<span data-ttu-id="f76ca-153">Общее время загрузки устройства аналитики пользовательского интерфейса в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="f76ca-153">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="f76ca-154">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f76ca-154">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="f76ca-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f76ca-155">Int32</span></span>|<span data-ttu-id="f76ca-156">Время входа в группу политик пользовательского интерфейса для аналитики устройств в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="f76ca-156">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="f76ca-157">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f76ca-157">coreLoginTimeInMs</span></span>|<span data-ttu-id="f76ca-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f76ca-158">Int32</span></span>|<span data-ttu-id="f76ca-159">Время входа основного устройства для аналитики пользовательского интерфейса в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="f76ca-159">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="f76ca-160">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f76ca-160">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="f76ca-161">Int32</span><span class="sxs-lookup"><span data-stu-id="f76ca-161">Int32</span></span>|<span data-ttu-id="f76ca-162">Аналитика пользовательского интерфейса реагирует на время рабочего стола в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="f76ca-162">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="f76ca-163">totalLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f76ca-163">totalLoginTimeInMs</span></span>|<span data-ttu-id="f76ca-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f76ca-164">Int32</span></span>|<span data-ttu-id="f76ca-165">Общее время входа устройства аналитики пользовательского интерфейса в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="f76ca-165">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="f76ca-166">isFirstLogin</span><span class="sxs-lookup"><span data-stu-id="f76ca-166">isFirstLogin</span></span>|<span data-ttu-id="f76ca-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="f76ca-167">Boolean</span></span>|<span data-ttu-id="f76ca-168">Устройство аналитики пользовательского интерфейса сначала входит в систему.</span><span class="sxs-lookup"><span data-stu-id="f76ca-168">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="f76ca-169">isFeatureUpdate</span><span class="sxs-lookup"><span data-stu-id="f76ca-169">isFeatureUpdate</span></span>|<span data-ttu-id="f76ca-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="f76ca-170">Boolean</span></span>|<span data-ttu-id="f76ca-171">Запись загрузки устройства для аналитики пользовательского интерфейса — это обновление функций.</span><span class="sxs-lookup"><span data-stu-id="f76ca-171">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="f76ca-172">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="f76ca-172">operatingSystemVersion</span></span>|<span data-ttu-id="f76ca-173">String</span><span class="sxs-lookup"><span data-stu-id="f76ca-173">String</span></span>|<span data-ttu-id="f76ca-174">Версия операционной системы записи операционной системы для аналитики пользовательского интерфейса устройства.</span><span class="sxs-lookup"><span data-stu-id="f76ca-174">The user experience analytics device boot record's operating system version.</span></span>|
|<span data-ttu-id="f76ca-175">restartCategory</span><span class="sxs-lookup"><span data-stu-id="f76ca-175">restartCategory</span></span>|[<span data-ttu-id="f76ca-176">userExperienceAnalyticsOperatingSystemRestartCategory</span><span class="sxs-lookup"><span data-stu-id="f76ca-176">userExperienceAnalyticsOperatingSystemRestartCategory</span></span>](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|<span data-ttu-id="f76ca-177">Категория перезапуска ОС.</span><span class="sxs-lookup"><span data-stu-id="f76ca-177">OS restart category.</span></span> <span data-ttu-id="f76ca-178">Возможные значения: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.</span><span class="sxs-lookup"><span data-stu-id="f76ca-178">Possible values are: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.</span></span>|
|<span data-ttu-id="f76ca-179">restartStopCode</span><span class="sxs-lookup"><span data-stu-id="f76ca-179">restartStopCode</span></span>|<span data-ttu-id="f76ca-180">Строка</span><span class="sxs-lookup"><span data-stu-id="f76ca-180">String</span></span>|<span data-ttu-id="f76ca-181">Код остановки перезапуска ОС.</span><span class="sxs-lookup"><span data-stu-id="f76ca-181">OS restart stop code.</span></span> <span data-ttu-id="f76ca-182">Здесь показан код проверки ошибок, который можно использовать для проверки причины синего экрана.</span><span class="sxs-lookup"><span data-stu-id="f76ca-182">This shows the bug check code which can be used to look up the blue screen reason.</span></span>|
|<span data-ttu-id="f76ca-183">restartFaultBucket</span><span class="sxs-lookup"><span data-stu-id="f76ca-183">restartFaultBucket</span></span>|<span data-ttu-id="f76ca-184">Строка</span><span class="sxs-lookup"><span data-stu-id="f76ca-184">String</span></span>|<span data-ttu-id="f76ca-185">Ковш перезапуска неисправности ОС.</span><span class="sxs-lookup"><span data-stu-id="f76ca-185">OS restart fault bucket.</span></span> <span data-ttu-id="f76ca-186">Ведро неисправностей используется для поиска дополнительных сведений о сбое системы.</span><span class="sxs-lookup"><span data-stu-id="f76ca-186">The fault bucket is used to find additional information about a system crash.</span></span>|



## <a name="response"></a><span data-ttu-id="f76ca-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="f76ca-187">Response</span></span>
<span data-ttu-id="f76ca-188">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f76ca-188">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f76ca-189">Пример</span><span class="sxs-lookup"><span data-stu-id="f76ca-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="f76ca-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="f76ca-190">Request</span></span>
<span data-ttu-id="f76ca-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f76ca-191">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f76ca-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="f76ca-192">Response</span></span>
<span data-ttu-id="f76ca-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f76ca-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




