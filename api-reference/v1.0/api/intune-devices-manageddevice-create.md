---
title: Create managedDevice
description: Создание объекта managedDevice.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa68138f59cc713d3af87d2bd87bbc262a92b2cf
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257381"
---
# <a name="create-manageddevice"></a><span data-ttu-id="3fd18-103">Create managedDevice</span><span class="sxs-lookup"><span data-stu-id="3fd18-103">Create managedDevice</span></span>

> <span data-ttu-id="3fd18-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3fd18-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fd18-105">Создание объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3fd18-105">Create a new [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fd18-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3fd18-106">Prerequisites</span></span>
<span data-ttu-id="3fd18-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3fd18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3fd18-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fd18-109">Permission type</span></span>|<span data-ttu-id="3fd18-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fd18-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fd18-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fd18-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3fd18-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fd18-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3fd18-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fd18-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fd18-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fd18-114">Not supported.</span></span>|
|<span data-ttu-id="3fd18-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fd18-115">Application</span></span>|<span data-ttu-id="3fd18-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fd18-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fd18-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fd18-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="3fd18-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fd18-118">Request headers</span></span>
|<span data-ttu-id="3fd18-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3fd18-119">Header</span></span>|<span data-ttu-id="3fd18-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3fd18-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fd18-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3fd18-121">Authorization</span></span>|<span data-ttu-id="3fd18-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3fd18-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fd18-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3fd18-123">Accept</span></span>|<span data-ttu-id="3fd18-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3fd18-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fd18-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3fd18-125">Request body</span></span>
<span data-ttu-id="3fd18-126">В тексте запроса добавьте представление объекта managedDevice в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fd18-126">In the request body, supply a JSON representation for the managedDevice object.</span></span>

<span data-ttu-id="3fd18-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedDevice.</span><span class="sxs-lookup"><span data-stu-id="3fd18-127">The following table shows the properties that are required when you create the managedDevice.</span></span>

