---
title: Обновление Девицеманажементаутопилотевент
description: Обновление свойств объекта Девицеманажементаутопилотевент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ea3703d23eb45e9c91dd40cbd3cb3031b7e2cd30
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800237"
---
# <a name="update-devicemanagementautopilotevent"></a><span data-ttu-id="d96e2-103">Обновление Девицеманажементаутопилотевент</span><span class="sxs-lookup"><span data-stu-id="d96e2-103">Update deviceManagementAutopilotEvent</span></span>

> <span data-ttu-id="d96e2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d96e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d96e2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d96e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d96e2-106">Обновление свойств объекта [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="d96e2-106">Update the properties of a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d96e2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d96e2-107">Prerequisites</span></span>
<span data-ttu-id="d96e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d96e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d96e2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d96e2-110">Permission type</span></span>|<span data-ttu-id="d96e2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d96e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d96e2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d96e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d96e2-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d96e2-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d96e2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d96e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d96e2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d96e2-115">Not supported.</span></span>|
|<span data-ttu-id="d96e2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d96e2-116">Application</span></span>|<span data-ttu-id="d96e2-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d96e2-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d96e2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d96e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

## <a name="request-headers"></a><span data-ttu-id="d96e2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d96e2-119">Request headers</span></span>
|<span data-ttu-id="d96e2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d96e2-120">Header</span></span>|<span data-ttu-id="d96e2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d96e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d96e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d96e2-122">Authorization</span></span>|<span data-ttu-id="d96e2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d96e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d96e2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d96e2-124">Accept</span></span>|<span data-ttu-id="d96e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d96e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d96e2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d96e2-126">Request body</span></span>
<span data-ttu-id="d96e2-127">В тексте запроса добавьте представление объекта [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d96e2-127">In the request body, supply a JSON representation for the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

<span data-ttu-id="d96e2-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).</span><span class="sxs-lookup"><span data-stu-id="d96e2-128">The following table shows the properties that are required when you create the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).</span></span>

|<span data-ttu-id="d96e2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d96e2-129">Property</span></span>|<span data-ttu-id="d96e2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d96e2-130">Type</span></span>|<span data-ttu-id="d96e2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d96e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d96e2-132">id</span><span class="sxs-lookup"><span data-stu-id="d96e2-132">id</span></span>|<span data-ttu-id="d96e2-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d96e2-133">String</span></span>|<span data-ttu-id="d96e2-134">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="d96e2-134">UUID for the object</span></span>|
|<span data-ttu-id="d96e2-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="d96e2-135">deviceId</span></span>|<span data-ttu-id="d96e2-136">String</span><span class="sxs-lookup"><span data-stu-id="d96e2-136">String</span></span>|<span data-ttu-id="d96e2-137">Идентификатор устройства, связанный с объектом</span><span class="sxs-lookup"><span data-stu-id="d96e2-137">Device id associated with the object</span></span>|
|<span data-ttu-id="d96e2-138">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="d96e2-138">eventDateTime</span></span>|<span data-ttu-id="d96e2-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d96e2-139">DateTimeOffset</span></span>|<span data-ttu-id="d96e2-140">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="d96e2-140">Time when the event occurred .</span></span>|
|<span data-ttu-id="d96e2-141">девицерегистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="d96e2-141">deviceRegisteredDateTime</span></span>|<span data-ttu-id="d96e2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d96e2-142">DateTimeOffset</span></span>|<span data-ttu-id="d96e2-143">Дата регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="d96e2-143">Device registration date.</span></span>|
|<span data-ttu-id="d96e2-144">енроллментстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="d96e2-144">enrollmentStartDateTime</span></span>|<span data-ttu-id="d96e2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d96e2-145">DateTimeOffset</span></span>|<span data-ttu-id="d96e2-146">Дата начала регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="d96e2-146">Device enrollment start date.</span></span>|
|<span data-ttu-id="d96e2-147">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="d96e2-147">enrollmentType</span></span>|[<span data-ttu-id="d96e2-148">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d96e2-148">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="d96e2-149">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="d96e2-149">Enrollment type.</span></span> <span data-ttu-id="d96e2-150">Возможные значения: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span><span class="sxs-lookup"><span data-stu-id="d96e2-150">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="d96e2-151">девицесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="d96e2-151">deviceSerialNumber</span></span>|<span data-ttu-id="d96e2-152">String</span><span class="sxs-lookup"><span data-stu-id="d96e2-152">String</span></span>|<span data-ttu-id="d96e2-153">Серийный номер устройства.</span><span class="sxs-lookup"><span data-stu-id="d96e2-153">Device serial number.</span></span>|
|<span data-ttu-id="d96e2-154">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="d96e2-154">managedDeviceName</span></span>|<span data-ttu-id="d96e2-155">String</span><span class="sxs-lookup"><span data-stu-id="d96e2-155">String</span></span>|<span data-ttu-id="d96e2-156">Управляемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="d96e2-156">Managed device name.</span></span>|
|<span data-ttu-id="d96e2-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d96e2-157">userPrincipalName</span></span>|<span data-ttu-id="d96e2-158">String</span><span class="sxs-lookup"><span data-stu-id="d96e2-158">String</span></span>|<span data-ttu-id="d96e2-159">Имя участника пользователя, используемое для регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="d96e2-159">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="d96e2-160">виндовсаутопилотдеплойментпрофиледисплайнаме</span><span class="sxs-lookup"><span data-stu-id="d96e2-160">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="d96e2-161">String</span><span class="sxs-lookup"><span data-stu-id="d96e2-161">String</span></span>|<span data-ttu-id="d96e2-162">Имя профиля для автопилота.</span><span class="sxs-lookup"><span data-stu-id="d96e2-162">Autopilot profile name.</span></span>|
|<span data-ttu-id="d96e2-163">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="d96e2-163">enrollmentState</span></span>|[<span data-ttu-id="d96e2-164">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="d96e2-164">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="d96e2-165">Не удалось зарегистрировать состояние регистрации, например "зарегистрировано".</span><span class="sxs-lookup"><span data-stu-id="d96e2-165">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="d96e2-166">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="d96e2-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="d96e2-167">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="d96e2-167">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="d96e2-168">String</span><span class="sxs-lookup"><span data-stu-id="d96e2-168">String</span></span>|<span data-ttu-id="d96e2-169">Имя профиля страницы состояния регистрации</span><span class="sxs-lookup"><span data-stu-id="d96e2-169">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="d96e2-170">деплойментстате</span><span class="sxs-lookup"><span data-stu-id="d96e2-170">deploymentState</span></span>|[<span data-ttu-id="d96e2-171">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="d96e2-171">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="d96e2-172">Состояние развертывания, например успешное выполнение, сбой, выполнение, Сукцессвистимеаут.</span><span class="sxs-lookup"><span data-stu-id="d96e2-172">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="d96e2-173">Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span><span class="sxs-lookup"><span data-stu-id="d96e2-173">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span></span>|
|<span data-ttu-id="d96e2-174">osVersion</span><span class="sxs-lookup"><span data-stu-id="d96e2-174">osVersion</span></span>|<span data-ttu-id="d96e2-175">String</span><span class="sxs-lookup"><span data-stu-id="d96e2-175">String</span></span>|<span data-ttu-id="d96e2-176">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="d96e2-176">Device operating system version.</span></span>|
|<span data-ttu-id="d96e2-177">деплойментдуратион</span><span class="sxs-lookup"><span data-stu-id="d96e2-177">deploymentDuration</span></span>|<span data-ttu-id="d96e2-178">Длительность</span><span class="sxs-lookup"><span data-stu-id="d96e2-178">Duration</span></span>|<span data-ttu-id="d96e2-179">Длительность развертывания с автопилотной версией, включая регистрацию.</span><span class="sxs-lookup"><span data-stu-id="d96e2-179">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="d96e2-180">деплойменттоталдуратион</span><span class="sxs-lookup"><span data-stu-id="d96e2-180">deploymentTotalDuration</span></span>|<span data-ttu-id="d96e2-181">Длительность</span><span class="sxs-lookup"><span data-stu-id="d96e2-181">Duration</span></span>|<span data-ttu-id="d96e2-182">Общее время развертывания с экрана регистрации на рабочем столе.</span><span class="sxs-lookup"><span data-stu-id="d96e2-182">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="d96e2-183">девицепрепаратиондуратион</span><span class="sxs-lookup"><span data-stu-id="d96e2-183">devicePreparationDuration</span></span>|<span data-ttu-id="d96e2-184">Длительность</span><span class="sxs-lookup"><span data-stu-id="d96e2-184">Duration</span></span>|<span data-ttu-id="d96e2-185">Время, затраченное на регистрацию устройств.</span><span class="sxs-lookup"><span data-stu-id="d96e2-185">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="d96e2-186">девицесетупдуратион</span><span class="sxs-lookup"><span data-stu-id="d96e2-186">deviceSetupDuration</span></span>|<span data-ttu-id="d96e2-187">Длительность</span><span class="sxs-lookup"><span data-stu-id="d96e2-187">Duration</span></span>|<span data-ttu-id="d96e2-188">Время, затраченное на устройство ESP.</span><span class="sxs-lookup"><span data-stu-id="d96e2-188">Time spent in device ESP.</span></span>|
|<span data-ttu-id="d96e2-189">аккаунтсетупдуратион</span><span class="sxs-lookup"><span data-stu-id="d96e2-189">accountSetupDuration</span></span>|<span data-ttu-id="d96e2-190">Длительность</span><span class="sxs-lookup"><span data-stu-id="d96e2-190">Duration</span></span>|<span data-ttu-id="d96e2-191">Время, затраченное на ESP пользователем.</span><span class="sxs-lookup"><span data-stu-id="d96e2-191">Time spent in user ESP.</span></span>|
|<span data-ttu-id="d96e2-192">деплойментстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="d96e2-192">deploymentStartDateTime</span></span>|<span data-ttu-id="d96e2-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d96e2-193">DateTimeOffset</span></span>|<span data-ttu-id="d96e2-194">Время начала развертывания.</span><span class="sxs-lookup"><span data-stu-id="d96e2-194">Deployment start time.</span></span>|
|<span data-ttu-id="d96e2-195">деплойментенддатетиме</span><span class="sxs-lookup"><span data-stu-id="d96e2-195">deploymentEndDateTime</span></span>|<span data-ttu-id="d96e2-196">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d96e2-196">DateTimeOffset</span></span>|<span data-ttu-id="d96e2-197">Время окончания развертывания.</span><span class="sxs-lookup"><span data-stu-id="d96e2-197">Deployment end time.</span></span>|
|<span data-ttu-id="d96e2-198">таржетедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="d96e2-198">targetedAppCount</span></span>|<span data-ttu-id="d96e2-199">Int32</span><span class="sxs-lookup"><span data-stu-id="d96e2-199">Int32</span></span>|<span data-ttu-id="d96e2-200">Количество целевых приложений.</span><span class="sxs-lookup"><span data-stu-id="d96e2-200">Count of applications targeted.</span></span>|
|<span data-ttu-id="d96e2-201">таржетедполицикаунт</span><span class="sxs-lookup"><span data-stu-id="d96e2-201">targetedPolicyCount</span></span>|<span data-ttu-id="d96e2-202">Int32</span><span class="sxs-lookup"><span data-stu-id="d96e2-202">Int32</span></span>|<span data-ttu-id="d96e2-203">Количество целевых политик.</span><span class="sxs-lookup"><span data-stu-id="d96e2-203">Count of policies targeted.</span></span>|
|<span data-ttu-id="d96e2-204">енроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="d96e2-204">enrollmentFailureDetails</span></span>|<span data-ttu-id="d96e2-205">String</span><span class="sxs-lookup"><span data-stu-id="d96e2-205">String</span></span>|<span data-ttu-id="d96e2-206">Сведения о сбоях при регистрации.</span><span class="sxs-lookup"><span data-stu-id="d96e2-206">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="d96e2-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="d96e2-207">Response</span></span>
<span data-ttu-id="d96e2-208">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d96e2-208">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d96e2-209">Пример</span><span class="sxs-lookup"><span data-stu-id="d96e2-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="d96e2-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="d96e2-210">Request</span></span>
<span data-ttu-id="d96e2-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d96e2-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
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

### <a name="response"></a><span data-ttu-id="d96e2-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="d96e2-212">Response</span></span>
<span data-ttu-id="d96e2-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d96e2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




