---
title: Создание userExperienceAnalyticsDeviceStartupHistory
description: Создание нового объекта userExperienceAnalyticsDeviceStartupHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7ba56bf1f1463b3f079522ee86d3ae33f1a5b82a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154142"
---
# <a name="create-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="9bcd2-103">Создание userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="9bcd2-103">Create userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="9bcd2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bcd2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bcd2-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bcd2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bcd2-107">Создание нового [объекта userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)</span><span class="sxs-lookup"><span data-stu-id="9bcd2-107">Create a new [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bcd2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9bcd2-108">Prerequisites</span></span>
<span data-ttu-id="9bcd2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bcd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bcd2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bcd2-111">Permission type</span></span>|<span data-ttu-id="9bcd2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bcd2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bcd2-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bcd2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9bcd2-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bcd2-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9bcd2-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bcd2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bcd2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-116">Not supported.</span></span>|
|<span data-ttu-id="9bcd2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9bcd2-117">Application</span></span>|<span data-ttu-id="9bcd2-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bcd2-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bcd2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bcd2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a><span data-ttu-id="9bcd2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9bcd2-120">Request headers</span></span>
|<span data-ttu-id="9bcd2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9bcd2-121">Header</span></span>|<span data-ttu-id="9bcd2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9bcd2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bcd2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bcd2-123">Authorization</span></span>|<span data-ttu-id="9bcd2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bcd2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9bcd2-125">Accept</span></span>|<span data-ttu-id="9bcd2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9bcd2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bcd2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9bcd2-127">Request body</span></span>
<span data-ttu-id="9bcd2-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsDeviceStartupHistory.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupHistory object.</span></span>

<span data-ttu-id="9bcd2-129">В следующей таблице показаны свойства, необходимые при создании пользователяExperienceAnalyticsDeviceStartupHistory.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupHistory.</span></span>

