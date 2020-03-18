---
title: Создание Девицеманажементаутопилотевент
description: Создание нового объекта Девицеманажементаутопилотевент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e33ab0fc0b48284457785702d3591f462039505c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800265"
---
# <a name="create-devicemanagementautopilotevent"></a><span data-ttu-id="76614-103">Создание Девицеманажементаутопилотевент</span><span class="sxs-lookup"><span data-stu-id="76614-103">Create deviceManagementAutopilotEvent</span></span>

> <span data-ttu-id="76614-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76614-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76614-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76614-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76614-106">Создание нового объекта [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="76614-106">Create a new [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76614-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="76614-107">Prerequisites</span></span>
<span data-ttu-id="76614-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76614-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76614-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76614-110">Permission type</span></span>|<span data-ttu-id="76614-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="76614-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76614-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76614-112">Delegated (work or school account)</span></span>|<span data-ttu-id="76614-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76614-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="76614-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76614-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76614-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76614-115">Not supported.</span></span>|
|<span data-ttu-id="76614-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="76614-116">Application</span></span>|<span data-ttu-id="76614-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76614-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76614-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76614-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="76614-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="76614-119">Request headers</span></span>
|<span data-ttu-id="76614-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76614-120">Header</span></span>|<span data-ttu-id="76614-121">Значение</span><span class="sxs-lookup"><span data-stu-id="76614-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76614-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="76614-122">Authorization</span></span>|<span data-ttu-id="76614-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76614-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76614-124">Accept</span><span class="sxs-lookup"><span data-stu-id="76614-124">Accept</span></span>|<span data-ttu-id="76614-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76614-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76614-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76614-126">Request body</span></span>
<span data-ttu-id="76614-127">В тексте запроса добавьте представление объекта Девицеманажементаутопилотевент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76614-127">In the request body, supply a JSON representation for the deviceManagementAutopilotEvent object.</span></span>

<span data-ttu-id="76614-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементаутопилотевент.</span><span class="sxs-lookup"><span data-stu-id="76614-128">The following table shows the properties that are required when you create the deviceManagementAutopilotEvent.</span></span>

|<span data-ttu-id="76614-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="76614-129">Property</span></span>|<span data-ttu-id="76614-130">Тип</span><span class="sxs-lookup"><span data-stu-id="76614-130">Type</span></span>|<span data-ttu-id="76614-131">Описание</span><span class="sxs-lookup"><span data-stu-id="76614-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76614-132">id</span><span class="sxs-lookup"><span data-stu-id="76614-132">id</span></span>|<span data-ttu-id="76614-133">Строка</span><span class="sxs-lookup"><span data-stu-id="76614-133">String</span></span>|<span data-ttu-id="76614-134">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="76614-134">UUID for the object</span></span>|
|<span data-ttu-id="76614-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="76614-135">deviceId</span></span>|<span data-ttu-id="76614-136">String</span><span class="sxs-lookup"><span data-stu-id="76614-136">String</span></span>|<span data-ttu-id="76614-137">Идентификатор устройства, связанный с объектом</span><span class="sxs-lookup"><span data-stu-id="76614-137">Device id associated with the object</span></span>|
|<span data-ttu-id="76614-138">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="76614-138">eventDateTime</span></span>|<span data-ttu-id="76614-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76614-139">DateTimeOffset</span></span>|<span data-ttu-id="76614-140">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="76614-140">Time when the event occurred .</span></span>|
|<span data-ttu-id="76614-141">девицерегистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="76614-141">deviceRegisteredDateTime</span></span>|<span data-ttu-id="76614-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76614-142">DateTimeOffset</span></span>|<span data-ttu-id="76614-143">Дата регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="76614-143">Device registration date.</span></span>|
|<span data-ttu-id="76614-144">енроллментстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="76614-144">enrollmentStartDateTime</span></span>|<span data-ttu-id="76614-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76614-145">DateTimeOffset</span></span>|<span data-ttu-id="76614-146">Дата начала регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="76614-146">Device enrollment start date.</span></span>|
|<span data-ttu-id="76614-147">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="76614-147">enrollmentType</span></span>|[<span data-ttu-id="76614-148">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="76614-148">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="76614-149">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="76614-149">Enrollment type.</span></span> <span data-ttu-id="76614-150">Возможные значения: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span><span class="sxs-lookup"><span data-stu-id="76614-150">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="76614-151">девицесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="76614-151">deviceSerialNumber</span></span>|<span data-ttu-id="76614-152">String</span><span class="sxs-lookup"><span data-stu-id="76614-152">String</span></span>|<span data-ttu-id="76614-153">Серийный номер устройства.</span><span class="sxs-lookup"><span data-stu-id="76614-153">Device serial number.</span></span>|
|<span data-ttu-id="76614-154">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="76614-154">managedDeviceName</span></span>|<span data-ttu-id="76614-155">String</span><span class="sxs-lookup"><span data-stu-id="76614-155">String</span></span>|<span data-ttu-id="76614-156">Управляемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="76614-156">Managed device name.</span></span>|
|<span data-ttu-id="76614-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="76614-157">userPrincipalName</span></span>|<span data-ttu-id="76614-158">String</span><span class="sxs-lookup"><span data-stu-id="76614-158">String</span></span>|<span data-ttu-id="76614-159">Имя участника пользователя, используемое для регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="76614-159">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="76614-160">виндовсаутопилотдеплойментпрофиледисплайнаме</span><span class="sxs-lookup"><span data-stu-id="76614-160">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="76614-161">String</span><span class="sxs-lookup"><span data-stu-id="76614-161">String</span></span>|<span data-ttu-id="76614-162">Имя профиля для автопилота.</span><span class="sxs-lookup"><span data-stu-id="76614-162">Autopilot profile name.</span></span>|
|<span data-ttu-id="76614-163">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="76614-163">enrollmentState</span></span>|[<span data-ttu-id="76614-164">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="76614-164">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="76614-165">Не удалось зарегистрировать состояние регистрации, например "зарегистрировано".</span><span class="sxs-lookup"><span data-stu-id="76614-165">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="76614-166">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="76614-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="76614-167">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="76614-167">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="76614-168">String</span><span class="sxs-lookup"><span data-stu-id="76614-168">String</span></span>|<span data-ttu-id="76614-169">Имя профиля страницы состояния регистрации</span><span class="sxs-lookup"><span data-stu-id="76614-169">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="76614-170">деплойментстате</span><span class="sxs-lookup"><span data-stu-id="76614-170">deploymentState</span></span>|[<span data-ttu-id="76614-171">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="76614-171">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="76614-172">Состояние развертывания, например успешное выполнение, сбой, выполнение, Сукцессвистимеаут.</span><span class="sxs-lookup"><span data-stu-id="76614-172">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="76614-173">Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span><span class="sxs-lookup"><span data-stu-id="76614-173">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span></span>|
|<span data-ttu-id="76614-174">osVersion</span><span class="sxs-lookup"><span data-stu-id="76614-174">osVersion</span></span>|<span data-ttu-id="76614-175">String</span><span class="sxs-lookup"><span data-stu-id="76614-175">String</span></span>|<span data-ttu-id="76614-176">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="76614-176">Device operating system version.</span></span>|
|<span data-ttu-id="76614-177">деплойментдуратион</span><span class="sxs-lookup"><span data-stu-id="76614-177">deploymentDuration</span></span>|<span data-ttu-id="76614-178">Длительность</span><span class="sxs-lookup"><span data-stu-id="76614-178">Duration</span></span>|<span data-ttu-id="76614-179">Длительность развертывания с автопилотной версией, включая регистрацию.</span><span class="sxs-lookup"><span data-stu-id="76614-179">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="76614-180">деплойменттоталдуратион</span><span class="sxs-lookup"><span data-stu-id="76614-180">deploymentTotalDuration</span></span>|<span data-ttu-id="76614-181">Длительность</span><span class="sxs-lookup"><span data-stu-id="76614-181">Duration</span></span>|<span data-ttu-id="76614-182">Общее время развертывания с экрана регистрации на рабочем столе.</span><span class="sxs-lookup"><span data-stu-id="76614-182">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="76614-183">девицепрепаратиондуратион</span><span class="sxs-lookup"><span data-stu-id="76614-183">devicePreparationDuration</span></span>|<span data-ttu-id="76614-184">Длительность</span><span class="sxs-lookup"><span data-stu-id="76614-184">Duration</span></span>|<span data-ttu-id="76614-185">Время, затраченное на регистрацию устройств.</span><span class="sxs-lookup"><span data-stu-id="76614-185">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="76614-186">девицесетупдуратион</span><span class="sxs-lookup"><span data-stu-id="76614-186">deviceSetupDuration</span></span>|<span data-ttu-id="76614-187">Длительность</span><span class="sxs-lookup"><span data-stu-id="76614-187">Duration</span></span>|<span data-ttu-id="76614-188">Время, затраченное на устройство ESP.</span><span class="sxs-lookup"><span data-stu-id="76614-188">Time spent in device ESP.</span></span>|
|<span data-ttu-id="76614-189">аккаунтсетупдуратион</span><span class="sxs-lookup"><span data-stu-id="76614-189">accountSetupDuration</span></span>|<span data-ttu-id="76614-190">Длительность</span><span class="sxs-lookup"><span data-stu-id="76614-190">Duration</span></span>|<span data-ttu-id="76614-191">Время, затраченное на ESP пользователем.</span><span class="sxs-lookup"><span data-stu-id="76614-191">Time spent in user ESP.</span></span>|
|<span data-ttu-id="76614-192">деплойментстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="76614-192">deploymentStartDateTime</span></span>|<span data-ttu-id="76614-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76614-193">DateTimeOffset</span></span>|<span data-ttu-id="76614-194">Время начала развертывания.</span><span class="sxs-lookup"><span data-stu-id="76614-194">Deployment start time.</span></span>|
|<span data-ttu-id="76614-195">деплойментенддатетиме</span><span class="sxs-lookup"><span data-stu-id="76614-195">deploymentEndDateTime</span></span>|<span data-ttu-id="76614-196">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76614-196">DateTimeOffset</span></span>|<span data-ttu-id="76614-197">Время окончания развертывания.</span><span class="sxs-lookup"><span data-stu-id="76614-197">Deployment end time.</span></span>|
|<span data-ttu-id="76614-198">таржетедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="76614-198">targetedAppCount</span></span>|<span data-ttu-id="76614-199">Int32</span><span class="sxs-lookup"><span data-stu-id="76614-199">Int32</span></span>|<span data-ttu-id="76614-200">Количество целевых приложений.</span><span class="sxs-lookup"><span data-stu-id="76614-200">Count of applications targeted.</span></span>|
|<span data-ttu-id="76614-201">таржетедполицикаунт</span><span class="sxs-lookup"><span data-stu-id="76614-201">targetedPolicyCount</span></span>|<span data-ttu-id="76614-202">Int32</span><span class="sxs-lookup"><span data-stu-id="76614-202">Int32</span></span>|<span data-ttu-id="76614-203">Количество целевых политик.</span><span class="sxs-lookup"><span data-stu-id="76614-203">Count of policies targeted.</span></span>|
|<span data-ttu-id="76614-204">енроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="76614-204">enrollmentFailureDetails</span></span>|<span data-ttu-id="76614-205">String</span><span class="sxs-lookup"><span data-stu-id="76614-205">String</span></span>|<span data-ttu-id="76614-206">Сведения о сбоях при регистрации.</span><span class="sxs-lookup"><span data-stu-id="76614-206">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="76614-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="76614-207">Response</span></span>
<span data-ttu-id="76614-208">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="76614-208">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76614-209">Пример</span><span class="sxs-lookup"><span data-stu-id="76614-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="76614-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="76614-210">Request</span></span>
<span data-ttu-id="76614-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76614-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
Content-type: application/json
Content-length: 1357

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "deviceId": "Device Id value",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "deviceRegisteredDateTime": "2017-01-01T00:02:48.7185581-08:00",
  "enrollmentStartDateTime": "2017-01-01T00:00:19.6280481-08:00",
  "enrollmentType": "azureADJoinedWithAutopilotProfile",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "enrolled",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "deploymentState": "success",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT3M21.5549443S",
  "deploymentTotalDuration": "PT1M43.5284261S",
  "devicePreparationDuration": "-PT1M32.1347897S",
  "deviceSetupDuration": "-PT2M57.2190107S",
  "accountSetupDuration": "-PT2M32.0507894S",
  "deploymentStartDateTime": "2016-12-31T23:59:37.257201-08:00",
  "deploymentEndDateTime": "2017-01-01T00:00:46.5128291-08:00",
  "targetedAppCount": 0,
  "targetedPolicyCount": 3,
  "enrollmentFailureDetails": "Enrollment Failure Details value"
}
```

### <a name="response"></a><span data-ttu-id="76614-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="76614-212">Response</span></span>
<span data-ttu-id="76614-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76614-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1406

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "3e455cab-5cab-3e45-ab5c-453eab5c453e",
  "deviceId": "Device Id value",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "deviceRegisteredDateTime": "2017-01-01T00:02:48.7185581-08:00",
  "enrollmentStartDateTime": "2017-01-01T00:00:19.6280481-08:00",
  "enrollmentType": "azureADJoinedWithAutopilotProfile",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "enrolled",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "deploymentState": "success",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT3M21.5549443S",
  "deploymentTotalDuration": "PT1M43.5284261S",
  "devicePreparationDuration": "-PT1M32.1347897S",
  "deviceSetupDuration": "-PT2M57.2190107S",
  "accountSetupDuration": "-PT2M32.0507894S",
  "deploymentStartDateTime": "2016-12-31T23:59:37.257201-08:00",
  "deploymentEndDateTime": "2017-01-01T00:00:46.5128291-08:00",
  "targetedAppCount": 0,
  "targetedPolicyCount": 3,
  "enrollmentFailureDetails": "Enrollment Failure Details value"
}
```




