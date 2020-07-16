---
title: Обновление managedDevice
description: Обновление свойств объекта managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 36c81bfb08c6656c3c5d314a60f8b0cf56e2ab46
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792158"
---
# <a name="update-manageddevice"></a><span data-ttu-id="57dac-103">Обновление managedDevice</span><span class="sxs-lookup"><span data-stu-id="57dac-103">Update managedDevice</span></span>

<span data-ttu-id="57dac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57dac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57dac-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57dac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57dac-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57dac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57dac-107">Обновление свойств объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="57dac-107">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57dac-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="57dac-108">Prerequisites</span></span>
<span data-ttu-id="57dac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57dac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57dac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57dac-111">Permission type</span></span>|<span data-ttu-id="57dac-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="57dac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57dac-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57dac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57dac-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57dac-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="57dac-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57dac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57dac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57dac-116">Not supported.</span></span>|
|<span data-ttu-id="57dac-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57dac-117">Application</span></span>|<span data-ttu-id="57dac-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57dac-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57dac-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57dac-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="57dac-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="57dac-120">Request headers</span></span>
|<span data-ttu-id="57dac-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57dac-121">Header</span></span>|<span data-ttu-id="57dac-122">Значение</span><span class="sxs-lookup"><span data-stu-id="57dac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57dac-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57dac-123">Authorization</span></span>|<span data-ttu-id="57dac-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57dac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57dac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="57dac-125">Accept</span></span>|<span data-ttu-id="57dac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57dac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57dac-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="57dac-127">Request body</span></span>
<span data-ttu-id="57dac-128">В теле запроса добавьте представление объекта [managedDevice](../resources/intune-devices-manageddevice.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57dac-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="57dac-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="57dac-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="57dac-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="57dac-130">Property</span></span>|<span data-ttu-id="57dac-131">Тип</span><span class="sxs-lookup"><span data-stu-id="57dac-131">Type</span></span>|<span data-ttu-id="57dac-132">Описание</span><span class="sxs-lookup"><span data-stu-id="57dac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57dac-133">id</span><span class="sxs-lookup"><span data-stu-id="57dac-133">id</span></span>|<span data-ttu-id="57dac-134">Строка</span><span class="sxs-lookup"><span data-stu-id="57dac-134">String</span></span>|<span data-ttu-id="57dac-135">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-135">Unique Identifier for the device.</span></span> <span data-ttu-id="57dac-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-136">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-137">userId</span><span class="sxs-lookup"><span data-stu-id="57dac-137">userId</span></span>|<span data-ttu-id="57dac-138">String</span><span class="sxs-lookup"><span data-stu-id="57dac-138">String</span></span>|<span data-ttu-id="57dac-139">Уникальный идентификатор пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="57dac-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="57dac-140">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-140">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="57dac-141">deviceName</span></span>|<span data-ttu-id="57dac-142">String</span><span class="sxs-lookup"><span data-stu-id="57dac-142">String</span></span>|<span data-ttu-id="57dac-143">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-143">Name of the device.</span></span> <span data-ttu-id="57dac-144">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-144">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-145">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="57dac-145">hardwareInformation</span></span>|[<span data-ttu-id="57dac-146">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="57dac-146">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="57dac-147">Сведения о хардвард для устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-147">The hardward details for the device.</span></span>  <span data-ttu-id="57dac-148">Включает такие сведения, как место хранения, производитель, серийный номер и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-148">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span>|
|<span data-ttu-id="57dac-149">ownerType</span><span class="sxs-lookup"><span data-stu-id="57dac-149">ownerType</span></span>|[<span data-ttu-id="57dac-150">ownerType</span><span class="sxs-lookup"><span data-stu-id="57dac-150">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="57dac-151">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="57dac-151">Ownership of the device.</span></span> <span data-ttu-id="57dac-152">Может быть "Company" или "Personal".</span><span class="sxs-lookup"><span data-stu-id="57dac-152">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="57dac-153">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="57dac-153">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="57dac-154">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="57dac-154">managedDeviceOwnerType</span></span>|[<span data-ttu-id="57dac-155">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="57dac-155">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="57dac-156">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="57dac-156">Ownership of the device.</span></span> <span data-ttu-id="57dac-157">Может быть "Company" или "Personal".</span><span class="sxs-lookup"><span data-stu-id="57dac-157">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="57dac-158">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="57dac-158">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="57dac-159">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="57dac-159">deviceActionResults</span></span>|<span data-ttu-id="57dac-160">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="57dac-160">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="57dac-161">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="57dac-161">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="57dac-162">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-162">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-163">манажементстате</span><span class="sxs-lookup"><span data-stu-id="57dac-163">managementState</span></span>|[<span data-ttu-id="57dac-164">манажементстате</span><span class="sxs-lookup"><span data-stu-id="57dac-164">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="57dac-165">Состояние управления для устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-165">Management state of the device.</span></span> <span data-ttu-id="57dac-166">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-166">This property is read-only.</span></span> <span data-ttu-id="57dac-167">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="57dac-167">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="57dac-168">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="57dac-168">enrolledDateTime</span></span>|<span data-ttu-id="57dac-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57dac-169">DateTimeOffset</span></span>|<span data-ttu-id="57dac-170">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-170">Enrollment time of the device.</span></span> <span data-ttu-id="57dac-171">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-171">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-172">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="57dac-172">lastSyncDateTime</span></span>|<span data-ttu-id="57dac-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57dac-173">DateTimeOffset</span></span>|<span data-ttu-id="57dac-174">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="57dac-174">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="57dac-175">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-175">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-176">чассистипе</span><span class="sxs-lookup"><span data-stu-id="57dac-176">chassisType</span></span>|[<span data-ttu-id="57dac-177">чассистипе</span><span class="sxs-lookup"><span data-stu-id="57dac-177">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="57dac-178">Тип корпуса устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-178">Chassis type of the device.</span></span> <span data-ttu-id="57dac-179">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-179">This property is read-only.</span></span> <span data-ttu-id="57dac-180">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="57dac-180">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="57dac-181">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="57dac-181">operatingSystem</span></span>|<span data-ttu-id="57dac-182">String</span><span class="sxs-lookup"><span data-stu-id="57dac-182">String</span></span>|<span data-ttu-id="57dac-183">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-183">Operating system of the device.</span></span> <span data-ttu-id="57dac-184">Windows, iOS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-184">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="57dac-185">deviceType</span><span class="sxs-lookup"><span data-stu-id="57dac-185">deviceType</span></span>|[<span data-ttu-id="57dac-186">deviceType</span><span class="sxs-lookup"><span data-stu-id="57dac-186">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="57dac-187">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-187">Platform of the device.</span></span> <span data-ttu-id="57dac-188">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-188">This property is read-only.</span></span> <span data-ttu-id="57dac-189">Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` , `macMDM` , `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `blackberry` `palm` `unknown` ,,,,,,,,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="57dac-189">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="57dac-190">complianceState</span><span class="sxs-lookup"><span data-stu-id="57dac-190">complianceState</span></span>|[<span data-ttu-id="57dac-191">complianceState</span><span class="sxs-lookup"><span data-stu-id="57dac-191">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="57dac-192">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="57dac-192">Compliance state of the device.</span></span> <span data-ttu-id="57dac-193">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-193">This property is read-only.</span></span> <span data-ttu-id="57dac-194">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="57dac-194">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="57dac-195">jailBroken</span><span class="sxs-lookup"><span data-stu-id="57dac-195">jailBroken</span></span>|<span data-ttu-id="57dac-196">String</span><span class="sxs-lookup"><span data-stu-id="57dac-196">String</span></span>|<span data-ttu-id="57dac-197">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="57dac-197">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="57dac-198">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-198">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-199">managementAgent</span><span class="sxs-lookup"><span data-stu-id="57dac-199">managementAgent</span></span>|[<span data-ttu-id="57dac-200">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="57dac-200">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="57dac-201">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="57dac-201">Management channel of the device.</span></span> <span data-ttu-id="57dac-202">Intune, EAS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-202">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="57dac-203">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="57dac-203">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="57dac-204">osVersion</span><span class="sxs-lookup"><span data-stu-id="57dac-204">osVersion</span></span>|<span data-ttu-id="57dac-205">String</span><span class="sxs-lookup"><span data-stu-id="57dac-205">String</span></span>|<span data-ttu-id="57dac-206">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-206">Operating system version of the device.</span></span> <span data-ttu-id="57dac-207">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-207">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-208">easActivated</span><span class="sxs-lookup"><span data-stu-id="57dac-208">easActivated</span></span>|<span data-ttu-id="57dac-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="57dac-209">Boolean</span></span>|<span data-ttu-id="57dac-210">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="57dac-210">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="57dac-211">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-211">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-212">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="57dac-212">easDeviceId</span></span>|<span data-ttu-id="57dac-213">String</span><span class="sxs-lookup"><span data-stu-id="57dac-213">String</span></span>|<span data-ttu-id="57dac-214">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="57dac-214">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="57dac-215">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-215">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-216">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="57dac-216">easActivationDateTime</span></span>|<span data-ttu-id="57dac-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57dac-217">DateTimeOffset</span></span>|<span data-ttu-id="57dac-218">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="57dac-218">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="57dac-219">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-219">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-220">аадрегистеред</span><span class="sxs-lookup"><span data-stu-id="57dac-220">aadRegistered</span></span>|<span data-ttu-id="57dac-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="57dac-221">Boolean</span></span>|<span data-ttu-id="57dac-222">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="57dac-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="57dac-223">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-223">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-224">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="57dac-224">azureADRegistered</span></span>|<span data-ttu-id="57dac-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="57dac-225">Boolean</span></span>|<span data-ttu-id="57dac-226">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="57dac-226">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="57dac-227">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-227">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-228">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="57dac-228">deviceEnrollmentType</span></span>|[<span data-ttu-id="57dac-229">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="57dac-229">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="57dac-230">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-230">Enrollment type of the device.</span></span> <span data-ttu-id="57dac-231">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-231">This property is read-only.</span></span> <span data-ttu-id="57dac-232">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="57dac-232">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="57dac-233">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="57dac-233">lostModeState</span></span>|[<span data-ttu-id="57dac-234">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="57dac-234">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="57dac-235">Указывает, включен ли режим потерянных или отключенных.</span><span class="sxs-lookup"><span data-stu-id="57dac-235">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="57dac-236">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-236">This property is read-only.</span></span> <span data-ttu-id="57dac-237">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="57dac-237">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="57dac-238">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="57dac-238">activationLockBypassCode</span></span>|<span data-ttu-id="57dac-239">String</span><span class="sxs-lookup"><span data-stu-id="57dac-239">String</span></span>|<span data-ttu-id="57dac-240">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="57dac-240">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="57dac-241">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-241">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-242">emailAddress</span><span class="sxs-lookup"><span data-stu-id="57dac-242">emailAddress</span></span>|<span data-ttu-id="57dac-243">String</span><span class="sxs-lookup"><span data-stu-id="57dac-243">String</span></span>|<span data-ttu-id="57dac-244">Сообщения электронной почты пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="57dac-244">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="57dac-245">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-245">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-246">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="57dac-246">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="57dac-247">String</span><span class="sxs-lookup"><span data-stu-id="57dac-247">String</span></span>|<span data-ttu-id="57dac-248">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="57dac-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="57dac-249">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-249">Read only.</span></span> <span data-ttu-id="57dac-250">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-250">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-251">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="57dac-251">azureADDeviceId</span></span>|<span data-ttu-id="57dac-252">String</span><span class="sxs-lookup"><span data-stu-id="57dac-252">String</span></span>|<span data-ttu-id="57dac-253">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="57dac-253">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="57dac-254">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-254">Read only.</span></span> <span data-ttu-id="57dac-255">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-255">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-256">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="57dac-256">deviceRegistrationState</span></span>|[<span data-ttu-id="57dac-257">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="57dac-257">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="57dac-258">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-258">Device registration state.</span></span> <span data-ttu-id="57dac-259">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-259">This property is read-only.</span></span> <span data-ttu-id="57dac-260">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="57dac-260">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="57dac-261">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="57dac-261">deviceCategoryDisplayName</span></span>|<span data-ttu-id="57dac-262">String</span><span class="sxs-lookup"><span data-stu-id="57dac-262">String</span></span>|<span data-ttu-id="57dac-263">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="57dac-263">Device category display name.</span></span> <span data-ttu-id="57dac-264">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-264">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-265">isSupervised</span><span class="sxs-lookup"><span data-stu-id="57dac-265">isSupervised</span></span>|<span data-ttu-id="57dac-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="57dac-266">Boolean</span></span>|<span data-ttu-id="57dac-267">Состояние контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-267">Device supervised status.</span></span> <span data-ttu-id="57dac-268">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-268">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-269">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="57dac-269">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="57dac-270">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57dac-270">DateTimeOffset</span></span>|<span data-ttu-id="57dac-271">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="57dac-271">Last time the device contacted Exchange.</span></span> <span data-ttu-id="57dac-272">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-272">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-273">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="57dac-273">exchangeAccessState</span></span>|[<span data-ttu-id="57dac-274">девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="57dac-274">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="57dac-275">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="57dac-275">The Access State of the device in Exchange.</span></span> <span data-ttu-id="57dac-276">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-276">This property is read-only.</span></span> <span data-ttu-id="57dac-277">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="57dac-277">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="57dac-278">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="57dac-278">exchangeAccessStateReason</span></span>|[<span data-ttu-id="57dac-279">девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="57dac-279">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="57dac-280">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="57dac-280">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="57dac-281">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-281">This property is read-only.</span></span> <span data-ttu-id="57dac-282">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="57dac-282">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="57dac-283">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="57dac-283">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="57dac-284">String</span><span class="sxs-lookup"><span data-stu-id="57dac-284">String</span></span>|<span data-ttu-id="57dac-285">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="57dac-285">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="57dac-286">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-286">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-287">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="57dac-287">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="57dac-288">String</span><span class="sxs-lookup"><span data-stu-id="57dac-288">String</span></span>|<span data-ttu-id="57dac-289">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="57dac-289">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="57dac-290">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-290">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-291">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="57dac-291">isEncrypted</span></span>|<span data-ttu-id="57dac-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="57dac-292">Boolean</span></span>|<span data-ttu-id="57dac-293">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-293">Device encryption status.</span></span> <span data-ttu-id="57dac-294">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-294">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-295">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="57dac-295">userPrincipalName</span></span>|<span data-ttu-id="57dac-296">String</span><span class="sxs-lookup"><span data-stu-id="57dac-296">String</span></span>|<span data-ttu-id="57dac-297">Имя участника пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-297">Device user principal name.</span></span> <span data-ttu-id="57dac-298">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-298">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-299">model</span><span class="sxs-lookup"><span data-stu-id="57dac-299">model</span></span>|<span data-ttu-id="57dac-300">String</span><span class="sxs-lookup"><span data-stu-id="57dac-300">String</span></span>|<span data-ttu-id="57dac-301">Модель устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-301">Model of the device.</span></span> <span data-ttu-id="57dac-302">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-302">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-303">manufacturer</span><span class="sxs-lookup"><span data-stu-id="57dac-303">manufacturer</span></span>|<span data-ttu-id="57dac-304">String</span><span class="sxs-lookup"><span data-stu-id="57dac-304">String</span></span>|<span data-ttu-id="57dac-305">Производитель устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-305">Manufacturer of the device.</span></span> <span data-ttu-id="57dac-306">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-306">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-307">imei</span><span class="sxs-lookup"><span data-stu-id="57dac-307">imei</span></span>|<span data-ttu-id="57dac-308">String</span><span class="sxs-lookup"><span data-stu-id="57dac-308">String</span></span>|<span data-ttu-id="57dac-309">IMEI.</span><span class="sxs-lookup"><span data-stu-id="57dac-309">IMEI.</span></span> <span data-ttu-id="57dac-310">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-310">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-311">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="57dac-311">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="57dac-312">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57dac-312">DateTimeOffset</span></span>|<span data-ttu-id="57dac-313">Дата и время истечения льготного периода соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="57dac-313">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="57dac-314">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-314">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-315">serialNumber</span><span class="sxs-lookup"><span data-stu-id="57dac-315">serialNumber</span></span>|<span data-ttu-id="57dac-316">Строка</span><span class="sxs-lookup"><span data-stu-id="57dac-316">String</span></span>|<span data-ttu-id="57dac-317">Серийный.</span><span class="sxs-lookup"><span data-stu-id="57dac-317">SerialNumber.</span></span> <span data-ttu-id="57dac-318">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-318">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-319">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="57dac-319">phoneNumber</span></span>|<span data-ttu-id="57dac-320">String</span><span class="sxs-lookup"><span data-stu-id="57dac-320">String</span></span>|<span data-ttu-id="57dac-321">Номер телефона устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-321">Phone number of the device.</span></span> <span data-ttu-id="57dac-322">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-322">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-323">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="57dac-323">androidSecurityPatchLevel</span></span>|<span data-ttu-id="57dac-324">String</span><span class="sxs-lookup"><span data-stu-id="57dac-324">String</span></span>|<span data-ttu-id="57dac-325">Уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="57dac-325">Android security patch level.</span></span> <span data-ttu-id="57dac-326">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-326">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-327">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="57dac-327">userDisplayName</span></span>|<span data-ttu-id="57dac-328">String</span><span class="sxs-lookup"><span data-stu-id="57dac-328">String</span></span>|<span data-ttu-id="57dac-329">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="57dac-329">User display name.</span></span> <span data-ttu-id="57dac-330">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-330">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-331">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="57dac-331">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="57dac-332">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="57dac-332">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="57dac-333">Функции, поддерживающие клиент Конфигрмгр.</span><span class="sxs-lookup"><span data-stu-id="57dac-333">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="57dac-334">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-334">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-335">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="57dac-335">wiFiMacAddress</span></span>|<span data-ttu-id="57dac-336">String</span><span class="sxs-lookup"><span data-stu-id="57dac-336">String</span></span>|<span data-ttu-id="57dac-337">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="57dac-337">Wi-Fi MAC.</span></span> <span data-ttu-id="57dac-338">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-338">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-339">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="57dac-339">deviceHealthAttestationState</span></span>|[<span data-ttu-id="57dac-340">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="57dac-340">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="57dac-341">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-341">The device health attestation state.</span></span> <span data-ttu-id="57dac-342">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-342">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-343">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="57dac-343">subscriberCarrier</span></span>|<span data-ttu-id="57dac-344">String</span><span class="sxs-lookup"><span data-stu-id="57dac-344">String</span></span>|<span data-ttu-id="57dac-345">Перевозчик абонента.</span><span class="sxs-lookup"><span data-stu-id="57dac-345">Subscriber Carrier.</span></span> <span data-ttu-id="57dac-346">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-346">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-347">meid</span><span class="sxs-lookup"><span data-stu-id="57dac-347">meid</span></span>|<span data-ttu-id="57dac-348">String</span><span class="sxs-lookup"><span data-stu-id="57dac-348">String</span></span>|<span data-ttu-id="57dac-349">MEID.</span><span class="sxs-lookup"><span data-stu-id="57dac-349">MEID.</span></span> <span data-ttu-id="57dac-350">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-350">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-351">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="57dac-351">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="57dac-352">Int64</span><span class="sxs-lookup"><span data-stu-id="57dac-352">Int64</span></span>|<span data-ttu-id="57dac-353">Общий объем хранилища в байтах.</span><span class="sxs-lookup"><span data-stu-id="57dac-353">Total Storage in Bytes.</span></span> <span data-ttu-id="57dac-354">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-354">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-355">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="57dac-355">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="57dac-356">Int64</span><span class="sxs-lookup"><span data-stu-id="57dac-356">Int64</span></span>|<span data-ttu-id="57dac-357">Свободное хранилище в байтах.</span><span class="sxs-lookup"><span data-stu-id="57dac-357">Free Storage in Bytes.</span></span> <span data-ttu-id="57dac-358">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-358">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-359">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="57dac-359">managedDeviceName</span></span>|<span data-ttu-id="57dac-360">String</span><span class="sxs-lookup"><span data-stu-id="57dac-360">String</span></span>|<span data-ttu-id="57dac-361">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-361">Automatically generated name to identify a device.</span></span> <span data-ttu-id="57dac-362">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="57dac-362">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="57dac-363">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="57dac-363">partnerReportedThreatState</span></span>|[<span data-ttu-id="57dac-364">манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="57dac-364">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="57dac-365">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="57dac-365">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="57dac-366">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-366">Read Only.</span></span> <span data-ttu-id="57dac-367">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-367">This property is read-only.</span></span> <span data-ttu-id="57dac-368">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="57dac-368">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="57dac-369">ретиреафтердатетиме</span><span class="sxs-lookup"><span data-stu-id="57dac-369">retireAfterDateTime</span></span>|<span data-ttu-id="57dac-370">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57dac-370">DateTimeOffset</span></span>|<span data-ttu-id="57dac-371">Указывает время, по истечении которого устройство будет автоматически снято из-за запланированного действия.</span><span class="sxs-lookup"><span data-stu-id="57dac-371">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="57dac-372">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-372">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-373">усерслогжедон</span><span class="sxs-lookup"><span data-stu-id="57dac-373">usersLoggedOn</span></span>|<span data-ttu-id="57dac-374">Коллекция [логжедонусер](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="57dac-374">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="57dac-375">Указывает последнего вошедшего в систему пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-375">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="57dac-376">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-376">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-377">префермдмоверграупполициапплиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="57dac-377">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="57dac-378">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57dac-378">DateTimeOffset</span></span>|<span data-ttu-id="57dac-379">Сообщает о значении DateTime, заданном параметром Префермдмоверграупполици.</span><span class="sxs-lookup"><span data-stu-id="57dac-379">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="57dac-380">Если этот параметр установлен, параметры групповой политики в случае конфликта будут переопределяться параметрами групповой политики.</span><span class="sxs-lookup"><span data-stu-id="57dac-380">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="57dac-381">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-381">Read Only.</span></span> <span data-ttu-id="57dac-382">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-382">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-383">аутопилотенроллед</span><span class="sxs-lookup"><span data-stu-id="57dac-383">autopilotEnrolled</span></span>|<span data-ttu-id="57dac-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="57dac-384">Boolean</span></span>|<span data-ttu-id="57dac-385">Сообщает, зарегистрировано ли управляемое устройство через Автоматический пилот.</span><span class="sxs-lookup"><span data-stu-id="57dac-385">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="57dac-386">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-386">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-387">рекуиреусеренроллментаппровал</span><span class="sxs-lookup"><span data-stu-id="57dac-387">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="57dac-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="57dac-388">Boolean</span></span>|<span data-ttu-id="57dac-389">Указывает, является ли управляемое устройство iOS регистрацией на утверждение пользователя.</span><span class="sxs-lookup"><span data-stu-id="57dac-389">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="57dac-390">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-390">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-391">манажементцертификатикспиратиондате</span><span class="sxs-lookup"><span data-stu-id="57dac-391">managementCertificateExpirationDate</span></span>|<span data-ttu-id="57dac-392">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57dac-392">DateTimeOffset</span></span>|<span data-ttu-id="57dac-393">Дата окончания срока действия сертификата управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="57dac-393">Reports device management certificate expiration date.</span></span> <span data-ttu-id="57dac-394">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-394">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-395">икЦид</span><span class="sxs-lookup"><span data-stu-id="57dac-395">iccid</span></span>|<span data-ttu-id="57dac-396">String</span><span class="sxs-lookup"><span data-stu-id="57dac-396">String</span></span>|<span data-ttu-id="57dac-397">Идентификатор встроенной карты — это уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="57dac-397">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="57dac-398">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-398">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-399">удид</span><span class="sxs-lookup"><span data-stu-id="57dac-399">udid</span></span>|<span data-ttu-id="57dac-400">String</span><span class="sxs-lookup"><span data-stu-id="57dac-400">String</span></span>|<span data-ttu-id="57dac-401">Уникальный идентификатор устройства для устройств iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="57dac-401">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="57dac-402">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-402">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-403">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="57dac-403">roleScopeTagIds</span></span>|<span data-ttu-id="57dac-404">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="57dac-404">String collection</span></span>|<span data-ttu-id="57dac-405">Список идентификаторов тегов области для этого экземпляра устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-405">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="57dac-406">виндовсактивемалварекаунт</span><span class="sxs-lookup"><span data-stu-id="57dac-406">windowsActiveMalwareCount</span></span>|<span data-ttu-id="57dac-407">Int32</span><span class="sxs-lookup"><span data-stu-id="57dac-407">Int32</span></span>|<span data-ttu-id="57dac-408">Количество активных вредоносных программ для этого устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="57dac-408">Count of active malware for this windows device.</span></span> <span data-ttu-id="57dac-409">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-409">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-410">виндовсремедиатедмалварекаунт</span><span class="sxs-lookup"><span data-stu-id="57dac-410">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="57dac-411">Int32</span><span class="sxs-lookup"><span data-stu-id="57dac-411">Int32</span></span>|<span data-ttu-id="57dac-412">Количество исправленных вредоносных программ для этого устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="57dac-412">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="57dac-413">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-413">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-414">notes</span><span class="sxs-lookup"><span data-stu-id="57dac-414">notes</span></span>|<span data-ttu-id="57dac-415">String</span><span class="sxs-lookup"><span data-stu-id="57dac-415">String</span></span>|<span data-ttu-id="57dac-416">Примечания к устройству, созданному ИТ ИТ Admin</span><span class="sxs-lookup"><span data-stu-id="57dac-416">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="57dac-417">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="57dac-417">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="57dac-418">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="57dac-418">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="57dac-419">Состояние работоспособности клиента Configuration Manager, действительно только для устройств под управлением агентов MDM/ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="57dac-419">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="57dac-420">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="57dac-420">configurationManagerClientInformation</span></span>|[<span data-ttu-id="57dac-421">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="57dac-421">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="57dac-422">Сведения о клиенте Configuration Manager, действительные только для управляемых устройств, управляемых дуел или управляемых с помощью агентов ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="57dac-422">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|
|<span data-ttu-id="57dac-423">есернетмакаддресс</span><span class="sxs-lookup"><span data-stu-id="57dac-423">ethernetMacAddress</span></span>|<span data-ttu-id="57dac-424">String</span><span class="sxs-lookup"><span data-stu-id="57dac-424">String</span></span>|<span data-ttu-id="57dac-425">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="57dac-425">Ethernet MAC.</span></span> <span data-ttu-id="57dac-426">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-426">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-427">фисикалмеморинбитес</span><span class="sxs-lookup"><span data-stu-id="57dac-427">physicalMemoryInBytes</span></span>|<span data-ttu-id="57dac-428">Int64</span><span class="sxs-lookup"><span data-stu-id="57dac-428">Int64</span></span>|<span data-ttu-id="57dac-429">Общий объем памяти в байтах.</span><span class="sxs-lookup"><span data-stu-id="57dac-429">Total Memory in Bytes.</span></span> <span data-ttu-id="57dac-430">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-430">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-431">процессорарчитектуре</span><span class="sxs-lookup"><span data-stu-id="57dac-431">processorArchitecture</span></span>|[<span data-ttu-id="57dac-432">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="57dac-432">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="57dac-433">Архитектура процессора.</span><span class="sxs-lookup"><span data-stu-id="57dac-433">Processor architecture.</span></span> <span data-ttu-id="57dac-434">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-434">This property is read-only.</span></span> <span data-ttu-id="57dac-435">Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="57dac-435">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="57dac-436">спеЦификатионверсион</span><span class="sxs-lookup"><span data-stu-id="57dac-436">specificationVersion</span></span>|<span data-ttu-id="57dac-437">String</span><span class="sxs-lookup"><span data-stu-id="57dac-437">String</span></span>|<span data-ttu-id="57dac-438">Версия спецификации.</span><span class="sxs-lookup"><span data-stu-id="57dac-438">Specification version.</span></span> <span data-ttu-id="57dac-439">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57dac-439">This property is read-only.</span></span>|
|<span data-ttu-id="57dac-440">joinType</span><span class="sxs-lookup"><span data-stu-id="57dac-440">joinType</span></span>|[<span data-ttu-id="57dac-441">joinType</span><span class="sxs-lookup"><span data-stu-id="57dac-441">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="57dac-442">Тип присоединения устройства.</span><span class="sxs-lookup"><span data-stu-id="57dac-442">Device join type.</span></span> <span data-ttu-id="57dac-443">Возможные значения: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span><span class="sxs-lookup"><span data-stu-id="57dac-443">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="57dac-444">скуфамили</span><span class="sxs-lookup"><span data-stu-id="57dac-444">skuFamily</span></span>|<span data-ttu-id="57dac-445">String</span><span class="sxs-lookup"><span data-stu-id="57dac-445">String</span></span>|<span data-ttu-id="57dac-446">Семейство SKU устройств</span><span class="sxs-lookup"><span data-stu-id="57dac-446">Device sku family</span></span>|



## <a name="response"></a><span data-ttu-id="57dac-447">Отклик</span><span class="sxs-lookup"><span data-stu-id="57dac-447">Response</span></span>
<span data-ttu-id="57dac-448">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDevice](../resources/intune-devices-manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="57dac-448">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57dac-449">Пример</span><span class="sxs-lookup"><span data-stu-id="57dac-449">Example</span></span>

### <a name="request"></a><span data-ttu-id="57dac-450">Запрос</span><span class="sxs-lookup"><span data-stu-id="57dac-450">Request</span></span>
<span data-ttu-id="57dac-451">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57dac-451">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7823

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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
    "osBuildNumber": "Os Build Number value",
    "operatingSystemProductType": 10
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
  "skuFamily": "Sku Family value"
}
```

### <a name="response"></a><span data-ttu-id="57dac-452">Отклик</span><span class="sxs-lookup"><span data-stu-id="57dac-452">Response</span></span>
<span data-ttu-id="57dac-p172">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57dac-p172">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7872

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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
    "osBuildNumber": "Os Build Number value",
    "operatingSystemProductType": 10
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
  "skuFamily": "Sku Family value"
}
```



