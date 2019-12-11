---
title: Обновление managedDevice
description: Обновление свойств объекта managedDevice.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ba4ae0e36abe36b92cbc177ab1b7c1eabf46c6e0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944661"
---
# <a name="update-manageddevice"></a><span data-ttu-id="e8d1d-103">Обновление managedDevice</span><span class="sxs-lookup"><span data-stu-id="e8d1d-103">Update managedDevice</span></span>

> <span data-ttu-id="e8d1d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8d1d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8d1d-106">Обновление свойств объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="e8d1d-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8d1d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e8d1d-107">Prerequisites</span></span>
<span data-ttu-id="e8d1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8d1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8d1d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8d1d-110">Permission type</span></span>|<span data-ttu-id="e8d1d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8d1d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8d1d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8d1d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8d1d-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8d1d-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e8d1d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8d1d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8d1d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-115">Not supported.</span></span>|
|<span data-ttu-id="e8d1d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8d1d-116">Application</span></span>|<span data-ttu-id="e8d1d-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8d1d-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8d1d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8d1d-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e8d1d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e8d1d-119">Request headers</span></span>
|<span data-ttu-id="e8d1d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8d1d-120">Header</span></span>|<span data-ttu-id="e8d1d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e8d1d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8d1d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8d1d-122">Authorization</span></span>|<span data-ttu-id="e8d1d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8d1d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e8d1d-124">Accept</span></span>|<span data-ttu-id="e8d1d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8d1d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8d1d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e8d1d-126">Request body</span></span>
<span data-ttu-id="e8d1d-127">В теле запроса добавьте представление объекта [managedDevice](../resources/intune-devices-manageddevice.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="e8d1d-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="e8d1d-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="e8d1d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8d1d-129">Property</span></span>|<span data-ttu-id="e8d1d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e8d1d-130">Type</span></span>|<span data-ttu-id="e8d1d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e8d1d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8d1d-132">id</span><span class="sxs-lookup"><span data-stu-id="e8d1d-132">id</span></span>|<span data-ttu-id="e8d1d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-133">String</span></span>|<span data-ttu-id="e8d1d-134">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-134">Unique Identifier for the device.</span></span> <span data-ttu-id="e8d1d-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-135">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-136">userId</span><span class="sxs-lookup"><span data-stu-id="e8d1d-136">userId</span></span>|<span data-ttu-id="e8d1d-137">String</span><span class="sxs-lookup"><span data-stu-id="e8d1d-137">String</span></span>|<span data-ttu-id="e8d1d-138">Уникальный идентификатор пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-138">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="e8d1d-139">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-139">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-140">deviceName</span><span class="sxs-lookup"><span data-stu-id="e8d1d-140">deviceName</span></span>|<span data-ttu-id="e8d1d-141">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-141">String</span></span>|<span data-ttu-id="e8d1d-142">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-142">Name of the device.</span></span> <span data-ttu-id="e8d1d-143">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-143">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-144">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-144">hardwareInformation</span></span>|[<span data-ttu-id="e8d1d-145">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-145">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="e8d1d-146">Сведения о хардвард для устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-146">The hardward details for the device.</span></span>  <span data-ttu-id="e8d1d-147">Включает такие сведения, как место хранения, производитель, серийный номер и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-147">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-148">ownerType</span><span class="sxs-lookup"><span data-stu-id="e8d1d-148">ownerType</span></span>|[<span data-ttu-id="e8d1d-149">ownerType</span><span class="sxs-lookup"><span data-stu-id="e8d1d-149">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="e8d1d-150">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-150">Ownership of the device.</span></span> <span data-ttu-id="e8d1d-151">Может быть "Company" или "Personal".</span><span class="sxs-lookup"><span data-stu-id="e8d1d-151">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="e8d1d-152">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-152">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="e8d1d-153">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="e8d1d-153">managedDeviceOwnerType</span></span>|[<span data-ttu-id="e8d1d-154">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="e8d1d-154">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="e8d1d-155">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-155">Ownership of the device.</span></span> <span data-ttu-id="e8d1d-156">Может быть "Company" или "Personal".</span><span class="sxs-lookup"><span data-stu-id="e8d1d-156">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="e8d1d-157">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="e8d1d-158">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="e8d1d-158">deviceActionResults</span></span>|<span data-ttu-id="e8d1d-159">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e8d1d-159">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="e8d1d-160">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="e8d1d-160">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="e8d1d-161">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-161">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-162">манажементстате</span><span class="sxs-lookup"><span data-stu-id="e8d1d-162">managementState</span></span>|[<span data-ttu-id="e8d1d-163">манажементстате</span><span class="sxs-lookup"><span data-stu-id="e8d1d-163">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="e8d1d-164">Состояние управления для устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-164">Management state of the device.</span></span> <span data-ttu-id="e8d1d-165">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-165">This property is read-only.</span></span> <span data-ttu-id="e8d1d-166">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-166">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="e8d1d-167">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="e8d1d-167">enrolledDateTime</span></span>|<span data-ttu-id="e8d1d-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8d1d-168">DateTimeOffset</span></span>|<span data-ttu-id="e8d1d-169">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-169">Enrollment time of the device.</span></span> <span data-ttu-id="e8d1d-170">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-170">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-171">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e8d1d-171">lastSyncDateTime</span></span>|<span data-ttu-id="e8d1d-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8d1d-172">DateTimeOffset</span></span>|<span data-ttu-id="e8d1d-173">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-173">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="e8d1d-174">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-174">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-175">чассистипе</span><span class="sxs-lookup"><span data-stu-id="e8d1d-175">chassisType</span></span>|[<span data-ttu-id="e8d1d-176">чассистипе</span><span class="sxs-lookup"><span data-stu-id="e8d1d-176">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="e8d1d-177">Тип корпуса устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-177">Chassis type of the device.</span></span> <span data-ttu-id="e8d1d-178">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-178">This property is read-only.</span></span> <span data-ttu-id="e8d1d-179">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-179">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="e8d1d-180">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="e8d1d-180">operatingSystem</span></span>|<span data-ttu-id="e8d1d-181">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-181">String</span></span>|<span data-ttu-id="e8d1d-182">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-182">Operating system of the device.</span></span> <span data-ttu-id="e8d1d-183">Windows, iOS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-183">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-184">deviceType</span><span class="sxs-lookup"><span data-stu-id="e8d1d-184">deviceType</span></span>|[<span data-ttu-id="e8d1d-185">deviceType</span><span class="sxs-lookup"><span data-stu-id="e8d1d-185">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="e8d1d-186">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-186">Platform of the device.</span></span> <span data-ttu-id="e8d1d-187">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-187">This property is read-only.</span></span> <span data-ttu-id="e8d1d-188">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `iSocConsumer` `unknown`,,,,,,,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`</span><span class="sxs-lookup"><span data-stu-id="e8d1d-188">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="e8d1d-189">complianceState</span><span class="sxs-lookup"><span data-stu-id="e8d1d-189">complianceState</span></span>|[<span data-ttu-id="e8d1d-190">complianceState</span><span class="sxs-lookup"><span data-stu-id="e8d1d-190">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="e8d1d-191">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-191">Compliance state of the device.</span></span> <span data-ttu-id="e8d1d-192">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-192">This property is read-only.</span></span> <span data-ttu-id="e8d1d-193">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-193">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="e8d1d-194">jailBroken</span><span class="sxs-lookup"><span data-stu-id="e8d1d-194">jailBroken</span></span>|<span data-ttu-id="e8d1d-195">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-195">String</span></span>|<span data-ttu-id="e8d1d-196">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-196">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="e8d1d-197">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-197">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-198">managementAgent</span><span class="sxs-lookup"><span data-stu-id="e8d1d-198">managementAgent</span></span>|[<span data-ttu-id="e8d1d-199">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="e8d1d-199">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="e8d1d-200">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-200">Management channel of the device.</span></span> <span data-ttu-id="e8d1d-201">Intune, EAS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-201">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="e8d1d-202">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-202">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="e8d1d-203">osVersion</span><span class="sxs-lookup"><span data-stu-id="e8d1d-203">osVersion</span></span>|<span data-ttu-id="e8d1d-204">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-204">String</span></span>|<span data-ttu-id="e8d1d-205">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-205">Operating system version of the device.</span></span> <span data-ttu-id="e8d1d-206">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-206">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-207">easActivated</span><span class="sxs-lookup"><span data-stu-id="e8d1d-207">easActivated</span></span>|<span data-ttu-id="e8d1d-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8d1d-208">Boolean</span></span>|<span data-ttu-id="e8d1d-209">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-209">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="e8d1d-210">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-210">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-211">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="e8d1d-211">easDeviceId</span></span>|<span data-ttu-id="e8d1d-212">String</span><span class="sxs-lookup"><span data-stu-id="e8d1d-212">String</span></span>|<span data-ttu-id="e8d1d-213">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-213">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="e8d1d-214">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-214">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-215">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="e8d1d-215">easActivationDateTime</span></span>|<span data-ttu-id="e8d1d-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8d1d-216">DateTimeOffset</span></span>|<span data-ttu-id="e8d1d-217">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-217">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="e8d1d-218">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-218">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-219">аадрегистеред</span><span class="sxs-lookup"><span data-stu-id="e8d1d-219">aadRegistered</span></span>|<span data-ttu-id="e8d1d-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8d1d-220">Boolean</span></span>|<span data-ttu-id="e8d1d-221">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-221">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="e8d1d-222">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-222">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-223">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="e8d1d-223">azureADRegistered</span></span>|<span data-ttu-id="e8d1d-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8d1d-224">Boolean</span></span>|<span data-ttu-id="e8d1d-225">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-225">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="e8d1d-226">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-226">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-227">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="e8d1d-227">deviceEnrollmentType</span></span>|[<span data-ttu-id="e8d1d-228">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="e8d1d-228">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="e8d1d-229">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-229">Enrollment type of the device.</span></span> <span data-ttu-id="e8d1d-230">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-230">This property is read-only.</span></span> <span data-ttu-id="e8d1d-231">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-231">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="e8d1d-232">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="e8d1d-232">lostModeState</span></span>|[<span data-ttu-id="e8d1d-233">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="e8d1d-233">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="e8d1d-234">Указывает, включен ли режим потерянных или отключенных.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-234">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="e8d1d-235">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-235">This property is read-only.</span></span> <span data-ttu-id="e8d1d-236">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-236">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="e8d1d-237">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="e8d1d-237">activationLockBypassCode</span></span>|<span data-ttu-id="e8d1d-238">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-238">String</span></span>|<span data-ttu-id="e8d1d-239">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-239">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="e8d1d-240">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-240">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-241">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e8d1d-241">emailAddress</span></span>|<span data-ttu-id="e8d1d-242">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-242">String</span></span>|<span data-ttu-id="e8d1d-243">Сообщения электронной почты пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-243">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="e8d1d-244">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-244">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-245">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="e8d1d-245">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="e8d1d-246">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-246">String</span></span>|<span data-ttu-id="e8d1d-247">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="e8d1d-248">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-248">Read only.</span></span> <span data-ttu-id="e8d1d-249">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-249">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-250">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="e8d1d-250">azureADDeviceId</span></span>|<span data-ttu-id="e8d1d-251">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-251">String</span></span>|<span data-ttu-id="e8d1d-252">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-252">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="e8d1d-253">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-253">Read only.</span></span> <span data-ttu-id="e8d1d-254">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-254">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-255">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="e8d1d-255">deviceRegistrationState</span></span>|[<span data-ttu-id="e8d1d-256">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="e8d1d-256">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="e8d1d-257">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-257">Device registration state.</span></span> <span data-ttu-id="e8d1d-258">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-258">This property is read-only.</span></span> <span data-ttu-id="e8d1d-259">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-259">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="e8d1d-260">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="e8d1d-260">deviceCategoryDisplayName</span></span>|<span data-ttu-id="e8d1d-261">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-261">String</span></span>|<span data-ttu-id="e8d1d-262">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-262">Device category display name.</span></span> <span data-ttu-id="e8d1d-263">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-263">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-264">isSupervised</span><span class="sxs-lookup"><span data-stu-id="e8d1d-264">isSupervised</span></span>|<span data-ttu-id="e8d1d-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8d1d-265">Boolean</span></span>|<span data-ttu-id="e8d1d-266">Состояние контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-266">Device supervised status.</span></span> <span data-ttu-id="e8d1d-267">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-267">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-268">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e8d1d-268">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="e8d1d-269">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8d1d-269">DateTimeOffset</span></span>|<span data-ttu-id="e8d1d-270">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-270">Last time the device contacted Exchange.</span></span> <span data-ttu-id="e8d1d-271">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-271">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-272">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="e8d1d-272">exchangeAccessState</span></span>|[<span data-ttu-id="e8d1d-273">девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="e8d1d-273">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="e8d1d-274">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-274">The Access State of the device in Exchange.</span></span> <span data-ttu-id="e8d1d-275">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-275">This property is read-only.</span></span> <span data-ttu-id="e8d1d-276">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-276">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="e8d1d-277">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="e8d1d-277">exchangeAccessStateReason</span></span>|[<span data-ttu-id="e8d1d-278">девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="e8d1d-278">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="e8d1d-279">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-279">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="e8d1d-280">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-280">This property is read-only.</span></span> <span data-ttu-id="e8d1d-281">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-281">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="e8d1d-282">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="e8d1d-282">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="e8d1d-283">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-283">String</span></span>|<span data-ttu-id="e8d1d-284">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-284">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="e8d1d-285">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-285">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-286">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e8d1d-286">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="e8d1d-287">String</span><span class="sxs-lookup"><span data-stu-id="e8d1d-287">String</span></span>|<span data-ttu-id="e8d1d-288">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-288">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="e8d1d-289">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-289">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-290">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="e8d1d-290">isEncrypted</span></span>|<span data-ttu-id="e8d1d-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8d1d-291">Boolean</span></span>|<span data-ttu-id="e8d1d-292">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-292">Device encryption status.</span></span> <span data-ttu-id="e8d1d-293">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-293">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-294">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e8d1d-294">userPrincipalName</span></span>|<span data-ttu-id="e8d1d-295">String</span><span class="sxs-lookup"><span data-stu-id="e8d1d-295">String</span></span>|<span data-ttu-id="e8d1d-296">Имя участника пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-296">Device user principal name.</span></span> <span data-ttu-id="e8d1d-297">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-297">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-298">model</span><span class="sxs-lookup"><span data-stu-id="e8d1d-298">model</span></span>|<span data-ttu-id="e8d1d-299">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-299">String</span></span>|<span data-ttu-id="e8d1d-300">Модель устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-300">Model of the device.</span></span> <span data-ttu-id="e8d1d-301">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-301">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-302">manufacturer</span><span class="sxs-lookup"><span data-stu-id="e8d1d-302">manufacturer</span></span>|<span data-ttu-id="e8d1d-303">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-303">String</span></span>|<span data-ttu-id="e8d1d-304">Производитель устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-304">Manufacturer of the device.</span></span> <span data-ttu-id="e8d1d-305">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-305">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-306">imei</span><span class="sxs-lookup"><span data-stu-id="e8d1d-306">imei</span></span>|<span data-ttu-id="e8d1d-307">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-307">String</span></span>|<span data-ttu-id="e8d1d-308">IMEI.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-308">IMEI.</span></span> <span data-ttu-id="e8d1d-309">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-309">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-310">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e8d1d-310">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="e8d1d-311">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8d1d-311">DateTimeOffset</span></span>|<span data-ttu-id="e8d1d-312">Дата и время истечения льготного периода соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-312">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="e8d1d-313">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-313">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-314">serialNumber</span><span class="sxs-lookup"><span data-stu-id="e8d1d-314">serialNumber</span></span>|<span data-ttu-id="e8d1d-315">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-315">String</span></span>|<span data-ttu-id="e8d1d-316">Серийный.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-316">SerialNumber.</span></span> <span data-ttu-id="e8d1d-317">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-317">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-318">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="e8d1d-318">phoneNumber</span></span>|<span data-ttu-id="e8d1d-319">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-319">String</span></span>|<span data-ttu-id="e8d1d-320">Номер телефона устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-320">Phone number of the device.</span></span> <span data-ttu-id="e8d1d-321">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-321">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-322">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="e8d1d-322">androidSecurityPatchLevel</span></span>|<span data-ttu-id="e8d1d-323">String</span><span class="sxs-lookup"><span data-stu-id="e8d1d-323">String</span></span>|<span data-ttu-id="e8d1d-324">Уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-324">Android security patch level.</span></span> <span data-ttu-id="e8d1d-325">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-325">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-326">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e8d1d-326">userDisplayName</span></span>|<span data-ttu-id="e8d1d-327">String</span><span class="sxs-lookup"><span data-stu-id="e8d1d-327">String</span></span>|<span data-ttu-id="e8d1d-328">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-328">User display name.</span></span> <span data-ttu-id="e8d1d-329">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-329">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-330">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="e8d1d-330">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="e8d1d-331">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="e8d1d-331">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="e8d1d-332">Функции, поддерживающие клиент Конфигрмгр.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-332">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="e8d1d-333">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-333">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-334">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="e8d1d-334">wiFiMacAddress</span></span>|<span data-ttu-id="e8d1d-335">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-335">String</span></span>|<span data-ttu-id="e8d1d-336">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-336">Wi-Fi MAC.</span></span> <span data-ttu-id="e8d1d-337">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-337">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-338">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="e8d1d-338">deviceHealthAttestationState</span></span>|[<span data-ttu-id="e8d1d-339">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="e8d1d-339">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="e8d1d-340">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-340">The device health attestation state.</span></span> <span data-ttu-id="e8d1d-341">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-341">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-342">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="e8d1d-342">subscriberCarrier</span></span>|<span data-ttu-id="e8d1d-343">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-343">String</span></span>|<span data-ttu-id="e8d1d-344">Перевозчик абонента.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-344">Subscriber Carrier.</span></span> <span data-ttu-id="e8d1d-345">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-345">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-346">meid</span><span class="sxs-lookup"><span data-stu-id="e8d1d-346">meid</span></span>|<span data-ttu-id="e8d1d-347">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-347">String</span></span>|<span data-ttu-id="e8d1d-348">MEID.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-348">MEID.</span></span> <span data-ttu-id="e8d1d-349">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-349">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-350">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="e8d1d-350">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="e8d1d-351">Int64</span><span class="sxs-lookup"><span data-stu-id="e8d1d-351">Int64</span></span>|<span data-ttu-id="e8d1d-352">Общий объем хранилища в байтах.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-352">Total Storage in Bytes.</span></span> <span data-ttu-id="e8d1d-353">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-353">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-354">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="e8d1d-354">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="e8d1d-355">Int64</span><span class="sxs-lookup"><span data-stu-id="e8d1d-355">Int64</span></span>|<span data-ttu-id="e8d1d-356">Свободное хранилище в байтах.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-356">Free Storage in Bytes.</span></span> <span data-ttu-id="e8d1d-357">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-357">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-358">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="e8d1d-358">managedDeviceName</span></span>|<span data-ttu-id="e8d1d-359">String</span><span class="sxs-lookup"><span data-stu-id="e8d1d-359">String</span></span>|<span data-ttu-id="e8d1d-360">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-360">Automatically generated name to identify a device.</span></span> <span data-ttu-id="e8d1d-361">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-361">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="e8d1d-362">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="e8d1d-362">partnerReportedThreatState</span></span>|[<span data-ttu-id="e8d1d-363">манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="e8d1d-363">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="e8d1d-364">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="e8d1d-364">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="e8d1d-365">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-365">Read Only.</span></span> <span data-ttu-id="e8d1d-366">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-366">This property is read-only.</span></span> <span data-ttu-id="e8d1d-367">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-367">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="e8d1d-368">ретиреафтердатетиме</span><span class="sxs-lookup"><span data-stu-id="e8d1d-368">retireAfterDateTime</span></span>|<span data-ttu-id="e8d1d-369">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8d1d-369">DateTimeOffset</span></span>|<span data-ttu-id="e8d1d-370">Указывает время, по истечении которого устройство будет автоматически снято из-за запланированного действия.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-370">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="e8d1d-371">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-371">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-372">усерслогжедон</span><span class="sxs-lookup"><span data-stu-id="e8d1d-372">usersLoggedOn</span></span>|<span data-ttu-id="e8d1d-373">Коллекция [логжедонусер](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="e8d1d-373">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="e8d1d-374">Указывает последнего вошедшего в систему пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-374">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="e8d1d-375">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-375">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-376">префермдмоверграупполициапплиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="e8d1d-376">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="e8d1d-377">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8d1d-377">DateTimeOffset</span></span>|<span data-ttu-id="e8d1d-378">Сообщает о значении DateTime, заданном параметром Префермдмоверграупполици.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-378">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="e8d1d-379">Если этот параметр установлен, параметры групповой политики в случае конфликта будут переопределяться параметрами групповой политики.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-379">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="e8d1d-380">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-380">Read Only.</span></span> <span data-ttu-id="e8d1d-381">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-381">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-382">аутопилотенроллед</span><span class="sxs-lookup"><span data-stu-id="e8d1d-382">autopilotEnrolled</span></span>|<span data-ttu-id="e8d1d-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8d1d-383">Boolean</span></span>|<span data-ttu-id="e8d1d-384">Сообщает, зарегистрировано ли управляемое устройство через Автоматический пилот.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-384">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="e8d1d-385">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-385">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-386">рекуиреусеренроллментаппровал</span><span class="sxs-lookup"><span data-stu-id="e8d1d-386">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="e8d1d-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8d1d-387">Boolean</span></span>|<span data-ttu-id="e8d1d-388">Указывает, является ли управляемое устройство iOS регистрацией на утверждение пользователя.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-388">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="e8d1d-389">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-389">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-390">манажементцертификатикспиратиондате</span><span class="sxs-lookup"><span data-stu-id="e8d1d-390">managementCertificateExpirationDate</span></span>|<span data-ttu-id="e8d1d-391">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8d1d-391">DateTimeOffset</span></span>|<span data-ttu-id="e8d1d-392">Дата окончания срока действия сертификата управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-392">Reports device management certificate expiration date.</span></span> <span data-ttu-id="e8d1d-393">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-393">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-394">икЦид</span><span class="sxs-lookup"><span data-stu-id="e8d1d-394">iccid</span></span>|<span data-ttu-id="e8d1d-395">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-395">String</span></span>|<span data-ttu-id="e8d1d-396">Идентификатор встроенной карты — это уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-396">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="e8d1d-397">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-397">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-398">удид</span><span class="sxs-lookup"><span data-stu-id="e8d1d-398">udid</span></span>|<span data-ttu-id="e8d1d-399">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-399">String</span></span>|<span data-ttu-id="e8d1d-400">Уникальный идентификатор устройства для устройств iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-400">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="e8d1d-401">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-401">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-402">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e8d1d-402">roleScopeTagIds</span></span>|<span data-ttu-id="e8d1d-403">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e8d1d-403">String collection</span></span>|<span data-ttu-id="e8d1d-404">Список идентификаторов тегов области для этого экземпляра устройства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-404">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="e8d1d-405">виндовсактивемалварекаунт</span><span class="sxs-lookup"><span data-stu-id="e8d1d-405">windowsActiveMalwareCount</span></span>|<span data-ttu-id="e8d1d-406">Int32</span><span class="sxs-lookup"><span data-stu-id="e8d1d-406">Int32</span></span>|<span data-ttu-id="e8d1d-407">Количество активных вредоносных программ для этого устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-407">Count of active malware for this windows device.</span></span> <span data-ttu-id="e8d1d-408">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-408">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-409">виндовсремедиатедмалварекаунт</span><span class="sxs-lookup"><span data-stu-id="e8d1d-409">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="e8d1d-410">Int32</span><span class="sxs-lookup"><span data-stu-id="e8d1d-410">Int32</span></span>|<span data-ttu-id="e8d1d-411">Количество исправленных вредоносных программ для этого устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-411">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="e8d1d-412">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-412">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-413">notes</span><span class="sxs-lookup"><span data-stu-id="e8d1d-413">notes</span></span>|<span data-ttu-id="e8d1d-414">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-414">String</span></span>|<span data-ttu-id="e8d1d-415">Примечания к устройству, созданному ИТ ИТ Admin</span><span class="sxs-lookup"><span data-stu-id="e8d1d-415">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="e8d1d-416">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="e8d1d-416">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="e8d1d-417">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="e8d1d-417">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="e8d1d-418">Состояние работоспособности клиента Configuration Manager, действительно только для устройств под управлением агентов MDM/ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="e8d1d-418">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="e8d1d-419">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="e8d1d-419">configurationManagerClientInformation</span></span>|[<span data-ttu-id="e8d1d-420">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="e8d1d-420">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="e8d1d-421">Сведения о клиенте Configuration Manager, действительные только для управляемых устройств, управляемых дуел или управляемых с помощью агентов ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="e8d1d-421">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|
|<span data-ttu-id="e8d1d-422">есернетмакаддресс</span><span class="sxs-lookup"><span data-stu-id="e8d1d-422">ethernetMacAddress</span></span>|<span data-ttu-id="e8d1d-423">Строка</span><span class="sxs-lookup"><span data-stu-id="e8d1d-423">String</span></span>|<span data-ttu-id="e8d1d-424">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-424">Ethernet MAC.</span></span> <span data-ttu-id="e8d1d-425">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-425">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-426">фисикалмеморинбитес</span><span class="sxs-lookup"><span data-stu-id="e8d1d-426">physicalMemoryInBytes</span></span>|<span data-ttu-id="e8d1d-427">Int64</span><span class="sxs-lookup"><span data-stu-id="e8d1d-427">Int64</span></span>|<span data-ttu-id="e8d1d-428">Общий объем памяти в байтах.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-428">Total Memory in Bytes.</span></span> <span data-ttu-id="e8d1d-429">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-429">This property is read-only.</span></span>|
|<span data-ttu-id="e8d1d-430">процессорарчитектуре</span><span class="sxs-lookup"><span data-stu-id="e8d1d-430">processorArchitecture</span></span>|[<span data-ttu-id="e8d1d-431">манажеддевицеарчитектуре</span><span class="sxs-lookup"><span data-stu-id="e8d1d-431">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="e8d1d-432">Архитектура процессора.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-432">Processor architecture.</span></span> <span data-ttu-id="e8d1d-433">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-433">This property is read-only.</span></span> <span data-ttu-id="e8d1d-434">Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-434">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|



## <a name="response"></a><span data-ttu-id="e8d1d-435">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8d1d-435">Response</span></span>
<span data-ttu-id="e8d1d-436">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDevice](../resources/intune-devices-manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-436">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8d1d-437">Пример</span><span class="sxs-lookup"><span data-stu-id="e8d1d-437">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8d1d-438">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8d1d-438">Request</span></span>
<span data-ttu-id="e8d1d-439">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-439">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e8d1d-440">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8d1d-440">Response</span></span>
<span data-ttu-id="e8d1d-p170">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8d1d-p170">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





