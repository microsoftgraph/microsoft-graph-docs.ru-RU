---
title: Обновление managedDevice
description: Обновление свойств объекта managedDevice.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 31c1b1a497dcd5cabf4b7b97b56811dbbedb2a5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858613"
---
# <a name="update-manageddevice"></a><span data-ttu-id="a8073-103">Обновление managedDevice</span><span class="sxs-lookup"><span data-stu-id="a8073-103">Update managedDevice</span></span>

> <span data-ttu-id="a8073-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a8073-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8073-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8073-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8073-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a8073-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8073-107">Обновление свойств объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="a8073-107">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8073-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a8073-108">Prerequisites</span></span>
<span data-ttu-id="a8073-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8073-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8073-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8073-111">Permission type</span></span>|<span data-ttu-id="a8073-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8073-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8073-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8073-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8073-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8073-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a8073-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8073-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8073-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8073-116">Not supported.</span></span>|
|<span data-ttu-id="a8073-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8073-117">Application</span></span>|<span data-ttu-id="a8073-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8073-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8073-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8073-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="a8073-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8073-120">Request headers</span></span>
|<span data-ttu-id="a8073-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8073-121">Header</span></span>|<span data-ttu-id="a8073-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a8073-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8073-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8073-123">Authorization</span></span>|<span data-ttu-id="a8073-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a8073-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8073-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a8073-125">Accept</span></span>|<span data-ttu-id="a8073-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8073-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8073-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a8073-127">Request body</span></span>
<span data-ttu-id="a8073-128">В теле запроса добавьте представление объекта [managedDevice](../resources/intune-devices-manageddevice.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8073-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="a8073-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="a8073-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="a8073-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8073-130">Property</span></span>|<span data-ttu-id="a8073-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a8073-131">Type</span></span>|<span data-ttu-id="a8073-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a8073-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8073-133">id</span><span class="sxs-lookup"><span data-stu-id="a8073-133">id</span></span>|<span data-ttu-id="a8073-134">String</span><span class="sxs-lookup"><span data-stu-id="a8073-134">String</span></span>|<span data-ttu-id="a8073-135">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="a8073-135">Unique Identifier for the device</span></span>|
|<span data-ttu-id="a8073-136">userId</span><span class="sxs-lookup"><span data-stu-id="a8073-136">userId</span></span>|<span data-ttu-id="a8073-137">String</span><span class="sxs-lookup"><span data-stu-id="a8073-137">String</span></span>|<span data-ttu-id="a8073-138">Уникальный идентификатор пользователя, связанного с устройством.
</span><span class="sxs-lookup"><span data-stu-id="a8073-138">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="a8073-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="a8073-139">deviceName</span></span>|<span data-ttu-id="a8073-140">String</span><span class="sxs-lookup"><span data-stu-id="a8073-140">String</span></span>|<span data-ttu-id="a8073-141">Название устройства</span><span class="sxs-lookup"><span data-stu-id="a8073-141">Name of the device</span></span>|
|<span data-ttu-id="a8073-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="a8073-142">hardwareInformation</span></span>|[<span data-ttu-id="a8073-143">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="a8073-143">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="a8073-144">Сведения о объектами для устройства.</span><span class="sxs-lookup"><span data-stu-id="a8073-144">The hardward details for the device.</span></span>  <span data-ttu-id="a8073-145">Содержит сведения, такие как дисковое пространство, производителя, серийный номер, и т.д.</span><span class="sxs-lookup"><span data-stu-id="a8073-145">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="a8073-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="a8073-146">ownerType</span></span>|[<span data-ttu-id="a8073-147">ownerType</span><span class="sxs-lookup"><span data-stu-id="a8073-147">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="a8073-148">Владельцем устройства.</span><span class="sxs-lookup"><span data-stu-id="a8073-148">Ownership of the device.</span></span> <span data-ttu-id="a8073-149">Может быть «компания» или «личные».</span><span class="sxs-lookup"><span data-stu-id="a8073-149">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="a8073-150">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="a8073-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="a8073-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="a8073-151">managedDeviceOwnerType</span></span>|[<span data-ttu-id="a8073-152">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="a8073-152">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="a8073-153">Владельцем устройства.</span><span class="sxs-lookup"><span data-stu-id="a8073-153">Ownership of the device.</span></span> <span data-ttu-id="a8073-154">Может быть «компания» или «личные».</span><span class="sxs-lookup"><span data-stu-id="a8073-154">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="a8073-155">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="a8073-155">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="a8073-156">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="a8073-156">deviceActionResults</span></span>|<span data-ttu-id="a8073-157">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a8073-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="a8073-158">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="a8073-158">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="a8073-159">managementState</span><span class="sxs-lookup"><span data-stu-id="a8073-159">managementState</span></span>|[<span data-ttu-id="a8073-160">managementState</span><span class="sxs-lookup"><span data-stu-id="a8073-160">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="a8073-161">Состояние управления устройства.</span><span class="sxs-lookup"><span data-stu-id="a8073-161">Management state of the device.</span></span> <span data-ttu-id="a8073-162">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="a8073-162">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="a8073-163">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="a8073-163">enrolledDateTime</span></span>|<span data-ttu-id="a8073-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8073-164">DateTimeOffset</span></span>|<span data-ttu-id="a8073-165">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="a8073-165">Enrollment time of the device.</span></span>|
|<span data-ttu-id="a8073-166">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a8073-166">lastSyncDateTime</span></span>|<span data-ttu-id="a8073-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8073-167">DateTimeOffset</span></span>|<span data-ttu-id="a8073-168">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="a8073-168">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="a8073-169">Тип корпуса</span><span class="sxs-lookup"><span data-stu-id="a8073-169">chassisType</span></span>|[<span data-ttu-id="a8073-170">Тип корпуса</span><span class="sxs-lookup"><span data-stu-id="a8073-170">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="a8073-171">Тип корпуса устройства.</span><span class="sxs-lookup"><span data-stu-id="a8073-171">Chassis type of the device.</span></span> <span data-ttu-id="a8073-172">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="a8073-172">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="a8073-173">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="a8073-173">operatingSystem</span></span>|<span data-ttu-id="a8073-174">String</span><span class="sxs-lookup"><span data-stu-id="a8073-174">String</span></span>|<span data-ttu-id="a8073-175">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="a8073-175">Operating system of the device.</span></span> <span data-ttu-id="a8073-176">Windows, iOS и т. д.</span><span class="sxs-lookup"><span data-stu-id="a8073-176">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="a8073-177">deviceType</span><span class="sxs-lookup"><span data-stu-id="a8073-177">deviceType</span></span>|[<span data-ttu-id="a8073-178">deviceType</span><span class="sxs-lookup"><span data-stu-id="a8073-178">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="a8073-179">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="a8073-179">Platform of the device.</span></span> <span data-ttu-id="a8073-180">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a8073-180">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="a8073-181">complianceState</span><span class="sxs-lookup"><span data-stu-id="a8073-181">complianceState</span></span>|[<span data-ttu-id="a8073-182">complianceState</span><span class="sxs-lookup"><span data-stu-id="a8073-182">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="a8073-183">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="a8073-183">Compliance state of the device.</span></span> <span data-ttu-id="a8073-184">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="a8073-184">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="a8073-185">jailBroken</span><span class="sxs-lookup"><span data-stu-id="a8073-185">jailBroken</span></span>|<span data-ttu-id="a8073-186">String</span><span class="sxs-lookup"><span data-stu-id="a8073-186">String</span></span>|<span data-ttu-id="a8073-187">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="a8073-187">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="a8073-188">managementAgent</span><span class="sxs-lookup"><span data-stu-id="a8073-188">managementAgent</span></span>|[<span data-ttu-id="a8073-189">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="a8073-189">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="a8073-190">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="a8073-190">Management channel of the device.</span></span> <span data-ttu-id="a8073-191">Intune, EAS, и т.д. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="a8073-191">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="a8073-192">osVersion</span><span class="sxs-lookup"><span data-stu-id="a8073-192">osVersion</span></span>|<span data-ttu-id="a8073-193">String</span><span class="sxs-lookup"><span data-stu-id="a8073-193">String</span></span>|<span data-ttu-id="a8073-194">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="a8073-194">Operating system version of the device.</span></span>|
|<span data-ttu-id="a8073-195">easActivated</span><span class="sxs-lookup"><span data-stu-id="a8073-195">easActivated</span></span>|<span data-ttu-id="a8073-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8073-196">Boolean</span></span>|<span data-ttu-id="a8073-197">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="a8073-197">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="a8073-198">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="a8073-198">easDeviceId</span></span>|<span data-ttu-id="a8073-199">String</span><span class="sxs-lookup"><span data-stu-id="a8073-199">String</span></span>|<span data-ttu-id="a8073-200">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="a8073-200">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="a8073-201">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="a8073-201">easActivationDateTime</span></span>|<span data-ttu-id="a8073-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8073-202">DateTimeOffset</span></span>|<span data-ttu-id="a8073-203">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="a8073-203">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="a8073-204">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="a8073-204">aadRegistered</span></span>|<span data-ttu-id="a8073-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8073-205">Boolean</span></span>|<span data-ttu-id="a8073-206">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a8073-206">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="a8073-207">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="a8073-207">azureADRegistered</span></span>|<span data-ttu-id="a8073-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8073-208">Boolean</span></span>|<span data-ttu-id="a8073-209">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a8073-209">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="a8073-210">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a8073-210">deviceEnrollmentType</span></span>|[<span data-ttu-id="a8073-211">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a8073-211">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="a8073-212">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="a8073-212">Enrollment type of the device.</span></span> <span data-ttu-id="a8073-213">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="a8073-213">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="a8073-214">lostModeState</span><span class="sxs-lookup"><span data-stu-id="a8073-214">lostModeState</span></span>|[<span data-ttu-id="a8073-215">lostModeState</span><span class="sxs-lookup"><span data-stu-id="a8073-215">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="a8073-216">Указывает, включен ли режим потеряны.</span><span class="sxs-lookup"><span data-stu-id="a8073-216">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="a8073-217">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="a8073-217">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="a8073-218">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="a8073-218">activationLockBypassCode</span></span>|<span data-ttu-id="a8073-219">String</span><span class="sxs-lookup"><span data-stu-id="a8073-219">String</span></span>|<span data-ttu-id="a8073-220">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a8073-220">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="a8073-221">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a8073-221">emailAddress</span></span>|<span data-ttu-id="a8073-222">String</span><span class="sxs-lookup"><span data-stu-id="a8073-222">String</span></span>|<span data-ttu-id="a8073-223">Адреса электронной почты пользователя, связанного с устройством</span><span class="sxs-lookup"><span data-stu-id="a8073-223">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="a8073-224">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="a8073-224">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="a8073-225">String</span><span class="sxs-lookup"><span data-stu-id="a8073-225">String</span></span>|<span data-ttu-id="a8073-226">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a8073-226">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="a8073-227">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8073-227">Read only.</span></span>|
|<span data-ttu-id="a8073-228">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="a8073-228">azureADDeviceId</span></span>|<span data-ttu-id="a8073-229">String</span><span class="sxs-lookup"><span data-stu-id="a8073-229">String</span></span>|<span data-ttu-id="a8073-230">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a8073-230">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="a8073-231">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8073-231">Read only.</span></span>|
|<span data-ttu-id="a8073-232">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="a8073-232">deviceRegistrationState</span></span>|[<span data-ttu-id="a8073-233">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="a8073-233">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="a8073-234">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="a8073-234">Device registration state.</span></span> <span data-ttu-id="a8073-235">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a8073-235">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="a8073-236">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="a8073-236">deviceCategoryDisplayName</span></span>|<span data-ttu-id="a8073-237">String</span><span class="sxs-lookup"><span data-stu-id="a8073-237">String</span></span>|<span data-ttu-id="a8073-238">Отображаемое имя категории устройства</span><span class="sxs-lookup"><span data-stu-id="a8073-238">Device category display name</span></span>|
|<span data-ttu-id="a8073-239">isSupervised</span><span class="sxs-lookup"><span data-stu-id="a8073-239">isSupervised</span></span>|<span data-ttu-id="a8073-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8073-240">Boolean</span></span>|<span data-ttu-id="a8073-241">Состояние защиты устройства</span><span class="sxs-lookup"><span data-stu-id="a8073-241">Device supervised status</span></span>|
|<span data-ttu-id="a8073-242">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a8073-242">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="a8073-243">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8073-243">DateTimeOffset</span></span>|<span data-ttu-id="a8073-244">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8073-244">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="a8073-245">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="a8073-245">exchangeAccessState</span></span>|[<span data-ttu-id="a8073-246">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="a8073-246">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="a8073-247">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8073-247">The Access State of the device in Exchange.</span></span> <span data-ttu-id="a8073-248">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="a8073-248">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="a8073-249">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="a8073-249">exchangeAccessStateReason</span></span>|[<span data-ttu-id="a8073-250">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="a8073-250">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="a8073-251">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8073-251">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="a8073-252">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="a8073-252">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="a8073-253">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="a8073-253">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="a8073-254">String</span><span class="sxs-lookup"><span data-stu-id="a8073-254">String</span></span>|<span data-ttu-id="a8073-255">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="a8073-255">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="a8073-256">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="a8073-256">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="a8073-257">String</span><span class="sxs-lookup"><span data-stu-id="a8073-257">String</span></span>|<span data-ttu-id="a8073-258">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="a8073-258">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="a8073-259">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="a8073-259">isEncrypted</span></span>|<span data-ttu-id="a8073-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8073-260">Boolean</span></span>|<span data-ttu-id="a8073-261">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="a8073-261">Device encryption status</span></span>|
|<span data-ttu-id="a8073-262">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a8073-262">userPrincipalName</span></span>|<span data-ttu-id="a8073-263">String</span><span class="sxs-lookup"><span data-stu-id="a8073-263">String</span></span>|<span data-ttu-id="a8073-264">Имя участника-пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="a8073-264">Device user principal name</span></span>|
|<span data-ttu-id="a8073-265">model</span><span class="sxs-lookup"><span data-stu-id="a8073-265">model</span></span>|<span data-ttu-id="a8073-266">String</span><span class="sxs-lookup"><span data-stu-id="a8073-266">String</span></span>|<span data-ttu-id="a8073-267">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="a8073-267">Model of the device</span></span>|
|<span data-ttu-id="a8073-268">manufacturer</span><span class="sxs-lookup"><span data-stu-id="a8073-268">manufacturer</span></span>|<span data-ttu-id="a8073-269">String</span><span class="sxs-lookup"><span data-stu-id="a8073-269">String</span></span>|<span data-ttu-id="a8073-270">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="a8073-270">Manufacturer of the device</span></span>|
|<span data-ttu-id="a8073-271">imei</span><span class="sxs-lookup"><span data-stu-id="a8073-271">imei</span></span>|<span data-ttu-id="a8073-272">String</span><span class="sxs-lookup"><span data-stu-id="a8073-272">String</span></span>|<span data-ttu-id="a8073-273">IMEI</span><span class="sxs-lookup"><span data-stu-id="a8073-273">IMEI</span></span>|
|<span data-ttu-id="a8073-274">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a8073-274">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a8073-275">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8073-275">DateTimeOffset</span></span>|<span data-ttu-id="a8073-276">Дата и время истечения льготного периода соответствия устройства требованиям</span><span class="sxs-lookup"><span data-stu-id="a8073-276">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="a8073-277">serialNumber</span><span class="sxs-lookup"><span data-stu-id="a8073-277">serialNumber</span></span>|<span data-ttu-id="a8073-278">String</span><span class="sxs-lookup"><span data-stu-id="a8073-278">String</span></span>|<span data-ttu-id="a8073-279">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="a8073-279">SerialNumber</span></span>|
|<span data-ttu-id="a8073-280">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="a8073-280">phoneNumber</span></span>|<span data-ttu-id="a8073-281">String</span><span class="sxs-lookup"><span data-stu-id="a8073-281">String</span></span>|<span data-ttu-id="a8073-282">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="a8073-282">Phone number of the device</span></span>|
|<span data-ttu-id="a8073-283">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="a8073-283">androidSecurityPatchLevel</span></span>|<span data-ttu-id="a8073-284">String</span><span class="sxs-lookup"><span data-stu-id="a8073-284">String</span></span>|<span data-ttu-id="a8073-285">Уровень обновления для системы безопасности Android</span><span class="sxs-lookup"><span data-stu-id="a8073-285">Android security patch level</span></span>|
|<span data-ttu-id="a8073-286">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a8073-286">userDisplayName</span></span>|<span data-ttu-id="a8073-287">String</span><span class="sxs-lookup"><span data-stu-id="a8073-287">String</span></span>|<span data-ttu-id="a8073-288">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="a8073-288">User display name</span></span>|
|<span data-ttu-id="a8073-289">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="a8073-289">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="a8073-290">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="a8073-290">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="a8073-291">Включенные функции клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="a8073-291">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="a8073-292">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="a8073-292">wiFiMacAddress</span></span>|<span data-ttu-id="a8073-293">String</span><span class="sxs-lookup"><span data-stu-id="a8073-293">String</span></span>|<span data-ttu-id="a8073-294">MAC-адрес сети Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="a8073-294">Wi-Fi MAC</span></span>|
|<span data-ttu-id="a8073-295">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="a8073-295">deviceHealthAttestationState</span></span>|[<span data-ttu-id="a8073-296">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="a8073-296">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="a8073-297">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="a8073-297">The device health attestation state.</span></span>|
|<span data-ttu-id="a8073-298">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="a8073-298">subscriberCarrier</span></span>|<span data-ttu-id="a8073-299">String</span><span class="sxs-lookup"><span data-stu-id="a8073-299">String</span></span>|<span data-ttu-id="a8073-300">Оператор сотовой связи, используемый абонентом</span><span class="sxs-lookup"><span data-stu-id="a8073-300">Subscriber Carrier</span></span>|
|<span data-ttu-id="a8073-301">meid</span><span class="sxs-lookup"><span data-stu-id="a8073-301">meid</span></span>|<span data-ttu-id="a8073-302">String</span><span class="sxs-lookup"><span data-stu-id="a8073-302">String</span></span>|<span data-ttu-id="a8073-303">MEID</span><span class="sxs-lookup"><span data-stu-id="a8073-303">MEID</span></span>|
|<span data-ttu-id="a8073-304">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="a8073-304">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="a8073-305">Int64</span><span class="sxs-lookup"><span data-stu-id="a8073-305">Int64</span></span>|<span data-ttu-id="a8073-306">Общий объем хранилища в байтах</span><span class="sxs-lookup"><span data-stu-id="a8073-306">Total Storage in Bytes</span></span>|
|<span data-ttu-id="a8073-307">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="a8073-307">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="a8073-308">Int64</span><span class="sxs-lookup"><span data-stu-id="a8073-308">Int64</span></span>|<span data-ttu-id="a8073-309">Свободный объем хранилища в байтах
</span><span class="sxs-lookup"><span data-stu-id="a8073-309">Free Storage in Bytes</span></span>|
|<span data-ttu-id="a8073-310">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="a8073-310">managedDeviceName</span></span>|<span data-ttu-id="a8073-311">String</span><span class="sxs-lookup"><span data-stu-id="a8073-311">String</span></span>|<span data-ttu-id="a8073-312">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="a8073-312">Automatically generated name to identify a device.</span></span> <span data-ttu-id="a8073-313">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="a8073-313">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="a8073-314">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="a8073-314">partnerReportedThreatState</span></span>|[<span data-ttu-id="a8073-315">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="a8073-315">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="a8073-316">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="a8073-316">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="a8073-317">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8073-317">Read Only.</span></span> <span data-ttu-id="a8073-318">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="a8073-318">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="a8073-319">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="a8073-319">usersLoggedOn</span></span>|<span data-ttu-id="a8073-320">[loggedOnUser](../resources/intune-devices-loggedonuser.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a8073-320">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="a8073-321">Указывает последний вход в систему пользователей устройства</span><span class="sxs-lookup"><span data-stu-id="a8073-321">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="a8073-322">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8073-322">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="a8073-323">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8073-323">DateTimeOffset</span></span>|<span data-ttu-id="a8073-324">Отчеты о DateTime параметр preferMdmOverGroupPolicy имеет значение.</span><span class="sxs-lookup"><span data-stu-id="a8073-324">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="a8073-325">Если задано, параметры Intune MDM переопределяет параметры групповой политики в случае конфликта.</span><span class="sxs-lookup"><span data-stu-id="a8073-325">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="a8073-326">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8073-326">Read Only.</span></span>|
|<span data-ttu-id="a8073-327">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="a8073-327">autopilotEnrolled</span></span>|<span data-ttu-id="a8073-328">Логический</span><span class="sxs-lookup"><span data-stu-id="a8073-328">Boolean</span></span>|<span data-ttu-id="a8073-329">Отчеты при регистрации управляемой устройство через автопилот.</span><span class="sxs-lookup"><span data-stu-id="a8073-329">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="a8073-330">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="a8073-330">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="a8073-331">Логический</span><span class="sxs-lookup"><span data-stu-id="a8073-331">Boolean</span></span>|<span data-ttu-id="a8073-332">Отчеты, если устройство управляемых iOS утверждения регистрации пользователя.</span><span class="sxs-lookup"><span data-stu-id="a8073-332">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="a8073-333">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="a8073-333">managementCertificateExpirationDate</span></span>|<span data-ttu-id="a8073-334">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8073-334">DateTimeOffset</span></span>|<span data-ttu-id="a8073-335">Дата окончания срока действия сертификата управления устройства отчетов</span><span class="sxs-lookup"><span data-stu-id="a8073-335">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="a8073-336">iccid</span><span class="sxs-lookup"><span data-stu-id="a8073-336">iccid</span></span>|<span data-ttu-id="a8073-337">Строка</span><span class="sxs-lookup"><span data-stu-id="a8073-337">String</span></span>|<span data-ttu-id="a8073-338">Идентификатор карты интегральной, это уникальный идентификационный номер карты диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="a8073-338">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="a8073-339">UDID</span><span class="sxs-lookup"><span data-stu-id="a8073-339">udid</span></span>|<span data-ttu-id="a8073-340">Строка</span><span class="sxs-lookup"><span data-stu-id="a8073-340">String</span></span>|<span data-ttu-id="a8073-341">Уникальный идентификатор устройства для операций ввода-вывода и macOS устройств.</span><span class="sxs-lookup"><span data-stu-id="a8073-341">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="a8073-342">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a8073-342">roleScopeTagIds</span></span>|<span data-ttu-id="a8073-343">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a8073-343">String collection</span></span>|<span data-ttu-id="a8073-344">Список идентификаторов тег области для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="a8073-344">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="a8073-345">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="a8073-345">windowsActiveMalwareCount</span></span>|<span data-ttu-id="a8073-346">Int32</span><span class="sxs-lookup"><span data-stu-id="a8073-346">Int32</span></span>|<span data-ttu-id="a8073-347">Число активных вредоносных программ для этого устройства windows</span><span class="sxs-lookup"><span data-stu-id="a8073-347">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="a8073-348">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="a8073-348">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="a8073-349">Int32</span><span class="sxs-lookup"><span data-stu-id="a8073-349">Int32</span></span>|<span data-ttu-id="a8073-350">Число проверка вредоносных программ для этого устройства windows</span><span class="sxs-lookup"><span data-stu-id="a8073-350">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="a8073-351">notes</span><span class="sxs-lookup"><span data-stu-id="a8073-351">notes</span></span>|<span data-ttu-id="a8073-352">String</span><span class="sxs-lookup"><span data-stu-id="a8073-352">String</span></span>|<span data-ttu-id="a8073-353">Заметки на устройстве, созданные в ИТ-администратор</span><span class="sxs-lookup"><span data-stu-id="a8073-353">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="a8073-354">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="a8073-354">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="a8073-355">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="a8073-355">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="a8073-356">Конфигурация диспетчера состоянием работоспособности клиента, только для устройств, управляемых MDM/ConfigMgr агента</span><span class="sxs-lookup"><span data-stu-id="a8073-356">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="a8073-357">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8073-357">Response</span></span>
<span data-ttu-id="a8073-358">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDevice](../resources/intune-devices-manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a8073-358">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8073-359">Пример</span><span class="sxs-lookup"><span data-stu-id="a8073-359">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8073-360">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8073-360">Request</span></span>
<span data-ttu-id="a8073-361">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8073-361">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7114

{
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

### <a name="response"></a><span data-ttu-id="a8073-362">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8073-362">Response</span></span>
<span data-ttu-id="a8073-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a8073-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7215

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





