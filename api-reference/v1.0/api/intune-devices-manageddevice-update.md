---
title: Обновление managedDevice
description: Обновление свойств объекта managedDevice.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 242b9416b94072348fb1bfa1adc07d93274e45d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835702"
---
# <a name="update-manageddevice"></a><span data-ttu-id="a1eef-103">Обновление managedDevice</span><span class="sxs-lookup"><span data-stu-id="a1eef-103">Update managedDevice</span></span>

> <span data-ttu-id="a1eef-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a1eef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1eef-105">Обновление свойств объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="a1eef-105">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1eef-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a1eef-106">Prerequisites</span></span>
<span data-ttu-id="a1eef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1eef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1eef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1eef-109">Permission type</span></span>|<span data-ttu-id="a1eef-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1eef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1eef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1eef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a1eef-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1eef-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a1eef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1eef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1eef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1eef-114">Not supported.</span></span>|
|<span data-ttu-id="a1eef-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1eef-115">Application</span></span>|<span data-ttu-id="a1eef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1eef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1eef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1eef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="a1eef-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1eef-118">Request headers</span></span>
|<span data-ttu-id="a1eef-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1eef-119">Header</span></span>|<span data-ttu-id="a1eef-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a1eef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1eef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1eef-121">Authorization</span></span>|<span data-ttu-id="a1eef-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a1eef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1eef-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a1eef-123">Accept</span></span>|<span data-ttu-id="a1eef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a1eef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1eef-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1eef-125">Request body</span></span>
<span data-ttu-id="a1eef-126">В теле запроса добавьте представление объекта [managedDevice](../resources/intune-devices-manageddevice.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1eef-126">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="a1eef-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="a1eef-127">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="a1eef-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1eef-128">Property</span></span>|<span data-ttu-id="a1eef-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a1eef-129">Type</span></span>|<span data-ttu-id="a1eef-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a1eef-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1eef-131">id</span><span class="sxs-lookup"><span data-stu-id="a1eef-131">id</span></span>|<span data-ttu-id="a1eef-132">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-132">String</span></span>|<span data-ttu-id="a1eef-133">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="a1eef-133">Unique Identifier for the device</span></span>|
|<span data-ttu-id="a1eef-134">userId</span><span class="sxs-lookup"><span data-stu-id="a1eef-134">userId</span></span>|<span data-ttu-id="a1eef-135">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-135">String</span></span>|<span data-ttu-id="a1eef-136">Уникальный идентификатор пользователя, связанного с устройством.
</span><span class="sxs-lookup"><span data-stu-id="a1eef-136">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="a1eef-137">deviceName</span><span class="sxs-lookup"><span data-stu-id="a1eef-137">deviceName</span></span>|<span data-ttu-id="a1eef-138">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-138">String</span></span>|<span data-ttu-id="a1eef-139">Название устройства</span><span class="sxs-lookup"><span data-stu-id="a1eef-139">Name of the device</span></span>|
|<span data-ttu-id="a1eef-140">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="a1eef-140">managedDeviceOwnerType</span></span>|[<span data-ttu-id="a1eef-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="a1eef-141">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="a1eef-142">Владельцем устройства.</span><span class="sxs-lookup"><span data-stu-id="a1eef-142">Ownership of the device.</span></span> <span data-ttu-id="a1eef-143">Может быть «компания» или «личные».</span><span class="sxs-lookup"><span data-stu-id="a1eef-143">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="a1eef-144">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="a1eef-144">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="a1eef-145">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="a1eef-145">deviceActionResults</span></span>|<span data-ttu-id="a1eef-146">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a1eef-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="a1eef-147">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="a1eef-147">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="a1eef-148">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="a1eef-148">enrolledDateTime</span></span>|<span data-ttu-id="a1eef-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1eef-149">DateTimeOffset</span></span>|<span data-ttu-id="a1eef-150">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="a1eef-150">Enrollment time of the device.</span></span>|
|<span data-ttu-id="a1eef-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a1eef-151">lastSyncDateTime</span></span>|<span data-ttu-id="a1eef-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1eef-152">DateTimeOffset</span></span>|<span data-ttu-id="a1eef-153">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="a1eef-153">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="a1eef-154">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="a1eef-154">operatingSystem</span></span>|<span data-ttu-id="a1eef-155">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-155">String</span></span>|<span data-ttu-id="a1eef-156">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="a1eef-156">Operating system of the device.</span></span> <span data-ttu-id="a1eef-157">Windows, iOS и т. д.</span><span class="sxs-lookup"><span data-stu-id="a1eef-157">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="a1eef-158">complianceState</span><span class="sxs-lookup"><span data-stu-id="a1eef-158">complianceState</span></span>|[<span data-ttu-id="a1eef-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="a1eef-159">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="a1eef-160">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="a1eef-160">Compliance state of the device.</span></span> <span data-ttu-id="a1eef-161">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="a1eef-161">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="a1eef-162">jailBroken</span><span class="sxs-lookup"><span data-stu-id="a1eef-162">jailBroken</span></span>|<span data-ttu-id="a1eef-163">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-163">String</span></span>|<span data-ttu-id="a1eef-164">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="a1eef-164">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="a1eef-165">managementAgent</span><span class="sxs-lookup"><span data-stu-id="a1eef-165">managementAgent</span></span>|[<span data-ttu-id="a1eef-166">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="a1eef-166">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="a1eef-167">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="a1eef-167">Management channel of the device.</span></span> <span data-ttu-id="a1eef-168">Intune, EAS и т. д. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="a1eef-168">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="a1eef-169">osVersion</span><span class="sxs-lookup"><span data-stu-id="a1eef-169">osVersion</span></span>|<span data-ttu-id="a1eef-170">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-170">String</span></span>|<span data-ttu-id="a1eef-171">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="a1eef-171">Operating system version of the device.</span></span>|
|<span data-ttu-id="a1eef-172">easActivated</span><span class="sxs-lookup"><span data-stu-id="a1eef-172">easActivated</span></span>|<span data-ttu-id="a1eef-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1eef-173">Boolean</span></span>|<span data-ttu-id="a1eef-174">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="a1eef-174">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="a1eef-175">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="a1eef-175">easDeviceId</span></span>|<span data-ttu-id="a1eef-176">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-176">String</span></span>|<span data-ttu-id="a1eef-177">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="a1eef-177">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="a1eef-178">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="a1eef-178">easActivationDateTime</span></span>|<span data-ttu-id="a1eef-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1eef-179">DateTimeOffset</span></span>|<span data-ttu-id="a1eef-180">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="a1eef-180">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="a1eef-181">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="a1eef-181">azureADRegistered</span></span>|<span data-ttu-id="a1eef-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1eef-182">Boolean</span></span>|<span data-ttu-id="a1eef-183">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a1eef-183">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="a1eef-184">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a1eef-184">deviceEnrollmentType</span></span>|[<span data-ttu-id="a1eef-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a1eef-185">deviceEnrollmentType</span></span>](../resources/intune-devices-deviceenrollmenttype.md)|<span data-ttu-id="a1eef-186">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="a1eef-186">Enrollment type of the device.</span></span> <span data-ttu-id="a1eef-187">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="a1eef-187">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="a1eef-188">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="a1eef-188">activationLockBypassCode</span></span>|<span data-ttu-id="a1eef-189">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-189">String</span></span>|<span data-ttu-id="a1eef-190">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a1eef-190">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="a1eef-191">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a1eef-191">emailAddress</span></span>|<span data-ttu-id="a1eef-192">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-192">String</span></span>|<span data-ttu-id="a1eef-193">Адреса электронной почты пользователя, связанного с устройством</span><span class="sxs-lookup"><span data-stu-id="a1eef-193">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="a1eef-194">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="a1eef-194">azureADDeviceId</span></span>|<span data-ttu-id="a1eef-195">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-195">String</span></span>|<span data-ttu-id="a1eef-196">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a1eef-196">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="a1eef-197">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a1eef-197">Read only.</span></span>|
|<span data-ttu-id="a1eef-198">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="a1eef-198">deviceRegistrationState</span></span>|[<span data-ttu-id="a1eef-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="a1eef-199">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="a1eef-200">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="a1eef-200">Device registration state.</span></span> <span data-ttu-id="a1eef-201">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a1eef-201">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="a1eef-202">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="a1eef-202">deviceCategoryDisplayName</span></span>|<span data-ttu-id="a1eef-203">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-203">String</span></span>|<span data-ttu-id="a1eef-204">Отображаемое имя категории устройства</span><span class="sxs-lookup"><span data-stu-id="a1eef-204">Device category display name</span></span>|
|<span data-ttu-id="a1eef-205">isSupervised</span><span class="sxs-lookup"><span data-stu-id="a1eef-205">isSupervised</span></span>|<span data-ttu-id="a1eef-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1eef-206">Boolean</span></span>|<span data-ttu-id="a1eef-207">Состояние защиты устройства</span><span class="sxs-lookup"><span data-stu-id="a1eef-207">Device supervised status</span></span>|
|<span data-ttu-id="a1eef-208">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a1eef-208">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="a1eef-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1eef-209">DateTimeOffset</span></span>|<span data-ttu-id="a1eef-210">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1eef-210">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="a1eef-211">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="a1eef-211">exchangeAccessState</span></span>|[<span data-ttu-id="a1eef-212">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="a1eef-212">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="a1eef-213">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1eef-213">The Access State of the device in Exchange.</span></span> <span data-ttu-id="a1eef-214">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="a1eef-214">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="a1eef-215">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="a1eef-215">exchangeAccessStateReason</span></span>|[<span data-ttu-id="a1eef-216">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="a1eef-216">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="a1eef-217">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1eef-217">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="a1eef-218">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="a1eef-218">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="a1eef-219">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="a1eef-219">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="a1eef-220">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-220">String</span></span>|<span data-ttu-id="a1eef-221">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="a1eef-221">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="a1eef-222">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="a1eef-222">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="a1eef-223">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-223">String</span></span>|<span data-ttu-id="a1eef-224">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="a1eef-224">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="a1eef-225">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="a1eef-225">isEncrypted</span></span>|<span data-ttu-id="a1eef-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1eef-226">Boolean</span></span>|<span data-ttu-id="a1eef-227">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="a1eef-227">Device encryption status</span></span>|
|<span data-ttu-id="a1eef-228">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a1eef-228">userPrincipalName</span></span>|<span data-ttu-id="a1eef-229">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-229">String</span></span>|<span data-ttu-id="a1eef-230">Имя участника-пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="a1eef-230">Device user principal name</span></span>|
|<span data-ttu-id="a1eef-231">model</span><span class="sxs-lookup"><span data-stu-id="a1eef-231">model</span></span>|<span data-ttu-id="a1eef-232">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-232">String</span></span>|<span data-ttu-id="a1eef-233">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="a1eef-233">Model of the device</span></span>|
|<span data-ttu-id="a1eef-234">manufacturer</span><span class="sxs-lookup"><span data-stu-id="a1eef-234">manufacturer</span></span>|<span data-ttu-id="a1eef-235">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-235">String</span></span>|<span data-ttu-id="a1eef-236">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="a1eef-236">Manufacturer of the device</span></span>|
|<span data-ttu-id="a1eef-237">imei</span><span class="sxs-lookup"><span data-stu-id="a1eef-237">imei</span></span>|<span data-ttu-id="a1eef-238">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-238">String</span></span>|<span data-ttu-id="a1eef-239">IMEI</span><span class="sxs-lookup"><span data-stu-id="a1eef-239">IMEI</span></span>|
|<span data-ttu-id="a1eef-240">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a1eef-240">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a1eef-241">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1eef-241">DateTimeOffset</span></span>|<span data-ttu-id="a1eef-242">Дата и время истечения льготного периода соответствия устройства требованиям</span><span class="sxs-lookup"><span data-stu-id="a1eef-242">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="a1eef-243">serialNumber</span><span class="sxs-lookup"><span data-stu-id="a1eef-243">serialNumber</span></span>|<span data-ttu-id="a1eef-244">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-244">String</span></span>|<span data-ttu-id="a1eef-245">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="a1eef-245">SerialNumber</span></span>|
|<span data-ttu-id="a1eef-246">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="a1eef-246">phoneNumber</span></span>|<span data-ttu-id="a1eef-247">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-247">String</span></span>|<span data-ttu-id="a1eef-248">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="a1eef-248">Phone number of the device</span></span>|
|<span data-ttu-id="a1eef-249">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="a1eef-249">androidSecurityPatchLevel</span></span>|<span data-ttu-id="a1eef-250">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-250">String</span></span>|<span data-ttu-id="a1eef-251">Уровень обновления для системы безопасности Android</span><span class="sxs-lookup"><span data-stu-id="a1eef-251">Android security patch level</span></span>|
|<span data-ttu-id="a1eef-252">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a1eef-252">userDisplayName</span></span>|<span data-ttu-id="a1eef-253">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-253">String</span></span>|<span data-ttu-id="a1eef-254">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="a1eef-254">User display name</span></span>|
|<span data-ttu-id="a1eef-255">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="a1eef-255">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="a1eef-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="a1eef-256">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="a1eef-257">Включенные функции клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="a1eef-257">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="a1eef-258">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="a1eef-258">wiFiMacAddress</span></span>|<span data-ttu-id="a1eef-259">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-259">String</span></span>|<span data-ttu-id="a1eef-260">MAC-адрес сети Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="a1eef-260">Wi-Fi MAC</span></span>|
|<span data-ttu-id="a1eef-261">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="a1eef-261">deviceHealthAttestationState</span></span>|[<span data-ttu-id="a1eef-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="a1eef-262">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="a1eef-263">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="a1eef-263">The device health attestation state.</span></span>|
|<span data-ttu-id="a1eef-264">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="a1eef-264">subscriberCarrier</span></span>|<span data-ttu-id="a1eef-265">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-265">String</span></span>|<span data-ttu-id="a1eef-266">Оператор сотовой связи, используемый абонентом</span><span class="sxs-lookup"><span data-stu-id="a1eef-266">Subscriber Carrier</span></span>|
|<span data-ttu-id="a1eef-267">meid</span><span class="sxs-lookup"><span data-stu-id="a1eef-267">meid</span></span>|<span data-ttu-id="a1eef-268">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-268">String</span></span>|<span data-ttu-id="a1eef-269">MEID</span><span class="sxs-lookup"><span data-stu-id="a1eef-269">MEID</span></span>|
|<span data-ttu-id="a1eef-270">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="a1eef-270">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="a1eef-271">Int64</span><span class="sxs-lookup"><span data-stu-id="a1eef-271">Int64</span></span>|<span data-ttu-id="a1eef-272">Общий объем хранилища в байтах</span><span class="sxs-lookup"><span data-stu-id="a1eef-272">Total Storage in Bytes</span></span>|
|<span data-ttu-id="a1eef-273">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="a1eef-273">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="a1eef-274">Int64</span><span class="sxs-lookup"><span data-stu-id="a1eef-274">Int64</span></span>|<span data-ttu-id="a1eef-275">Свободный объем хранилища в байтах
</span><span class="sxs-lookup"><span data-stu-id="a1eef-275">Free Storage in Bytes</span></span>|
|<span data-ttu-id="a1eef-276">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="a1eef-276">managedDeviceName</span></span>|<span data-ttu-id="a1eef-277">String</span><span class="sxs-lookup"><span data-stu-id="a1eef-277">String</span></span>|<span data-ttu-id="a1eef-278">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="a1eef-278">Automatically generated name to identify a device.</span></span> <span data-ttu-id="a1eef-279">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="a1eef-279">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="a1eef-280">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="a1eef-280">partnerReportedThreatState</span></span>|[<span data-ttu-id="a1eef-281">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="a1eef-281">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="a1eef-282">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="a1eef-282">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="a1eef-283">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a1eef-283">Read Only.</span></span> <span data-ttu-id="a1eef-284">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="a1eef-284">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="a1eef-285">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1eef-285">Response</span></span>
<span data-ttu-id="a1eef-286">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDevice](../resources/intune-devices-manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a1eef-286">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1eef-287">Пример</span><span class="sxs-lookup"><span data-stu-id="a1eef-287">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1eef-288">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1eef-288">Request</span></span>
<span data-ttu-id="a1eef-289">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1eef-289">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 4656

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
  "partnerReportedThreatState": "activated"
}
```

### <a name="response"></a><span data-ttu-id="a1eef-290">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1eef-290">Response</span></span>
<span data-ttu-id="a1eef-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a1eef-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4705

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
  "partnerReportedThreatState": "activated"
}
```



