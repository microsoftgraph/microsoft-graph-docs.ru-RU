---
title: Обновление Девицеманажементаутопилотевент
description: Обновление свойств объекта Девицеманажементаутопилотевент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db30ad9e855ae7371b055e033e4b1d8c6036125d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457715"
---
# <a name="update-devicemanagementautopilotevent"></a><span data-ttu-id="f6856-103">Обновление Девицеманажементаутопилотевент</span><span class="sxs-lookup"><span data-stu-id="f6856-103">Update deviceManagementAutopilotEvent</span></span>

<span data-ttu-id="f6856-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f6856-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6856-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6856-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6856-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6856-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6856-107">Обновление свойств объекта [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="f6856-107">Update the properties of a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6856-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f6856-108">Prerequisites</span></span>
<span data-ttu-id="f6856-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6856-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6856-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6856-111">Permission type</span></span>|<span data-ttu-id="f6856-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6856-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6856-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6856-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6856-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6856-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f6856-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6856-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6856-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6856-116">Not supported.</span></span>|
|<span data-ttu-id="f6856-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6856-117">Application</span></span>|<span data-ttu-id="f6856-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6856-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6856-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6856-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

## <a name="request-headers"></a><span data-ttu-id="f6856-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f6856-120">Request headers</span></span>
|<span data-ttu-id="f6856-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6856-121">Header</span></span>|<span data-ttu-id="f6856-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f6856-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6856-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6856-123">Authorization</span></span>|<span data-ttu-id="f6856-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6856-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6856-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f6856-125">Accept</span></span>|<span data-ttu-id="f6856-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6856-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6856-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6856-127">Request body</span></span>
<span data-ttu-id="f6856-128">В тексте запроса добавьте представление объекта [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6856-128">In the request body, supply a JSON representation for the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

<span data-ttu-id="f6856-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).</span><span class="sxs-lookup"><span data-stu-id="f6856-129">The following table shows the properties that are required when you create the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).</span></span>

|<span data-ttu-id="f6856-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6856-130">Property</span></span>|<span data-ttu-id="f6856-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f6856-131">Type</span></span>|<span data-ttu-id="f6856-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f6856-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6856-133">id</span><span class="sxs-lookup"><span data-stu-id="f6856-133">id</span></span>|<span data-ttu-id="f6856-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f6856-134">String</span></span>|<span data-ttu-id="f6856-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="f6856-135">UUID for the object</span></span>|
|<span data-ttu-id="f6856-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="f6856-136">eventDateTime</span></span>|<span data-ttu-id="f6856-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6856-137">DateTimeOffset</span></span>|<span data-ttu-id="f6856-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="f6856-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="f6856-139">девицерегистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="f6856-139">deviceRegisteredDateTime</span></span>|<span data-ttu-id="f6856-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6856-140">DateTimeOffset</span></span>|<span data-ttu-id="f6856-141">Дата регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="f6856-141">Device registration date.</span></span>|
|<span data-ttu-id="f6856-142">енроллментстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="f6856-142">enrollmentStartDateTime</span></span>|<span data-ttu-id="f6856-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6856-143">DateTimeOffset</span></span>|<span data-ttu-id="f6856-144">Дата начала регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="f6856-144">Device enrollment start date.</span></span>|
|<span data-ttu-id="f6856-145">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="f6856-145">enrollmentType</span></span>|[<span data-ttu-id="f6856-146">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f6856-146">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="f6856-147">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="f6856-147">Enrollment type.</span></span> <span data-ttu-id="f6856-148">Возможные значения: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span><span class="sxs-lookup"><span data-stu-id="f6856-148">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="f6856-149">девицесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="f6856-149">deviceSerialNumber</span></span>|<span data-ttu-id="f6856-150">String</span><span class="sxs-lookup"><span data-stu-id="f6856-150">String</span></span>|<span data-ttu-id="f6856-151">Серийный номер устройства.</span><span class="sxs-lookup"><span data-stu-id="f6856-151">Device serial number.</span></span>|
|<span data-ttu-id="f6856-152">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="f6856-152">managedDeviceName</span></span>|<span data-ttu-id="f6856-153">String</span><span class="sxs-lookup"><span data-stu-id="f6856-153">String</span></span>|<span data-ttu-id="f6856-154">Управляемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="f6856-154">Managed device name.</span></span>|
|<span data-ttu-id="f6856-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f6856-155">userPrincipalName</span></span>|<span data-ttu-id="f6856-156">String</span><span class="sxs-lookup"><span data-stu-id="f6856-156">String</span></span>|<span data-ttu-id="f6856-157">Имя участника пользователя, используемое для регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="f6856-157">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="f6856-158">виндовсаутопилотдеплойментпрофиледисплайнаме</span><span class="sxs-lookup"><span data-stu-id="f6856-158">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="f6856-159">String</span><span class="sxs-lookup"><span data-stu-id="f6856-159">String</span></span>|<span data-ttu-id="f6856-160">Имя профиля для автопилота.</span><span class="sxs-lookup"><span data-stu-id="f6856-160">Autopilot profile name.</span></span>|
|<span data-ttu-id="f6856-161">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="f6856-161">enrollmentState</span></span>|[<span data-ttu-id="f6856-162">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="f6856-162">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="f6856-163">Не удалось зарегистрировать состояние регистрации, например "зарегистрировано".</span><span class="sxs-lookup"><span data-stu-id="f6856-163">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="f6856-164">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="f6856-164">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="f6856-165">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="f6856-165">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="f6856-166">String</span><span class="sxs-lookup"><span data-stu-id="f6856-166">String</span></span>|<span data-ttu-id="f6856-167">Имя профиля страницы состояния регистрации</span><span class="sxs-lookup"><span data-stu-id="f6856-167">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="f6856-168">деплойментстате</span><span class="sxs-lookup"><span data-stu-id="f6856-168">deploymentState</span></span>|[<span data-ttu-id="f6856-169">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="f6856-169">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="f6856-170">Состояние развертывания, например успешное выполнение, сбой, выполнение, Сукцессвистимеаут.</span><span class="sxs-lookup"><span data-stu-id="f6856-170">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="f6856-171">Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span><span class="sxs-lookup"><span data-stu-id="f6856-171">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span></span>|
|<span data-ttu-id="f6856-172">osVersion</span><span class="sxs-lookup"><span data-stu-id="f6856-172">osVersion</span></span>|<span data-ttu-id="f6856-173">String</span><span class="sxs-lookup"><span data-stu-id="f6856-173">String</span></span>|<span data-ttu-id="f6856-174">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="f6856-174">Device operating system version.</span></span>|
|<span data-ttu-id="f6856-175">деплойментдуратион</span><span class="sxs-lookup"><span data-stu-id="f6856-175">deploymentDuration</span></span>|<span data-ttu-id="f6856-176">Длительность</span><span class="sxs-lookup"><span data-stu-id="f6856-176">Duration</span></span>|<span data-ttu-id="f6856-177">Длительность развертывания с автопилотной версией, включая регистрацию.</span><span class="sxs-lookup"><span data-stu-id="f6856-177">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="f6856-178">деплойменттоталдуратион</span><span class="sxs-lookup"><span data-stu-id="f6856-178">deploymentTotalDuration</span></span>|<span data-ttu-id="f6856-179">Длительность</span><span class="sxs-lookup"><span data-stu-id="f6856-179">Duration</span></span>|<span data-ttu-id="f6856-180">Общее время развертывания с экрана регистрации на рабочем столе.</span><span class="sxs-lookup"><span data-stu-id="f6856-180">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="f6856-181">девицепрепаратиондуратион</span><span class="sxs-lookup"><span data-stu-id="f6856-181">devicePreparationDuration</span></span>|<span data-ttu-id="f6856-182">Длительность</span><span class="sxs-lookup"><span data-stu-id="f6856-182">Duration</span></span>|<span data-ttu-id="f6856-183">Время, затраченное на регистрацию устройств.</span><span class="sxs-lookup"><span data-stu-id="f6856-183">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="f6856-184">девицесетупдуратион</span><span class="sxs-lookup"><span data-stu-id="f6856-184">deviceSetupDuration</span></span>|<span data-ttu-id="f6856-185">Длительность</span><span class="sxs-lookup"><span data-stu-id="f6856-185">Duration</span></span>|<span data-ttu-id="f6856-186">Время, затраченное на устройство ESP.</span><span class="sxs-lookup"><span data-stu-id="f6856-186">Time spent in device ESP.</span></span>|
|<span data-ttu-id="f6856-187">аккаунтсетупдуратион</span><span class="sxs-lookup"><span data-stu-id="f6856-187">accountSetupDuration</span></span>|<span data-ttu-id="f6856-188">Длительность</span><span class="sxs-lookup"><span data-stu-id="f6856-188">Duration</span></span>|<span data-ttu-id="f6856-189">Время, затраченное на ESP пользователем.</span><span class="sxs-lookup"><span data-stu-id="f6856-189">Time spent in user ESP.</span></span>|
|<span data-ttu-id="f6856-190">деплойментстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="f6856-190">deploymentStartDateTime</span></span>|<span data-ttu-id="f6856-191">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6856-191">DateTimeOffset</span></span>|<span data-ttu-id="f6856-192">Время начала развертывания.</span><span class="sxs-lookup"><span data-stu-id="f6856-192">Deployment start time.</span></span>|
|<span data-ttu-id="f6856-193">деплойментенддатетиме</span><span class="sxs-lookup"><span data-stu-id="f6856-193">deploymentEndDateTime</span></span>|<span data-ttu-id="f6856-194">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6856-194">DateTimeOffset</span></span>|<span data-ttu-id="f6856-195">Время окончания развертывания.</span><span class="sxs-lookup"><span data-stu-id="f6856-195">Deployment end time.</span></span>|
|<span data-ttu-id="f6856-196">таржетедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="f6856-196">targetedAppCount</span></span>|<span data-ttu-id="f6856-197">Int32</span><span class="sxs-lookup"><span data-stu-id="f6856-197">Int32</span></span>|<span data-ttu-id="f6856-198">Количество целевых приложений.</span><span class="sxs-lookup"><span data-stu-id="f6856-198">Count of applications targeted.</span></span>|
|<span data-ttu-id="f6856-199">таржетедполицикаунт</span><span class="sxs-lookup"><span data-stu-id="f6856-199">targetedPolicyCount</span></span>|<span data-ttu-id="f6856-200">Int32</span><span class="sxs-lookup"><span data-stu-id="f6856-200">Int32</span></span>|<span data-ttu-id="f6856-201">Количество целевых политик.</span><span class="sxs-lookup"><span data-stu-id="f6856-201">Count of policies targeted.</span></span>|
|<span data-ttu-id="f6856-202">енроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="f6856-202">enrollmentFailureDetails</span></span>|<span data-ttu-id="f6856-203">String</span><span class="sxs-lookup"><span data-stu-id="f6856-203">String</span></span>|<span data-ttu-id="f6856-204">Сведения о сбоях при регистрации.</span><span class="sxs-lookup"><span data-stu-id="f6856-204">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="f6856-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6856-205">Response</span></span>
<span data-ttu-id="f6856-206">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6856-206">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6856-207">Пример</span><span class="sxs-lookup"><span data-stu-id="f6856-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6856-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6856-208">Request</span></span>
<span data-ttu-id="f6856-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6856-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
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

### <a name="response"></a><span data-ttu-id="f6856-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6856-210">Response</span></span>
<span data-ttu-id="f6856-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6856-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





