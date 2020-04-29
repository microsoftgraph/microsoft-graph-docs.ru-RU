---
title: Обновление managedDevice
description: Обновление свойств объекта managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 55e63802783035e7a418ea6dd3041240685c228c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474487"
---
# <a name="update-manageddevice"></a><span data-ttu-id="1a396-103">Обновление managedDevice</span><span class="sxs-lookup"><span data-stu-id="1a396-103">Update managedDevice</span></span>

<span data-ttu-id="1a396-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a396-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a396-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a396-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a396-106">Обновление свойств объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1a396-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a396-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1a396-107">Prerequisites</span></span>
<span data-ttu-id="1a396-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a396-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a396-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a396-110">Permission type</span></span>|<span data-ttu-id="1a396-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a396-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a396-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a396-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a396-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a396-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1a396-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a396-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a396-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a396-115">Not supported.</span></span>|
|<span data-ttu-id="1a396-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a396-116">Application</span></span>|<span data-ttu-id="1a396-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a396-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a396-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a396-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="1a396-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1a396-119">Request headers</span></span>
|<span data-ttu-id="1a396-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a396-120">Header</span></span>|<span data-ttu-id="1a396-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1a396-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a396-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a396-122">Authorization</span></span>|<span data-ttu-id="1a396-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a396-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a396-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1a396-124">Accept</span></span>|<span data-ttu-id="1a396-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a396-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a396-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a396-126">Request body</span></span>
<span data-ttu-id="1a396-127">В теле запроса добавьте представление объекта [managedDevice](../resources/intune-devices-manageddevice.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a396-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="1a396-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1a396-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="1a396-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a396-129">Property</span></span>|<span data-ttu-id="1a396-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1a396-130">Type</span></span>|<span data-ttu-id="1a396-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1a396-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a396-132">id</span><span class="sxs-lookup"><span data-stu-id="1a396-132">id</span></span>|<span data-ttu-id="1a396-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1a396-133">String</span></span>|<span data-ttu-id="1a396-134">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="1a396-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="1a396-135">userId</span><span class="sxs-lookup"><span data-stu-id="1a396-135">userId</span></span>|<span data-ttu-id="1a396-136">String</span><span class="sxs-lookup"><span data-stu-id="1a396-136">String</span></span>|<span data-ttu-id="1a396-137">Уникальный идентификатор пользователя, связанного с устройством.
</span><span class="sxs-lookup"><span data-stu-id="1a396-137">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="1a396-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="1a396-138">deviceName</span></span>|<span data-ttu-id="1a396-139">String</span><span class="sxs-lookup"><span data-stu-id="1a396-139">String</span></span>|<span data-ttu-id="1a396-140">Название устройства</span><span class="sxs-lookup"><span data-stu-id="1a396-140">Name of the device</span></span>|
|<span data-ttu-id="1a396-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="1a396-141">managedDeviceOwnerType</span></span>|[<span data-ttu-id="1a396-142">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="1a396-142">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="1a396-143">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="1a396-143">Ownership of the device.</span></span> <span data-ttu-id="1a396-144">Может быть "Company" или "Personal".</span><span class="sxs-lookup"><span data-stu-id="1a396-144">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="1a396-145">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="1a396-145">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="1a396-146">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="1a396-146">deviceActionResults</span></span>|<span data-ttu-id="1a396-147">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1a396-147">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="1a396-148">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="1a396-148">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="1a396-149">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="1a396-149">enrolledDateTime</span></span>|<span data-ttu-id="1a396-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a396-150">DateTimeOffset</span></span>|<span data-ttu-id="1a396-151">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="1a396-151">Enrollment time of the device.</span></span>|
|<span data-ttu-id="1a396-152">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1a396-152">lastSyncDateTime</span></span>|<span data-ttu-id="1a396-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a396-153">DateTimeOffset</span></span>|<span data-ttu-id="1a396-154">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="1a396-154">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="1a396-155">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="1a396-155">operatingSystem</span></span>|<span data-ttu-id="1a396-156">String</span><span class="sxs-lookup"><span data-stu-id="1a396-156">String</span></span>|<span data-ttu-id="1a396-157">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="1a396-157">Operating system of the device.</span></span> <span data-ttu-id="1a396-158">Windows, iOS и т. д.</span><span class="sxs-lookup"><span data-stu-id="1a396-158">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="1a396-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="1a396-159">complianceState</span></span>|[<span data-ttu-id="1a396-160">complianceState</span><span class="sxs-lookup"><span data-stu-id="1a396-160">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="1a396-161">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="1a396-161">Compliance state of the device.</span></span> <span data-ttu-id="1a396-162">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="1a396-162">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="1a396-163">jailBroken</span><span class="sxs-lookup"><span data-stu-id="1a396-163">jailBroken</span></span>|<span data-ttu-id="1a396-164">String</span><span class="sxs-lookup"><span data-stu-id="1a396-164">String</span></span>|<span data-ttu-id="1a396-165">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="1a396-165">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="1a396-166">managementAgent</span><span class="sxs-lookup"><span data-stu-id="1a396-166">managementAgent</span></span>|[<span data-ttu-id="1a396-167">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="1a396-167">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="1a396-168">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="1a396-168">Management channel of the device.</span></span> <span data-ttu-id="1a396-169">Intune, EAS и т. д. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="1a396-169">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="1a396-170">osVersion</span><span class="sxs-lookup"><span data-stu-id="1a396-170">osVersion</span></span>|<span data-ttu-id="1a396-171">String</span><span class="sxs-lookup"><span data-stu-id="1a396-171">String</span></span>|<span data-ttu-id="1a396-172">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="1a396-172">Operating system version of the device.</span></span>|
|<span data-ttu-id="1a396-173">easActivated</span><span class="sxs-lookup"><span data-stu-id="1a396-173">easActivated</span></span>|<span data-ttu-id="1a396-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a396-174">Boolean</span></span>|<span data-ttu-id="1a396-175">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="1a396-175">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="1a396-176">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="1a396-176">easDeviceId</span></span>|<span data-ttu-id="1a396-177">String</span><span class="sxs-lookup"><span data-stu-id="1a396-177">String</span></span>|<span data-ttu-id="1a396-178">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="1a396-178">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="1a396-179">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="1a396-179">easActivationDateTime</span></span>|<span data-ttu-id="1a396-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a396-180">DateTimeOffset</span></span>|<span data-ttu-id="1a396-181">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="1a396-181">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="1a396-182">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="1a396-182">azureADRegistered</span></span>|<span data-ttu-id="1a396-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a396-183">Boolean</span></span>|<span data-ttu-id="1a396-184">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1a396-184">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="1a396-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="1a396-185">deviceEnrollmentType</span></span>|[<span data-ttu-id="1a396-186">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="1a396-186">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="1a396-187">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="1a396-187">Enrollment type of the device.</span></span> <span data-ttu-id="1a396-188">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="1a396-188">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="1a396-189">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="1a396-189">activationLockBypassCode</span></span>|<span data-ttu-id="1a396-190">String</span><span class="sxs-lookup"><span data-stu-id="1a396-190">String</span></span>|<span data-ttu-id="1a396-191">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="1a396-191">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="1a396-192">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1a396-192">emailAddress</span></span>|<span data-ttu-id="1a396-193">String</span><span class="sxs-lookup"><span data-stu-id="1a396-193">String</span></span>|<span data-ttu-id="1a396-194">Адреса электронной почты пользователя, связанного с устройством</span><span class="sxs-lookup"><span data-stu-id="1a396-194">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="1a396-195">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="1a396-195">azureADDeviceId</span></span>|<span data-ttu-id="1a396-196">String</span><span class="sxs-lookup"><span data-stu-id="1a396-196">String</span></span>|<span data-ttu-id="1a396-197">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1a396-197">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="1a396-198">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1a396-198">Read only.</span></span>|
|<span data-ttu-id="1a396-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="1a396-199">deviceRegistrationState</span></span>|[<span data-ttu-id="1a396-200">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="1a396-200">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="1a396-201">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="1a396-201">Device registration state.</span></span> <span data-ttu-id="1a396-202">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="1a396-202">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="1a396-203">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="1a396-203">deviceCategoryDisplayName</span></span>|<span data-ttu-id="1a396-204">String</span><span class="sxs-lookup"><span data-stu-id="1a396-204">String</span></span>|<span data-ttu-id="1a396-205">Отображаемое имя категории устройства</span><span class="sxs-lookup"><span data-stu-id="1a396-205">Device category display name</span></span>|
|<span data-ttu-id="1a396-206">isSupervised</span><span class="sxs-lookup"><span data-stu-id="1a396-206">isSupervised</span></span>|<span data-ttu-id="1a396-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a396-207">Boolean</span></span>|<span data-ttu-id="1a396-208">Состояние защиты устройства</span><span class="sxs-lookup"><span data-stu-id="1a396-208">Device supervised status</span></span>|
|<span data-ttu-id="1a396-209">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1a396-209">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="1a396-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a396-210">DateTimeOffset</span></span>|<span data-ttu-id="1a396-211">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a396-211">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="1a396-212">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="1a396-212">exchangeAccessState</span></span>|[<span data-ttu-id="1a396-213">девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="1a396-213">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="1a396-214">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a396-214">The Access State of the device in Exchange.</span></span> <span data-ttu-id="1a396-215">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="1a396-215">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="1a396-216">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="1a396-216">exchangeAccessStateReason</span></span>|[<span data-ttu-id="1a396-217">девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="1a396-217">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="1a396-218">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a396-218">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="1a396-219">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="1a396-219">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="1a396-220">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="1a396-220">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="1a396-221">String</span><span class="sxs-lookup"><span data-stu-id="1a396-221">String</span></span>|<span data-ttu-id="1a396-222">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="1a396-222">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="1a396-223">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="1a396-223">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="1a396-224">String</span><span class="sxs-lookup"><span data-stu-id="1a396-224">String</span></span>|<span data-ttu-id="1a396-225">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="1a396-225">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="1a396-226">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="1a396-226">isEncrypted</span></span>|<span data-ttu-id="1a396-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a396-227">Boolean</span></span>|<span data-ttu-id="1a396-228">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="1a396-228">Device encryption status</span></span>|
|<span data-ttu-id="1a396-229">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1a396-229">userPrincipalName</span></span>|<span data-ttu-id="1a396-230">String</span><span class="sxs-lookup"><span data-stu-id="1a396-230">String</span></span>|<span data-ttu-id="1a396-231">Имя участника-пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="1a396-231">Device user principal name</span></span>|
|<span data-ttu-id="1a396-232">model</span><span class="sxs-lookup"><span data-stu-id="1a396-232">model</span></span>|<span data-ttu-id="1a396-233">String</span><span class="sxs-lookup"><span data-stu-id="1a396-233">String</span></span>|<span data-ttu-id="1a396-234">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="1a396-234">Model of the device</span></span>|
|<span data-ttu-id="1a396-235">manufacturer</span><span class="sxs-lookup"><span data-stu-id="1a396-235">manufacturer</span></span>|<span data-ttu-id="1a396-236">String</span><span class="sxs-lookup"><span data-stu-id="1a396-236">String</span></span>|<span data-ttu-id="1a396-237">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="1a396-237">Manufacturer of the device</span></span>|
|<span data-ttu-id="1a396-238">imei</span><span class="sxs-lookup"><span data-stu-id="1a396-238">imei</span></span>|<span data-ttu-id="1a396-239">String</span><span class="sxs-lookup"><span data-stu-id="1a396-239">String</span></span>|<span data-ttu-id="1a396-240">IMEI</span><span class="sxs-lookup"><span data-stu-id="1a396-240">IMEI</span></span>|
|<span data-ttu-id="1a396-241">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1a396-241">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="1a396-242">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a396-242">DateTimeOffset</span></span>|<span data-ttu-id="1a396-243">Дата и время истечения льготного периода соответствия устройства требованиям</span><span class="sxs-lookup"><span data-stu-id="1a396-243">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="1a396-244">serialNumber</span><span class="sxs-lookup"><span data-stu-id="1a396-244">serialNumber</span></span>|<span data-ttu-id="1a396-245">Строка</span><span class="sxs-lookup"><span data-stu-id="1a396-245">String</span></span>|<span data-ttu-id="1a396-246">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="1a396-246">SerialNumber</span></span>|
|<span data-ttu-id="1a396-247">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="1a396-247">phoneNumber</span></span>|<span data-ttu-id="1a396-248">String</span><span class="sxs-lookup"><span data-stu-id="1a396-248">String</span></span>|<span data-ttu-id="1a396-249">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="1a396-249">Phone number of the device</span></span>|
|<span data-ttu-id="1a396-250">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="1a396-250">androidSecurityPatchLevel</span></span>|<span data-ttu-id="1a396-251">String</span><span class="sxs-lookup"><span data-stu-id="1a396-251">String</span></span>|<span data-ttu-id="1a396-252">Уровень обновления для системы безопасности Android</span><span class="sxs-lookup"><span data-stu-id="1a396-252">Android security patch level</span></span>|
|<span data-ttu-id="1a396-253">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1a396-253">userDisplayName</span></span>|<span data-ttu-id="1a396-254">String</span><span class="sxs-lookup"><span data-stu-id="1a396-254">String</span></span>|<span data-ttu-id="1a396-255">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="1a396-255">User display name</span></span>|
|<span data-ttu-id="1a396-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="1a396-256">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="1a396-257">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="1a396-257">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="1a396-258">Включенные функции клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="1a396-258">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="1a396-259">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="1a396-259">wiFiMacAddress</span></span>|<span data-ttu-id="1a396-260">String</span><span class="sxs-lookup"><span data-stu-id="1a396-260">String</span></span>|<span data-ttu-id="1a396-261">MAC-адрес сети Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="1a396-261">Wi-Fi MAC</span></span>|
|<span data-ttu-id="1a396-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="1a396-262">deviceHealthAttestationState</span></span>|[<span data-ttu-id="1a396-263">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="1a396-263">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="1a396-264">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="1a396-264">The device health attestation state.</span></span>|
|<span data-ttu-id="1a396-265">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="1a396-265">subscriberCarrier</span></span>|<span data-ttu-id="1a396-266">String</span><span class="sxs-lookup"><span data-stu-id="1a396-266">String</span></span>|<span data-ttu-id="1a396-267">Оператор сотовой связи, используемый абонентом</span><span class="sxs-lookup"><span data-stu-id="1a396-267">Subscriber Carrier</span></span>|
|<span data-ttu-id="1a396-268">meid</span><span class="sxs-lookup"><span data-stu-id="1a396-268">meid</span></span>|<span data-ttu-id="1a396-269">String</span><span class="sxs-lookup"><span data-stu-id="1a396-269">String</span></span>|<span data-ttu-id="1a396-270">MEID</span><span class="sxs-lookup"><span data-stu-id="1a396-270">MEID</span></span>|
|<span data-ttu-id="1a396-271">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="1a396-271">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="1a396-272">Int64</span><span class="sxs-lookup"><span data-stu-id="1a396-272">Int64</span></span>|<span data-ttu-id="1a396-273">Общий объем хранилища в байтах</span><span class="sxs-lookup"><span data-stu-id="1a396-273">Total Storage in Bytes</span></span>|
|<span data-ttu-id="1a396-274">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="1a396-274">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="1a396-275">Int64</span><span class="sxs-lookup"><span data-stu-id="1a396-275">Int64</span></span>|<span data-ttu-id="1a396-276">Свободный объем хранилища в байтах
</span><span class="sxs-lookup"><span data-stu-id="1a396-276">Free Storage in Bytes</span></span>|
|<span data-ttu-id="1a396-277">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="1a396-277">managedDeviceName</span></span>|<span data-ttu-id="1a396-278">String</span><span class="sxs-lookup"><span data-stu-id="1a396-278">String</span></span>|<span data-ttu-id="1a396-279">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="1a396-279">Automatically generated name to identify a device.</span></span> <span data-ttu-id="1a396-280">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="1a396-280">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="1a396-281">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="1a396-281">partnerReportedThreatState</span></span>|[<span data-ttu-id="1a396-282">манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="1a396-282">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="1a396-283">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="1a396-283">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="1a396-284">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1a396-284">Read Only.</span></span> <span data-ttu-id="1a396-285">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="1a396-285">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="1a396-286">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a396-286">Response</span></span>
<span data-ttu-id="1a396-287">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDevice](../resources/intune-devices-manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1a396-287">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a396-288">Пример</span><span class="sxs-lookup"><span data-stu-id="1a396-288">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a396-289">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a396-289">Request</span></span>
<span data-ttu-id="1a396-290">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a396-290">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1a396-291">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a396-291">Response</span></span>
<span data-ttu-id="1a396-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a396-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






