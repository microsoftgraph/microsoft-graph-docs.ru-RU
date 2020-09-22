---
title: Create managedDevice
description: Создание объекта managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f78891af7a5175381e5ea7a9dd73dd5552b5ca57
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009515"
---
# <a name="create-manageddevice"></a><span data-ttu-id="0bdda-103">Create managedDevice</span><span class="sxs-lookup"><span data-stu-id="0bdda-103">Create managedDevice</span></span>

<span data-ttu-id="0bdda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bdda-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bdda-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0bdda-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bdda-106">Создание объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="0bdda-106">Create a new [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bdda-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0bdda-107">Prerequisites</span></span>
<span data-ttu-id="0bdda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bdda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bdda-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0bdda-110">Permission type</span></span>|<span data-ttu-id="0bdda-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0bdda-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bdda-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0bdda-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0bdda-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bdda-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0bdda-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0bdda-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bdda-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bdda-115">Not supported.</span></span>|
|<span data-ttu-id="0bdda-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0bdda-116">Application</span></span>|<span data-ttu-id="0bdda-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bdda-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bdda-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0bdda-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="0bdda-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0bdda-119">Request headers</span></span>
|<span data-ttu-id="0bdda-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0bdda-120">Header</span></span>|<span data-ttu-id="0bdda-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0bdda-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bdda-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bdda-122">Authorization</span></span>|<span data-ttu-id="0bdda-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0bdda-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bdda-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0bdda-124">Accept</span></span>|<span data-ttu-id="0bdda-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0bdda-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bdda-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0bdda-126">Request body</span></span>
<span data-ttu-id="0bdda-127">В тексте запроса добавьте представление объекта managedDevice в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0bdda-127">In the request body, supply a JSON representation for the managedDevice object.</span></span>

<span data-ttu-id="0bdda-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedDevice.</span><span class="sxs-lookup"><span data-stu-id="0bdda-128">The following table shows the properties that are required when you create the managedDevice.</span></span>

|<span data-ttu-id="0bdda-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0bdda-129">Property</span></span>|<span data-ttu-id="0bdda-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0bdda-130">Type</span></span>|<span data-ttu-id="0bdda-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0bdda-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bdda-132">id</span><span class="sxs-lookup"><span data-stu-id="0bdda-132">id</span></span>|<span data-ttu-id="0bdda-133">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-133">String</span></span>|<span data-ttu-id="0bdda-134">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="0bdda-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="0bdda-135">userId</span><span class="sxs-lookup"><span data-stu-id="0bdda-135">userId</span></span>|<span data-ttu-id="0bdda-136">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-136">String</span></span>|<span data-ttu-id="0bdda-137">Уникальный идентификатор пользователя, связанного с устройством.
</span><span class="sxs-lookup"><span data-stu-id="0bdda-137">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="0bdda-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="0bdda-138">deviceName</span></span>|<span data-ttu-id="0bdda-139">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-139">String</span></span>|<span data-ttu-id="0bdda-140">Название устройства</span><span class="sxs-lookup"><span data-stu-id="0bdda-140">Name of the device</span></span>|
|<span data-ttu-id="0bdda-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="0bdda-141">managedDeviceOwnerType</span></span>|[<span data-ttu-id="0bdda-142">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="0bdda-142">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="0bdda-143">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="0bdda-143">Ownership of the device.</span></span> <span data-ttu-id="0bdda-144">Может быть "Company" или "Personal".</span><span class="sxs-lookup"><span data-stu-id="0bdda-144">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="0bdda-145">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="0bdda-145">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="0bdda-146">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="0bdda-146">deviceActionResults</span></span>|<span data-ttu-id="0bdda-147">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0bdda-147">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="0bdda-148">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="0bdda-148">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="0bdda-149">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="0bdda-149">enrolledDateTime</span></span>|<span data-ttu-id="0bdda-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bdda-150">DateTimeOffset</span></span>|<span data-ttu-id="0bdda-151">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="0bdda-151">Enrollment time of the device.</span></span>|
|<span data-ttu-id="0bdda-152">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0bdda-152">lastSyncDateTime</span></span>|<span data-ttu-id="0bdda-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bdda-153">DateTimeOffset</span></span>|<span data-ttu-id="0bdda-154">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="0bdda-154">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="0bdda-155">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="0bdda-155">operatingSystem</span></span>|<span data-ttu-id="0bdda-156">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-156">String</span></span>|<span data-ttu-id="0bdda-157">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="0bdda-157">Operating system of the device.</span></span> <span data-ttu-id="0bdda-158">Windows, iOS и т. д.</span><span class="sxs-lookup"><span data-stu-id="0bdda-158">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="0bdda-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="0bdda-159">complianceState</span></span>|[<span data-ttu-id="0bdda-160">complianceState</span><span class="sxs-lookup"><span data-stu-id="0bdda-160">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="0bdda-161">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="0bdda-161">Compliance state of the device.</span></span> <span data-ttu-id="0bdda-162">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="0bdda-162">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="0bdda-163">jailBroken</span><span class="sxs-lookup"><span data-stu-id="0bdda-163">jailBroken</span></span>|<span data-ttu-id="0bdda-164">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-164">String</span></span>|<span data-ttu-id="0bdda-165">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="0bdda-165">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="0bdda-166">managementAgent</span><span class="sxs-lookup"><span data-stu-id="0bdda-166">managementAgent</span></span>|[<span data-ttu-id="0bdda-167">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="0bdda-167">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="0bdda-168">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="0bdda-168">Management channel of the device.</span></span> <span data-ttu-id="0bdda-169">Intune, EAS и т. д. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="0bdda-169">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="0bdda-170">osVersion</span><span class="sxs-lookup"><span data-stu-id="0bdda-170">osVersion</span></span>|<span data-ttu-id="0bdda-171">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-171">String</span></span>|<span data-ttu-id="0bdda-172">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="0bdda-172">Operating system version of the device.</span></span>|
|<span data-ttu-id="0bdda-173">easActivated</span><span class="sxs-lookup"><span data-stu-id="0bdda-173">easActivated</span></span>|<span data-ttu-id="0bdda-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bdda-174">Boolean</span></span>|<span data-ttu-id="0bdda-175">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="0bdda-175">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="0bdda-176">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="0bdda-176">easDeviceId</span></span>|<span data-ttu-id="0bdda-177">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-177">String</span></span>|<span data-ttu-id="0bdda-178">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="0bdda-178">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="0bdda-179">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="0bdda-179">easActivationDateTime</span></span>|<span data-ttu-id="0bdda-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bdda-180">DateTimeOffset</span></span>|<span data-ttu-id="0bdda-181">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="0bdda-181">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="0bdda-182">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="0bdda-182">azureADRegistered</span></span>|<span data-ttu-id="0bdda-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bdda-183">Boolean</span></span>|<span data-ttu-id="0bdda-184">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0bdda-184">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="0bdda-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0bdda-185">deviceEnrollmentType</span></span>|[<span data-ttu-id="0bdda-186">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0bdda-186">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="0bdda-187">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="0bdda-187">Enrollment type of the device.</span></span> <span data-ttu-id="0bdda-188">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="0bdda-188">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="0bdda-189">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="0bdda-189">activationLockBypassCode</span></span>|<span data-ttu-id="0bdda-190">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-190">String</span></span>|<span data-ttu-id="0bdda-191">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="0bdda-191">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="0bdda-192">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0bdda-192">emailAddress</span></span>|<span data-ttu-id="0bdda-193">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-193">String</span></span>|<span data-ttu-id="0bdda-194">Адреса электронной почты пользователя, связанного с устройством</span><span class="sxs-lookup"><span data-stu-id="0bdda-194">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="0bdda-195">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="0bdda-195">azureADDeviceId</span></span>|<span data-ttu-id="0bdda-196">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-196">String</span></span>|<span data-ttu-id="0bdda-197">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0bdda-197">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="0bdda-198">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0bdda-198">Read only.</span></span>|
|<span data-ttu-id="0bdda-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="0bdda-199">deviceRegistrationState</span></span>|[<span data-ttu-id="0bdda-200">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="0bdda-200">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="0bdda-201">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="0bdda-201">Device registration state.</span></span> <span data-ttu-id="0bdda-202">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0bdda-202">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="0bdda-203">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="0bdda-203">deviceCategoryDisplayName</span></span>|<span data-ttu-id="0bdda-204">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-204">String</span></span>|<span data-ttu-id="0bdda-205">Отображаемое имя категории устройства</span><span class="sxs-lookup"><span data-stu-id="0bdda-205">Device category display name</span></span>|
|<span data-ttu-id="0bdda-206">isSupervised</span><span class="sxs-lookup"><span data-stu-id="0bdda-206">isSupervised</span></span>|<span data-ttu-id="0bdda-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bdda-207">Boolean</span></span>|<span data-ttu-id="0bdda-208">Состояние защиты устройства</span><span class="sxs-lookup"><span data-stu-id="0bdda-208">Device supervised status</span></span>|
|<span data-ttu-id="0bdda-209">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0bdda-209">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="0bdda-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bdda-210">DateTimeOffset</span></span>|<span data-ttu-id="0bdda-211">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bdda-211">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="0bdda-212">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="0bdda-212">exchangeAccessState</span></span>|[<span data-ttu-id="0bdda-213">девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="0bdda-213">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="0bdda-214">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bdda-214">The Access State of the device in Exchange.</span></span> <span data-ttu-id="0bdda-215">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="0bdda-215">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="0bdda-216">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="0bdda-216">exchangeAccessStateReason</span></span>|[<span data-ttu-id="0bdda-217">девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="0bdda-217">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="0bdda-218">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bdda-218">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="0bdda-219">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="0bdda-219">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="0bdda-220">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="0bdda-220">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="0bdda-221">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-221">String</span></span>|<span data-ttu-id="0bdda-222">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="0bdda-222">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="0bdda-223">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="0bdda-223">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="0bdda-224">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-224">String</span></span>|<span data-ttu-id="0bdda-225">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="0bdda-225">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="0bdda-226">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="0bdda-226">isEncrypted</span></span>|<span data-ttu-id="0bdda-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bdda-227">Boolean</span></span>|<span data-ttu-id="0bdda-228">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="0bdda-228">Device encryption status</span></span>|
|<span data-ttu-id="0bdda-229">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0bdda-229">userPrincipalName</span></span>|<span data-ttu-id="0bdda-230">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-230">String</span></span>|<span data-ttu-id="0bdda-231">Имя участника-пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="0bdda-231">Device user principal name</span></span>|
|<span data-ttu-id="0bdda-232">model</span><span class="sxs-lookup"><span data-stu-id="0bdda-232">model</span></span>|<span data-ttu-id="0bdda-233">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-233">String</span></span>|<span data-ttu-id="0bdda-234">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="0bdda-234">Model of the device</span></span>|
|<span data-ttu-id="0bdda-235">manufacturer</span><span class="sxs-lookup"><span data-stu-id="0bdda-235">manufacturer</span></span>|<span data-ttu-id="0bdda-236">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-236">String</span></span>|<span data-ttu-id="0bdda-237">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="0bdda-237">Manufacturer of the device</span></span>|
|<span data-ttu-id="0bdda-238">imei</span><span class="sxs-lookup"><span data-stu-id="0bdda-238">imei</span></span>|<span data-ttu-id="0bdda-239">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-239">String</span></span>|<span data-ttu-id="0bdda-240">IMEI</span><span class="sxs-lookup"><span data-stu-id="0bdda-240">IMEI</span></span>|
|<span data-ttu-id="0bdda-241">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0bdda-241">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="0bdda-242">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bdda-242">DateTimeOffset</span></span>|<span data-ttu-id="0bdda-243">Дата и время истечения льготного периода соответствия устройства требованиям</span><span class="sxs-lookup"><span data-stu-id="0bdda-243">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="0bdda-244">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0bdda-244">serialNumber</span></span>|<span data-ttu-id="0bdda-245">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-245">String</span></span>|<span data-ttu-id="0bdda-246">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="0bdda-246">SerialNumber</span></span>|
|<span data-ttu-id="0bdda-247">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="0bdda-247">phoneNumber</span></span>|<span data-ttu-id="0bdda-248">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-248">String</span></span>|<span data-ttu-id="0bdda-249">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="0bdda-249">Phone number of the device</span></span>|
|<span data-ttu-id="0bdda-250">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="0bdda-250">androidSecurityPatchLevel</span></span>|<span data-ttu-id="0bdda-251">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-251">String</span></span>|<span data-ttu-id="0bdda-252">Уровень обновления для системы безопасности Android</span><span class="sxs-lookup"><span data-stu-id="0bdda-252">Android security patch level</span></span>|
|<span data-ttu-id="0bdda-253">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0bdda-253">userDisplayName</span></span>|<span data-ttu-id="0bdda-254">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-254">String</span></span>|<span data-ttu-id="0bdda-255">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="0bdda-255">User display name</span></span>|
|<span data-ttu-id="0bdda-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0bdda-256">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="0bdda-257">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0bdda-257">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="0bdda-258">Включенные функции клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="0bdda-258">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="0bdda-259">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="0bdda-259">wiFiMacAddress</span></span>|<span data-ttu-id="0bdda-260">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-260">String</span></span>|<span data-ttu-id="0bdda-261">MAC-адрес сети Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="0bdda-261">Wi-Fi MAC</span></span>|
|<span data-ttu-id="0bdda-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0bdda-262">deviceHealthAttestationState</span></span>|[<span data-ttu-id="0bdda-263">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0bdda-263">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="0bdda-264">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="0bdda-264">The device health attestation state.</span></span>|
|<span data-ttu-id="0bdda-265">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="0bdda-265">subscriberCarrier</span></span>|<span data-ttu-id="0bdda-266">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-266">String</span></span>|<span data-ttu-id="0bdda-267">Оператор сотовой связи, используемый абонентом</span><span class="sxs-lookup"><span data-stu-id="0bdda-267">Subscriber Carrier</span></span>|
|<span data-ttu-id="0bdda-268">meid</span><span class="sxs-lookup"><span data-stu-id="0bdda-268">meid</span></span>|<span data-ttu-id="0bdda-269">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-269">String</span></span>|<span data-ttu-id="0bdda-270">MEID</span><span class="sxs-lookup"><span data-stu-id="0bdda-270">MEID</span></span>|
|<span data-ttu-id="0bdda-271">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="0bdda-271">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="0bdda-272">Int64</span><span class="sxs-lookup"><span data-stu-id="0bdda-272">Int64</span></span>|<span data-ttu-id="0bdda-273">Общий объем хранилища в байтах</span><span class="sxs-lookup"><span data-stu-id="0bdda-273">Total Storage in Bytes</span></span>|
|<span data-ttu-id="0bdda-274">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="0bdda-274">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="0bdda-275">Int64</span><span class="sxs-lookup"><span data-stu-id="0bdda-275">Int64</span></span>|<span data-ttu-id="0bdda-276">Свободный объем хранилища в байтах
</span><span class="sxs-lookup"><span data-stu-id="0bdda-276">Free Storage in Bytes</span></span>|
|<span data-ttu-id="0bdda-277">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="0bdda-277">managedDeviceName</span></span>|<span data-ttu-id="0bdda-278">String</span><span class="sxs-lookup"><span data-stu-id="0bdda-278">String</span></span>|<span data-ttu-id="0bdda-279">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="0bdda-279">Automatically generated name to identify a device.</span></span> <span data-ttu-id="0bdda-280">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="0bdda-280">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="0bdda-281">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="0bdda-281">partnerReportedThreatState</span></span>|[<span data-ttu-id="0bdda-282">манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="0bdda-282">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="0bdda-283">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="0bdda-283">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="0bdda-284">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0bdda-284">Read Only.</span></span> <span data-ttu-id="0bdda-285">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="0bdda-285">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="0bdda-286">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bdda-286">Response</span></span>
<span data-ttu-id="0bdda-287">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedDevice](../resources/intune-devices-manageddevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0bdda-287">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bdda-288">Пример</span><span class="sxs-lookup"><span data-stu-id="0bdda-288">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bdda-289">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdda-289">Request</span></span>
<span data-ttu-id="0bdda-290">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0bdda-290">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
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

### <a name="response"></a><span data-ttu-id="0bdda-291">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bdda-291">Response</span></span>
<span data-ttu-id="0bdda-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0bdda-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