|<span data-ttu-id="3fd18-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fd18-128">Property</span></span>|<span data-ttu-id="3fd18-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3fd18-129">Type</span></span>|<span data-ttu-id="3fd18-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3fd18-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fd18-131">id</span><span class="sxs-lookup"><span data-stu-id="3fd18-131">id</span></span>|<span data-ttu-id="3fd18-132">Строка</span><span class="sxs-lookup"><span data-stu-id="3fd18-132">String</span></span>|<span data-ttu-id="3fd18-133">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="3fd18-133">Unique Identifier for the device</span></span>|
|<span data-ttu-id="3fd18-134">userId</span><span class="sxs-lookup"><span data-stu-id="3fd18-134">userId</span></span>|<span data-ttu-id="3fd18-135">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-135">String</span></span>|<span data-ttu-id="3fd18-136">Уникальный идентификатор пользователя, связанного с устройством.
</span><span class="sxs-lookup"><span data-stu-id="3fd18-136">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="3fd18-137">deviceName</span><span class="sxs-lookup"><span data-stu-id="3fd18-137">deviceName</span></span>|<span data-ttu-id="3fd18-138">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-138">String</span></span>|<span data-ttu-id="3fd18-139">Название устройства</span><span class="sxs-lookup"><span data-stu-id="3fd18-139">Name of the device</span></span>|
|<span data-ttu-id="3fd18-140">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="3fd18-140">managedDeviceOwnerType</span></span>|[<span data-ttu-id="3fd18-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="3fd18-141">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="3fd18-142">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="3fd18-142">Ownership of the device.</span></span> <span data-ttu-id="3fd18-143">Может быть "Company" или "Personal".</span><span class="sxs-lookup"><span data-stu-id="3fd18-143">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="3fd18-144">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="3fd18-144">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="3fd18-145">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="3fd18-145">deviceActionResults</span></span>|<span data-ttu-id="3fd18-146">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3fd18-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="3fd18-147">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="3fd18-147">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="3fd18-148">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="3fd18-148">enrolledDateTime</span></span>|<span data-ttu-id="3fd18-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fd18-149">DateTimeOffset</span></span>|<span data-ttu-id="3fd18-150">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="3fd18-150">Enrollment time of the device.</span></span>|
|<span data-ttu-id="3fd18-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3fd18-151">lastSyncDateTime</span></span>|<span data-ttu-id="3fd18-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fd18-152">DateTimeOffset</span></span>|<span data-ttu-id="3fd18-153">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="3fd18-153">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="3fd18-154">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="3fd18-154">operatingSystem</span></span>|<span data-ttu-id="3fd18-155">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-155">String</span></span>|<span data-ttu-id="3fd18-156">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="3fd18-156">Operating system of the device.</span></span> <span data-ttu-id="3fd18-157">Windows, iOS и т. д.</span><span class="sxs-lookup"><span data-stu-id="3fd18-157">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="3fd18-158">complianceState</span><span class="sxs-lookup"><span data-stu-id="3fd18-158">complianceState</span></span>|[<span data-ttu-id="3fd18-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="3fd18-159">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="3fd18-160">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="3fd18-160">Compliance state of the device.</span></span> <span data-ttu-id="3fd18-161">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="3fd18-161">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="3fd18-162">jailBroken</span><span class="sxs-lookup"><span data-stu-id="3fd18-162">jailBroken</span></span>|<span data-ttu-id="3fd18-163">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-163">String</span></span>|<span data-ttu-id="3fd18-164">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="3fd18-164">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="3fd18-165">managementAgent</span><span class="sxs-lookup"><span data-stu-id="3fd18-165">managementAgent</span></span>|[<span data-ttu-id="3fd18-166">Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="3fd18-166">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="3fd18-167">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="3fd18-167">Management channel of the device.</span></span> <span data-ttu-id="3fd18-168">Intune, EAS и т. д. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="3fd18-168">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="3fd18-169">osVersion</span><span class="sxs-lookup"><span data-stu-id="3fd18-169">osVersion</span></span>|<span data-ttu-id="3fd18-170">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-170">String</span></span>|<span data-ttu-id="3fd18-171">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="3fd18-171">Operating system version of the device.</span></span>|
|<span data-ttu-id="3fd18-172">easActivated</span><span class="sxs-lookup"><span data-stu-id="3fd18-172">easActivated</span></span>|<span data-ttu-id="3fd18-173">Логический</span><span class="sxs-lookup"><span data-stu-id="3fd18-173">Boolean</span></span>|<span data-ttu-id="3fd18-174">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="3fd18-174">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="3fd18-175">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="3fd18-175">easDeviceId</span></span>|<span data-ttu-id="3fd18-176">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-176">String</span></span>|<span data-ttu-id="3fd18-177">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="3fd18-177">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="3fd18-178">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="3fd18-178">easActivationDateTime</span></span>|<span data-ttu-id="3fd18-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fd18-179">DateTimeOffset</span></span>|<span data-ttu-id="3fd18-180">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="3fd18-180">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="3fd18-181">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="3fd18-181">azureADRegistered</span></span>|<span data-ttu-id="3fd18-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fd18-182">Boolean</span></span>|<span data-ttu-id="3fd18-183">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3fd18-183">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="3fd18-184">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="3fd18-184">deviceEnrollmentType</span></span>|[<span data-ttu-id="3fd18-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="3fd18-185">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="3fd18-186">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="3fd18-186">Enrollment type of the device.</span></span> <span data-ttu-id="3fd18-187">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="3fd18-187">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="3fd18-188">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="3fd18-188">activationLockBypassCode</span></span>|<span data-ttu-id="3fd18-189">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-189">String</span></span>|<span data-ttu-id="3fd18-190">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="3fd18-190">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="3fd18-191">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3fd18-191">emailAddress</span></span>|<span data-ttu-id="3fd18-192">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-192">String</span></span>|<span data-ttu-id="3fd18-193">Адреса электронной почты пользователя, связанного с устройством</span><span class="sxs-lookup"><span data-stu-id="3fd18-193">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="3fd18-194">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="3fd18-194">azureADDeviceId</span></span>|<span data-ttu-id="3fd18-195">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-195">String</span></span>|<span data-ttu-id="3fd18-196">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3fd18-196">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="3fd18-197">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fd18-197">Read only.</span></span>|
|<span data-ttu-id="3fd18-198">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="3fd18-198">deviceRegistrationState</span></span>|[<span data-ttu-id="3fd18-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="3fd18-199">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="3fd18-200">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="3fd18-200">Device registration state.</span></span> <span data-ttu-id="3fd18-201">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="3fd18-201">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="3fd18-202">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="3fd18-202">deviceCategoryDisplayName</span></span>|<span data-ttu-id="3fd18-203">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-203">String</span></span>|<span data-ttu-id="3fd18-204">Отображаемое имя категории устройства</span><span class="sxs-lookup"><span data-stu-id="3fd18-204">Device category display name</span></span>|
|<span data-ttu-id="3fd18-205">isSupervised</span><span class="sxs-lookup"><span data-stu-id="3fd18-205">isSupervised</span></span>|<span data-ttu-id="3fd18-206">Логический</span><span class="sxs-lookup"><span data-stu-id="3fd18-206">Boolean</span></span>|<span data-ttu-id="3fd18-207">Состояние защиты устройства</span><span class="sxs-lookup"><span data-stu-id="3fd18-207">Device supervised status</span></span>|
|<span data-ttu-id="3fd18-208">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3fd18-208">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="3fd18-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fd18-209">DateTimeOffset</span></span>|<span data-ttu-id="3fd18-210">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="3fd18-210">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="3fd18-211">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="3fd18-211">exchangeAccessState</span></span>|[<span data-ttu-id="3fd18-212">Девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="3fd18-212">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="3fd18-213">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="3fd18-213">The Access State of the device in Exchange.</span></span> <span data-ttu-id="3fd18-214">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="3fd18-214">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="3fd18-215">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="3fd18-215">exchangeAccessStateReason</span></span>|[<span data-ttu-id="3fd18-216">Девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="3fd18-216">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="3fd18-217">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="3fd18-217">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="3fd18-218">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="3fd18-218">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="3fd18-219">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="3fd18-219">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="3fd18-220">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-220">String</span></span>|<span data-ttu-id="3fd18-221">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="3fd18-221">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="3fd18-222">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3fd18-222">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="3fd18-223">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-223">String</span></span>|<span data-ttu-id="3fd18-224">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="3fd18-224">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="3fd18-225">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="3fd18-225">isEncrypted</span></span>|<span data-ttu-id="3fd18-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fd18-226">Boolean</span></span>|<span data-ttu-id="3fd18-227">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="3fd18-227">Device encryption status</span></span>|
|<span data-ttu-id="3fd18-228">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3fd18-228">userPrincipalName</span></span>|<span data-ttu-id="3fd18-229">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-229">String</span></span>|<span data-ttu-id="3fd18-230">Имя участника-пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="3fd18-230">Device user principal name</span></span>|
|<span data-ttu-id="3fd18-231">model</span><span class="sxs-lookup"><span data-stu-id="3fd18-231">model</span></span>|<span data-ttu-id="3fd18-232">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-232">String</span></span>|<span data-ttu-id="3fd18-233">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="3fd18-233">Model of the device</span></span>|
|<span data-ttu-id="3fd18-234">manufacturer</span><span class="sxs-lookup"><span data-stu-id="3fd18-234">manufacturer</span></span>|<span data-ttu-id="3fd18-235">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-235">String</span></span>|<span data-ttu-id="3fd18-236">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="3fd18-236">Manufacturer of the device</span></span>|
|<span data-ttu-id="3fd18-237">imei</span><span class="sxs-lookup"><span data-stu-id="3fd18-237">imei</span></span>|<span data-ttu-id="3fd18-238">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-238">String</span></span>|<span data-ttu-id="3fd18-239">IMEI</span><span class="sxs-lookup"><span data-stu-id="3fd18-239">IMEI</span></span>|
|<span data-ttu-id="3fd18-240">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3fd18-240">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="3fd18-241">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fd18-241">DateTimeOffset</span></span>|<span data-ttu-id="3fd18-242">Дата и время истечения льготного периода соответствия устройства требованиям</span><span class="sxs-lookup"><span data-stu-id="3fd18-242">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="3fd18-243">serialNumber</span><span class="sxs-lookup"><span data-stu-id="3fd18-243">serialNumber</span></span>|<span data-ttu-id="3fd18-244">Строка</span><span class="sxs-lookup"><span data-stu-id="3fd18-244">String</span></span>|<span data-ttu-id="3fd18-245">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="3fd18-245">SerialNumber</span></span>|
|<span data-ttu-id="3fd18-246">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="3fd18-246">phoneNumber</span></span>|<span data-ttu-id="3fd18-247">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-247">String</span></span>|<span data-ttu-id="3fd18-248">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="3fd18-248">Phone number of the device</span></span>|
|<span data-ttu-id="3fd18-249">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="3fd18-249">androidSecurityPatchLevel</span></span>|<span data-ttu-id="3fd18-250">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-250">String</span></span>|<span data-ttu-id="3fd18-251">Уровень обновления для системы безопасности Android</span><span class="sxs-lookup"><span data-stu-id="3fd18-251">Android security patch level</span></span>|
|<span data-ttu-id="3fd18-252">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3fd18-252">userDisplayName</span></span>|<span data-ttu-id="3fd18-253">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-253">String</span></span>|<span data-ttu-id="3fd18-254">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="3fd18-254">User display name</span></span>|
|<span data-ttu-id="3fd18-255">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="3fd18-255">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="3fd18-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="3fd18-256">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="3fd18-257">Включенные функции клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="3fd18-257">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="3fd18-258">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="3fd18-258">wiFiMacAddress</span></span>|<span data-ttu-id="3fd18-259">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-259">String</span></span>|<span data-ttu-id="3fd18-260">MAC-адрес сети Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="3fd18-260">Wi-Fi MAC</span></span>|
|<span data-ttu-id="3fd18-261">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="3fd18-261">deviceHealthAttestationState</span></span>|[<span data-ttu-id="3fd18-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="3fd18-262">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="3fd18-263">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="3fd18-263">The device health attestation state.</span></span>|
|<span data-ttu-id="3fd18-264">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="3fd18-264">subscriberCarrier</span></span>|<span data-ttu-id="3fd18-265">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-265">String</span></span>|<span data-ttu-id="3fd18-266">Оператор сотовой связи, используемый абонентом</span><span class="sxs-lookup"><span data-stu-id="3fd18-266">Subscriber Carrier</span></span>|
|<span data-ttu-id="3fd18-267">meid</span><span class="sxs-lookup"><span data-stu-id="3fd18-267">meid</span></span>|<span data-ttu-id="3fd18-268">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-268">String</span></span>|<span data-ttu-id="3fd18-269">MEID</span><span class="sxs-lookup"><span data-stu-id="3fd18-269">MEID</span></span>|
|<span data-ttu-id="3fd18-270">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="3fd18-270">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="3fd18-271">Int64</span><span class="sxs-lookup"><span data-stu-id="3fd18-271">Int64</span></span>|<span data-ttu-id="3fd18-272">Общий объем хранилища в байтах</span><span class="sxs-lookup"><span data-stu-id="3fd18-272">Total Storage in Bytes</span></span>|
|<span data-ttu-id="3fd18-273">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="3fd18-273">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="3fd18-274">Int64</span><span class="sxs-lookup"><span data-stu-id="3fd18-274">Int64</span></span>|<span data-ttu-id="3fd18-275">Свободный объем хранилища в байтах
</span><span class="sxs-lookup"><span data-stu-id="3fd18-275">Free Storage in Bytes</span></span>|
|<span data-ttu-id="3fd18-276">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="3fd18-276">managedDeviceName</span></span>|<span data-ttu-id="3fd18-277">String</span><span class="sxs-lookup"><span data-stu-id="3fd18-277">String</span></span>|<span data-ttu-id="3fd18-278">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="3fd18-278">Automatically generated name to identify a device.</span></span> <span data-ttu-id="3fd18-279">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="3fd18-279">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="3fd18-280">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="3fd18-280">partnerReportedThreatState</span></span>|[<span data-ttu-id="3fd18-281">Манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="3fd18-281">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="3fd18-282">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="3fd18-282">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="3fd18-283">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fd18-283">Read Only.</span></span> <span data-ttu-id="3fd18-284">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="3fd18-284">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="3fd18-285">Ответ</span><span class="sxs-lookup"><span data-stu-id="3fd18-285">Response</span></span>
<span data-ttu-id="3fd18-286">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedDevice](../resources/intune-devices-manageddevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3fd18-286">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fd18-287">Пример</span><span class="sxs-lookup"><span data-stu-id="3fd18-287">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fd18-288">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fd18-288">Request</span></span>
<span data-ttu-id="3fd18-289">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fd18-289">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3fd18-290">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fd18-290">Response</span></span>
<span data-ttu-id="3fd18-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3fd18-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