|<span data-ttu-id="9bcd2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bcd2-130">Property</span></span>|<span data-ttu-id="9bcd2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9bcd2-131">Type</span></span>|<span data-ttu-id="9bcd2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9bcd2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bcd2-133">id</span><span class="sxs-lookup"><span data-stu-id="9bcd2-133">id</span></span>|<span data-ttu-id="9bcd2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9bcd2-134">String</span></span>|<span data-ttu-id="9bcd2-135">Уникальный идентификатор истории запуска устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-135">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="9bcd2-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="9bcd2-136">deviceId</span></span>|<span data-ttu-id="9bcd2-137">String</span><span class="sxs-lookup"><span data-stu-id="9bcd2-137">String</span></span>|<span data-ttu-id="9bcd2-138">ID устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="9bcd2-139">startTime</span><span class="sxs-lookup"><span data-stu-id="9bcd2-139">startTime</span></span>|<span data-ttu-id="9bcd2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bcd2-140">DateTimeOffset</span></span>|<span data-ttu-id="9bcd2-141">Время запуска загрузки устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-141">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="9bcd2-142">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9bcd2-142">coreBootTimeInMs</span></span>|<span data-ttu-id="9bcd2-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9bcd2-143">Int32</span></span>|<span data-ttu-id="9bcd2-144">Основное время загрузки устройства для аналитики пользовательского интерфейса в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-144">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="9bcd2-145">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9bcd2-145">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="9bcd2-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9bcd2-146">Int32</span></span>|<span data-ttu-id="9bcd2-147">Время загрузки групповой политики пользовательского интерфейса устройства в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-147">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="9bcd2-148">featureUpdateBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9bcd2-148">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="9bcd2-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9bcd2-149">Int32</span></span>|<span data-ttu-id="9bcd2-150">Время обновления устройства аналитики пользовательского интерфейса в миллисекундном периоде.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-150">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="9bcd2-151">totalBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9bcd2-151">totalBootTimeInMs</span></span>|<span data-ttu-id="9bcd2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9bcd2-152">Int32</span></span>|<span data-ttu-id="9bcd2-153">Общее время загрузки устройства аналитики пользовательского интерфейса в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-153">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="9bcd2-154">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9bcd2-154">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="9bcd2-155">Int32</span><span class="sxs-lookup"><span data-stu-id="9bcd2-155">Int32</span></span>|<span data-ttu-id="9bcd2-156">Время входа в группу политик пользовательского интерфейса для аналитики устройств в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-156">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="9bcd2-157">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9bcd2-157">coreLoginTimeInMs</span></span>|<span data-ttu-id="9bcd2-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9bcd2-158">Int32</span></span>|<span data-ttu-id="9bcd2-159">Время входа основного устройства для аналитики пользовательского интерфейса в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-159">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="9bcd2-160">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9bcd2-160">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="9bcd2-161">Int32</span><span class="sxs-lookup"><span data-stu-id="9bcd2-161">Int32</span></span>|<span data-ttu-id="9bcd2-162">Аналитика пользовательского интерфейса реагирует на время рабочего стола в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-162">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="9bcd2-163">totalLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9bcd2-163">totalLoginTimeInMs</span></span>|<span data-ttu-id="9bcd2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9bcd2-164">Int32</span></span>|<span data-ttu-id="9bcd2-165">Общее время входа устройства аналитики пользовательского интерфейса в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-165">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="9bcd2-166">isFirstLogin</span><span class="sxs-lookup"><span data-stu-id="9bcd2-166">isFirstLogin</span></span>|<span data-ttu-id="9bcd2-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bcd2-167">Boolean</span></span>|<span data-ttu-id="9bcd2-168">Устройство аналитики пользовательского интерфейса сначала входит в систему.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-168">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="9bcd2-169">isFeatureUpdate</span><span class="sxs-lookup"><span data-stu-id="9bcd2-169">isFeatureUpdate</span></span>|<span data-ttu-id="9bcd2-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bcd2-170">Boolean</span></span>|<span data-ttu-id="9bcd2-171">Запись загрузки устройства для аналитики пользовательского интерфейса — это обновление функций.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-171">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="9bcd2-172">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="9bcd2-172">operatingSystemVersion</span></span>|<span data-ttu-id="9bcd2-173">String</span><span class="sxs-lookup"><span data-stu-id="9bcd2-173">String</span></span>|<span data-ttu-id="9bcd2-174">Версия операционной системы записи операционной системы для аналитики пользовательского интерфейса устройства.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-174">The user experience analytics device boot record's operating system version.</span></span>|
|<span data-ttu-id="9bcd2-175">restartCategory</span><span class="sxs-lookup"><span data-stu-id="9bcd2-175">restartCategory</span></span>|[<span data-ttu-id="9bcd2-176">userExperienceAnalyticsOperatingSystemRestartCategory</span><span class="sxs-lookup"><span data-stu-id="9bcd2-176">userExperienceAnalyticsOperatingSystemRestartCategory</span></span>](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|<span data-ttu-id="9bcd2-177">Категория перезапуска ОС.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-177">OS restart category.</span></span> <span data-ttu-id="9bcd2-178">Возможные значения: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-178">Possible values are: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.</span></span>|
|<span data-ttu-id="9bcd2-179">restartStopCode</span><span class="sxs-lookup"><span data-stu-id="9bcd2-179">restartStopCode</span></span>|<span data-ttu-id="9bcd2-180">Строка</span><span class="sxs-lookup"><span data-stu-id="9bcd2-180">String</span></span>|<span data-ttu-id="9bcd2-181">Код остановки перезапуска ОС.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-181">OS restart stop code.</span></span> <span data-ttu-id="9bcd2-182">Здесь показан код проверки ошибок, который можно использовать для проверки причины синего экрана.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-182">This shows the bug check code which can be used to look up the blue screen reason.</span></span>|
|<span data-ttu-id="9bcd2-183">restartFaultBucket</span><span class="sxs-lookup"><span data-stu-id="9bcd2-183">restartFaultBucket</span></span>|<span data-ttu-id="9bcd2-184">Строка</span><span class="sxs-lookup"><span data-stu-id="9bcd2-184">String</span></span>|<span data-ttu-id="9bcd2-185">Ковш перезапуска неисправности ОС.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-185">OS restart fault bucket.</span></span> <span data-ttu-id="9bcd2-186">Ведро неисправностей используется для поиска дополнительных сведений о сбое системы.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-186">The fault bucket is used to find additional information about a system crash.</span></span>|



## <a name="response"></a><span data-ttu-id="9bcd2-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bcd2-187">Response</span></span>
<span data-ttu-id="9bcd2-188">В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-188">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bcd2-189">Пример</span><span class="sxs-lookup"><span data-stu-id="9bcd2-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bcd2-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bcd2-190">Request</span></span>
<span data-ttu-id="9bcd2-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-191">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
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

### <a name="response"></a><span data-ttu-id="9bcd2-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bcd2-192">Response</span></span>
<span data-ttu-id="9bcd2-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9bcd2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




