---
title: Создание Девицеманажементаутопилотевент
description: Создание нового объекта Девицеманажементаутопилотевент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d71b7d55ae550ea28f32ec5be2cc736c61697a3a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201111"
---
# <a name="create-devicemanagementautopilotevent"></a><span data-ttu-id="2c607-103">Создание Девицеманажементаутопилотевент</span><span class="sxs-lookup"><span data-stu-id="2c607-103">Create deviceManagementAutopilotEvent</span></span>

> <span data-ttu-id="2c607-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c607-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c607-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c607-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c607-106">Создание нового объекта [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="2c607-106">Create a new [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c607-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2c607-107">Prerequisites</span></span>
<span data-ttu-id="2c607-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c607-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c607-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c607-110">Permission type</span></span>|<span data-ttu-id="2c607-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c607-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c607-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c607-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c607-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c607-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2c607-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c607-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c607-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c607-115">Not supported.</span></span>|
|<span data-ttu-id="2c607-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c607-116">Application</span></span>|<span data-ttu-id="2c607-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c607-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c607-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c607-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="2c607-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c607-119">Request headers</span></span>
|<span data-ttu-id="2c607-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c607-120">Header</span></span>|<span data-ttu-id="2c607-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2c607-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c607-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c607-122">Authorization</span></span>|<span data-ttu-id="2c607-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c607-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c607-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2c607-124">Accept</span></span>|<span data-ttu-id="2c607-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2c607-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c607-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c607-126">Request body</span></span>
<span data-ttu-id="2c607-127">В тексте запроса добавьте представление объекта Девицеманажементаутопилотевент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c607-127">In the request body, supply a JSON representation for the deviceManagementAutopilotEvent object.</span></span>

<span data-ttu-id="2c607-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементаутопилотевент.</span><span class="sxs-lookup"><span data-stu-id="2c607-128">The following table shows the properties that are required when you create the deviceManagementAutopilotEvent.</span></span>

|<span data-ttu-id="2c607-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c607-129">Property</span></span>|<span data-ttu-id="2c607-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2c607-130">Type</span></span>|<span data-ttu-id="2c607-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2c607-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c607-132">id</span><span class="sxs-lookup"><span data-stu-id="2c607-132">id</span></span>|<span data-ttu-id="2c607-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2c607-133">String</span></span>|<span data-ttu-id="2c607-134">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="2c607-134">UUID for the object</span></span>|
|<span data-ttu-id="2c607-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="2c607-135">eventDateTime</span></span>|<span data-ttu-id="2c607-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c607-136">DateTimeOffset</span></span>|<span data-ttu-id="2c607-137">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="2c607-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="2c607-138">девицерегистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="2c607-138">deviceRegisteredDateTime</span></span>|<span data-ttu-id="2c607-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c607-139">DateTimeOffset</span></span>|<span data-ttu-id="2c607-140">Дата регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="2c607-140">Device registration date.</span></span>|
|<span data-ttu-id="2c607-141">енроллментстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="2c607-141">enrollmentStartDateTime</span></span>|<span data-ttu-id="2c607-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c607-142">DateTimeOffset</span></span>|<span data-ttu-id="2c607-143">Дата начала регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="2c607-143">Device enrollment start date.</span></span>|
|<span data-ttu-id="2c607-144">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="2c607-144">enrollmentType</span></span>|[<span data-ttu-id="2c607-145">виндовсаутопилотенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="2c607-145">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="2c607-146">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="2c607-146">Enrollment type.</span></span> <span data-ttu-id="2c607-147">Возможные значения: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span><span class="sxs-lookup"><span data-stu-id="2c607-147">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="2c607-148">девицесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="2c607-148">deviceSerialNumber</span></span>|<span data-ttu-id="2c607-149">String.</span><span class="sxs-lookup"><span data-stu-id="2c607-149">String</span></span>|<span data-ttu-id="2c607-150">Серийный номер устройства.</span><span class="sxs-lookup"><span data-stu-id="2c607-150">Device serial number.</span></span>|
|<span data-ttu-id="2c607-151">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="2c607-151">managedDeviceName</span></span>|<span data-ttu-id="2c607-152">String</span><span class="sxs-lookup"><span data-stu-id="2c607-152">String</span></span>|<span data-ttu-id="2c607-153">Управляемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="2c607-153">Managed device name.</span></span>|
|<span data-ttu-id="2c607-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2c607-154">userPrincipalName</span></span>|<span data-ttu-id="2c607-155">String</span><span class="sxs-lookup"><span data-stu-id="2c607-155">String</span></span>|<span data-ttu-id="2c607-156">Имя участника пользователя, используемое для регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="2c607-156">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="2c607-157">виндовсаутопилотдеплойментпрофиледисплайнаме</span><span class="sxs-lookup"><span data-stu-id="2c607-157">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="2c607-158">String.</span><span class="sxs-lookup"><span data-stu-id="2c607-158">String</span></span>|<span data-ttu-id="2c607-159">Имя профиля для автопилота.</span><span class="sxs-lookup"><span data-stu-id="2c607-159">Autopilot profile name.</span></span>|
|<span data-ttu-id="2c607-160">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="2c607-160">enrollmentState</span></span>|[<span data-ttu-id="2c607-161">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="2c607-161">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="2c607-162">Не удалось зарегистрировать состояние регистрации, например "зарегистрировано".</span><span class="sxs-lookup"><span data-stu-id="2c607-162">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="2c607-163">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="2c607-163">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="2c607-164">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="2c607-164">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="2c607-165">String.</span><span class="sxs-lookup"><span data-stu-id="2c607-165">String</span></span>|<span data-ttu-id="2c607-166">Имя профиля страницы состояния регистрации</span><span class="sxs-lookup"><span data-stu-id="2c607-166">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="2c607-167">деплойментстате</span><span class="sxs-lookup"><span data-stu-id="2c607-167">deploymentState</span></span>|[<span data-ttu-id="2c607-168">виндовсаутопилотдеплойментстате</span><span class="sxs-lookup"><span data-stu-id="2c607-168">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="2c607-169">Состояние развертывания, например успешное выполнение, сбой, выполнение, Сукцессвистимеаут.</span><span class="sxs-lookup"><span data-stu-id="2c607-169">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="2c607-170">Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span><span class="sxs-lookup"><span data-stu-id="2c607-170">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span></span>|
|<span data-ttu-id="2c607-171">osVersion</span><span class="sxs-lookup"><span data-stu-id="2c607-171">osVersion</span></span>|<span data-ttu-id="2c607-172">String.</span><span class="sxs-lookup"><span data-stu-id="2c607-172">String</span></span>|<span data-ttu-id="2c607-173">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="2c607-173">Device operating system version.</span></span>|
|<span data-ttu-id="2c607-174">деплойментдуратион</span><span class="sxs-lookup"><span data-stu-id="2c607-174">deploymentDuration</span></span>|<span data-ttu-id="2c607-175">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="2c607-175">Duration</span></span>|<span data-ttu-id="2c607-176">Длительность развертывания с автопилотной версией, включая регистрацию.</span><span class="sxs-lookup"><span data-stu-id="2c607-176">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="2c607-177">деплойменттоталдуратион</span><span class="sxs-lookup"><span data-stu-id="2c607-177">deploymentTotalDuration</span></span>|<span data-ttu-id="2c607-178">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="2c607-178">Duration</span></span>|<span data-ttu-id="2c607-179">Общее время развертывания с экрана регистрации на рабочем столе.</span><span class="sxs-lookup"><span data-stu-id="2c607-179">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="2c607-180">девицепрепаратиондуратион</span><span class="sxs-lookup"><span data-stu-id="2c607-180">devicePreparationDuration</span></span>|<span data-ttu-id="2c607-181">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="2c607-181">Duration</span></span>|<span data-ttu-id="2c607-182">Время, затраченное на регистрацию устройств.</span><span class="sxs-lookup"><span data-stu-id="2c607-182">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="2c607-183">девицесетупдуратион</span><span class="sxs-lookup"><span data-stu-id="2c607-183">deviceSetupDuration</span></span>|<span data-ttu-id="2c607-184">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="2c607-184">Duration</span></span>|<span data-ttu-id="2c607-185">Время, затраченное на устройство ESP.</span><span class="sxs-lookup"><span data-stu-id="2c607-185">Time spent in device ESP.</span></span>|
|<span data-ttu-id="2c607-186">аккаунтсетупдуратион</span><span class="sxs-lookup"><span data-stu-id="2c607-186">accountSetupDuration</span></span>|<span data-ttu-id="2c607-187">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="2c607-187">Duration</span></span>|<span data-ttu-id="2c607-188">Время, затраченное на ESP пользователем.</span><span class="sxs-lookup"><span data-stu-id="2c607-188">Time spent in user ESP.</span></span>|
|<span data-ttu-id="2c607-189">деплойментстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="2c607-189">deploymentStartDateTime</span></span>|<span data-ttu-id="2c607-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c607-190">DateTimeOffset</span></span>|<span data-ttu-id="2c607-191">Время начала развертывания.</span><span class="sxs-lookup"><span data-stu-id="2c607-191">Deployment start time.</span></span>|
|<span data-ttu-id="2c607-192">деплойментенддатетиме</span><span class="sxs-lookup"><span data-stu-id="2c607-192">deploymentEndDateTime</span></span>|<span data-ttu-id="2c607-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c607-193">DateTimeOffset</span></span>|<span data-ttu-id="2c607-194">Время окончания развертывания.</span><span class="sxs-lookup"><span data-stu-id="2c607-194">Deployment end time.</span></span>|
|<span data-ttu-id="2c607-195">таржетедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="2c607-195">targetedAppCount</span></span>|<span data-ttu-id="2c607-196">Int32</span><span class="sxs-lookup"><span data-stu-id="2c607-196">Int32</span></span>|<span data-ttu-id="2c607-197">Количество целевых приложений.</span><span class="sxs-lookup"><span data-stu-id="2c607-197">Count of applications targeted.</span></span>|
|<span data-ttu-id="2c607-198">таржетедполицикаунт</span><span class="sxs-lookup"><span data-stu-id="2c607-198">targetedPolicyCount</span></span>|<span data-ttu-id="2c607-199">Int32</span><span class="sxs-lookup"><span data-stu-id="2c607-199">Int32</span></span>|<span data-ttu-id="2c607-200">Количество целевых политик.</span><span class="sxs-lookup"><span data-stu-id="2c607-200">Count of policies targeted.</span></span>|
|<span data-ttu-id="2c607-201">енроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="2c607-201">enrollmentFailureDetails</span></span>|<span data-ttu-id="2c607-202">String.</span><span class="sxs-lookup"><span data-stu-id="2c607-202">String</span></span>|<span data-ttu-id="2c607-203">Сведения о сбоях при регистрации.</span><span class="sxs-lookup"><span data-stu-id="2c607-203">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="2c607-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c607-204">Response</span></span>
<span data-ttu-id="2c607-205">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2c607-205">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c607-206">Пример</span><span class="sxs-lookup"><span data-stu-id="2c607-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c607-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c607-207">Request</span></span>
<span data-ttu-id="2c607-208">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c607-208">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
Content-type: application/json
Content-length: 1323

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
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

### <a name="response"></a><span data-ttu-id="2c607-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c607-209">Response</span></span>
<span data-ttu-id="2c607-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c607-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1372

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "3e455cab-5cab-3e45-ab5c-453eab5c453e",
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




