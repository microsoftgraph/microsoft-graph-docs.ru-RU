---
title: Обновление managedDevice
description: Обновление свойств объекта managedDevice.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c7a0b95ff0ec3b5ad7cdd574405ccd4887e08dc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32519887"
---
# <a name="update-manageddevice"></a><span data-ttu-id="f582e-103">Обновление managedDevice</span><span class="sxs-lookup"><span data-stu-id="f582e-103">Update managedDevice</span></span>

> <span data-ttu-id="f582e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f582e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f582e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f582e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f582e-106">Обновление свойств объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f582e-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f582e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f582e-107">Prerequisites</span></span>
<span data-ttu-id="f582e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f582e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f582e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f582e-110">Permission type</span></span>|<span data-ttu-id="f582e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f582e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f582e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f582e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f582e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f582e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f582e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f582e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f582e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f582e-115">Not supported.</span></span>|
|<span data-ttu-id="f582e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f582e-116">Application</span></span>|<span data-ttu-id="f582e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f582e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f582e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f582e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="f582e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f582e-119">Request headers</span></span>
|<span data-ttu-id="f582e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f582e-120">Header</span></span>|<span data-ttu-id="f582e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f582e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f582e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f582e-122">Authorization</span></span>|<span data-ttu-id="f582e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f582e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f582e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f582e-124">Accept</span></span>|<span data-ttu-id="f582e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f582e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f582e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f582e-126">Request body</span></span>
<span data-ttu-id="f582e-127">В теле запроса добавьте представление объекта [managedDevice](../resources/intune-devices-manageddevice.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f582e-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="f582e-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f582e-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="f582e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f582e-129">Property</span></span>|<span data-ttu-id="f582e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f582e-130">Type</span></span>|<span data-ttu-id="f582e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f582e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f582e-132">id</span><span class="sxs-lookup"><span data-stu-id="f582e-132">id</span></span>|<span data-ttu-id="f582e-133">String</span><span class="sxs-lookup"><span data-stu-id="f582e-133">String</span></span>|<span data-ttu-id="f582e-134">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="f582e-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="f582e-135">userId</span><span class="sxs-lookup"><span data-stu-id="f582e-135">userId</span></span>|<span data-ttu-id="f582e-136">String</span><span class="sxs-lookup"><span data-stu-id="f582e-136">String</span></span>|<span data-ttu-id="f582e-137">Уникальный идентификатор пользователя, связанного с устройством.
</span><span class="sxs-lookup"><span data-stu-id="f582e-137">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="f582e-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="f582e-138">deviceName</span></span>|<span data-ttu-id="f582e-139">String</span><span class="sxs-lookup"><span data-stu-id="f582e-139">String</span></span>|<span data-ttu-id="f582e-140">Название устройства</span><span class="sxs-lookup"><span data-stu-id="f582e-140">Name of the device</span></span>|
|<span data-ttu-id="f582e-141">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="f582e-141">hardwareInformation</span></span>|[<span data-ttu-id="f582e-142">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="f582e-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="f582e-143">Сведения о хардвард для устройства.</span><span class="sxs-lookup"><span data-stu-id="f582e-143">The hardward details for the device.</span></span>  <span data-ttu-id="f582e-144">Включает такие сведения, как место хранения, производитель, серийный номер и т. д.</span><span class="sxs-lookup"><span data-stu-id="f582e-144">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="f582e-145">ownerType</span><span class="sxs-lookup"><span data-stu-id="f582e-145">ownerType</span></span>|[<span data-ttu-id="f582e-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="f582e-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="f582e-147">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="f582e-147">Ownership of the device.</span></span> <span data-ttu-id="f582e-148">Может быть "Company" или "Personal".</span><span class="sxs-lookup"><span data-stu-id="f582e-148">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="f582e-149">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="f582e-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="f582e-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="f582e-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="f582e-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="f582e-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="f582e-152">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="f582e-152">Ownership of the device.</span></span> <span data-ttu-id="f582e-153">Может быть "Company" или "Personal".</span><span class="sxs-lookup"><span data-stu-id="f582e-153">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="f582e-154">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="f582e-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="f582e-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="f582e-155">deviceActionResults</span></span>|<span data-ttu-id="f582e-156">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f582e-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="f582e-157">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="f582e-157">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="f582e-158">Манажементстате</span><span class="sxs-lookup"><span data-stu-id="f582e-158">managementState</span></span>|[<span data-ttu-id="f582e-159">Манажементстате</span><span class="sxs-lookup"><span data-stu-id="f582e-159">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="f582e-160">Состояние управления для устройства.</span><span class="sxs-lookup"><span data-stu-id="f582e-160">Management state of the device.</span></span> <span data-ttu-id="f582e-161">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="f582e-161">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="f582e-162">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="f582e-162">enrolledDateTime</span></span>|<span data-ttu-id="f582e-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f582e-163">DateTimeOffset</span></span>|<span data-ttu-id="f582e-164">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="f582e-164">Enrollment time of the device.</span></span>|
|<span data-ttu-id="f582e-165">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f582e-165">lastSyncDateTime</span></span>|<span data-ttu-id="f582e-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f582e-166">DateTimeOffset</span></span>|<span data-ttu-id="f582e-167">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="f582e-167">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="f582e-168">Чассистипе</span><span class="sxs-lookup"><span data-stu-id="f582e-168">chassisType</span></span>|[<span data-ttu-id="f582e-169">Чассистипе</span><span class="sxs-lookup"><span data-stu-id="f582e-169">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="f582e-170">Тип корпуса устройства.</span><span class="sxs-lookup"><span data-stu-id="f582e-170">Chassis type of the device.</span></span> <span data-ttu-id="f582e-171">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="f582e-171">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="f582e-172">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="f582e-172">operatingSystem</span></span>|<span data-ttu-id="f582e-173">String</span><span class="sxs-lookup"><span data-stu-id="f582e-173">String</span></span>|<span data-ttu-id="f582e-174">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="f582e-174">Operating system of the device.</span></span> <span data-ttu-id="f582e-175">Windows, iOS и т. д.</span><span class="sxs-lookup"><span data-stu-id="f582e-175">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="f582e-176">deviceType</span><span class="sxs-lookup"><span data-stu-id="f582e-176">deviceType</span></span>|[<span data-ttu-id="f582e-177">deviceType</span><span class="sxs-lookup"><span data-stu-id="f582e-177">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="f582e-178">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="f582e-178">Platform of the device.</span></span> <span data-ttu-id="f582e-179">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `android` `iSocConsumer`,,,,,,,,,,,,,,,,,,,,, `winEmbedded` `iPhone` `iPad` `iPod` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f582e-179">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="f582e-180">complianceState</span><span class="sxs-lookup"><span data-stu-id="f582e-180">complianceState</span></span>|[<span data-ttu-id="f582e-181">complianceState</span><span class="sxs-lookup"><span data-stu-id="f582e-181">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="f582e-182">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="f582e-182">Compliance state of the device.</span></span> <span data-ttu-id="f582e-183">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="f582e-183">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="f582e-184">jailBroken</span><span class="sxs-lookup"><span data-stu-id="f582e-184">jailBroken</span></span>|<span data-ttu-id="f582e-185">String</span><span class="sxs-lookup"><span data-stu-id="f582e-185">String</span></span>|<span data-ttu-id="f582e-186">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="f582e-186">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="f582e-187">managementAgent</span><span class="sxs-lookup"><span data-stu-id="f582e-187">managementAgent</span></span>|[<span data-ttu-id="f582e-188">Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="f582e-188">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="f582e-189">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="f582e-189">Management channel of the device.</span></span> <span data-ttu-id="f582e-190">Intune, EAS и т. д. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`,. `microsoft365ManagedMdm`</span><span class="sxs-lookup"><span data-stu-id="f582e-190">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="f582e-191">osVersion</span><span class="sxs-lookup"><span data-stu-id="f582e-191">osVersion</span></span>|<span data-ttu-id="f582e-192">String</span><span class="sxs-lookup"><span data-stu-id="f582e-192">String</span></span>|<span data-ttu-id="f582e-193">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="f582e-193">Operating system version of the device.</span></span>|
|<span data-ttu-id="f582e-194">easActivated</span><span class="sxs-lookup"><span data-stu-id="f582e-194">easActivated</span></span>|<span data-ttu-id="f582e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="f582e-195">Boolean</span></span>|<span data-ttu-id="f582e-196">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="f582e-196">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="f582e-197">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="f582e-197">easDeviceId</span></span>|<span data-ttu-id="f582e-198">String</span><span class="sxs-lookup"><span data-stu-id="f582e-198">String</span></span>|<span data-ttu-id="f582e-199">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="f582e-199">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="f582e-200">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="f582e-200">easActivationDateTime</span></span>|<span data-ttu-id="f582e-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f582e-201">DateTimeOffset</span></span>|<span data-ttu-id="f582e-202">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="f582e-202">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="f582e-203">Аадрегистеред</span><span class="sxs-lookup"><span data-stu-id="f582e-203">aadRegistered</span></span>|<span data-ttu-id="f582e-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="f582e-204">Boolean</span></span>|<span data-ttu-id="f582e-205">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f582e-205">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="f582e-206">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="f582e-206">azureADRegistered</span></span>|<span data-ttu-id="f582e-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="f582e-207">Boolean</span></span>|<span data-ttu-id="f582e-208">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f582e-208">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="f582e-209">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f582e-209">deviceEnrollmentType</span></span>|[<span data-ttu-id="f582e-210">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f582e-210">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="f582e-211">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="f582e-211">Enrollment type of the device.</span></span> <span data-ttu-id="f582e-212">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="f582e-212">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="f582e-213">Лостмодестате</span><span class="sxs-lookup"><span data-stu-id="f582e-213">lostModeState</span></span>|[<span data-ttu-id="f582e-214">Лостмодестате</span><span class="sxs-lookup"><span data-stu-id="f582e-214">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="f582e-215">Указывает, включен ли режим потерянных или отключенных.</span><span class="sxs-lookup"><span data-stu-id="f582e-215">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="f582e-216">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="f582e-216">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="f582e-217">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="f582e-217">activationLockBypassCode</span></span>|<span data-ttu-id="f582e-218">String</span><span class="sxs-lookup"><span data-stu-id="f582e-218">String</span></span>|<span data-ttu-id="f582e-219">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f582e-219">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="f582e-220">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f582e-220">emailAddress</span></span>|<span data-ttu-id="f582e-221">String</span><span class="sxs-lookup"><span data-stu-id="f582e-221">String</span></span>|<span data-ttu-id="f582e-222">Адреса электронной почты пользователя, связанного с устройством</span><span class="sxs-lookup"><span data-stu-id="f582e-222">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="f582e-223">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="f582e-223">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="f582e-224">String</span><span class="sxs-lookup"><span data-stu-id="f582e-224">String</span></span>|<span data-ttu-id="f582e-225">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f582e-225">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="f582e-226">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f582e-226">Read only.</span></span>|
|<span data-ttu-id="f582e-227">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="f582e-227">azureADDeviceId</span></span>|<span data-ttu-id="f582e-228">String</span><span class="sxs-lookup"><span data-stu-id="f582e-228">String</span></span>|<span data-ttu-id="f582e-229">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f582e-229">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="f582e-230">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f582e-230">Read only.</span></span>|
|<span data-ttu-id="f582e-231">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="f582e-231">deviceRegistrationState</span></span>|[<span data-ttu-id="f582e-232">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="f582e-232">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="f582e-233">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="f582e-233">Device registration state.</span></span> <span data-ttu-id="f582e-234">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f582e-234">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="f582e-235">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="f582e-235">deviceCategoryDisplayName</span></span>|<span data-ttu-id="f582e-236">String</span><span class="sxs-lookup"><span data-stu-id="f582e-236">String</span></span>|<span data-ttu-id="f582e-237">Отображаемое имя категории устройства</span><span class="sxs-lookup"><span data-stu-id="f582e-237">Device category display name</span></span>|
|<span data-ttu-id="f582e-238">isSupervised</span><span class="sxs-lookup"><span data-stu-id="f582e-238">isSupervised</span></span>|<span data-ttu-id="f582e-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="f582e-239">Boolean</span></span>|<span data-ttu-id="f582e-240">Состояние защиты устройства</span><span class="sxs-lookup"><span data-stu-id="f582e-240">Device supervised status</span></span>|
|<span data-ttu-id="f582e-241">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f582e-241">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="f582e-242">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f582e-242">DateTimeOffset</span></span>|<span data-ttu-id="f582e-243">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="f582e-243">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="f582e-244">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="f582e-244">exchangeAccessState</span></span>|[<span data-ttu-id="f582e-245">Девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="f582e-245">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="f582e-246">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="f582e-246">The Access State of the device in Exchange.</span></span> <span data-ttu-id="f582e-247">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="f582e-247">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="f582e-248">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="f582e-248">exchangeAccessStateReason</span></span>|[<span data-ttu-id="f582e-249">Девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="f582e-249">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="f582e-250">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="f582e-250">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="f582e-251">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="f582e-251">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="f582e-252">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="f582e-252">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="f582e-253">String</span><span class="sxs-lookup"><span data-stu-id="f582e-253">String</span></span>|<span data-ttu-id="f582e-254">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="f582e-254">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="f582e-255">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f582e-255">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="f582e-256">String</span><span class="sxs-lookup"><span data-stu-id="f582e-256">String</span></span>|<span data-ttu-id="f582e-257">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="f582e-257">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="f582e-258">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="f582e-258">isEncrypted</span></span>|<span data-ttu-id="f582e-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="f582e-259">Boolean</span></span>|<span data-ttu-id="f582e-260">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="f582e-260">Device encryption status</span></span>|
|<span data-ttu-id="f582e-261">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f582e-261">userPrincipalName</span></span>|<span data-ttu-id="f582e-262">String</span><span class="sxs-lookup"><span data-stu-id="f582e-262">String</span></span>|<span data-ttu-id="f582e-263">Имя участника-пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="f582e-263">Device user principal name</span></span>|
|<span data-ttu-id="f582e-264">model</span><span class="sxs-lookup"><span data-stu-id="f582e-264">model</span></span>|<span data-ttu-id="f582e-265">String</span><span class="sxs-lookup"><span data-stu-id="f582e-265">String</span></span>|<span data-ttu-id="f582e-266">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="f582e-266">Model of the device</span></span>|
|<span data-ttu-id="f582e-267">manufacturer</span><span class="sxs-lookup"><span data-stu-id="f582e-267">manufacturer</span></span>|<span data-ttu-id="f582e-268">String</span><span class="sxs-lookup"><span data-stu-id="f582e-268">String</span></span>|<span data-ttu-id="f582e-269">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="f582e-269">Manufacturer of the device</span></span>|
|<span data-ttu-id="f582e-270">imei</span><span class="sxs-lookup"><span data-stu-id="f582e-270">imei</span></span>|<span data-ttu-id="f582e-271">String</span><span class="sxs-lookup"><span data-stu-id="f582e-271">String</span></span>|<span data-ttu-id="f582e-272">IMEI</span><span class="sxs-lookup"><span data-stu-id="f582e-272">IMEI</span></span>|
|<span data-ttu-id="f582e-273">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f582e-273">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f582e-274">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f582e-274">DateTimeOffset</span></span>|<span data-ttu-id="f582e-275">Дата и время истечения льготного периода соответствия устройства требованиям</span><span class="sxs-lookup"><span data-stu-id="f582e-275">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="f582e-276">serialNumber</span><span class="sxs-lookup"><span data-stu-id="f582e-276">serialNumber</span></span>|<span data-ttu-id="f582e-277">Строка</span><span class="sxs-lookup"><span data-stu-id="f582e-277">String</span></span>|<span data-ttu-id="f582e-278">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="f582e-278">SerialNumber</span></span>|
|<span data-ttu-id="f582e-279">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="f582e-279">phoneNumber</span></span>|<span data-ttu-id="f582e-280">String</span><span class="sxs-lookup"><span data-stu-id="f582e-280">String</span></span>|<span data-ttu-id="f582e-281">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="f582e-281">Phone number of the device</span></span>|
|<span data-ttu-id="f582e-282">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="f582e-282">androidSecurityPatchLevel</span></span>|<span data-ttu-id="f582e-283">String</span><span class="sxs-lookup"><span data-stu-id="f582e-283">String</span></span>|<span data-ttu-id="f582e-284">Уровень обновления для системы безопасности Android</span><span class="sxs-lookup"><span data-stu-id="f582e-284">Android security patch level</span></span>|
|<span data-ttu-id="f582e-285">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f582e-285">userDisplayName</span></span>|<span data-ttu-id="f582e-286">String</span><span class="sxs-lookup"><span data-stu-id="f582e-286">String</span></span>|<span data-ttu-id="f582e-287">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="f582e-287">User display name</span></span>|
|<span data-ttu-id="f582e-288">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="f582e-288">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="f582e-289">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="f582e-289">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="f582e-290">Включенные функции клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="f582e-290">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="f582e-291">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="f582e-291">wiFiMacAddress</span></span>|<span data-ttu-id="f582e-292">String</span><span class="sxs-lookup"><span data-stu-id="f582e-292">String</span></span>|<span data-ttu-id="f582e-293">MAC-адрес сети Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="f582e-293">Wi-Fi MAC</span></span>|
|<span data-ttu-id="f582e-294">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="f582e-294">deviceHealthAttestationState</span></span>|[<span data-ttu-id="f582e-295">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="f582e-295">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="f582e-296">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="f582e-296">The device health attestation state.</span></span>|
|<span data-ttu-id="f582e-297">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="f582e-297">subscriberCarrier</span></span>|<span data-ttu-id="f582e-298">String</span><span class="sxs-lookup"><span data-stu-id="f582e-298">String</span></span>|<span data-ttu-id="f582e-299">Оператор сотовой связи, используемый абонентом</span><span class="sxs-lookup"><span data-stu-id="f582e-299">Subscriber Carrier</span></span>|
|<span data-ttu-id="f582e-300">meid</span><span class="sxs-lookup"><span data-stu-id="f582e-300">meid</span></span>|<span data-ttu-id="f582e-301">String</span><span class="sxs-lookup"><span data-stu-id="f582e-301">String</span></span>|<span data-ttu-id="f582e-302">MEID</span><span class="sxs-lookup"><span data-stu-id="f582e-302">MEID</span></span>|
|<span data-ttu-id="f582e-303">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="f582e-303">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="f582e-304">Int64</span><span class="sxs-lookup"><span data-stu-id="f582e-304">Int64</span></span>|<span data-ttu-id="f582e-305">Общий объем хранилища в байтах</span><span class="sxs-lookup"><span data-stu-id="f582e-305">Total Storage in Bytes</span></span>|
|<span data-ttu-id="f582e-306">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="f582e-306">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="f582e-307">Int64</span><span class="sxs-lookup"><span data-stu-id="f582e-307">Int64</span></span>|<span data-ttu-id="f582e-308">Свободный объем хранилища в байтах
</span><span class="sxs-lookup"><span data-stu-id="f582e-308">Free Storage in Bytes</span></span>|
|<span data-ttu-id="f582e-309">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="f582e-309">managedDeviceName</span></span>|<span data-ttu-id="f582e-310">String</span><span class="sxs-lookup"><span data-stu-id="f582e-310">String</span></span>|<span data-ttu-id="f582e-311">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="f582e-311">Automatically generated name to identify a device.</span></span> <span data-ttu-id="f582e-312">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="f582e-312">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="f582e-313">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="f582e-313">partnerReportedThreatState</span></span>|[<span data-ttu-id="f582e-314">Манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="f582e-314">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="f582e-315">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="f582e-315">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="f582e-316">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f582e-316">Read Only.</span></span> <span data-ttu-id="f582e-317">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="f582e-317">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="f582e-318">Усерслогжедон</span><span class="sxs-lookup"><span data-stu-id="f582e-318">usersLoggedOn</span></span>|<span data-ttu-id="f582e-319">Коллекция [логжедонусер](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="f582e-319">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="f582e-320">Указывает последнего пользователя, выполнившего вход в систему на устройстве</span><span class="sxs-lookup"><span data-stu-id="f582e-320">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="f582e-321">Префермдмоверграупполициапплиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="f582e-321">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="f582e-322">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f582e-322">DateTimeOffset</span></span>|<span data-ttu-id="f582e-323">Сообщает о значении DateTime, заданном параметром Префермдмоверграупполици.</span><span class="sxs-lookup"><span data-stu-id="f582e-323">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="f582e-324">Если этот параметр установлен, параметры групповой политики в случае конфликта будут переопределяться параметрами групповой политики.</span><span class="sxs-lookup"><span data-stu-id="f582e-324">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="f582e-325">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f582e-325">Read Only.</span></span>|
|<span data-ttu-id="f582e-326">Аутопилотенроллед</span><span class="sxs-lookup"><span data-stu-id="f582e-326">autopilotEnrolled</span></span>|<span data-ttu-id="f582e-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="f582e-327">Boolean</span></span>|<span data-ttu-id="f582e-328">Сообщает, зарегистрировано ли управляемое устройство через Автоматический пилот.</span><span class="sxs-lookup"><span data-stu-id="f582e-328">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="f582e-329">Рекуиреусеренроллментаппровал</span><span class="sxs-lookup"><span data-stu-id="f582e-329">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="f582e-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="f582e-330">Boolean</span></span>|<span data-ttu-id="f582e-331">Указывает, является ли управляемое устройство iOS регистрацией на утверждение пользователя.</span><span class="sxs-lookup"><span data-stu-id="f582e-331">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="f582e-332">Манажементцертификатикспиратиондате</span><span class="sxs-lookup"><span data-stu-id="f582e-332">managementCertificateExpirationDate</span></span>|<span data-ttu-id="f582e-333">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f582e-333">DateTimeOffset</span></span>|<span data-ttu-id="f582e-334">Дата окончания срока действия сертификата управления устройствами</span><span class="sxs-lookup"><span data-stu-id="f582e-334">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="f582e-335">икЦид</span><span class="sxs-lookup"><span data-stu-id="f582e-335">iccid</span></span>|<span data-ttu-id="f582e-336">String</span><span class="sxs-lookup"><span data-stu-id="f582e-336">String</span></span>|<span data-ttu-id="f582e-337">Идентификатор встроенной карты — это уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="f582e-337">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="f582e-338">удид</span><span class="sxs-lookup"><span data-stu-id="f582e-338">udid</span></span>|<span data-ttu-id="f582e-339">String</span><span class="sxs-lookup"><span data-stu-id="f582e-339">String</span></span>|<span data-ttu-id="f582e-340">Уникальный идентификатор устройства для устройств iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="f582e-340">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="f582e-341">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f582e-341">roleScopeTagIds</span></span>|<span data-ttu-id="f582e-342">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f582e-342">String collection</span></span>|<span data-ttu-id="f582e-343">Список идентификаторов тегов области для этого экземпляра устройства.</span><span class="sxs-lookup"><span data-stu-id="f582e-343">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="f582e-344">Виндовсактивемалварекаунт</span><span class="sxs-lookup"><span data-stu-id="f582e-344">windowsActiveMalwareCount</span></span>|<span data-ttu-id="f582e-345">Int32</span><span class="sxs-lookup"><span data-stu-id="f582e-345">Int32</span></span>|<span data-ttu-id="f582e-346">Число активных вредоносных программ для этого устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="f582e-346">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="f582e-347">Виндовсремедиатедмалварекаунт</span><span class="sxs-lookup"><span data-stu-id="f582e-347">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="f582e-348">Int32</span><span class="sxs-lookup"><span data-stu-id="f582e-348">Int32</span></span>|<span data-ttu-id="f582e-349">Количество исправленных вредоносных программ для этого устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="f582e-349">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="f582e-350">notes</span><span class="sxs-lookup"><span data-stu-id="f582e-350">notes</span></span>|<span data-ttu-id="f582e-351">String</span><span class="sxs-lookup"><span data-stu-id="f582e-351">String</span></span>|<span data-ttu-id="f582e-352">Примечания к устройству, созданному ИТ ИТ Admin</span><span class="sxs-lookup"><span data-stu-id="f582e-352">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="f582e-353">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="f582e-353">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="f582e-354">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="f582e-354">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="f582e-355">Состояние работоспособности клиента Configuration Manager, действительно только для устройств под управлением агентов MDM/ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="f582e-355">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="f582e-356">Отклик</span><span class="sxs-lookup"><span data-stu-id="f582e-356">Response</span></span>
<span data-ttu-id="f582e-357">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDevice](../resources/intune-devices-manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f582e-357">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f582e-358">Пример</span><span class="sxs-lookup"><span data-stu-id="f582e-358">Example</span></span>

### <a name="request"></a><span data-ttu-id="f582e-359">Запрос</span><span class="sxs-lookup"><span data-stu-id="f582e-359">Request</span></span>
<span data-ttu-id="f582e-360">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f582e-360">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7224

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
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
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```

### <a name="response"></a><span data-ttu-id="f582e-361">Отклик</span><span class="sxs-lookup"><span data-stu-id="f582e-361">Response</span></span>
<span data-ttu-id="f582e-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f582e-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7273

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
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
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```





