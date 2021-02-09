---
title: Обновление userExperienceAnalyticsDeviceStartupHistory
description: Обновление свойств объекта userExperienceAnalyticsDeviceStartupHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4bf2ddc2ad60d850ba1511c6a1a7339a48326ec2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159670"
---
# <a name="update-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="75395-103">Обновление userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="75395-103">Update userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="75395-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75395-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75395-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75395-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75395-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75395-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75395-107">Обновление свойств объекта [userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)</span><span class="sxs-lookup"><span data-stu-id="75395-107">Update the properties of a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75395-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="75395-108">Prerequisites</span></span>
<span data-ttu-id="75395-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75395-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75395-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75395-111">Permission type</span></span>|<span data-ttu-id="75395-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75395-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75395-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75395-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75395-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75395-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="75395-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75395-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75395-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75395-116">Not supported.</span></span>|
|<span data-ttu-id="75395-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75395-117">Application</span></span>|<span data-ttu-id="75395-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75395-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75395-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75395-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="75395-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="75395-120">Request headers</span></span>
|<span data-ttu-id="75395-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75395-121">Header</span></span>|<span data-ttu-id="75395-122">Значение</span><span class="sxs-lookup"><span data-stu-id="75395-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75395-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75395-123">Authorization</span></span>|<span data-ttu-id="75395-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75395-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75395-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75395-125">Accept</span></span>|<span data-ttu-id="75395-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75395-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75395-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75395-127">Request body</span></span>
<span data-ttu-id="75395-128">В теле запроса укажу представление объекта [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="75395-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

<span data-ttu-id="75395-129">В следующей таблице показаны свойства, необходимые при создании [объекта userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)</span><span class="sxs-lookup"><span data-stu-id="75395-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).</span></span>

|<span data-ttu-id="75395-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="75395-130">Property</span></span>|<span data-ttu-id="75395-131">Тип</span><span class="sxs-lookup"><span data-stu-id="75395-131">Type</span></span>|<span data-ttu-id="75395-132">Описание</span><span class="sxs-lookup"><span data-stu-id="75395-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75395-133">id</span><span class="sxs-lookup"><span data-stu-id="75395-133">id</span></span>|<span data-ttu-id="75395-134">String</span><span class="sxs-lookup"><span data-stu-id="75395-134">String</span></span>|<span data-ttu-id="75395-135">Уникальный идентификатор истории запуска устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="75395-135">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="75395-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="75395-136">deviceId</span></span>|<span data-ttu-id="75395-137">String</span><span class="sxs-lookup"><span data-stu-id="75395-137">String</span></span>|<span data-ttu-id="75395-138">ИД устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="75395-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="75395-139">startTime</span><span class="sxs-lookup"><span data-stu-id="75395-139">startTime</span></span>|<span data-ttu-id="75395-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75395-140">DateTimeOffset</span></span>|<span data-ttu-id="75395-141">Время начала загрузки устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="75395-141">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="75395-142">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="75395-142">coreBootTimeInMs</span></span>|<span data-ttu-id="75395-143">Int32</span><span class="sxs-lookup"><span data-stu-id="75395-143">Int32</span></span>|<span data-ttu-id="75395-144">Время загрузки основного устройства аналитики пользовательского интерфейса в миллисекунах.</span><span class="sxs-lookup"><span data-stu-id="75395-144">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="75395-145">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="75395-145">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="75395-146">Int32</span><span class="sxs-lookup"><span data-stu-id="75395-146">Int32</span></span>|<span data-ttu-id="75395-147">Время загрузки групповой политики устройства аналитики пользовательского интерфейса в миллисекунах.</span><span class="sxs-lookup"><span data-stu-id="75395-147">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="75395-148">featureUpdateBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="75395-148">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="75395-149">Int32</span><span class="sxs-lookup"><span data-stu-id="75395-149">Int32</span></span>|<span data-ttu-id="75395-150">Время обновления функции устройства аналитики пользовательского интерфейса в миллисекунах.</span><span class="sxs-lookup"><span data-stu-id="75395-150">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="75395-151">totalBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="75395-151">totalBootTimeInMs</span></span>|<span data-ttu-id="75395-152">Int32</span><span class="sxs-lookup"><span data-stu-id="75395-152">Int32</span></span>|<span data-ttu-id="75395-153">Общее время загрузки устройства аналитики пользовательского интерфейса в миллисекунах.</span><span class="sxs-lookup"><span data-stu-id="75395-153">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="75395-154">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="75395-154">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="75395-155">Int32</span><span class="sxs-lookup"><span data-stu-id="75395-155">Int32</span></span>|<span data-ttu-id="75395-156">Время входа в групповую политику устройства аналитики пользовательского интерфейса (в миллисекунах).</span><span class="sxs-lookup"><span data-stu-id="75395-156">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="75395-157">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="75395-157">coreLoginTimeInMs</span></span>|<span data-ttu-id="75395-158">Int32</span><span class="sxs-lookup"><span data-stu-id="75395-158">Int32</span></span>|<span data-ttu-id="75395-159">Время входа в систему устройства аналитики пользовательского интерфейса в миллисекунах.</span><span class="sxs-lookup"><span data-stu-id="75395-159">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="75395-160">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="75395-160">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="75395-161">Int32</span><span class="sxs-lookup"><span data-stu-id="75395-161">Int32</span></span>|<span data-ttu-id="75395-162">Аналитика пользовательского интерфейса отвечает за время рабочего стола в миллисекунах.</span><span class="sxs-lookup"><span data-stu-id="75395-162">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="75395-163">totalLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="75395-163">totalLoginTimeInMs</span></span>|<span data-ttu-id="75395-164">Int32</span><span class="sxs-lookup"><span data-stu-id="75395-164">Int32</span></span>|<span data-ttu-id="75395-165">Общее время входа устройства аналитики пользовательского интерфейса в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="75395-165">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="75395-166">isFirstLogin</span><span class="sxs-lookup"><span data-stu-id="75395-166">isFirstLogin</span></span>|<span data-ttu-id="75395-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="75395-167">Boolean</span></span>|<span data-ttu-id="75395-168">Устройство аналитики пользовательского интерфейса сначала входит в систему.</span><span class="sxs-lookup"><span data-stu-id="75395-168">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="75395-169">isFeatureUpdate</span><span class="sxs-lookup"><span data-stu-id="75395-169">isFeatureUpdate</span></span>|<span data-ttu-id="75395-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="75395-170">Boolean</span></span>|<span data-ttu-id="75395-171">Запись загрузки устройства аналитики пользовательского интерфейса является обновлением функций.</span><span class="sxs-lookup"><span data-stu-id="75395-171">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="75395-172">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="75395-172">operatingSystemVersion</span></span>|<span data-ttu-id="75395-173">String</span><span class="sxs-lookup"><span data-stu-id="75395-173">String</span></span>|<span data-ttu-id="75395-174">Версия операционной системы записи загрузки устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="75395-174">The user experience analytics device boot record's operating system version.</span></span>|
|<span data-ttu-id="75395-175">restartCategory</span><span class="sxs-lookup"><span data-stu-id="75395-175">restartCategory</span></span>|[<span data-ttu-id="75395-176">userExperienceAnalyticsOperatingSystemRestartCategory</span><span class="sxs-lookup"><span data-stu-id="75395-176">userExperienceAnalyticsOperatingSystemRestartCategory</span></span>](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|<span data-ttu-id="75395-177">Категория перезапуска ОС.</span><span class="sxs-lookup"><span data-stu-id="75395-177">OS restart category.</span></span> <span data-ttu-id="75395-178">Возможные значения: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.</span><span class="sxs-lookup"><span data-stu-id="75395-178">Possible values are: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.</span></span>|
|<span data-ttu-id="75395-179">restartStopCode</span><span class="sxs-lookup"><span data-stu-id="75395-179">restartStopCode</span></span>|<span data-ttu-id="75395-180">String</span><span class="sxs-lookup"><span data-stu-id="75395-180">String</span></span>|<span data-ttu-id="75395-181">Код остановки перезапуска ОС.</span><span class="sxs-lookup"><span data-stu-id="75395-181">OS restart stop code.</span></span> <span data-ttu-id="75395-182">Здесь показан код проверки ошибок, который можно использовать для отслеживания причины синего экрана.</span><span class="sxs-lookup"><span data-stu-id="75395-182">This shows the bug check code which can be used to look up the blue screen reason.</span></span>|
|<span data-ttu-id="75395-183">restartFaultBucket</span><span class="sxs-lookup"><span data-stu-id="75395-183">restartFaultBucket</span></span>|<span data-ttu-id="75395-184">String</span><span class="sxs-lookup"><span data-stu-id="75395-184">String</span></span>|<span data-ttu-id="75395-185">Сегмент сбоя перезапуска ОС.</span><span class="sxs-lookup"><span data-stu-id="75395-185">OS restart fault bucket.</span></span> <span data-ttu-id="75395-186">Сегмент сбоя используется для поиска дополнительных сведений о сбое системы.</span><span class="sxs-lookup"><span data-stu-id="75395-186">The fault bucket is used to find additional information about a system crash.</span></span>|



## <a name="response"></a><span data-ttu-id="75395-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="75395-187">Response</span></span>
<span data-ttu-id="75395-188">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75395-188">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75395-189">Пример</span><span class="sxs-lookup"><span data-stu-id="75395-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="75395-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="75395-190">Request</span></span>
<span data-ttu-id="75395-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75395-191">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="75395-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="75395-192">Response</span></span>
<span data-ttu-id="75395-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75395-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




