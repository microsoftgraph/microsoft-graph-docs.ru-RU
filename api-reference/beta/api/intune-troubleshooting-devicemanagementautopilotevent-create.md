---
title: Создание Девицеманажементаутопилотевент
description: Создание нового объекта Девицеманажементаутопилотевент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8fc6a38851497e68861a788083c23fd9936e9fe7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457743"
---
# <a name="create-devicemanagementautopilotevent"></a><span data-ttu-id="b2cbd-103">Создание Девицеманажементаутопилотевент</span><span class="sxs-lookup"><span data-stu-id="b2cbd-103">Create deviceManagementAutopilotEvent</span></span>

<span data-ttu-id="b2cbd-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b2cbd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2cbd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2cbd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2cbd-107">Создание нового объекта [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="b2cbd-107">Create a new [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2cbd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b2cbd-108">Prerequisites</span></span>
<span data-ttu-id="b2cbd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2cbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2cbd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2cbd-111">Permission type</span></span>|<span data-ttu-id="b2cbd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2cbd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2cbd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2cbd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2cbd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2cbd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b2cbd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2cbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2cbd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-116">Not supported.</span></span>|
|<span data-ttu-id="b2cbd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2cbd-117">Application</span></span>|<span data-ttu-id="b2cbd-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2cbd-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2cbd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2cbd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="b2cbd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b2cbd-120">Request headers</span></span>
|<span data-ttu-id="b2cbd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2cbd-121">Header</span></span>|<span data-ttu-id="b2cbd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b2cbd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2cbd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2cbd-123">Authorization</span></span>|<span data-ttu-id="b2cbd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2cbd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b2cbd-125">Accept</span></span>|<span data-ttu-id="b2cbd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2cbd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2cbd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2cbd-127">Request body</span></span>
<span data-ttu-id="b2cbd-128">В тексте запроса добавьте представление объекта Девицеманажементаутопилотевент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-128">In the request body, supply a JSON representation for the deviceManagementAutopilotEvent object.</span></span>

<span data-ttu-id="b2cbd-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементаутопилотевент.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-129">The following table shows the properties that are required when you create the deviceManagementAutopilotEvent.</span></span>

|<span data-ttu-id="b2cbd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2cbd-130">Property</span></span>|<span data-ttu-id="b2cbd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b2cbd-131">Type</span></span>|<span data-ttu-id="b2cbd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b2cbd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2cbd-133">id</span><span class="sxs-lookup"><span data-stu-id="b2cbd-133">id</span></span>|<span data-ttu-id="b2cbd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b2cbd-134">String</span></span>|<span data-ttu-id="b2cbd-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-135">UUID for the object</span></span>|
|<span data-ttu-id="b2cbd-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="b2cbd-136">eventDateTime</span></span>|<span data-ttu-id="b2cbd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2cbd-137">DateTimeOffset</span></span>|<span data-ttu-id="b2cbd-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="b2cbd-139">девицерегистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="b2cbd-139">deviceRegisteredDateTime</span></span>|<span data-ttu-id="b2cbd-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2cbd-140">DateTimeOffset</span></span>|<span data-ttu-id="b2cbd-141">Дата регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-141">Device registration date.</span></span>|
|<span data-ttu-id="b2cbd-142">енроллментстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="b2cbd-142">enrollmentStartDateTime</span></span>|<span data-ttu-id="b2cbd-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2cbd-143">DateTimeOffset</span></span>|<span data-ttu-id="b2cbd-144">Дата начала регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-144">Device enrollment start date.</span></span>|
|<span data-ttu-id="b2cbd-145">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="b2cbd-145">enrollmentType</span></span>|[<span data-ttu-id="b2cbd-146">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="b2cbd-146">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="b2cbd-147">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-147">Enrollment type.</span></span> <span data-ttu-id="b2cbd-148">Возможные значения: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-148">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="b2cbd-149">девицесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="b2cbd-149">deviceSerialNumber</span></span>|<span data-ttu-id="b2cbd-150">String</span><span class="sxs-lookup"><span data-stu-id="b2cbd-150">String</span></span>|<span data-ttu-id="b2cbd-151">Серийный номер устройства.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-151">Device serial number.</span></span>|
|<span data-ttu-id="b2cbd-152">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="b2cbd-152">managedDeviceName</span></span>|<span data-ttu-id="b2cbd-153">String</span><span class="sxs-lookup"><span data-stu-id="b2cbd-153">String</span></span>|<span data-ttu-id="b2cbd-154">Управляемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-154">Managed device name.</span></span>|
|<span data-ttu-id="b2cbd-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b2cbd-155">userPrincipalName</span></span>|<span data-ttu-id="b2cbd-156">String</span><span class="sxs-lookup"><span data-stu-id="b2cbd-156">String</span></span>|<span data-ttu-id="b2cbd-157">Имя участника пользователя, используемое для регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-157">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="b2cbd-158">виндовсаутопилотдеплойментпрофиледисплайнаме</span><span class="sxs-lookup"><span data-stu-id="b2cbd-158">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="b2cbd-159">String</span><span class="sxs-lookup"><span data-stu-id="b2cbd-159">String</span></span>|<span data-ttu-id="b2cbd-160">Имя профиля для автопилота.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-160">Autopilot profile name.</span></span>|
|<span data-ttu-id="b2cbd-161">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="b2cbd-161">enrollmentState</span></span>|[<span data-ttu-id="b2cbd-162">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="b2cbd-162">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="b2cbd-163">Не удалось зарегистрировать состояние регистрации, например "зарегистрировано".</span><span class="sxs-lookup"><span data-stu-id="b2cbd-163">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="b2cbd-164">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-164">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="b2cbd-165">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="b2cbd-165">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="b2cbd-166">String</span><span class="sxs-lookup"><span data-stu-id="b2cbd-166">String</span></span>|<span data-ttu-id="b2cbd-167">Имя профиля страницы состояния регистрации</span><span class="sxs-lookup"><span data-stu-id="b2cbd-167">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="b2cbd-168">деплойментстате</span><span class="sxs-lookup"><span data-stu-id="b2cbd-168">deploymentState</span></span>|[<span data-ttu-id="b2cbd-169">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="b2cbd-169">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="b2cbd-170">Состояние развертывания, например успешное выполнение, сбой, выполнение, Сукцессвистимеаут.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-170">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="b2cbd-171">Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-171">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span></span>|
|<span data-ttu-id="b2cbd-172">osVersion</span><span class="sxs-lookup"><span data-stu-id="b2cbd-172">osVersion</span></span>|<span data-ttu-id="b2cbd-173">String</span><span class="sxs-lookup"><span data-stu-id="b2cbd-173">String</span></span>|<span data-ttu-id="b2cbd-174">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-174">Device operating system version.</span></span>|
|<span data-ttu-id="b2cbd-175">деплойментдуратион</span><span class="sxs-lookup"><span data-stu-id="b2cbd-175">deploymentDuration</span></span>|<span data-ttu-id="b2cbd-176">Длительность</span><span class="sxs-lookup"><span data-stu-id="b2cbd-176">Duration</span></span>|<span data-ttu-id="b2cbd-177">Длительность развертывания с автопилотной версией, включая регистрацию.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-177">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="b2cbd-178">деплойменттоталдуратион</span><span class="sxs-lookup"><span data-stu-id="b2cbd-178">deploymentTotalDuration</span></span>|<span data-ttu-id="b2cbd-179">Длительность</span><span class="sxs-lookup"><span data-stu-id="b2cbd-179">Duration</span></span>|<span data-ttu-id="b2cbd-180">Общее время развертывания с экрана регистрации на рабочем столе.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-180">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="b2cbd-181">девицепрепаратиондуратион</span><span class="sxs-lookup"><span data-stu-id="b2cbd-181">devicePreparationDuration</span></span>|<span data-ttu-id="b2cbd-182">Длительность</span><span class="sxs-lookup"><span data-stu-id="b2cbd-182">Duration</span></span>|<span data-ttu-id="b2cbd-183">Время, затраченное на регистрацию устройств.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-183">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="b2cbd-184">девицесетупдуратион</span><span class="sxs-lookup"><span data-stu-id="b2cbd-184">deviceSetupDuration</span></span>|<span data-ttu-id="b2cbd-185">Длительность</span><span class="sxs-lookup"><span data-stu-id="b2cbd-185">Duration</span></span>|<span data-ttu-id="b2cbd-186">Время, затраченное на устройство ESP.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-186">Time spent in device ESP.</span></span>|
|<span data-ttu-id="b2cbd-187">аккаунтсетупдуратион</span><span class="sxs-lookup"><span data-stu-id="b2cbd-187">accountSetupDuration</span></span>|<span data-ttu-id="b2cbd-188">Длительность</span><span class="sxs-lookup"><span data-stu-id="b2cbd-188">Duration</span></span>|<span data-ttu-id="b2cbd-189">Время, затраченное на ESP пользователем.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-189">Time spent in user ESP.</span></span>|
|<span data-ttu-id="b2cbd-190">деплойментстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="b2cbd-190">deploymentStartDateTime</span></span>|<span data-ttu-id="b2cbd-191">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2cbd-191">DateTimeOffset</span></span>|<span data-ttu-id="b2cbd-192">Время начала развертывания.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-192">Deployment start time.</span></span>|
|<span data-ttu-id="b2cbd-193">деплойментенддатетиме</span><span class="sxs-lookup"><span data-stu-id="b2cbd-193">deploymentEndDateTime</span></span>|<span data-ttu-id="b2cbd-194">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2cbd-194">DateTimeOffset</span></span>|<span data-ttu-id="b2cbd-195">Время окончания развертывания.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-195">Deployment end time.</span></span>|
|<span data-ttu-id="b2cbd-196">таржетедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="b2cbd-196">targetedAppCount</span></span>|<span data-ttu-id="b2cbd-197">Int32</span><span class="sxs-lookup"><span data-stu-id="b2cbd-197">Int32</span></span>|<span data-ttu-id="b2cbd-198">Количество целевых приложений.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-198">Count of applications targeted.</span></span>|
|<span data-ttu-id="b2cbd-199">таржетедполицикаунт</span><span class="sxs-lookup"><span data-stu-id="b2cbd-199">targetedPolicyCount</span></span>|<span data-ttu-id="b2cbd-200">Int32</span><span class="sxs-lookup"><span data-stu-id="b2cbd-200">Int32</span></span>|<span data-ttu-id="b2cbd-201">Количество целевых политик.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-201">Count of policies targeted.</span></span>|
|<span data-ttu-id="b2cbd-202">енроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="b2cbd-202">enrollmentFailureDetails</span></span>|<span data-ttu-id="b2cbd-203">String</span><span class="sxs-lookup"><span data-stu-id="b2cbd-203">String</span></span>|<span data-ttu-id="b2cbd-204">Сведения о сбоях при регистрации.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-204">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="b2cbd-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2cbd-205">Response</span></span>
<span data-ttu-id="b2cbd-206">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-206">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2cbd-207">Пример</span><span class="sxs-lookup"><span data-stu-id="b2cbd-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2cbd-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2cbd-208">Request</span></span>
<span data-ttu-id="b2cbd-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-209">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b2cbd-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2cbd-210">Response</span></span>
<span data-ttu-id="b2cbd-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2cbd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





