---
title: Создание deviceManagementAutopilotEvent
description: Создание объекта deviceManagementAutopilotEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 411e7dd15a8f3fe75d726f0caab38c7592b3a8a6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159215"
---
# <a name="create-devicemanagementautopilotevent"></a><span data-ttu-id="7b240-103">Создание deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="7b240-103">Create deviceManagementAutopilotEvent</span></span>

<span data-ttu-id="7b240-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b240-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b240-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b240-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b240-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b240-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b240-107">Создание объекта [deviceManagementAutopilotEvent.](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)</span><span class="sxs-lookup"><span data-stu-id="7b240-107">Create a new [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b240-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7b240-108">Prerequisites</span></span>
<span data-ttu-id="7b240-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b240-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b240-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b240-111">Permission type</span></span>|<span data-ttu-id="7b240-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b240-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b240-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b240-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b240-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b240-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7b240-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b240-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b240-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b240-116">Not supported.</span></span>|
|<span data-ttu-id="7b240-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b240-117">Application</span></span>|<span data-ttu-id="7b240-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b240-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b240-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b240-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="7b240-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7b240-120">Request headers</span></span>
|<span data-ttu-id="7b240-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b240-121">Header</span></span>|<span data-ttu-id="7b240-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7b240-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b240-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b240-123">Authorization</span></span>|<span data-ttu-id="7b240-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b240-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b240-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7b240-125">Accept</span></span>|<span data-ttu-id="7b240-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b240-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b240-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b240-127">Request body</span></span>
<span data-ttu-id="7b240-128">В теле запроса укажу представление объекта deviceManagementAutopilotEvent в JSON.</span><span class="sxs-lookup"><span data-stu-id="7b240-128">In the request body, supply a JSON representation for the deviceManagementAutopilotEvent object.</span></span>

<span data-ttu-id="7b240-129">В следующей таблице показаны свойства, необходимые при создании объекта deviceManagementAutopilotEvent.</span><span class="sxs-lookup"><span data-stu-id="7b240-129">The following table shows the properties that are required when you create the deviceManagementAutopilotEvent.</span></span>

|<span data-ttu-id="7b240-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b240-130">Property</span></span>|<span data-ttu-id="7b240-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7b240-131">Type</span></span>|<span data-ttu-id="7b240-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7b240-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b240-133">id</span><span class="sxs-lookup"><span data-stu-id="7b240-133">id</span></span>|<span data-ttu-id="7b240-134">String</span><span class="sxs-lookup"><span data-stu-id="7b240-134">String</span></span>|<span data-ttu-id="7b240-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="7b240-135">UUID for the object</span></span>|
|<span data-ttu-id="7b240-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="7b240-136">deviceId</span></span>|<span data-ttu-id="7b240-137">String</span><span class="sxs-lookup"><span data-stu-id="7b240-137">String</span></span>|<span data-ttu-id="7b240-138">ИД устройства, связанный с объектом</span><span class="sxs-lookup"><span data-stu-id="7b240-138">Device id associated with the object</span></span>|
|<span data-ttu-id="7b240-139">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="7b240-139">eventDateTime</span></span>|<span data-ttu-id="7b240-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b240-140">DateTimeOffset</span></span>|<span data-ttu-id="7b240-141">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="7b240-141">Time when the event occurred .</span></span>|
|<span data-ttu-id="7b240-142">deviceRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="7b240-142">deviceRegisteredDateTime</span></span>|<span data-ttu-id="7b240-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b240-143">DateTimeOffset</span></span>|<span data-ttu-id="7b240-144">Дата регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b240-144">Device registration date.</span></span>|
|<span data-ttu-id="7b240-145">enrollmentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="7b240-145">enrollmentStartDateTime</span></span>|<span data-ttu-id="7b240-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b240-146">DateTimeOffset</span></span>|<span data-ttu-id="7b240-147">Дата начала регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b240-147">Device enrollment start date.</span></span>|
|<span data-ttu-id="7b240-148">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="7b240-148">enrollmentType</span></span>|[<span data-ttu-id="7b240-149">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="7b240-149">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="7b240-150">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="7b240-150">Enrollment type.</span></span> <span data-ttu-id="7b240-151">Возможные значения: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span><span class="sxs-lookup"><span data-stu-id="7b240-151">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="7b240-152">deviceSerialNumber</span><span class="sxs-lookup"><span data-stu-id="7b240-152">deviceSerialNumber</span></span>|<span data-ttu-id="7b240-153">String</span><span class="sxs-lookup"><span data-stu-id="7b240-153">String</span></span>|<span data-ttu-id="7b240-154">Серийный номер устройства.</span><span class="sxs-lookup"><span data-stu-id="7b240-154">Device serial number.</span></span>|
|<span data-ttu-id="7b240-155">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="7b240-155">managedDeviceName</span></span>|<span data-ttu-id="7b240-156">String</span><span class="sxs-lookup"><span data-stu-id="7b240-156">String</span></span>|<span data-ttu-id="7b240-157">Имя управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="7b240-157">Managed device name.</span></span>|
|<span data-ttu-id="7b240-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7b240-158">userPrincipalName</span></span>|<span data-ttu-id="7b240-159">String</span><span class="sxs-lookup"><span data-stu-id="7b240-159">String</span></span>|<span data-ttu-id="7b240-160">Имя основного пользователя, используемая для регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b240-160">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="7b240-161">windowsAutopilotDeploymentProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="7b240-161">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="7b240-162">String</span><span class="sxs-lookup"><span data-stu-id="7b240-162">String</span></span>|<span data-ttu-id="7b240-163">Имя профиля Autopilot.</span><span class="sxs-lookup"><span data-stu-id="7b240-163">Autopilot profile name.</span></span>|
|<span data-ttu-id="7b240-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7b240-164">enrollmentState</span></span>|[<span data-ttu-id="7b240-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7b240-165">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="7b240-166">Состояние регистрации, например "Зарегистрировано", "Сбой".</span><span class="sxs-lookup"><span data-stu-id="7b240-166">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="7b240-167">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="7b240-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="7b240-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="7b240-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="7b240-169">String</span><span class="sxs-lookup"><span data-stu-id="7b240-169">String</span></span>|<span data-ttu-id="7b240-170">Имя профиля страницы состояния регистрации</span><span class="sxs-lookup"><span data-stu-id="7b240-170">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="7b240-171">windows10EnrollmentCompletionPageConfigurationId</span><span class="sxs-lookup"><span data-stu-id="7b240-171">windows10EnrollmentCompletionPageConfigurationId</span></span>|<span data-ttu-id="7b240-172">String</span><span class="sxs-lookup"><span data-stu-id="7b240-172">String</span></span>|<span data-ttu-id="7b240-173">ИД профиля страницы состояния регистрации</span><span class="sxs-lookup"><span data-stu-id="7b240-173">Enrollment Status Page profile ID</span></span>|
|<span data-ttu-id="7b240-174">deploymentState</span><span class="sxs-lookup"><span data-stu-id="7b240-174">deploymentState</span></span>|[<span data-ttu-id="7b240-175">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="7b240-175">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="7b240-176">Состояние развертывания, например Success, Failure, InProgress, SuccessWithTimeout.</span><span class="sxs-lookup"><span data-stu-id="7b240-176">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="7b240-177">Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="7b240-177">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span></span>|
|<span data-ttu-id="7b240-178">deviceSetupStatus</span><span class="sxs-lookup"><span data-stu-id="7b240-178">deviceSetupStatus</span></span>|[<span data-ttu-id="7b240-179">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="7b240-179">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="7b240-180">Состояние развертывания для этапа настройки устройства страницы состояния регистрации.</span><span class="sxs-lookup"><span data-stu-id="7b240-180">Deployment status for the enrollment status page device setup phase.</span></span> <span data-ttu-id="7b240-181">Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="7b240-181">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span></span>|
|<span data-ttu-id="7b240-182">accountSetupStatus</span><span class="sxs-lookup"><span data-stu-id="7b240-182">accountSetupStatus</span></span>|[<span data-ttu-id="7b240-183">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="7b240-183">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="7b240-184">Состояние развертывания для этапа настройки учетной записи страницы состояния регистрации.</span><span class="sxs-lookup"><span data-stu-id="7b240-184">Deployment status for the enrollment status page account setup phase.</span></span> <span data-ttu-id="7b240-185">Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="7b240-185">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span></span>|
|<span data-ttu-id="7b240-186">osVersion</span><span class="sxs-lookup"><span data-stu-id="7b240-186">osVersion</span></span>|<span data-ttu-id="7b240-187">String</span><span class="sxs-lookup"><span data-stu-id="7b240-187">String</span></span>|<span data-ttu-id="7b240-188">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="7b240-188">Device operating system version.</span></span>|
|<span data-ttu-id="7b240-189">deploymentDuration</span><span class="sxs-lookup"><span data-stu-id="7b240-189">deploymentDuration</span></span>|<span data-ttu-id="7b240-190">Duration</span><span class="sxs-lookup"><span data-stu-id="7b240-190">Duration</span></span>|<span data-ttu-id="7b240-191">Продолжительность развертывания Autopilot, включая регистрацию.</span><span class="sxs-lookup"><span data-stu-id="7b240-191">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="7b240-192">deploymentTotalDuration</span><span class="sxs-lookup"><span data-stu-id="7b240-192">deploymentTotalDuration</span></span>|<span data-ttu-id="7b240-193">Duration</span><span class="sxs-lookup"><span data-stu-id="7b240-193">Duration</span></span>|<span data-ttu-id="7b240-194">Общая продолжительность развертывания от регистрации до экрана рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="7b240-194">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="7b240-195">devicePreparationDuration</span><span class="sxs-lookup"><span data-stu-id="7b240-195">devicePreparationDuration</span></span>|<span data-ttu-id="7b240-196">Duration</span><span class="sxs-lookup"><span data-stu-id="7b240-196">Duration</span></span>|<span data-ttu-id="7b240-197">Время, затраченное на регистрацию устройств.</span><span class="sxs-lookup"><span data-stu-id="7b240-197">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="7b240-198">deviceSetupDuration</span><span class="sxs-lookup"><span data-stu-id="7b240-198">deviceSetupDuration</span></span>|<span data-ttu-id="7b240-199">Duration</span><span class="sxs-lookup"><span data-stu-id="7b240-199">Duration</span></span>|<span data-ttu-id="7b240-200">Время, затраченное на ESP устройства.</span><span class="sxs-lookup"><span data-stu-id="7b240-200">Time spent in device ESP.</span></span>|
|<span data-ttu-id="7b240-201">accountSetupDuration</span><span class="sxs-lookup"><span data-stu-id="7b240-201">accountSetupDuration</span></span>|<span data-ttu-id="7b240-202">Duration</span><span class="sxs-lookup"><span data-stu-id="7b240-202">Duration</span></span>|<span data-ttu-id="7b240-203">Время, затраченное на esp пользователя.</span><span class="sxs-lookup"><span data-stu-id="7b240-203">Time spent in user ESP.</span></span>|
|<span data-ttu-id="7b240-204">deploymentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="7b240-204">deploymentStartDateTime</span></span>|<span data-ttu-id="7b240-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b240-205">DateTimeOffset</span></span>|<span data-ttu-id="7b240-206">Время начала развертывания.</span><span class="sxs-lookup"><span data-stu-id="7b240-206">Deployment start time.</span></span>|
|<span data-ttu-id="7b240-207">deploymentEndDateTime</span><span class="sxs-lookup"><span data-stu-id="7b240-207">deploymentEndDateTime</span></span>|<span data-ttu-id="7b240-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b240-208">DateTimeOffset</span></span>|<span data-ttu-id="7b240-209">Время окончания развертывания.</span><span class="sxs-lookup"><span data-stu-id="7b240-209">Deployment end time.</span></span>|
|<span data-ttu-id="7b240-210">targetedAppCount</span><span class="sxs-lookup"><span data-stu-id="7b240-210">targetedAppCount</span></span>|<span data-ttu-id="7b240-211">Int32</span><span class="sxs-lookup"><span data-stu-id="7b240-211">Int32</span></span>|<span data-ttu-id="7b240-212">Количество целевых приложений.</span><span class="sxs-lookup"><span data-stu-id="7b240-212">Count of applications targeted.</span></span>|
|<span data-ttu-id="7b240-213">targetedPolicyCount</span><span class="sxs-lookup"><span data-stu-id="7b240-213">targetedPolicyCount</span></span>|<span data-ttu-id="7b240-214">Int32</span><span class="sxs-lookup"><span data-stu-id="7b240-214">Int32</span></span>|<span data-ttu-id="7b240-215">Количество целевых политик.</span><span class="sxs-lookup"><span data-stu-id="7b240-215">Count of policies targeted.</span></span>|
|<span data-ttu-id="7b240-216">enrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="7b240-216">enrollmentFailureDetails</span></span>|<span data-ttu-id="7b240-217">String</span><span class="sxs-lookup"><span data-stu-id="7b240-217">String</span></span>|<span data-ttu-id="7b240-218">Сведения о сбое регистрации.</span><span class="sxs-lookup"><span data-stu-id="7b240-218">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="7b240-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b240-219">Response</span></span>
<span data-ttu-id="7b240-220">В случае успешного выполнения этот метод возвращает код отклика и объект `201 Created` [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7b240-220">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b240-221">Пример</span><span class="sxs-lookup"><span data-stu-id="7b240-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b240-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b240-222">Request</span></span>
<span data-ttu-id="7b240-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b240-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
Content-type: application/json
Content-length: 1545

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
  "windows10EnrollmentCompletionPageConfigurationId": "Windows10Enrollment Completion Page Configuration Id value",
  "deploymentState": "success",
  "deviceSetupStatus": "success",
  "accountSetupStatus": "success",
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

### <a name="response"></a><span data-ttu-id="7b240-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b240-224">Response</span></span>
<span data-ttu-id="7b240-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b240-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1594

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
  "windows10EnrollmentCompletionPageConfigurationId": "Windows10Enrollment Completion Page Configuration Id value",
  "deploymentState": "success",
  "deviceSetupStatus": "success",
  "accountSetupStatus": "success",
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




