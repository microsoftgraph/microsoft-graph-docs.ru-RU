---
title: Создание userExperienceAnalyticsDevicePerformance
description: Создание нового объекта userExperienceAnalyticsDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc40612bd3aa5a2d7452eaa1d3f9535d73191205
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154233"
---
# <a name="create-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="664db-103">Создание userExperienceAnalyticsDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="664db-103">Create userExperienceAnalyticsDevicePerformance</span></span>

<span data-ttu-id="664db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="664db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="664db-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="664db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="664db-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="664db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="664db-107">Создание нового [объекта userExperienceAnalyticsDevicePerformance.](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="664db-107">Create a new [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="664db-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="664db-108">Prerequisites</span></span>
<span data-ttu-id="664db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="664db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="664db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="664db-111">Permission type</span></span>|<span data-ttu-id="664db-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="664db-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="664db-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="664db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="664db-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="664db-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="664db-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="664db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="664db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="664db-116">Not supported.</span></span>|
|<span data-ttu-id="664db-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="664db-117">Application</span></span>|<span data-ttu-id="664db-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="664db-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="664db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="664db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="664db-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="664db-120">Request headers</span></span>
|<span data-ttu-id="664db-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="664db-121">Header</span></span>|<span data-ttu-id="664db-122">Значение</span><span class="sxs-lookup"><span data-stu-id="664db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="664db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="664db-123">Authorization</span></span>|<span data-ttu-id="664db-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="664db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="664db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="664db-125">Accept</span></span>|<span data-ttu-id="664db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="664db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="664db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="664db-127">Request body</span></span>
<span data-ttu-id="664db-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsDevicePerformance.</span><span class="sxs-lookup"><span data-stu-id="664db-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDevicePerformance object.</span></span>

<span data-ttu-id="664db-129">В следующей таблице показаны свойства, необходимые при создании пользователяExperienceAnalyticsDevicePerformance.</span><span class="sxs-lookup"><span data-stu-id="664db-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDevicePerformance.</span></span>

|<span data-ttu-id="664db-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="664db-130">Property</span></span>|<span data-ttu-id="664db-131">Тип</span><span class="sxs-lookup"><span data-stu-id="664db-131">Type</span></span>|<span data-ttu-id="664db-132">Описание</span><span class="sxs-lookup"><span data-stu-id="664db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="664db-133">id</span><span class="sxs-lookup"><span data-stu-id="664db-133">id</span></span>|<span data-ttu-id="664db-134">Строка</span><span class="sxs-lookup"><span data-stu-id="664db-134">String</span></span>|<span data-ttu-id="664db-135">Уникальный идентификатор устройства загрузки загрузочного устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="664db-135">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="664db-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="664db-136">deviceName</span></span>|<span data-ttu-id="664db-137">String</span><span class="sxs-lookup"><span data-stu-id="664db-137">String</span></span>|<span data-ttu-id="664db-138">Имя устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="664db-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="664db-139">model</span><span class="sxs-lookup"><span data-stu-id="664db-139">model</span></span>|<span data-ttu-id="664db-140">String</span><span class="sxs-lookup"><span data-stu-id="664db-140">String</span></span>|<span data-ttu-id="664db-141">Модель устройства аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="664db-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="664db-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="664db-142">manufacturer</span></span>|<span data-ttu-id="664db-143">String</span><span class="sxs-lookup"><span data-stu-id="664db-143">String</span></span>|<span data-ttu-id="664db-144">Производитель устройств аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="664db-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="664db-145">diskType</span><span class="sxs-lookup"><span data-stu-id="664db-145">diskType</span></span>|[<span data-ttu-id="664db-146">diskType</span><span class="sxs-lookup"><span data-stu-id="664db-146">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="664db-147">Тип диска для аналитики пользовательского интерфейса устройства.</span><span class="sxs-lookup"><span data-stu-id="664db-147">The user experience analytics device disk type.</span></span> <span data-ttu-id="664db-148">Возможные значения: `unkown`, `hdd`, `ssd`.</span><span class="sxs-lookup"><span data-stu-id="664db-148">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="664db-149">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="664db-149">operatingSystemVersion</span></span>|<span data-ttu-id="664db-150">String</span><span class="sxs-lookup"><span data-stu-id="664db-150">String</span></span>|<span data-ttu-id="664db-151">Версия операционной системы для аналитики пользовательского интерфейса устройства.</span><span class="sxs-lookup"><span data-stu-id="664db-151">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="664db-152">bootScore</span><span class="sxs-lookup"><span data-stu-id="664db-152">bootScore</span></span>|<span data-ttu-id="664db-153">Int32</span><span class="sxs-lookup"><span data-stu-id="664db-153">Int32</span></span>|<span data-ttu-id="664db-154">Оценка загрузки устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="664db-154">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="664db-155">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="664db-155">coreBootTimeInMs</span></span>|<span data-ttu-id="664db-156">Int32</span><span class="sxs-lookup"><span data-stu-id="664db-156">Int32</span></span>|<span data-ttu-id="664db-157">Основное время загрузки устройства для аналитики пользовательского интерфейса в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="664db-157">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="664db-158">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="664db-158">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="664db-159">Int32</span><span class="sxs-lookup"><span data-stu-id="664db-159">Int32</span></span>|<span data-ttu-id="664db-160">Время загрузки групповой политики устройств для пользовательского интерфейса в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="664db-160">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="664db-161">healthStatus</span><span class="sxs-lookup"><span data-stu-id="664db-161">healthStatus</span></span>|[<span data-ttu-id="664db-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="664db-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="664db-163">Состояние здоровья устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="664db-163">The health state of the user experience analytics device.</span></span> <span data-ttu-id="664db-164">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="664db-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="664db-165">loginScore</span><span class="sxs-lookup"><span data-stu-id="664db-165">loginScore</span></span>|<span data-ttu-id="664db-166">Int32</span><span class="sxs-lookup"><span data-stu-id="664db-166">Int32</span></span>|<span data-ttu-id="664db-167">Оценка входа устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="664db-167">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="664db-168">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="664db-168">coreLoginTimeInMs</span></span>|<span data-ttu-id="664db-169">Int32</span><span class="sxs-lookup"><span data-stu-id="664db-169">Int32</span></span>|<span data-ttu-id="664db-170">Время входа основного устройства для аналитики пользовательского интерфейса в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="664db-170">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="664db-171">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="664db-171">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="664db-172">Int32</span><span class="sxs-lookup"><span data-stu-id="664db-172">Int32</span></span>|<span data-ttu-id="664db-173">Время входа в группу политик пользовательского интерфейса для аналитики устройств в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="664db-173">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="664db-174">deviceCount</span><span class="sxs-lookup"><span data-stu-id="664db-174">deviceCount</span></span>|<span data-ttu-id="664db-175">Int64</span><span class="sxs-lookup"><span data-stu-id="664db-175">Int64</span></span>|<span data-ttu-id="664db-176">Аналитика пользовательских интерфейсов суммирует количество устройств.</span><span class="sxs-lookup"><span data-stu-id="664db-176">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="664db-177">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="664db-177">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="664db-178">Int32</span><span class="sxs-lookup"><span data-stu-id="664db-178">Int32</span></span>|<span data-ttu-id="664db-179">Аналитика пользовательского интерфейса реагирует на время рабочего стола в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="664db-179">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="664db-180">blueScreenCount</span><span class="sxs-lookup"><span data-stu-id="664db-180">blueScreenCount</span></span>|<span data-ttu-id="664db-181">Int32</span><span class="sxs-lookup"><span data-stu-id="664db-181">Int32</span></span>|<span data-ttu-id="664db-182">Количество синих экранов за последние 14 дней.</span><span class="sxs-lookup"><span data-stu-id="664db-182">Number of Blue Screens in the last 14 days.</span></span> <span data-ttu-id="664db-183">Допустимые значения от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="664db-183">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="664db-184">restartCount</span><span class="sxs-lookup"><span data-stu-id="664db-184">restartCount</span></span>|<span data-ttu-id="664db-185">Int32</span><span class="sxs-lookup"><span data-stu-id="664db-185">Int32</span></span>|<span data-ttu-id="664db-186">Количество перезапусков за последние 14 дней.</span><span class="sxs-lookup"><span data-stu-id="664db-186">Number of Restarts in the last 14 days.</span></span> <span data-ttu-id="664db-187">Допустимые значения от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="664db-187">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="664db-188">averageBlueScreens</span><span class="sxs-lookup"><span data-stu-id="664db-188">averageBlueScreens</span></span>|<span data-ttu-id="664db-189">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="664db-189">Double</span></span>|<span data-ttu-id="664db-190">Среднее (среднее) число синих экранов на устройство за последние 14 дней.</span><span class="sxs-lookup"><span data-stu-id="664db-190">Average (mean) number of Blue Screens per device in the last 14 days.</span></span> <span data-ttu-id="664db-191">Допустимые значения от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="664db-191">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="664db-192">averageRestarts</span><span class="sxs-lookup"><span data-stu-id="664db-192">averageRestarts</span></span>|<span data-ttu-id="664db-193">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="664db-193">Double</span></span>|<span data-ttu-id="664db-194">Среднее (среднее) число перезапусков на устройство за последние 14 дней.</span><span class="sxs-lookup"><span data-stu-id="664db-194">Average (mean) number of Restarts per device in the last 14 days.</span></span> <span data-ttu-id="664db-195">Допустимые значения от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="664db-195">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="664db-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="664db-196">Response</span></span>
<span data-ttu-id="664db-197">В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="664db-197">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="664db-198">Пример</span><span class="sxs-lookup"><span data-stu-id="664db-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="664db-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="664db-199">Request</span></span>
<span data-ttu-id="664db-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="664db-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="664db-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="664db-201">Response</span></span>
<span data-ttu-id="664db-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="664db-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




