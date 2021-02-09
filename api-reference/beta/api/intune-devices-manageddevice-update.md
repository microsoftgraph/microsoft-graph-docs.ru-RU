---
title: Обновление managedDevice
description: Обновление свойств объекта managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af0b6c6f63df6c0575ce5d3901f3e77720d7943b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159691"
---
# <a name="update-manageddevice"></a><span data-ttu-id="0083e-103">Обновление managedDevice</span><span class="sxs-lookup"><span data-stu-id="0083e-103">Update managedDevice</span></span>

<span data-ttu-id="0083e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0083e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0083e-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0083e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0083e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0083e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0083e-107">Обновление свойств объекта [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="0083e-107">Update the properties of a [managedDevice](../resources/intune-shared-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0083e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0083e-108">Prerequisites</span></span>
<span data-ttu-id="0083e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0083e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0083e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0083e-111">Permission type</span></span>|<span data-ttu-id="0083e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0083e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0083e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0083e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0083e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0083e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0083e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0083e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0083e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0083e-116">Not supported.</span></span>|
|<span data-ttu-id="0083e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0083e-117">Application</span></span>|<span data-ttu-id="0083e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0083e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0083e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0083e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/comanagedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="0083e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0083e-120">Request headers</span></span>
|<span data-ttu-id="0083e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0083e-121">Header</span></span>|<span data-ttu-id="0083e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0083e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0083e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0083e-123">Authorization</span></span>|<span data-ttu-id="0083e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0083e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0083e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0083e-125">Accept</span></span>|<span data-ttu-id="0083e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0083e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0083e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0083e-127">Request body</span></span>
<span data-ttu-id="0083e-128">В теле запроса добавьте представление объекта [managedDevice](../resources/intune-shared-manageddevice.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0083e-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-shared-manageddevice.md) object.</span></span>

<span data-ttu-id="0083e-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="0083e-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-shared-manageddevice.md).</span></span>

|<span data-ttu-id="0083e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0083e-130">Property</span></span>|<span data-ttu-id="0083e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0083e-131">Type</span></span>|<span data-ttu-id="0083e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0083e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0083e-133">id</span><span class="sxs-lookup"><span data-stu-id="0083e-133">id</span></span>|<span data-ttu-id="0083e-134">String</span><span class="sxs-lookup"><span data-stu-id="0083e-134">String</span></span>|<span data-ttu-id="0083e-135">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-135">Unique Identifier for the device.</span></span> <span data-ttu-id="0083e-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-136">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-137">userId</span><span class="sxs-lookup"><span data-stu-id="0083e-137">userId</span></span>|<span data-ttu-id="0083e-138">String</span><span class="sxs-lookup"><span data-stu-id="0083e-138">String</span></span>|<span data-ttu-id="0083e-139">Уникальный идентификатор пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="0083e-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="0083e-140">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-140">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="0083e-141">deviceName</span></span>|<span data-ttu-id="0083e-142">String</span><span class="sxs-lookup"><span data-stu-id="0083e-142">String</span></span>|<span data-ttu-id="0083e-143">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-143">Name of the device.</span></span> <span data-ttu-id="0083e-144">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-144">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-145">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="0083e-145">hardwareInformation</span></span>|[<span data-ttu-id="0083e-146">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="0083e-146">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="0083e-147">Подробные сведения об устройстве.</span><span class="sxs-lookup"><span data-stu-id="0083e-147">The hardward details for the device.</span></span>  <span data-ttu-id="0083e-148">Включает такие сведения, как место в хранилище, изготовитель, серийный номер и т. д. Это свойство находится только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-148">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span>|
|<span data-ttu-id="0083e-149">ownerType</span><span class="sxs-lookup"><span data-stu-id="0083e-149">ownerType</span></span>|[<span data-ttu-id="0083e-150">ownerType</span><span class="sxs-lookup"><span data-stu-id="0083e-150">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="0083e-151">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="0083e-151">Ownership of the device.</span></span> <span data-ttu-id="0083e-152">Может быть "company" или "personal".</span><span class="sxs-lookup"><span data-stu-id="0083e-152">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="0083e-153">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="0083e-153">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="0083e-154">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="0083e-154">managedDeviceOwnerType</span></span>|[<span data-ttu-id="0083e-155">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="0083e-155">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="0083e-156">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="0083e-156">Ownership of the device.</span></span> <span data-ttu-id="0083e-157">Может быть "company" или "personal".</span><span class="sxs-lookup"><span data-stu-id="0083e-157">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="0083e-158">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="0083e-158">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="0083e-159">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="0083e-159">deviceActionResults</span></span>|<span data-ttu-id="0083e-160">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0083e-160">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="0083e-161">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="0083e-161">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="0083e-162">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-162">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-163">managementState</span><span class="sxs-lookup"><span data-stu-id="0083e-163">managementState</span></span>|[<span data-ttu-id="0083e-164">managementState</span><span class="sxs-lookup"><span data-stu-id="0083e-164">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="0083e-165">Состояние управления устройством.</span><span class="sxs-lookup"><span data-stu-id="0083e-165">Management state of the device.</span></span> <span data-ttu-id="0083e-166">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-166">This property is read-only.</span></span> <span data-ttu-id="0083e-167">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="0083e-167">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="0083e-168">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="0083e-168">enrolledDateTime</span></span>|<span data-ttu-id="0083e-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0083e-169">DateTimeOffset</span></span>|<span data-ttu-id="0083e-170">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-170">Enrollment time of the device.</span></span> <span data-ttu-id="0083e-171">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-171">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-172">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0083e-172">lastSyncDateTime</span></span>|<span data-ttu-id="0083e-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0083e-173">DateTimeOffset</span></span>|<span data-ttu-id="0083e-174">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="0083e-174">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="0083e-175">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-175">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-176">chassisType</span><span class="sxs-lookup"><span data-stu-id="0083e-176">chassisType</span></span>|[<span data-ttu-id="0083e-177">chassisType</span><span class="sxs-lookup"><span data-stu-id="0083e-177">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="0083e-178">Тип корпусов устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-178">Chassis type of the device.</span></span> <span data-ttu-id="0083e-179">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-179">This property is read-only.</span></span> <span data-ttu-id="0083e-180">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="0083e-180">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="0083e-181">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="0083e-181">operatingSystem</span></span>|<span data-ttu-id="0083e-182">String</span><span class="sxs-lookup"><span data-stu-id="0083e-182">String</span></span>|<span data-ttu-id="0083e-183">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-183">Operating system of the device.</span></span> <span data-ttu-id="0083e-184">Windows, iOS и т. д. Это свойство является свойством только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-184">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="0083e-185">deviceType</span><span class="sxs-lookup"><span data-stu-id="0083e-185">deviceType</span></span>|[<span data-ttu-id="0083e-186">deviceType</span><span class="sxs-lookup"><span data-stu-id="0083e-186">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="0083e-187">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-187">Platform of the device.</span></span> <span data-ttu-id="0083e-188">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-188">This property is read-only.</span></span> <span data-ttu-id="0083e-189">Возможные значения: `desktop` , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` , , `winEmbedded` , `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` , `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` `cloudPC` .</span><span class="sxs-lookup"><span data-stu-id="0083e-189">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="0083e-190">complianceState</span><span class="sxs-lookup"><span data-stu-id="0083e-190">complianceState</span></span>|[<span data-ttu-id="0083e-191">complianceState</span><span class="sxs-lookup"><span data-stu-id="0083e-191">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="0083e-192">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="0083e-192">Compliance state of the device.</span></span> <span data-ttu-id="0083e-193">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-193">This property is read-only.</span></span> <span data-ttu-id="0083e-194">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="0083e-194">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="0083e-195">jailBroken</span><span class="sxs-lookup"><span data-stu-id="0083e-195">jailBroken</span></span>|<span data-ttu-id="0083e-196">String</span><span class="sxs-lookup"><span data-stu-id="0083e-196">String</span></span>|<span data-ttu-id="0083e-197">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="0083e-197">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="0083e-198">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-198">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-199">managementAgent</span><span class="sxs-lookup"><span data-stu-id="0083e-199">managementAgent</span></span>|[<span data-ttu-id="0083e-200">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="0083e-200">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="0083e-201">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="0083e-201">Management channel of the device.</span></span> <span data-ttu-id="0083e-202">Intune, EAS и т. д. Это свойство является свойством только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-202">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="0083e-203">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="0083e-203">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="0083e-204">osVersion</span><span class="sxs-lookup"><span data-stu-id="0083e-204">osVersion</span></span>|<span data-ttu-id="0083e-205">String</span><span class="sxs-lookup"><span data-stu-id="0083e-205">String</span></span>|<span data-ttu-id="0083e-206">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-206">Operating system version of the device.</span></span> <span data-ttu-id="0083e-207">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-207">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-208">easActivated</span><span class="sxs-lookup"><span data-stu-id="0083e-208">easActivated</span></span>|<span data-ttu-id="0083e-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="0083e-209">Boolean</span></span>|<span data-ttu-id="0083e-210">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="0083e-210">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="0083e-211">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-211">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-212">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="0083e-212">easDeviceId</span></span>|<span data-ttu-id="0083e-213">String</span><span class="sxs-lookup"><span data-stu-id="0083e-213">String</span></span>|<span data-ttu-id="0083e-214">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="0083e-214">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="0083e-215">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-215">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-216">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="0083e-216">easActivationDateTime</span></span>|<span data-ttu-id="0083e-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0083e-217">DateTimeOffset</span></span>|<span data-ttu-id="0083e-218">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="0083e-218">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="0083e-219">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-219">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-220">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="0083e-220">aadRegistered</span></span>|<span data-ttu-id="0083e-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="0083e-221">Boolean</span></span>|<span data-ttu-id="0083e-222">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0083e-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="0083e-223">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-223">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-224">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="0083e-224">azureADRegistered</span></span>|<span data-ttu-id="0083e-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="0083e-225">Boolean</span></span>|<span data-ttu-id="0083e-226">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0083e-226">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="0083e-227">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-227">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-228">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0083e-228">deviceEnrollmentType</span></span>|[<span data-ttu-id="0083e-229">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0083e-229">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="0083e-230">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-230">Enrollment type of the device.</span></span> <span data-ttu-id="0083e-231">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-231">This property is read-only.</span></span> <span data-ttu-id="0083e-232">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="0083e-232">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="0083e-233">lostModeState</span><span class="sxs-lookup"><span data-stu-id="0083e-233">lostModeState</span></span>|[<span data-ttu-id="0083e-234">lostModeState</span><span class="sxs-lookup"><span data-stu-id="0083e-234">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="0083e-235">Указывает, включен ли режим потери.</span><span class="sxs-lookup"><span data-stu-id="0083e-235">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="0083e-236">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-236">This property is read-only.</span></span> <span data-ttu-id="0083e-237">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="0083e-237">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="0083e-238">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="0083e-238">activationLockBypassCode</span></span>|<span data-ttu-id="0083e-239">String</span><span class="sxs-lookup"><span data-stu-id="0083e-239">String</span></span>|<span data-ttu-id="0083e-240">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="0083e-240">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="0083e-241">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-241">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-242">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0083e-242">emailAddress</span></span>|<span data-ttu-id="0083e-243">String</span><span class="sxs-lookup"><span data-stu-id="0083e-243">String</span></span>|<span data-ttu-id="0083e-244">Электронная почта пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="0083e-244">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="0083e-245">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-245">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-246">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="0083e-246">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="0083e-247">String</span><span class="sxs-lookup"><span data-stu-id="0083e-247">String</span></span>|<span data-ttu-id="0083e-248">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0083e-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="0083e-249">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-249">Read only.</span></span> <span data-ttu-id="0083e-250">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-250">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-251">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="0083e-251">azureADDeviceId</span></span>|<span data-ttu-id="0083e-252">String</span><span class="sxs-lookup"><span data-stu-id="0083e-252">String</span></span>|<span data-ttu-id="0083e-253">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0083e-253">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="0083e-254">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-254">Read only.</span></span> <span data-ttu-id="0083e-255">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-255">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-256">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="0083e-256">deviceRegistrationState</span></span>|[<span data-ttu-id="0083e-257">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="0083e-257">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="0083e-258">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-258">Device registration state.</span></span> <span data-ttu-id="0083e-259">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-259">This property is read-only.</span></span> <span data-ttu-id="0083e-260">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0083e-260">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="0083e-261">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="0083e-261">deviceCategoryDisplayName</span></span>|<span data-ttu-id="0083e-262">String</span><span class="sxs-lookup"><span data-stu-id="0083e-262">String</span></span>|<span data-ttu-id="0083e-263">Отображаемая имя категории устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-263">Device category display name.</span></span> <span data-ttu-id="0083e-264">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-264">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-265">isSupervised</span><span class="sxs-lookup"><span data-stu-id="0083e-265">isSupervised</span></span>|<span data-ttu-id="0083e-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="0083e-266">Boolean</span></span>|<span data-ttu-id="0083e-267">Состояние устройства под контролем.</span><span class="sxs-lookup"><span data-stu-id="0083e-267">Device supervised status.</span></span> <span data-ttu-id="0083e-268">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-268">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-269">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0083e-269">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="0083e-270">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0083e-270">DateTimeOffset</span></span>|<span data-ttu-id="0083e-271">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="0083e-271">Last time the device contacted Exchange.</span></span> <span data-ttu-id="0083e-272">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-272">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-273">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="0083e-273">exchangeAccessState</span></span>|[<span data-ttu-id="0083e-274">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="0083e-274">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="0083e-275">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="0083e-275">The Access State of the device in Exchange.</span></span> <span data-ttu-id="0083e-276">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-276">This property is read-only.</span></span> <span data-ttu-id="0083e-277">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="0083e-277">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="0083e-278">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="0083e-278">exchangeAccessStateReason</span></span>|[<span data-ttu-id="0083e-279">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="0083e-279">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="0083e-280">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="0083e-280">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="0083e-281">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-281">This property is read-only.</span></span> <span data-ttu-id="0083e-282">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="0083e-282">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="0083e-283">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="0083e-283">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="0083e-284">String</span><span class="sxs-lookup"><span data-stu-id="0083e-284">String</span></span>|<span data-ttu-id="0083e-285">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="0083e-285">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="0083e-286">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-286">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-287">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="0083e-287">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="0083e-288">String</span><span class="sxs-lookup"><span data-stu-id="0083e-288">String</span></span>|<span data-ttu-id="0083e-289">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="0083e-289">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="0083e-290">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-290">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-291">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="0083e-291">isEncrypted</span></span>|<span data-ttu-id="0083e-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="0083e-292">Boolean</span></span>|<span data-ttu-id="0083e-293">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-293">Device encryption status.</span></span> <span data-ttu-id="0083e-294">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-294">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-295">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0083e-295">userPrincipalName</span></span>|<span data-ttu-id="0083e-296">String</span><span class="sxs-lookup"><span data-stu-id="0083e-296">String</span></span>|<span data-ttu-id="0083e-297">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-297">Device user principal name.</span></span> <span data-ttu-id="0083e-298">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-298">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-299">model</span><span class="sxs-lookup"><span data-stu-id="0083e-299">model</span></span>|<span data-ttu-id="0083e-300">String</span><span class="sxs-lookup"><span data-stu-id="0083e-300">String</span></span>|<span data-ttu-id="0083e-301">Модель устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-301">Model of the device.</span></span> <span data-ttu-id="0083e-302">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-302">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-303">manufacturer</span><span class="sxs-lookup"><span data-stu-id="0083e-303">manufacturer</span></span>|<span data-ttu-id="0083e-304">String</span><span class="sxs-lookup"><span data-stu-id="0083e-304">String</span></span>|<span data-ttu-id="0083e-305">Производитель устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-305">Manufacturer of the device.</span></span> <span data-ttu-id="0083e-306">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-306">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-307">imei</span><span class="sxs-lookup"><span data-stu-id="0083e-307">imei</span></span>|<span data-ttu-id="0083e-308">String</span><span class="sxs-lookup"><span data-stu-id="0083e-308">String</span></span>|<span data-ttu-id="0083e-309">IMEI.</span><span class="sxs-lookup"><span data-stu-id="0083e-309">IMEI.</span></span> <span data-ttu-id="0083e-310">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-310">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-311">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0083e-311">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="0083e-312">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0083e-312">DateTimeOffset</span></span>|<span data-ttu-id="0083e-313">Дата и время истечения льготного периода соответствия устройств требованиям.</span><span class="sxs-lookup"><span data-stu-id="0083e-313">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="0083e-314">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-314">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-315">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0083e-315">serialNumber</span></span>|<span data-ttu-id="0083e-316">String</span><span class="sxs-lookup"><span data-stu-id="0083e-316">String</span></span>|<span data-ttu-id="0083e-317">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="0083e-317">SerialNumber.</span></span> <span data-ttu-id="0083e-318">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-318">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-319">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="0083e-319">phoneNumber</span></span>|<span data-ttu-id="0083e-320">String</span><span class="sxs-lookup"><span data-stu-id="0083e-320">String</span></span>|<span data-ttu-id="0083e-321">Номер телефона устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-321">Phone number of the device.</span></span> <span data-ttu-id="0083e-322">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-322">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-323">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="0083e-323">androidSecurityPatchLevel</span></span>|<span data-ttu-id="0083e-324">String</span><span class="sxs-lookup"><span data-stu-id="0083e-324">String</span></span>|<span data-ttu-id="0083e-325">Уровень исправлений для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="0083e-325">Android security patch level.</span></span> <span data-ttu-id="0083e-326">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-326">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-327">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0083e-327">userDisplayName</span></span>|<span data-ttu-id="0083e-328">String</span><span class="sxs-lookup"><span data-stu-id="0083e-328">String</span></span>|<span data-ttu-id="0083e-329">Отображаемая имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="0083e-329">User display name.</span></span> <span data-ttu-id="0083e-330">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-330">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-331">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0083e-331">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="0083e-332">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0083e-332">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="0083e-333">Функции, включенные клиентом ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="0083e-333">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="0083e-334">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-334">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-335">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="0083e-335">wiFiMacAddress</span></span>|<span data-ttu-id="0083e-336">String</span><span class="sxs-lookup"><span data-stu-id="0083e-336">String</span></span>|<span data-ttu-id="0083e-337">Wi-Fi MAC.</span><span class="sxs-lookup"><span data-stu-id="0083e-337">Wi-Fi MAC.</span></span> <span data-ttu-id="0083e-338">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-338">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-339">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0083e-339">deviceHealthAttestationState</span></span>|[<span data-ttu-id="0083e-340">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0083e-340">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="0083e-341">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-341">The device health attestation state.</span></span> <span data-ttu-id="0083e-342">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-342">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-343">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="0083e-343">subscriberCarrier</span></span>|<span data-ttu-id="0083e-344">String</span><span class="sxs-lookup"><span data-stu-id="0083e-344">String</span></span>|<span data-ttu-id="0083e-345">Оператор подписчика.</span><span class="sxs-lookup"><span data-stu-id="0083e-345">Subscriber Carrier.</span></span> <span data-ttu-id="0083e-346">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-346">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-347">meid</span><span class="sxs-lookup"><span data-stu-id="0083e-347">meid</span></span>|<span data-ttu-id="0083e-348">String</span><span class="sxs-lookup"><span data-stu-id="0083e-348">String</span></span>|<span data-ttu-id="0083e-349">MEID.</span><span class="sxs-lookup"><span data-stu-id="0083e-349">MEID.</span></span> <span data-ttu-id="0083e-350">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-350">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-351">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="0083e-351">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="0083e-352">Int64</span><span class="sxs-lookup"><span data-stu-id="0083e-352">Int64</span></span>|<span data-ttu-id="0083e-353">Общее хранилище в bytes.</span><span class="sxs-lookup"><span data-stu-id="0083e-353">Total Storage in Bytes.</span></span> <span data-ttu-id="0083e-354">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-354">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-355">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="0083e-355">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="0083e-356">Int64</span><span class="sxs-lookup"><span data-stu-id="0083e-356">Int64</span></span>|<span data-ttu-id="0083e-357">Бесплатное хранилище в вайтах.</span><span class="sxs-lookup"><span data-stu-id="0083e-357">Free Storage in Bytes.</span></span> <span data-ttu-id="0083e-358">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-358">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-359">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="0083e-359">managedDeviceName</span></span>|<span data-ttu-id="0083e-360">String</span><span class="sxs-lookup"><span data-stu-id="0083e-360">String</span></span>|<span data-ttu-id="0083e-361">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-361">Automatically generated name to identify a device.</span></span> <span data-ttu-id="0083e-362">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="0083e-362">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="0083e-363">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="0083e-363">partnerReportedThreatState</span></span>|[<span data-ttu-id="0083e-364">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="0083e-364">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="0083e-365">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="0083e-365">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="0083e-366">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-366">Read Only.</span></span> <span data-ttu-id="0083e-367">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-367">This property is read-only.</span></span> <span data-ttu-id="0083e-368">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="0083e-368">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="0083e-369">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="0083e-369">retireAfterDateTime</span></span>|<span data-ttu-id="0083e-370">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0083e-370">DateTimeOffset</span></span>|<span data-ttu-id="0083e-371">Указывает время после автоматического выхода устройства из-за запланированного действия.</span><span class="sxs-lookup"><span data-stu-id="0083e-371">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="0083e-372">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-372">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-373">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="0083e-373">usersLoggedOn</span></span>|<span data-ttu-id="0083e-374">[коллекция loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="0083e-374">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="0083e-375">Указывает последних во время входа пользователей устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-375">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="0083e-376">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-376">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-377">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="0083e-377">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="0083e-378">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0083e-378">DateTimeOffset</span></span>|<span data-ttu-id="0083e-379">Сообщает dateTime, задав параметр preferMdmOverGroupPolicy.</span><span class="sxs-lookup"><span data-stu-id="0083e-379">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="0083e-380">Если этот параметр задан, параметры MDM Intune переопредят параметры групповой политики в случае конфликта.</span><span class="sxs-lookup"><span data-stu-id="0083e-380">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="0083e-381">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-381">Read Only.</span></span> <span data-ttu-id="0083e-382">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-382">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-383">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="0083e-383">autopilotEnrolled</span></span>|<span data-ttu-id="0083e-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="0083e-384">Boolean</span></span>|<span data-ttu-id="0083e-385">Сообщает, зарегистрировать ли управляемое устройство с помощью автоматического пилотного проекта.</span><span class="sxs-lookup"><span data-stu-id="0083e-385">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="0083e-386">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-386">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-387">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="0083e-387">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="0083e-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="0083e-388">Boolean</span></span>|<span data-ttu-id="0083e-389">Сообщает, является ли управляемое устройство iOS зарегистрированным пользователем.</span><span class="sxs-lookup"><span data-stu-id="0083e-389">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="0083e-390">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-390">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-391">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="0083e-391">managementCertificateExpirationDate</span></span>|<span data-ttu-id="0083e-392">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0083e-392">DateTimeOffset</span></span>|<span data-ttu-id="0083e-393">Сообщает дату окончания срока действия сертификата управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="0083e-393">Reports device management certificate expiration date.</span></span> <span data-ttu-id="0083e-394">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-394">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-395">iccid</span><span class="sxs-lookup"><span data-stu-id="0083e-395">iccid</span></span>|<span data-ttu-id="0083e-396">String</span><span class="sxs-lookup"><span data-stu-id="0083e-396">String</span></span>|<span data-ttu-id="0083e-397">Интегрированный идентификатор схемной карты — это уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="0083e-397">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="0083e-398">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-398">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-399">udid</span><span class="sxs-lookup"><span data-stu-id="0083e-399">udid</span></span>|<span data-ttu-id="0083e-400">String</span><span class="sxs-lookup"><span data-stu-id="0083e-400">String</span></span>|<span data-ttu-id="0083e-401">Уникальный идентификатор устройства для устройств с iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="0083e-401">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="0083e-402">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-402">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-403">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0083e-403">roleScopeTagIds</span></span>|<span data-ttu-id="0083e-404">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0083e-404">String collection</span></span>|<span data-ttu-id="0083e-405">Список ИД тегов области для этого экземпляра устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-405">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="0083e-406">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="0083e-406">windowsActiveMalwareCount</span></span>|<span data-ttu-id="0083e-407">Int32</span><span class="sxs-lookup"><span data-stu-id="0083e-407">Int32</span></span>|<span data-ttu-id="0083e-408">Количество активных вредоносных программ для этого устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="0083e-408">Count of active malware for this windows device.</span></span> <span data-ttu-id="0083e-409">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-409">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-410">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="0083e-410">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="0083e-411">Int32</span><span class="sxs-lookup"><span data-stu-id="0083e-411">Int32</span></span>|<span data-ttu-id="0083e-412">Количество исправленных вредоносных программ для этого устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="0083e-412">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="0083e-413">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-413">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-414">notes</span><span class="sxs-lookup"><span data-stu-id="0083e-414">notes</span></span>|<span data-ttu-id="0083e-415">String</span><span class="sxs-lookup"><span data-stu-id="0083e-415">String</span></span>|<span data-ttu-id="0083e-416">Заметки на устройстве, созданном ИТ-администратором</span><span class="sxs-lookup"><span data-stu-id="0083e-416">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="0083e-417">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="0083e-417">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="0083e-418">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="0083e-418">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="0083e-419">Состояние состояния клиента Configuration Manager, действительное только для устройств, управляемых агентом MDM/ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="0083e-419">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="0083e-420">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="0083e-420">configurationManagerClientInformation</span></span>|[<span data-ttu-id="0083e-421">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="0083e-421">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="0083e-422">Сведения о клиенте Configuration Manager, допустимые только для устройств, управляемых, управляемых duel или триуправленных агентом ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="0083e-422">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|
|<span data-ttu-id="0083e-423">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="0083e-423">ethernetMacAddress</span></span>|<span data-ttu-id="0083e-424">String</span><span class="sxs-lookup"><span data-stu-id="0083e-424">String</span></span>|<span data-ttu-id="0083e-425">Ethernet MAC.</span><span class="sxs-lookup"><span data-stu-id="0083e-425">Ethernet MAC.</span></span> <span data-ttu-id="0083e-426">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-426">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-427">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="0083e-427">physicalMemoryInBytes</span></span>|<span data-ttu-id="0083e-428">Int64</span><span class="sxs-lookup"><span data-stu-id="0083e-428">Int64</span></span>|<span data-ttu-id="0083e-429">Общий объем памяти в ветвях.</span><span class="sxs-lookup"><span data-stu-id="0083e-429">Total Memory in Bytes.</span></span> <span data-ttu-id="0083e-430">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-430">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-431">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="0083e-431">processorArchitecture</span></span>|[<span data-ttu-id="0083e-432">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="0083e-432">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="0083e-433">Архитектура процессора.</span><span class="sxs-lookup"><span data-stu-id="0083e-433">Processor architecture.</span></span> <span data-ttu-id="0083e-434">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-434">This property is read-only.</span></span> <span data-ttu-id="0083e-435">Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="0083e-435">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="0083e-436">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="0083e-436">specificationVersion</span></span>|<span data-ttu-id="0083e-437">String</span><span class="sxs-lookup"><span data-stu-id="0083e-437">String</span></span>|<span data-ttu-id="0083e-438">Версия спецификации.</span><span class="sxs-lookup"><span data-stu-id="0083e-438">Specification version.</span></span> <span data-ttu-id="0083e-439">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-439">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-440">joinType</span><span class="sxs-lookup"><span data-stu-id="0083e-440">joinType</span></span>|[<span data-ttu-id="0083e-441">joinType</span><span class="sxs-lookup"><span data-stu-id="0083e-441">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="0083e-442">Тип присоединяемого устройства.</span><span class="sxs-lookup"><span data-stu-id="0083e-442">Device join type.</span></span> <span data-ttu-id="0083e-443">Возможные значения: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span><span class="sxs-lookup"><span data-stu-id="0083e-443">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="0083e-444">skuFamily</span><span class="sxs-lookup"><span data-stu-id="0083e-444">skuFamily</span></span>|<span data-ttu-id="0083e-445">String</span><span class="sxs-lookup"><span data-stu-id="0083e-445">String</span></span>|<span data-ttu-id="0083e-446">Семейство SKU устройств</span><span class="sxs-lookup"><span data-stu-id="0083e-446">Device sku family</span></span>|
|<span data-ttu-id="0083e-447">skuNumber</span><span class="sxs-lookup"><span data-stu-id="0083e-447">skuNumber</span></span>|<span data-ttu-id="0083e-448">Int32</span><span class="sxs-lookup"><span data-stu-id="0083e-448">Int32</span></span>|<span data-ttu-id="0083e-449">Номер SKU устройства, см. также: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo .</span><span class="sxs-lookup"><span data-stu-id="0083e-449">Device sku number, see also: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo.</span></span> <span data-ttu-id="0083e-450">Допустимые значения: от 0 до 2 147 483 647.</span><span class="sxs-lookup"><span data-stu-id="0083e-450">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="0083e-451">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0083e-451">This property is read-only.</span></span>|
|<span data-ttu-id="0083e-452">managementFeatures</span><span class="sxs-lookup"><span data-stu-id="0083e-452">managementFeatures</span></span>|[<span data-ttu-id="0083e-453">managedDeviceManagementFeatures</span><span class="sxs-lookup"><span data-stu-id="0083e-453">managedDeviceManagementFeatures</span></span>](../resources/intune-devices-manageddevicemanagementfeatures.md)|<span data-ttu-id="0083e-454">Функции управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="0083e-454">Device management features.</span></span> <span data-ttu-id="0083e-455">Возможные значения: `none`, `microsoftManagedDesktop`.</span><span class="sxs-lookup"><span data-stu-id="0083e-455">Possible values are: `none`, `microsoftManagedDesktop`.</span></span>|



## <a name="response"></a><span data-ttu-id="0083e-456">Отклик</span><span class="sxs-lookup"><span data-stu-id="0083e-456">Response</span></span>
<span data-ttu-id="0083e-457">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDevice](../resources/intune-shared-manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0083e-457">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-shared-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0083e-458">Пример</span><span class="sxs-lookup"><span data-stu-id="0083e-458">Example</span></span>

### <a name="request"></a><span data-ttu-id="0083e-459">Запрос</span><span class="sxs-lookup"><span data-stu-id="0083e-459">Request</span></span>
<span data-ttu-id="0083e-460">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0083e-460">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 8108

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
    "batterySerialNumber": "Battery Serial Number value",
    "batteryHealthPercentage": 7,
    "batteryChargeCycles": 3,
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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
    "osBuildNumber": "Os Build Number value",
    "operatingSystemProductType": 10,
    "ipAddressV4": "Ip Address V4 value",
    "subnetAddress": "Subnet Address value"
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
  "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
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
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "Client Identifier value",
    "isBlocked": true
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86",
  "specificationVersion": "Specification Version value",
  "joinType": "azureADJoined",
  "skuFamily": "Sku Family value",
  "skuNumber": 9,
  "managementFeatures": "microsoftManagedDesktop"
}
```

### <a name="response"></a><span data-ttu-id="0083e-461">Отклик</span><span class="sxs-lookup"><span data-stu-id="0083e-461">Response</span></span>
<span data-ttu-id="0083e-p174">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0083e-p174">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8157

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
    "batterySerialNumber": "Battery Serial Number value",
    "batteryHealthPercentage": 7,
    "batteryChargeCycles": 3,
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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
    "osBuildNumber": "Os Build Number value",
    "operatingSystemProductType": 10,
    "ipAddressV4": "Ip Address V4 value",
    "subnetAddress": "Subnet Address value"
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
  "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
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
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "Client Identifier value",
    "isBlocked": true
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86",
  "specificationVersion": "Specification Version value",
  "joinType": "azureADJoined",
  "skuFamily": "Sku Family value",
  "skuNumber": 9,
  "managementFeatures": "microsoftManagedDesktop"
}
```




