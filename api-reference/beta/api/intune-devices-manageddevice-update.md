---
title: Обновление managedDevice
description: Обновление свойств объекта managedDevice.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eae50fb896661312a5489c4a842c84a850773944
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468735"
---
# <a name="update-manageddevice"></a><span data-ttu-id="3d953-103">Обновление managedDevice</span><span class="sxs-lookup"><span data-stu-id="3d953-103">Update managedDevice</span></span>

<span data-ttu-id="3d953-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3d953-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d953-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d953-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d953-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d953-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d953-107">Обновление свойств объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3d953-107">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d953-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3d953-108">Prerequisites</span></span>
<span data-ttu-id="3d953-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d953-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d953-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d953-111">Permission type</span></span>|<span data-ttu-id="3d953-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d953-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d953-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d953-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d953-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d953-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3d953-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d953-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d953-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d953-116">Not supported.</span></span>|
|<span data-ttu-id="3d953-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d953-117">Application</span></span>|<span data-ttu-id="3d953-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d953-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d953-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d953-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="3d953-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3d953-120">Request headers</span></span>
|<span data-ttu-id="3d953-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3d953-121">Header</span></span>|<span data-ttu-id="3d953-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3d953-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d953-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d953-123">Authorization</span></span>|<span data-ttu-id="3d953-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d953-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d953-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d953-125">Accept</span></span>|<span data-ttu-id="3d953-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d953-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d953-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d953-127">Request body</span></span>
<span data-ttu-id="3d953-128">В теле запроса добавьте представление объекта [managedDevice](../resources/intune-devices-manageddevice.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d953-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="3d953-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3d953-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="3d953-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d953-130">Property</span></span>|<span data-ttu-id="3d953-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3d953-131">Type</span></span>|<span data-ttu-id="3d953-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3d953-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d953-133">id</span><span class="sxs-lookup"><span data-stu-id="3d953-133">id</span></span>|<span data-ttu-id="3d953-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3d953-134">String</span></span>|<span data-ttu-id="3d953-135">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-135">Unique Identifier for the device.</span></span> <span data-ttu-id="3d953-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-136">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-137">userId</span><span class="sxs-lookup"><span data-stu-id="3d953-137">userId</span></span>|<span data-ttu-id="3d953-138">String</span><span class="sxs-lookup"><span data-stu-id="3d953-138">String</span></span>|<span data-ttu-id="3d953-139">Уникальный идентификатор пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="3d953-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="3d953-140">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-140">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="3d953-141">deviceName</span></span>|<span data-ttu-id="3d953-142">String</span><span class="sxs-lookup"><span data-stu-id="3d953-142">String</span></span>|<span data-ttu-id="3d953-143">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-143">Name of the device.</span></span> <span data-ttu-id="3d953-144">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-144">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-145">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="3d953-145">hardwareInformation</span></span>|[<span data-ttu-id="3d953-146">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="3d953-146">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="3d953-147">Сведения о хардвард для устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-147">The hardward details for the device.</span></span>  <span data-ttu-id="3d953-148">Включает такие сведения, как место хранения, производитель, серийный номер и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-148">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span>|
|<span data-ttu-id="3d953-149">ownerType</span><span class="sxs-lookup"><span data-stu-id="3d953-149">ownerType</span></span>|[<span data-ttu-id="3d953-150">ownerType</span><span class="sxs-lookup"><span data-stu-id="3d953-150">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="3d953-151">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="3d953-151">Ownership of the device.</span></span> <span data-ttu-id="3d953-152">Может быть "Company" или "Personal".</span><span class="sxs-lookup"><span data-stu-id="3d953-152">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="3d953-153">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="3d953-153">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="3d953-154">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="3d953-154">managedDeviceOwnerType</span></span>|[<span data-ttu-id="3d953-155">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="3d953-155">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="3d953-156">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="3d953-156">Ownership of the device.</span></span> <span data-ttu-id="3d953-157">Может быть "Company" или "Personal".</span><span class="sxs-lookup"><span data-stu-id="3d953-157">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="3d953-158">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="3d953-158">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="3d953-159">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="3d953-159">deviceActionResults</span></span>|<span data-ttu-id="3d953-160">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3d953-160">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="3d953-161">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="3d953-161">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="3d953-162">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-162">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-163">манажементстате</span><span class="sxs-lookup"><span data-stu-id="3d953-163">managementState</span></span>|[<span data-ttu-id="3d953-164">манажементстате</span><span class="sxs-lookup"><span data-stu-id="3d953-164">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="3d953-165">Состояние управления для устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-165">Management state of the device.</span></span> <span data-ttu-id="3d953-166">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-166">This property is read-only.</span></span> <span data-ttu-id="3d953-167">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="3d953-167">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="3d953-168">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="3d953-168">enrolledDateTime</span></span>|<span data-ttu-id="3d953-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d953-169">DateTimeOffset</span></span>|<span data-ttu-id="3d953-170">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-170">Enrollment time of the device.</span></span> <span data-ttu-id="3d953-171">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-171">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-172">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3d953-172">lastSyncDateTime</span></span>|<span data-ttu-id="3d953-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d953-173">DateTimeOffset</span></span>|<span data-ttu-id="3d953-174">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="3d953-174">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="3d953-175">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-175">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-176">чассистипе</span><span class="sxs-lookup"><span data-stu-id="3d953-176">chassisType</span></span>|[<span data-ttu-id="3d953-177">чассистипе</span><span class="sxs-lookup"><span data-stu-id="3d953-177">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="3d953-178">Тип корпуса устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-178">Chassis type of the device.</span></span> <span data-ttu-id="3d953-179">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-179">This property is read-only.</span></span> <span data-ttu-id="3d953-180">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="3d953-180">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="3d953-181">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="3d953-181">operatingSystem</span></span>|<span data-ttu-id="3d953-182">String</span><span class="sxs-lookup"><span data-stu-id="3d953-182">String</span></span>|<span data-ttu-id="3d953-183">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-183">Operating system of the device.</span></span> <span data-ttu-id="3d953-184">Windows, iOS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-184">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="3d953-185">deviceType</span><span class="sxs-lookup"><span data-stu-id="3d953-185">deviceType</span></span>|[<span data-ttu-id="3d953-186">deviceType</span><span class="sxs-lookup"><span data-stu-id="3d953-186">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="3d953-187">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-187">Platform of the device.</span></span> <span data-ttu-id="3d953-188">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-188">This property is read-only.</span></span> <span data-ttu-id="3d953-189">Возможные `desktop`значения:, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `blackberry` `palm` `unknown`,,,,,,, `iSocConsumer`,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`</span><span class="sxs-lookup"><span data-stu-id="3d953-189">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="3d953-190">complianceState</span><span class="sxs-lookup"><span data-stu-id="3d953-190">complianceState</span></span>|[<span data-ttu-id="3d953-191">complianceState</span><span class="sxs-lookup"><span data-stu-id="3d953-191">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="3d953-192">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="3d953-192">Compliance state of the device.</span></span> <span data-ttu-id="3d953-193">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-193">This property is read-only.</span></span> <span data-ttu-id="3d953-194">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="3d953-194">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="3d953-195">jailBroken</span><span class="sxs-lookup"><span data-stu-id="3d953-195">jailBroken</span></span>|<span data-ttu-id="3d953-196">String</span><span class="sxs-lookup"><span data-stu-id="3d953-196">String</span></span>|<span data-ttu-id="3d953-197">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="3d953-197">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="3d953-198">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-198">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-199">managementAgent</span><span class="sxs-lookup"><span data-stu-id="3d953-199">managementAgent</span></span>|[<span data-ttu-id="3d953-200">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="3d953-200">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="3d953-201">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="3d953-201">Management channel of the device.</span></span> <span data-ttu-id="3d953-202">Intune, EAS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-202">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="3d953-203">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="3d953-203">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="3d953-204">osVersion</span><span class="sxs-lookup"><span data-stu-id="3d953-204">osVersion</span></span>|<span data-ttu-id="3d953-205">String</span><span class="sxs-lookup"><span data-stu-id="3d953-205">String</span></span>|<span data-ttu-id="3d953-206">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-206">Operating system version of the device.</span></span> <span data-ttu-id="3d953-207">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-207">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-208">easActivated</span><span class="sxs-lookup"><span data-stu-id="3d953-208">easActivated</span></span>|<span data-ttu-id="3d953-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d953-209">Boolean</span></span>|<span data-ttu-id="3d953-210">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="3d953-210">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="3d953-211">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-211">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-212">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="3d953-212">easDeviceId</span></span>|<span data-ttu-id="3d953-213">String</span><span class="sxs-lookup"><span data-stu-id="3d953-213">String</span></span>|<span data-ttu-id="3d953-214">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="3d953-214">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="3d953-215">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-215">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-216">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="3d953-216">easActivationDateTime</span></span>|<span data-ttu-id="3d953-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d953-217">DateTimeOffset</span></span>|<span data-ttu-id="3d953-218">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="3d953-218">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="3d953-219">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-219">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-220">аадрегистеред</span><span class="sxs-lookup"><span data-stu-id="3d953-220">aadRegistered</span></span>|<span data-ttu-id="3d953-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d953-221">Boolean</span></span>|<span data-ttu-id="3d953-222">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3d953-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="3d953-223">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-223">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-224">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="3d953-224">azureADRegistered</span></span>|<span data-ttu-id="3d953-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d953-225">Boolean</span></span>|<span data-ttu-id="3d953-226">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3d953-226">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="3d953-227">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-227">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-228">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="3d953-228">deviceEnrollmentType</span></span>|[<span data-ttu-id="3d953-229">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="3d953-229">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="3d953-230">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-230">Enrollment type of the device.</span></span> <span data-ttu-id="3d953-231">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-231">This property is read-only.</span></span> <span data-ttu-id="3d953-232">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="3d953-232">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="3d953-233">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="3d953-233">lostModeState</span></span>|[<span data-ttu-id="3d953-234">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="3d953-234">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="3d953-235">Указывает, включен ли режим потерянных или отключенных.</span><span class="sxs-lookup"><span data-stu-id="3d953-235">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="3d953-236">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-236">This property is read-only.</span></span> <span data-ttu-id="3d953-237">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="3d953-237">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="3d953-238">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="3d953-238">activationLockBypassCode</span></span>|<span data-ttu-id="3d953-239">String</span><span class="sxs-lookup"><span data-stu-id="3d953-239">String</span></span>|<span data-ttu-id="3d953-240">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="3d953-240">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="3d953-241">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-241">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-242">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3d953-242">emailAddress</span></span>|<span data-ttu-id="3d953-243">String</span><span class="sxs-lookup"><span data-stu-id="3d953-243">String</span></span>|<span data-ttu-id="3d953-244">Сообщения электронной почты пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="3d953-244">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="3d953-245">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-245">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-246">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="3d953-246">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="3d953-247">String</span><span class="sxs-lookup"><span data-stu-id="3d953-247">String</span></span>|<span data-ttu-id="3d953-248">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3d953-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="3d953-249">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-249">Read only.</span></span> <span data-ttu-id="3d953-250">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-250">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-251">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="3d953-251">azureADDeviceId</span></span>|<span data-ttu-id="3d953-252">String</span><span class="sxs-lookup"><span data-stu-id="3d953-252">String</span></span>|<span data-ttu-id="3d953-253">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3d953-253">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="3d953-254">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-254">Read only.</span></span> <span data-ttu-id="3d953-255">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-255">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-256">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="3d953-256">deviceRegistrationState</span></span>|[<span data-ttu-id="3d953-257">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="3d953-257">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="3d953-258">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-258">Device registration state.</span></span> <span data-ttu-id="3d953-259">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-259">This property is read-only.</span></span> <span data-ttu-id="3d953-260">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="3d953-260">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="3d953-261">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="3d953-261">deviceCategoryDisplayName</span></span>|<span data-ttu-id="3d953-262">String</span><span class="sxs-lookup"><span data-stu-id="3d953-262">String</span></span>|<span data-ttu-id="3d953-263">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="3d953-263">Device category display name.</span></span> <span data-ttu-id="3d953-264">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-264">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-265">isSupervised</span><span class="sxs-lookup"><span data-stu-id="3d953-265">isSupervised</span></span>|<span data-ttu-id="3d953-266">Логический</span><span class="sxs-lookup"><span data-stu-id="3d953-266">Boolean</span></span>|<span data-ttu-id="3d953-267">Состояние контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-267">Device supervised status.</span></span> <span data-ttu-id="3d953-268">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-268">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-269">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3d953-269">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="3d953-270">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d953-270">DateTimeOffset</span></span>|<span data-ttu-id="3d953-271">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="3d953-271">Last time the device contacted Exchange.</span></span> <span data-ttu-id="3d953-272">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-272">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-273">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="3d953-273">exchangeAccessState</span></span>|[<span data-ttu-id="3d953-274">девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="3d953-274">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="3d953-275">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="3d953-275">The Access State of the device in Exchange.</span></span> <span data-ttu-id="3d953-276">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-276">This property is read-only.</span></span> <span data-ttu-id="3d953-277">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="3d953-277">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="3d953-278">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="3d953-278">exchangeAccessStateReason</span></span>|[<span data-ttu-id="3d953-279">девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="3d953-279">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="3d953-280">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="3d953-280">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="3d953-281">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-281">This property is read-only.</span></span> <span data-ttu-id="3d953-282">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="3d953-282">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="3d953-283">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="3d953-283">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="3d953-284">String</span><span class="sxs-lookup"><span data-stu-id="3d953-284">String</span></span>|<span data-ttu-id="3d953-285">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="3d953-285">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="3d953-286">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-286">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-287">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3d953-287">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="3d953-288">String</span><span class="sxs-lookup"><span data-stu-id="3d953-288">String</span></span>|<span data-ttu-id="3d953-289">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="3d953-289">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="3d953-290">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-290">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-291">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="3d953-291">isEncrypted</span></span>|<span data-ttu-id="3d953-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d953-292">Boolean</span></span>|<span data-ttu-id="3d953-293">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-293">Device encryption status.</span></span> <span data-ttu-id="3d953-294">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-294">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-295">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3d953-295">userPrincipalName</span></span>|<span data-ttu-id="3d953-296">String</span><span class="sxs-lookup"><span data-stu-id="3d953-296">String</span></span>|<span data-ttu-id="3d953-297">Имя участника пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-297">Device user principal name.</span></span> <span data-ttu-id="3d953-298">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-298">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-299">model</span><span class="sxs-lookup"><span data-stu-id="3d953-299">model</span></span>|<span data-ttu-id="3d953-300">String</span><span class="sxs-lookup"><span data-stu-id="3d953-300">String</span></span>|<span data-ttu-id="3d953-301">Модель устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-301">Model of the device.</span></span> <span data-ttu-id="3d953-302">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-302">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-303">manufacturer</span><span class="sxs-lookup"><span data-stu-id="3d953-303">manufacturer</span></span>|<span data-ttu-id="3d953-304">String</span><span class="sxs-lookup"><span data-stu-id="3d953-304">String</span></span>|<span data-ttu-id="3d953-305">Производитель устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-305">Manufacturer of the device.</span></span> <span data-ttu-id="3d953-306">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-306">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-307">imei</span><span class="sxs-lookup"><span data-stu-id="3d953-307">imei</span></span>|<span data-ttu-id="3d953-308">String</span><span class="sxs-lookup"><span data-stu-id="3d953-308">String</span></span>|<span data-ttu-id="3d953-309">IMEI.</span><span class="sxs-lookup"><span data-stu-id="3d953-309">IMEI.</span></span> <span data-ttu-id="3d953-310">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-310">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-311">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3d953-311">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="3d953-312">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d953-312">DateTimeOffset</span></span>|<span data-ttu-id="3d953-313">Дата и время истечения льготного периода соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="3d953-313">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="3d953-314">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-314">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-315">serialNumber</span><span class="sxs-lookup"><span data-stu-id="3d953-315">serialNumber</span></span>|<span data-ttu-id="3d953-316">Строка</span><span class="sxs-lookup"><span data-stu-id="3d953-316">String</span></span>|<span data-ttu-id="3d953-317">Серийный.</span><span class="sxs-lookup"><span data-stu-id="3d953-317">SerialNumber.</span></span> <span data-ttu-id="3d953-318">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-318">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-319">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="3d953-319">phoneNumber</span></span>|<span data-ttu-id="3d953-320">String</span><span class="sxs-lookup"><span data-stu-id="3d953-320">String</span></span>|<span data-ttu-id="3d953-321">Номер телефона устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-321">Phone number of the device.</span></span> <span data-ttu-id="3d953-322">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-322">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-323">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="3d953-323">androidSecurityPatchLevel</span></span>|<span data-ttu-id="3d953-324">String</span><span class="sxs-lookup"><span data-stu-id="3d953-324">String</span></span>|<span data-ttu-id="3d953-325">Уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="3d953-325">Android security patch level.</span></span> <span data-ttu-id="3d953-326">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-326">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-327">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3d953-327">userDisplayName</span></span>|<span data-ttu-id="3d953-328">String</span><span class="sxs-lookup"><span data-stu-id="3d953-328">String</span></span>|<span data-ttu-id="3d953-329">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="3d953-329">User display name.</span></span> <span data-ttu-id="3d953-330">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-330">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-331">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="3d953-331">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="3d953-332">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="3d953-332">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="3d953-333">Функции, поддерживающие клиент Конфигрмгр.</span><span class="sxs-lookup"><span data-stu-id="3d953-333">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="3d953-334">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-334">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-335">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="3d953-335">wiFiMacAddress</span></span>|<span data-ttu-id="3d953-336">String</span><span class="sxs-lookup"><span data-stu-id="3d953-336">String</span></span>|<span data-ttu-id="3d953-337">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="3d953-337">Wi-Fi MAC.</span></span> <span data-ttu-id="3d953-338">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-338">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-339">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="3d953-339">deviceHealthAttestationState</span></span>|[<span data-ttu-id="3d953-340">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="3d953-340">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="3d953-341">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-341">The device health attestation state.</span></span> <span data-ttu-id="3d953-342">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-342">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-343">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="3d953-343">subscriberCarrier</span></span>|<span data-ttu-id="3d953-344">String</span><span class="sxs-lookup"><span data-stu-id="3d953-344">String</span></span>|<span data-ttu-id="3d953-345">Перевозчик абонента.</span><span class="sxs-lookup"><span data-stu-id="3d953-345">Subscriber Carrier.</span></span> <span data-ttu-id="3d953-346">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-346">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-347">meid</span><span class="sxs-lookup"><span data-stu-id="3d953-347">meid</span></span>|<span data-ttu-id="3d953-348">String</span><span class="sxs-lookup"><span data-stu-id="3d953-348">String</span></span>|<span data-ttu-id="3d953-349">MEID.</span><span class="sxs-lookup"><span data-stu-id="3d953-349">MEID.</span></span> <span data-ttu-id="3d953-350">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-350">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-351">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="3d953-351">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="3d953-352">Int64</span><span class="sxs-lookup"><span data-stu-id="3d953-352">Int64</span></span>|<span data-ttu-id="3d953-353">Общий объем хранилища в байтах.</span><span class="sxs-lookup"><span data-stu-id="3d953-353">Total Storage in Bytes.</span></span> <span data-ttu-id="3d953-354">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-354">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-355">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="3d953-355">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="3d953-356">Int64</span><span class="sxs-lookup"><span data-stu-id="3d953-356">Int64</span></span>|<span data-ttu-id="3d953-357">Свободное хранилище в байтах.</span><span class="sxs-lookup"><span data-stu-id="3d953-357">Free Storage in Bytes.</span></span> <span data-ttu-id="3d953-358">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-358">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-359">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="3d953-359">managedDeviceName</span></span>|<span data-ttu-id="3d953-360">String</span><span class="sxs-lookup"><span data-stu-id="3d953-360">String</span></span>|<span data-ttu-id="3d953-361">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-361">Automatically generated name to identify a device.</span></span> <span data-ttu-id="3d953-362">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="3d953-362">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="3d953-363">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="3d953-363">partnerReportedThreatState</span></span>|[<span data-ttu-id="3d953-364">манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="3d953-364">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="3d953-365">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="3d953-365">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="3d953-366">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-366">Read Only.</span></span> <span data-ttu-id="3d953-367">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-367">This property is read-only.</span></span> <span data-ttu-id="3d953-368">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="3d953-368">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="3d953-369">ретиреафтердатетиме</span><span class="sxs-lookup"><span data-stu-id="3d953-369">retireAfterDateTime</span></span>|<span data-ttu-id="3d953-370">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d953-370">DateTimeOffset</span></span>|<span data-ttu-id="3d953-371">Указывает время, по истечении которого устройство будет автоматически снято из-за запланированного действия.</span><span class="sxs-lookup"><span data-stu-id="3d953-371">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="3d953-372">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-372">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-373">усерслогжедон</span><span class="sxs-lookup"><span data-stu-id="3d953-373">usersLoggedOn</span></span>|<span data-ttu-id="3d953-374">Коллекция [логжедонусер](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="3d953-374">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="3d953-375">Указывает последнего вошедшего в систему пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-375">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="3d953-376">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-376">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-377">префермдмоверграупполициапплиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="3d953-377">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="3d953-378">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d953-378">DateTimeOffset</span></span>|<span data-ttu-id="3d953-379">Сообщает о значении DateTime, заданном параметром Префермдмоверграупполици.</span><span class="sxs-lookup"><span data-stu-id="3d953-379">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="3d953-380">Если этот параметр установлен, параметры групповой политики в случае конфликта будут переопределяться параметрами групповой политики.</span><span class="sxs-lookup"><span data-stu-id="3d953-380">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="3d953-381">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-381">Read Only.</span></span> <span data-ttu-id="3d953-382">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-382">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-383">аутопилотенроллед</span><span class="sxs-lookup"><span data-stu-id="3d953-383">autopilotEnrolled</span></span>|<span data-ttu-id="3d953-384">Логический</span><span class="sxs-lookup"><span data-stu-id="3d953-384">Boolean</span></span>|<span data-ttu-id="3d953-385">Сообщает, зарегистрировано ли управляемое устройство через Автоматический пилот.</span><span class="sxs-lookup"><span data-stu-id="3d953-385">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="3d953-386">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-386">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-387">рекуиреусеренроллментаппровал</span><span class="sxs-lookup"><span data-stu-id="3d953-387">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="3d953-388">Логический</span><span class="sxs-lookup"><span data-stu-id="3d953-388">Boolean</span></span>|<span data-ttu-id="3d953-389">Указывает, является ли управляемое устройство iOS регистрацией на утверждение пользователя.</span><span class="sxs-lookup"><span data-stu-id="3d953-389">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="3d953-390">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-390">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-391">манажементцертификатикспиратиондате</span><span class="sxs-lookup"><span data-stu-id="3d953-391">managementCertificateExpirationDate</span></span>|<span data-ttu-id="3d953-392">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d953-392">DateTimeOffset</span></span>|<span data-ttu-id="3d953-393">Дата окончания срока действия сертификата управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="3d953-393">Reports device management certificate expiration date.</span></span> <span data-ttu-id="3d953-394">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-394">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-395">икЦид</span><span class="sxs-lookup"><span data-stu-id="3d953-395">iccid</span></span>|<span data-ttu-id="3d953-396">String</span><span class="sxs-lookup"><span data-stu-id="3d953-396">String</span></span>|<span data-ttu-id="3d953-397">Идентификатор встроенной карты — это уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="3d953-397">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="3d953-398">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-398">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-399">удид</span><span class="sxs-lookup"><span data-stu-id="3d953-399">udid</span></span>|<span data-ttu-id="3d953-400">String</span><span class="sxs-lookup"><span data-stu-id="3d953-400">String</span></span>|<span data-ttu-id="3d953-401">Уникальный идентификатор устройства для устройств iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="3d953-401">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="3d953-402">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-402">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-403">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3d953-403">roleScopeTagIds</span></span>|<span data-ttu-id="3d953-404">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3d953-404">String collection</span></span>|<span data-ttu-id="3d953-405">Список идентификаторов тегов области для этого экземпляра устройства.</span><span class="sxs-lookup"><span data-stu-id="3d953-405">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="3d953-406">виндовсактивемалварекаунт</span><span class="sxs-lookup"><span data-stu-id="3d953-406">windowsActiveMalwareCount</span></span>|<span data-ttu-id="3d953-407">Int32</span><span class="sxs-lookup"><span data-stu-id="3d953-407">Int32</span></span>|<span data-ttu-id="3d953-408">Количество активных вредоносных программ для этого устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="3d953-408">Count of active malware for this windows device.</span></span> <span data-ttu-id="3d953-409">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-409">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-410">виндовсремедиатедмалварекаунт</span><span class="sxs-lookup"><span data-stu-id="3d953-410">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="3d953-411">Int32</span><span class="sxs-lookup"><span data-stu-id="3d953-411">Int32</span></span>|<span data-ttu-id="3d953-412">Количество исправленных вредоносных программ для этого устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="3d953-412">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="3d953-413">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-413">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-414">notes</span><span class="sxs-lookup"><span data-stu-id="3d953-414">notes</span></span>|<span data-ttu-id="3d953-415">String</span><span class="sxs-lookup"><span data-stu-id="3d953-415">String</span></span>|<span data-ttu-id="3d953-416">Примечания к устройству, созданному ИТ ИТ Admin</span><span class="sxs-lookup"><span data-stu-id="3d953-416">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="3d953-417">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="3d953-417">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="3d953-418">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="3d953-418">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="3d953-419">Состояние работоспособности клиента Configuration Manager, действительно только для устройств под управлением агентов MDM/ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="3d953-419">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="3d953-420">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="3d953-420">configurationManagerClientInformation</span></span>|[<span data-ttu-id="3d953-421">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="3d953-421">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="3d953-422">Сведения о клиенте Configuration Manager, действительные только для управляемых устройств, управляемых дуел или управляемых с помощью агентов ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="3d953-422">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|
|<span data-ttu-id="3d953-423">есернетмакаддресс</span><span class="sxs-lookup"><span data-stu-id="3d953-423">ethernetMacAddress</span></span>|<span data-ttu-id="3d953-424">String</span><span class="sxs-lookup"><span data-stu-id="3d953-424">String</span></span>|<span data-ttu-id="3d953-425">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="3d953-425">Ethernet MAC.</span></span> <span data-ttu-id="3d953-426">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-426">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-427">фисикалмеморинбитес</span><span class="sxs-lookup"><span data-stu-id="3d953-427">physicalMemoryInBytes</span></span>|<span data-ttu-id="3d953-428">Int64</span><span class="sxs-lookup"><span data-stu-id="3d953-428">Int64</span></span>|<span data-ttu-id="3d953-429">Общий объем памяти в байтах.</span><span class="sxs-lookup"><span data-stu-id="3d953-429">Total Memory in Bytes.</span></span> <span data-ttu-id="3d953-430">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-430">This property is read-only.</span></span>|
|<span data-ttu-id="3d953-431">процессорарчитектуре</span><span class="sxs-lookup"><span data-stu-id="3d953-431">processorArchitecture</span></span>|[<span data-ttu-id="3d953-432">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="3d953-432">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="3d953-433">Архитектура процессора.</span><span class="sxs-lookup"><span data-stu-id="3d953-433">Processor architecture.</span></span> <span data-ttu-id="3d953-434">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d953-434">This property is read-only.</span></span> <span data-ttu-id="3d953-435">Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="3d953-435">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|



## <a name="response"></a><span data-ttu-id="3d953-436">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d953-436">Response</span></span>
<span data-ttu-id="3d953-437">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDevice](../resources/intune-devices-manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3d953-437">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d953-438">Пример</span><span class="sxs-lookup"><span data-stu-id="3d953-438">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d953-439">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d953-439">Request</span></span>
<span data-ttu-id="3d953-440">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d953-440">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7634

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
    "osBuildNumber": "Os Build Number value"
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
    "clientIdentifier": "Client Identifier value"
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86"
}
```

### <a name="response"></a><span data-ttu-id="3d953-441">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d953-441">Response</span></span>
<span data-ttu-id="3d953-p170">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d953-p170">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7683

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
    "osBuildNumber": "Os Build Number value"
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
    "clientIdentifier": "Client Identifier value"
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86"
}
```





