---
title: Обновление Девицеманажементаутопилотевент
description: Обновление свойств объекта Девицеманажементаутопилотевент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da7d507f2e86133fc8c955ff57be22b91c3e955f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49223579"
---
# <a name="update-devicemanagementautopilotevent"></a><span data-ttu-id="0f9f1-103">Обновление Девицеманажементаутопилотевент</span><span class="sxs-lookup"><span data-stu-id="0f9f1-103">Update deviceManagementAutopilotEvent</span></span>

<span data-ttu-id="0f9f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f9f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f9f1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f9f1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f9f1-107">Обновление свойств объекта [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="0f9f1-107">Update the properties of a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f9f1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0f9f1-108">Prerequisites</span></span>
<span data-ttu-id="0f9f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f9f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f9f1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f9f1-111">Permission type</span></span>|<span data-ttu-id="0f9f1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f9f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f9f1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f9f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f9f1-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f9f1-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0f9f1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f9f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f9f1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-116">Not supported.</span></span>|
|<span data-ttu-id="0f9f1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0f9f1-117">Application</span></span>|<span data-ttu-id="0f9f1-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f9f1-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f9f1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f9f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

## <a name="request-headers"></a><span data-ttu-id="0f9f1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0f9f1-120">Request headers</span></span>
|<span data-ttu-id="0f9f1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f9f1-121">Header</span></span>|<span data-ttu-id="0f9f1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0f9f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f9f1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f9f1-123">Authorization</span></span>|<span data-ttu-id="0f9f1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f9f1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0f9f1-125">Accept</span></span>|<span data-ttu-id="0f9f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f9f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f9f1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f9f1-127">Request body</span></span>
<span data-ttu-id="0f9f1-128">В тексте запроса добавьте представление объекта [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-128">In the request body, supply a JSON representation for the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

<span data-ttu-id="0f9f1-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).</span><span class="sxs-lookup"><span data-stu-id="0f9f1-129">The following table shows the properties that are required when you create the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).</span></span>

|<span data-ttu-id="0f9f1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f9f1-130">Property</span></span>|<span data-ttu-id="0f9f1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0f9f1-131">Type</span></span>|<span data-ttu-id="0f9f1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0f9f1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f9f1-133">id</span><span class="sxs-lookup"><span data-stu-id="0f9f1-133">id</span></span>|<span data-ttu-id="0f9f1-134">String</span><span class="sxs-lookup"><span data-stu-id="0f9f1-134">String</span></span>|<span data-ttu-id="0f9f1-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-135">UUID for the object</span></span>|
|<span data-ttu-id="0f9f1-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="0f9f1-136">deviceId</span></span>|<span data-ttu-id="0f9f1-137">String</span><span class="sxs-lookup"><span data-stu-id="0f9f1-137">String</span></span>|<span data-ttu-id="0f9f1-138">Идентификатор устройства, связанный с объектом</span><span class="sxs-lookup"><span data-stu-id="0f9f1-138">Device id associated with the object</span></span>|
|<span data-ttu-id="0f9f1-139">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="0f9f1-139">eventDateTime</span></span>|<span data-ttu-id="0f9f1-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f9f1-140">DateTimeOffset</span></span>|<span data-ttu-id="0f9f1-141">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-141">Time when the event occurred .</span></span>|
|<span data-ttu-id="0f9f1-142">девицерегистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="0f9f1-142">deviceRegisteredDateTime</span></span>|<span data-ttu-id="0f9f1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f9f1-143">DateTimeOffset</span></span>|<span data-ttu-id="0f9f1-144">Дата регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-144">Device registration date.</span></span>|
|<span data-ttu-id="0f9f1-145">енроллментстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="0f9f1-145">enrollmentStartDateTime</span></span>|<span data-ttu-id="0f9f1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f9f1-146">DateTimeOffset</span></span>|<span data-ttu-id="0f9f1-147">Дата начала регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-147">Device enrollment start date.</span></span>|
|<span data-ttu-id="0f9f1-148">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="0f9f1-148">enrollmentType</span></span>|[<span data-ttu-id="0f9f1-149">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0f9f1-149">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="0f9f1-150">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-150">Enrollment type.</span></span> <span data-ttu-id="0f9f1-151">Возможные значения: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-151">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="0f9f1-152">девицесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="0f9f1-152">deviceSerialNumber</span></span>|<span data-ttu-id="0f9f1-153">String</span><span class="sxs-lookup"><span data-stu-id="0f9f1-153">String</span></span>|<span data-ttu-id="0f9f1-154">Серийный номер устройства.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-154">Device serial number.</span></span>|
|<span data-ttu-id="0f9f1-155">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="0f9f1-155">managedDeviceName</span></span>|<span data-ttu-id="0f9f1-156">String</span><span class="sxs-lookup"><span data-stu-id="0f9f1-156">String</span></span>|<span data-ttu-id="0f9f1-157">Управляемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-157">Managed device name.</span></span>|
|<span data-ttu-id="0f9f1-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0f9f1-158">userPrincipalName</span></span>|<span data-ttu-id="0f9f1-159">String</span><span class="sxs-lookup"><span data-stu-id="0f9f1-159">String</span></span>|<span data-ttu-id="0f9f1-160">Имя участника пользователя, используемое для регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-160">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="0f9f1-161">виндовсаутопилотдеплойментпрофиледисплайнаме</span><span class="sxs-lookup"><span data-stu-id="0f9f1-161">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="0f9f1-162">String</span><span class="sxs-lookup"><span data-stu-id="0f9f1-162">String</span></span>|<span data-ttu-id="0f9f1-163">Имя профиля для автопилота.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-163">Autopilot profile name.</span></span>|
|<span data-ttu-id="0f9f1-164">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="0f9f1-164">enrollmentState</span></span>|[<span data-ttu-id="0f9f1-165">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="0f9f1-165">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="0f9f1-166">Не удалось зарегистрировать состояние регистрации, например "зарегистрировано".</span><span class="sxs-lookup"><span data-stu-id="0f9f1-166">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="0f9f1-167">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="0f9f1-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="0f9f1-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="0f9f1-169">String</span><span class="sxs-lookup"><span data-stu-id="0f9f1-169">String</span></span>|<span data-ttu-id="0f9f1-170">Имя профиля страницы состояния регистрации</span><span class="sxs-lookup"><span data-stu-id="0f9f1-170">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="0f9f1-171">деплойментстате</span><span class="sxs-lookup"><span data-stu-id="0f9f1-171">deploymentState</span></span>|[<span data-ttu-id="0f9f1-172">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="0f9f1-172">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="0f9f1-173">Состояние развертывания, например успешное выполнение, сбой, выполнение, Сукцессвистимеаут.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-173">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="0f9f1-174">Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-174">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span></span>|
|<span data-ttu-id="0f9f1-175">osVersion</span><span class="sxs-lookup"><span data-stu-id="0f9f1-175">osVersion</span></span>|<span data-ttu-id="0f9f1-176">String</span><span class="sxs-lookup"><span data-stu-id="0f9f1-176">String</span></span>|<span data-ttu-id="0f9f1-177">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-177">Device operating system version.</span></span>|
|<span data-ttu-id="0f9f1-178">деплойментдуратион</span><span class="sxs-lookup"><span data-stu-id="0f9f1-178">deploymentDuration</span></span>|<span data-ttu-id="0f9f1-179">Длительность</span><span class="sxs-lookup"><span data-stu-id="0f9f1-179">Duration</span></span>|<span data-ttu-id="0f9f1-180">Длительность развертывания с автопилотной версией, включая регистрацию.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-180">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="0f9f1-181">деплойменттоталдуратион</span><span class="sxs-lookup"><span data-stu-id="0f9f1-181">deploymentTotalDuration</span></span>|<span data-ttu-id="0f9f1-182">Длительность</span><span class="sxs-lookup"><span data-stu-id="0f9f1-182">Duration</span></span>|<span data-ttu-id="0f9f1-183">Общее время развертывания с экрана регистрации на рабочем столе.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-183">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="0f9f1-184">девицепрепаратиондуратион</span><span class="sxs-lookup"><span data-stu-id="0f9f1-184">devicePreparationDuration</span></span>|<span data-ttu-id="0f9f1-185">Длительность</span><span class="sxs-lookup"><span data-stu-id="0f9f1-185">Duration</span></span>|<span data-ttu-id="0f9f1-186">Время, затраченное на регистрацию устройств.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-186">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="0f9f1-187">девицесетупдуратион</span><span class="sxs-lookup"><span data-stu-id="0f9f1-187">deviceSetupDuration</span></span>|<span data-ttu-id="0f9f1-188">Длительность</span><span class="sxs-lookup"><span data-stu-id="0f9f1-188">Duration</span></span>|<span data-ttu-id="0f9f1-189">Время, затраченное на устройство ESP.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-189">Time spent in device ESP.</span></span>|
|<span data-ttu-id="0f9f1-190">аккаунтсетупдуратион</span><span class="sxs-lookup"><span data-stu-id="0f9f1-190">accountSetupDuration</span></span>|<span data-ttu-id="0f9f1-191">Длительность</span><span class="sxs-lookup"><span data-stu-id="0f9f1-191">Duration</span></span>|<span data-ttu-id="0f9f1-192">Время, затраченное на ESP пользователем.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-192">Time spent in user ESP.</span></span>|
|<span data-ttu-id="0f9f1-193">деплойментстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="0f9f1-193">deploymentStartDateTime</span></span>|<span data-ttu-id="0f9f1-194">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f9f1-194">DateTimeOffset</span></span>|<span data-ttu-id="0f9f1-195">Время начала развертывания.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-195">Deployment start time.</span></span>|
|<span data-ttu-id="0f9f1-196">деплойментенддатетиме</span><span class="sxs-lookup"><span data-stu-id="0f9f1-196">deploymentEndDateTime</span></span>|<span data-ttu-id="0f9f1-197">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f9f1-197">DateTimeOffset</span></span>|<span data-ttu-id="0f9f1-198">Время окончания развертывания.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-198">Deployment end time.</span></span>|
|<span data-ttu-id="0f9f1-199">таржетедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="0f9f1-199">targetedAppCount</span></span>|<span data-ttu-id="0f9f1-200">Int32</span><span class="sxs-lookup"><span data-stu-id="0f9f1-200">Int32</span></span>|<span data-ttu-id="0f9f1-201">Количество целевых приложений.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-201">Count of applications targeted.</span></span>|
|<span data-ttu-id="0f9f1-202">таржетедполицикаунт</span><span class="sxs-lookup"><span data-stu-id="0f9f1-202">targetedPolicyCount</span></span>|<span data-ttu-id="0f9f1-203">Int32</span><span class="sxs-lookup"><span data-stu-id="0f9f1-203">Int32</span></span>|<span data-ttu-id="0f9f1-204">Количество целевых политик.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-204">Count of policies targeted.</span></span>|
|<span data-ttu-id="0f9f1-205">енроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="0f9f1-205">enrollmentFailureDetails</span></span>|<span data-ttu-id="0f9f1-206">String</span><span class="sxs-lookup"><span data-stu-id="0f9f1-206">String</span></span>|<span data-ttu-id="0f9f1-207">Сведения о сбоях при регистрации.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-207">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="0f9f1-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f9f1-208">Response</span></span>
<span data-ttu-id="0f9f1-209">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-209">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f9f1-210">Пример</span><span class="sxs-lookup"><span data-stu-id="0f9f1-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f9f1-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f9f1-211">Request</span></span>
<span data-ttu-id="0f9f1-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0f9f1-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f9f1-213">Response</span></span>
<span data-ttu-id="0f9f1-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f9f1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




