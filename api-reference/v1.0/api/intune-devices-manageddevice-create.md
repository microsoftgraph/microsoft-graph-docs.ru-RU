---
title: Create managedDevice
description: Создание объекта managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4bdd3bc460148298b91386e6ce0988f743cc78e5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756157"
---
# <a name="create-manageddevice"></a><span data-ttu-id="696e3-103">Create managedDevice</span><span class="sxs-lookup"><span data-stu-id="696e3-103">Create managedDevice</span></span>

<span data-ttu-id="696e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="696e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="696e3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="696e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="696e3-106">Создание объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="696e3-106">Create a new [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="696e3-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="696e3-107">Prerequisites</span></span>
<span data-ttu-id="696e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="696e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="696e3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="696e3-110">Permission type</span></span>|<span data-ttu-id="696e3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="696e3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="696e3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="696e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="696e3-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="696e3-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="696e3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="696e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="696e3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="696e3-115">Not supported.</span></span>|
|<span data-ttu-id="696e3-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="696e3-116">Application</span></span>|<span data-ttu-id="696e3-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="696e3-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="696e3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="696e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="696e3-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="696e3-119">Request headers</span></span>
|<span data-ttu-id="696e3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="696e3-120">Header</span></span>|<span data-ttu-id="696e3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="696e3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="696e3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="696e3-122">Authorization</span></span>|<span data-ttu-id="696e3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="696e3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="696e3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="696e3-124">Accept</span></span>|<span data-ttu-id="696e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="696e3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="696e3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="696e3-126">Request body</span></span>
<span data-ttu-id="696e3-127">В тексте запроса добавьте представление объекта managedDevice в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="696e3-127">In the request body, supply a JSON representation for the managedDevice object.</span></span>

<span data-ttu-id="696e3-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedDevice.</span><span class="sxs-lookup"><span data-stu-id="696e3-128">The following table shows the properties that are required when you create the managedDevice.</span></span>

|<span data-ttu-id="696e3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="696e3-129">Property</span></span>|<span data-ttu-id="696e3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="696e3-130">Type</span></span>|<span data-ttu-id="696e3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="696e3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="696e3-132">id</span><span class="sxs-lookup"><span data-stu-id="696e3-132">id</span></span>|<span data-ttu-id="696e3-133">String</span><span class="sxs-lookup"><span data-stu-id="696e3-133">String</span></span>|<span data-ttu-id="696e3-134">Уникальный идентификатор для устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-134">Unique Identifier for the device.</span></span> <span data-ttu-id="696e3-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-135">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-136">userId</span><span class="sxs-lookup"><span data-stu-id="696e3-136">userId</span></span>|<span data-ttu-id="696e3-137">String</span><span class="sxs-lookup"><span data-stu-id="696e3-137">String</span></span>|<span data-ttu-id="696e3-138">Уникальный идентификатор для пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="696e3-138">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="696e3-139">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-139">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-140">deviceName</span><span class="sxs-lookup"><span data-stu-id="696e3-140">deviceName</span></span>|<span data-ttu-id="696e3-141">String</span><span class="sxs-lookup"><span data-stu-id="696e3-141">String</span></span>|<span data-ttu-id="696e3-142">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-142">Name of the device.</span></span> <span data-ttu-id="696e3-143">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-143">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-144">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="696e3-144">managedDeviceOwnerType</span></span>|[<span data-ttu-id="696e3-145">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="696e3-145">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="696e3-146">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="696e3-146">Ownership of the device.</span></span> <span data-ttu-id="696e3-147">Может быть "компания" или "личный".</span><span class="sxs-lookup"><span data-stu-id="696e3-147">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="696e3-148">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="696e3-148">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="696e3-149">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="696e3-149">deviceActionResults</span></span>|<span data-ttu-id="696e3-150">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="696e3-150">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="696e3-151">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="696e3-151">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="696e3-152">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-152">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-153">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="696e3-153">enrolledDateTime</span></span>|<span data-ttu-id="696e3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="696e3-154">DateTimeOffset</span></span>|<span data-ttu-id="696e3-155">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-155">Enrollment time of the device.</span></span> <span data-ttu-id="696e3-156">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-156">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-157">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="696e3-157">lastSyncDateTime</span></span>|<span data-ttu-id="696e3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="696e3-158">DateTimeOffset</span></span>|<span data-ttu-id="696e3-159">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="696e3-159">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="696e3-160">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-160">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-161">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="696e3-161">operatingSystem</span></span>|<span data-ttu-id="696e3-162">String</span><span class="sxs-lookup"><span data-stu-id="696e3-162">String</span></span>|<span data-ttu-id="696e3-163">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-163">Operating system of the device.</span></span> <span data-ttu-id="696e3-164">Windows, iOS и т. д. Это свойство только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-164">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="696e3-165">complianceState</span><span class="sxs-lookup"><span data-stu-id="696e3-165">complianceState</span></span>|[<span data-ttu-id="696e3-166">complianceState</span><span class="sxs-lookup"><span data-stu-id="696e3-166">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="696e3-167">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="696e3-167">Compliance state of the device.</span></span> <span data-ttu-id="696e3-168">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-168">This property is read-only.</span></span> <span data-ttu-id="696e3-169">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="696e3-169">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="696e3-170">jailBroken</span><span class="sxs-lookup"><span data-stu-id="696e3-170">jailBroken</span></span>|<span data-ttu-id="696e3-171">String</span><span class="sxs-lookup"><span data-stu-id="696e3-171">String</span></span>|<span data-ttu-id="696e3-172">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="696e3-172">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="696e3-173">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-173">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-174">managementAgent</span><span class="sxs-lookup"><span data-stu-id="696e3-174">managementAgent</span></span>|[<span data-ttu-id="696e3-175">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="696e3-175">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="696e3-176">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="696e3-176">Management channel of the device.</span></span> <span data-ttu-id="696e3-177">Intune, EAS и т. д. Это свойство только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-177">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="696e3-178">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="696e3-178">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="696e3-179">osVersion</span><span class="sxs-lookup"><span data-stu-id="696e3-179">osVersion</span></span>|<span data-ttu-id="696e3-180">String</span><span class="sxs-lookup"><span data-stu-id="696e3-180">String</span></span>|<span data-ttu-id="696e3-181">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-181">Operating system version of the device.</span></span> <span data-ttu-id="696e3-182">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-182">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-183">easActivated</span><span class="sxs-lookup"><span data-stu-id="696e3-183">easActivated</span></span>|<span data-ttu-id="696e3-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="696e3-184">Boolean</span></span>|<span data-ttu-id="696e3-185">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="696e3-185">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="696e3-186">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-186">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-187">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="696e3-187">easDeviceId</span></span>|<span data-ttu-id="696e3-188">String</span><span class="sxs-lookup"><span data-stu-id="696e3-188">String</span></span>|<span data-ttu-id="696e3-189">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="696e3-189">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="696e3-190">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-190">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-191">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="696e3-191">easActivationDateTime</span></span>|<span data-ttu-id="696e3-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="696e3-192">DateTimeOffset</span></span>|<span data-ttu-id="696e3-193">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="696e3-193">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="696e3-194">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-194">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-195">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="696e3-195">azureADRegistered</span></span>|<span data-ttu-id="696e3-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="696e3-196">Boolean</span></span>|<span data-ttu-id="696e3-197">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="696e3-197">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="696e3-198">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-198">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-199">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="696e3-199">deviceEnrollmentType</span></span>|[<span data-ttu-id="696e3-200">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="696e3-200">deviceEnrollmentType</span></span>](../resources/intune-devices-deviceenrollmenttype.md)|<span data-ttu-id="696e3-201">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-201">Enrollment type of the device.</span></span> <span data-ttu-id="696e3-202">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-202">This property is read-only.</span></span> <span data-ttu-id="696e3-203">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="696e3-203">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="696e3-204">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="696e3-204">activationLockBypassCode</span></span>|<span data-ttu-id="696e3-205">String</span><span class="sxs-lookup"><span data-stu-id="696e3-205">String</span></span>|<span data-ttu-id="696e3-206">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="696e3-206">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="696e3-207">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-207">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-208">emailAddress</span><span class="sxs-lookup"><span data-stu-id="696e3-208">emailAddress</span></span>|<span data-ttu-id="696e3-209">String</span><span class="sxs-lookup"><span data-stu-id="696e3-209">String</span></span>|<span data-ttu-id="696e3-210">Электронная почта (ы) для пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="696e3-210">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="696e3-211">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-211">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-212">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="696e3-212">azureADDeviceId</span></span>|<span data-ttu-id="696e3-213">String</span><span class="sxs-lookup"><span data-stu-id="696e3-213">String</span></span>|<span data-ttu-id="696e3-214">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="696e3-214">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="696e3-215">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-215">Read only.</span></span> <span data-ttu-id="696e3-216">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-216">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-217">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="696e3-217">deviceRegistrationState</span></span>|[<span data-ttu-id="696e3-218">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="696e3-218">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="696e3-219">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-219">Device registration state.</span></span> <span data-ttu-id="696e3-220">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-220">This property is read-only.</span></span> <span data-ttu-id="696e3-221">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="696e3-221">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="696e3-222">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="696e3-222">deviceCategoryDisplayName</span></span>|<span data-ttu-id="696e3-223">String</span><span class="sxs-lookup"><span data-stu-id="696e3-223">String</span></span>|<span data-ttu-id="696e3-224">Имя отображения категории устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-224">Device category display name.</span></span> <span data-ttu-id="696e3-225">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-225">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-226">isSupervised</span><span class="sxs-lookup"><span data-stu-id="696e3-226">isSupervised</span></span>|<span data-ttu-id="696e3-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="696e3-227">Boolean</span></span>|<span data-ttu-id="696e3-228">Состояние под контролем устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-228">Device supervised status.</span></span> <span data-ttu-id="696e3-229">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-229">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-230">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="696e3-230">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="696e3-231">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="696e3-231">DateTimeOffset</span></span>|<span data-ttu-id="696e3-232">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="696e3-232">Last time the device contacted Exchange.</span></span> <span data-ttu-id="696e3-233">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-233">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-234">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="696e3-234">exchangeAccessState</span></span>|[<span data-ttu-id="696e3-235">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="696e3-235">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="696e3-236">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="696e3-236">The Access State of the device in Exchange.</span></span> <span data-ttu-id="696e3-237">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-237">This property is read-only.</span></span> <span data-ttu-id="696e3-238">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="696e3-238">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="696e3-239">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="696e3-239">exchangeAccessStateReason</span></span>|[<span data-ttu-id="696e3-240">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="696e3-240">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="696e3-241">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="696e3-241">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="696e3-242">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-242">This property is read-only.</span></span> <span data-ttu-id="696e3-243">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="696e3-243">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="696e3-244">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="696e3-244">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="696e3-245">String</span><span class="sxs-lookup"><span data-stu-id="696e3-245">String</span></span>|<span data-ttu-id="696e3-246">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="696e3-246">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="696e3-247">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-247">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-248">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="696e3-248">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="696e3-249">String</span><span class="sxs-lookup"><span data-stu-id="696e3-249">String</span></span>|<span data-ttu-id="696e3-250">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="696e3-250">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="696e3-251">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-251">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-252">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="696e3-252">isEncrypted</span></span>|<span data-ttu-id="696e3-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="696e3-253">Boolean</span></span>|<span data-ttu-id="696e3-254">Состояние шифрования устройств.</span><span class="sxs-lookup"><span data-stu-id="696e3-254">Device encryption status.</span></span> <span data-ttu-id="696e3-255">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-255">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-256">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="696e3-256">userPrincipalName</span></span>|<span data-ttu-id="696e3-257">String</span><span class="sxs-lookup"><span data-stu-id="696e3-257">String</span></span>|<span data-ttu-id="696e3-258">Имя основного пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-258">Device user principal name.</span></span> <span data-ttu-id="696e3-259">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-259">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-260">model</span><span class="sxs-lookup"><span data-stu-id="696e3-260">model</span></span>|<span data-ttu-id="696e3-261">String</span><span class="sxs-lookup"><span data-stu-id="696e3-261">String</span></span>|<span data-ttu-id="696e3-262">Модель устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-262">Model of the device.</span></span> <span data-ttu-id="696e3-263">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-263">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-264">manufacturer</span><span class="sxs-lookup"><span data-stu-id="696e3-264">manufacturer</span></span>|<span data-ttu-id="696e3-265">String</span><span class="sxs-lookup"><span data-stu-id="696e3-265">String</span></span>|<span data-ttu-id="696e3-266">Производитель устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-266">Manufacturer of the device.</span></span> <span data-ttu-id="696e3-267">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-267">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-268">imei</span><span class="sxs-lookup"><span data-stu-id="696e3-268">imei</span></span>|<span data-ttu-id="696e3-269">String</span><span class="sxs-lookup"><span data-stu-id="696e3-269">String</span></span>|<span data-ttu-id="696e3-270">IMEI.</span><span class="sxs-lookup"><span data-stu-id="696e3-270">IMEI.</span></span> <span data-ttu-id="696e3-271">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-271">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-272">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="696e3-272">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="696e3-273">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="696e3-273">DateTimeOffset</span></span>|<span data-ttu-id="696e3-274">DateTime, когда истекает срок действия льготного периода соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-274">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="696e3-275">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-275">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-276">serialNumber</span><span class="sxs-lookup"><span data-stu-id="696e3-276">serialNumber</span></span>|<span data-ttu-id="696e3-277">String</span><span class="sxs-lookup"><span data-stu-id="696e3-277">String</span></span>|<span data-ttu-id="696e3-278">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="696e3-278">SerialNumber.</span></span> <span data-ttu-id="696e3-279">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-279">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-280">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="696e3-280">phoneNumber</span></span>|<span data-ttu-id="696e3-281">String</span><span class="sxs-lookup"><span data-stu-id="696e3-281">String</span></span>|<span data-ttu-id="696e3-282">Телефон номер устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-282">Phone number of the device.</span></span> <span data-ttu-id="696e3-283">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-283">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-284">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="696e3-284">androidSecurityPatchLevel</span></span>|<span data-ttu-id="696e3-285">String</span><span class="sxs-lookup"><span data-stu-id="696e3-285">String</span></span>|<span data-ttu-id="696e3-286">Уровень исправления безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="696e3-286">Android security patch level.</span></span> <span data-ttu-id="696e3-287">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-287">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-288">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="696e3-288">userDisplayName</span></span>|<span data-ttu-id="696e3-289">String</span><span class="sxs-lookup"><span data-stu-id="696e3-289">String</span></span>|<span data-ttu-id="696e3-290">Имя отображения пользователя.</span><span class="sxs-lookup"><span data-stu-id="696e3-290">User display name.</span></span> <span data-ttu-id="696e3-291">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-291">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-292">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="696e3-292">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="696e3-293">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="696e3-293">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="696e3-294">Функции с включенной поддержкой клиента ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="696e3-294">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="696e3-295">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-295">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-296">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="696e3-296">wiFiMacAddress</span></span>|<span data-ttu-id="696e3-297">String</span><span class="sxs-lookup"><span data-stu-id="696e3-297">String</span></span>|<span data-ttu-id="696e3-298">Wi-Fi MAC.</span><span class="sxs-lookup"><span data-stu-id="696e3-298">Wi-Fi MAC.</span></span> <span data-ttu-id="696e3-299">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-299">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-300">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="696e3-300">deviceHealthAttestationState</span></span>|[<span data-ttu-id="696e3-301">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="696e3-301">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="696e3-302">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-302">The device health attestation state.</span></span> <span data-ttu-id="696e3-303">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-303">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-304">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="696e3-304">subscriberCarrier</span></span>|<span data-ttu-id="696e3-305">String</span><span class="sxs-lookup"><span data-stu-id="696e3-305">String</span></span>|<span data-ttu-id="696e3-306">Оператор абонентов.</span><span class="sxs-lookup"><span data-stu-id="696e3-306">Subscriber Carrier.</span></span> <span data-ttu-id="696e3-307">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-307">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-308">meid</span><span class="sxs-lookup"><span data-stu-id="696e3-308">meid</span></span>|<span data-ttu-id="696e3-309">String</span><span class="sxs-lookup"><span data-stu-id="696e3-309">String</span></span>|<span data-ttu-id="696e3-310">MEID.</span><span class="sxs-lookup"><span data-stu-id="696e3-310">MEID.</span></span> <span data-ttu-id="696e3-311">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-311">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-312">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="696e3-312">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="696e3-313">Int64</span><span class="sxs-lookup"><span data-stu-id="696e3-313">Int64</span></span>|<span data-ttu-id="696e3-314">Итого служба хранилища в Bytes.</span><span class="sxs-lookup"><span data-stu-id="696e3-314">Total Storage in Bytes.</span></span> <span data-ttu-id="696e3-315">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-315">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-316">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="696e3-316">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="696e3-317">Int64</span><span class="sxs-lookup"><span data-stu-id="696e3-317">Int64</span></span>|<span data-ttu-id="696e3-318">Бесплатные служба хранилища в Bytes.</span><span class="sxs-lookup"><span data-stu-id="696e3-318">Free Storage in Bytes.</span></span> <span data-ttu-id="696e3-319">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-319">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-320">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="696e3-320">managedDeviceName</span></span>|<span data-ttu-id="696e3-321">String</span><span class="sxs-lookup"><span data-stu-id="696e3-321">String</span></span>|<span data-ttu-id="696e3-322">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="696e3-322">Automatically generated name to identify a device.</span></span> <span data-ttu-id="696e3-323">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="696e3-323">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="696e3-324">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="696e3-324">partnerReportedThreatState</span></span>|[<span data-ttu-id="696e3-325">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="696e3-325">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="696e3-326">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="696e3-326">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="696e3-327">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-327">Read Only.</span></span> <span data-ttu-id="696e3-328">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-328">This property is read-only.</span></span> <span data-ttu-id="696e3-329">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="696e3-329">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="696e3-330">iccid</span><span class="sxs-lookup"><span data-stu-id="696e3-330">iccid</span></span>|<span data-ttu-id="696e3-331">String</span><span class="sxs-lookup"><span data-stu-id="696e3-331">String</span></span>|<span data-ttu-id="696e3-332">Интегрированный идентификатор карты схемы — уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="696e3-332">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="696e3-333">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-333">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-334">udid</span><span class="sxs-lookup"><span data-stu-id="696e3-334">udid</span></span>|<span data-ttu-id="696e3-335">String</span><span class="sxs-lookup"><span data-stu-id="696e3-335">String</span></span>|<span data-ttu-id="696e3-336">Уникальный идентификатор устройства для устройств с iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="696e3-336">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="696e3-337">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-337">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-338">notes</span><span class="sxs-lookup"><span data-stu-id="696e3-338">notes</span></span>|<span data-ttu-id="696e3-339">String</span><span class="sxs-lookup"><span data-stu-id="696e3-339">String</span></span>|<span data-ttu-id="696e3-340">Заметки на устройстве, созданном ИТ-администратором</span><span class="sxs-lookup"><span data-stu-id="696e3-340">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="696e3-341">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="696e3-341">ethernetMacAddress</span></span>|<span data-ttu-id="696e3-342">String</span><span class="sxs-lookup"><span data-stu-id="696e3-342">String</span></span>|<span data-ttu-id="696e3-343">Mac Ethernet.</span><span class="sxs-lookup"><span data-stu-id="696e3-343">Ethernet MAC.</span></span> <span data-ttu-id="696e3-344">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-344">This property is read-only.</span></span>|
|<span data-ttu-id="696e3-345">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="696e3-345">physicalMemoryInBytes</span></span>|<span data-ttu-id="696e3-346">Int64</span><span class="sxs-lookup"><span data-stu-id="696e3-346">Int64</span></span>|<span data-ttu-id="696e3-347">Общая память в bytes.</span><span class="sxs-lookup"><span data-stu-id="696e3-347">Total Memory in Bytes.</span></span> <span data-ttu-id="696e3-348">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696e3-348">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="696e3-349">Ответ</span><span class="sxs-lookup"><span data-stu-id="696e3-349">Response</span></span>
<span data-ttu-id="696e3-350">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedDevice](../resources/intune-devices-manageddevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="696e3-350">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="696e3-351">Пример</span><span class="sxs-lookup"><span data-stu-id="696e3-351">Example</span></span>

### <a name="request"></a><span data-ttu-id="696e3-352">Запрос</span><span class="sxs-lookup"><span data-stu-id="696e3-352">Request</span></span>
<span data-ttu-id="696e3-353">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="696e3-353">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 4821

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "notes": "Notes value",
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5
}
```

### <a name="response"></a><span data-ttu-id="696e3-354">Отклик</span><span class="sxs-lookup"><span data-stu-id="696e3-354">Response</span></span>
<span data-ttu-id="696e3-p153">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="696e3-p153">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4870

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "notes": "Notes value",
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5
}
```




