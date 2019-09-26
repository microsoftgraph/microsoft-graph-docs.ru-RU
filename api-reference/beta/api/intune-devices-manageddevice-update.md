---
title: Обновление managedDevice
description: Обновление свойств объекта managedDevice.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 51982299fb65fbd295e39b4bd2b936fd92ce767e
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188293"
---
# <a name="update-manageddevice"></a><span data-ttu-id="81204-103">Обновление managedDevice</span><span class="sxs-lookup"><span data-stu-id="81204-103">Update managedDevice</span></span>

> <span data-ttu-id="81204-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81204-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81204-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81204-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81204-106">Обновление свойств объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="81204-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81204-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="81204-107">Prerequisites</span></span>
<span data-ttu-id="81204-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81204-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81204-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81204-110">Permission type</span></span>|<span data-ttu-id="81204-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="81204-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81204-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81204-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81204-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81204-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="81204-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81204-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81204-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81204-115">Not supported.</span></span>|
|<span data-ttu-id="81204-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81204-116">Application</span></span>|<span data-ttu-id="81204-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81204-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81204-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81204-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="81204-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81204-119">Request headers</span></span>
|<span data-ttu-id="81204-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81204-120">Header</span></span>|<span data-ttu-id="81204-121">Значение</span><span class="sxs-lookup"><span data-stu-id="81204-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81204-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81204-122">Authorization</span></span>|<span data-ttu-id="81204-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81204-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81204-124">Accept</span><span class="sxs-lookup"><span data-stu-id="81204-124">Accept</span></span>|<span data-ttu-id="81204-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81204-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81204-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="81204-126">Request body</span></span>
<span data-ttu-id="81204-127">В теле запроса добавьте представление объекта [managedDevice](../resources/intune-devices-manageddevice.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81204-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="81204-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="81204-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="81204-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="81204-129">Property</span></span>|<span data-ttu-id="81204-130">Тип</span><span class="sxs-lookup"><span data-stu-id="81204-130">Type</span></span>|<span data-ttu-id="81204-131">Описание</span><span class="sxs-lookup"><span data-stu-id="81204-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81204-132">id</span><span class="sxs-lookup"><span data-stu-id="81204-132">id</span></span>|<span data-ttu-id="81204-133">Строка</span><span class="sxs-lookup"><span data-stu-id="81204-133">String</span></span>|<span data-ttu-id="81204-134">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-134">Unique Identifier for the device.</span></span> <span data-ttu-id="81204-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-135">This property is read-only.</span></span>|
|<span data-ttu-id="81204-136">userId</span><span class="sxs-lookup"><span data-stu-id="81204-136">userId</span></span>|<span data-ttu-id="81204-137">String</span><span class="sxs-lookup"><span data-stu-id="81204-137">String</span></span>|<span data-ttu-id="81204-138">Уникальный идентификатор пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="81204-138">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="81204-139">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-139">This property is read-only.</span></span>|
|<span data-ttu-id="81204-140">deviceName</span><span class="sxs-lookup"><span data-stu-id="81204-140">deviceName</span></span>|<span data-ttu-id="81204-141">String.</span><span class="sxs-lookup"><span data-stu-id="81204-141">String</span></span>|<span data-ttu-id="81204-142">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-142">Name of the device.</span></span> <span data-ttu-id="81204-143">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-143">This property is read-only.</span></span>|
|<span data-ttu-id="81204-144">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="81204-144">hardwareInformation</span></span>|[<span data-ttu-id="81204-145">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="81204-145">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="81204-146">Сведения о хардвард для устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-146">The hardward details for the device.</span></span>  <span data-ttu-id="81204-147">Включает такие сведения, как место хранения, производитель, серийный номер и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-147">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span>|
|<span data-ttu-id="81204-148">ownerType</span><span class="sxs-lookup"><span data-stu-id="81204-148">ownerType</span></span>|[<span data-ttu-id="81204-149">ownerType</span><span class="sxs-lookup"><span data-stu-id="81204-149">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="81204-150">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="81204-150">Ownership of the device.</span></span> <span data-ttu-id="81204-151">Может быть "Company" или "Personal".</span><span class="sxs-lookup"><span data-stu-id="81204-151">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="81204-152">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="81204-152">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="81204-153">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="81204-153">managedDeviceOwnerType</span></span>|[<span data-ttu-id="81204-154">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="81204-154">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="81204-155">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="81204-155">Ownership of the device.</span></span> <span data-ttu-id="81204-156">Может быть "Company" или "Personal".</span><span class="sxs-lookup"><span data-stu-id="81204-156">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="81204-157">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="81204-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="81204-158">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="81204-158">deviceActionResults</span></span>|<span data-ttu-id="81204-159">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="81204-159">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="81204-160">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="81204-160">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="81204-161">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-161">This property is read-only.</span></span>|
|<span data-ttu-id="81204-162">манажементстате</span><span class="sxs-lookup"><span data-stu-id="81204-162">managementState</span></span>|[<span data-ttu-id="81204-163">манажементстате</span><span class="sxs-lookup"><span data-stu-id="81204-163">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="81204-164">Состояние управления для устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-164">Management state of the device.</span></span> <span data-ttu-id="81204-165">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-165">This property is read-only.</span></span> <span data-ttu-id="81204-166">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="81204-166">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="81204-167">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="81204-167">enrolledDateTime</span></span>|<span data-ttu-id="81204-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81204-168">DateTimeOffset</span></span>|<span data-ttu-id="81204-169">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-169">Enrollment time of the device.</span></span> <span data-ttu-id="81204-170">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-170">This property is read-only.</span></span>|
|<span data-ttu-id="81204-171">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="81204-171">lastSyncDateTime</span></span>|<span data-ttu-id="81204-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81204-172">DateTimeOffset</span></span>|<span data-ttu-id="81204-173">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="81204-173">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="81204-174">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-174">This property is read-only.</span></span>|
|<span data-ttu-id="81204-175">чассистипе</span><span class="sxs-lookup"><span data-stu-id="81204-175">chassisType</span></span>|[<span data-ttu-id="81204-176">чассистипе</span><span class="sxs-lookup"><span data-stu-id="81204-176">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="81204-177">Тип корпуса устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-177">Chassis type of the device.</span></span> <span data-ttu-id="81204-178">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-178">This property is read-only.</span></span> <span data-ttu-id="81204-179">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="81204-179">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="81204-180">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="81204-180">operatingSystem</span></span>|<span data-ttu-id="81204-181">String.</span><span class="sxs-lookup"><span data-stu-id="81204-181">String</span></span>|<span data-ttu-id="81204-182">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-182">Operating system of the device.</span></span> <span data-ttu-id="81204-183">Windows, iOS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-183">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="81204-184">deviceType</span><span class="sxs-lookup"><span data-stu-id="81204-184">deviceType</span></span>|[<span data-ttu-id="81204-185">deviceType</span><span class="sxs-lookup"><span data-stu-id="81204-185">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="81204-186">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-186">Platform of the device.</span></span> <span data-ttu-id="81204-187">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-187">This property is read-only.</span></span> <span data-ttu-id="81204-188">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `android` `iSocConsumer`,,,,,,,,,,,,,,,,,,,,, `winEmbedded` `iPhone` `iPad` `iPod` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="81204-188">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="81204-189">complianceState</span><span class="sxs-lookup"><span data-stu-id="81204-189">complianceState</span></span>|[<span data-ttu-id="81204-190">complianceState</span><span class="sxs-lookup"><span data-stu-id="81204-190">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="81204-191">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="81204-191">Compliance state of the device.</span></span> <span data-ttu-id="81204-192">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-192">This property is read-only.</span></span> <span data-ttu-id="81204-193">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="81204-193">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="81204-194">jailBroken</span><span class="sxs-lookup"><span data-stu-id="81204-194">jailBroken</span></span>|<span data-ttu-id="81204-195">String.</span><span class="sxs-lookup"><span data-stu-id="81204-195">String</span></span>|<span data-ttu-id="81204-196">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="81204-196">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="81204-197">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-197">This property is read-only.</span></span>|
|<span data-ttu-id="81204-198">managementAgent</span><span class="sxs-lookup"><span data-stu-id="81204-198">managementAgent</span></span>|[<span data-ttu-id="81204-199">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="81204-199">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="81204-200">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="81204-200">Management channel of the device.</span></span> <span data-ttu-id="81204-201">Intune, EAS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-201">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="81204-202">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="81204-202">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="81204-203">osVersion</span><span class="sxs-lookup"><span data-stu-id="81204-203">osVersion</span></span>|<span data-ttu-id="81204-204">String.</span><span class="sxs-lookup"><span data-stu-id="81204-204">String</span></span>|<span data-ttu-id="81204-205">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-205">Operating system version of the device.</span></span> <span data-ttu-id="81204-206">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-206">This property is read-only.</span></span>|
|<span data-ttu-id="81204-207">easActivated</span><span class="sxs-lookup"><span data-stu-id="81204-207">easActivated</span></span>|<span data-ttu-id="81204-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="81204-208">Boolean</span></span>|<span data-ttu-id="81204-209">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="81204-209">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="81204-210">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-210">This property is read-only.</span></span>|
|<span data-ttu-id="81204-211">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="81204-211">easDeviceId</span></span>|<span data-ttu-id="81204-212">String</span><span class="sxs-lookup"><span data-stu-id="81204-212">String</span></span>|<span data-ttu-id="81204-213">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="81204-213">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="81204-214">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-214">This property is read-only.</span></span>|
|<span data-ttu-id="81204-215">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="81204-215">easActivationDateTime</span></span>|<span data-ttu-id="81204-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81204-216">DateTimeOffset</span></span>|<span data-ttu-id="81204-217">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="81204-217">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="81204-218">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-218">This property is read-only.</span></span>|
|<span data-ttu-id="81204-219">аадрегистеред</span><span class="sxs-lookup"><span data-stu-id="81204-219">aadRegistered</span></span>|<span data-ttu-id="81204-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="81204-220">Boolean</span></span>|<span data-ttu-id="81204-221">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="81204-221">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="81204-222">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-222">This property is read-only.</span></span>|
|<span data-ttu-id="81204-223">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="81204-223">azureADRegistered</span></span>|<span data-ttu-id="81204-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="81204-224">Boolean</span></span>|<span data-ttu-id="81204-225">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="81204-225">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="81204-226">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-226">This property is read-only.</span></span>|
|<span data-ttu-id="81204-227">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="81204-227">deviceEnrollmentType</span></span>|[<span data-ttu-id="81204-228">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="81204-228">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="81204-229">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-229">Enrollment type of the device.</span></span> <span data-ttu-id="81204-230">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-230">This property is read-only.</span></span> <span data-ttu-id="81204-231">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `appleUserEnrollmentWithAzureAD`.</span><span class="sxs-lookup"><span data-stu-id="81204-231">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `appleUserEnrollmentWithAzureAD`.</span></span>|
|<span data-ttu-id="81204-232">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="81204-232">lostModeState</span></span>|[<span data-ttu-id="81204-233">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="81204-233">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="81204-234">Указывает, включен ли режим потерянных или отключенных.</span><span class="sxs-lookup"><span data-stu-id="81204-234">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="81204-235">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-235">This property is read-only.</span></span> <span data-ttu-id="81204-236">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="81204-236">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="81204-237">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="81204-237">activationLockBypassCode</span></span>|<span data-ttu-id="81204-238">String.</span><span class="sxs-lookup"><span data-stu-id="81204-238">String</span></span>|<span data-ttu-id="81204-239">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="81204-239">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="81204-240">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-240">This property is read-only.</span></span>|
|<span data-ttu-id="81204-241">emailAddress</span><span class="sxs-lookup"><span data-stu-id="81204-241">emailAddress</span></span>|<span data-ttu-id="81204-242">String.</span><span class="sxs-lookup"><span data-stu-id="81204-242">String</span></span>|<span data-ttu-id="81204-243">Сообщения электронной почты пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="81204-243">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="81204-244">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-244">This property is read-only.</span></span>|
|<span data-ttu-id="81204-245">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="81204-245">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="81204-246">String.</span><span class="sxs-lookup"><span data-stu-id="81204-246">String</span></span>|<span data-ttu-id="81204-247">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="81204-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="81204-248">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-248">Read only.</span></span> <span data-ttu-id="81204-249">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-249">This property is read-only.</span></span>|
|<span data-ttu-id="81204-250">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="81204-250">azureADDeviceId</span></span>|<span data-ttu-id="81204-251">String.</span><span class="sxs-lookup"><span data-stu-id="81204-251">String</span></span>|<span data-ttu-id="81204-252">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="81204-252">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="81204-253">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-253">Read only.</span></span> <span data-ttu-id="81204-254">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-254">This property is read-only.</span></span>|
|<span data-ttu-id="81204-255">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="81204-255">deviceRegistrationState</span></span>|[<span data-ttu-id="81204-256">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="81204-256">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="81204-257">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-257">Device registration state.</span></span> <span data-ttu-id="81204-258">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-258">This property is read-only.</span></span> <span data-ttu-id="81204-259">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="81204-259">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="81204-260">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="81204-260">deviceCategoryDisplayName</span></span>|<span data-ttu-id="81204-261">String.</span><span class="sxs-lookup"><span data-stu-id="81204-261">String</span></span>|<span data-ttu-id="81204-262">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="81204-262">Device category display name.</span></span> <span data-ttu-id="81204-263">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-263">This property is read-only.</span></span>|
|<span data-ttu-id="81204-264">isSupervised</span><span class="sxs-lookup"><span data-stu-id="81204-264">isSupervised</span></span>|<span data-ttu-id="81204-265">Boolean.</span><span class="sxs-lookup"><span data-stu-id="81204-265">Boolean</span></span>|<span data-ttu-id="81204-266">Состояние контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-266">Device supervised status.</span></span> <span data-ttu-id="81204-267">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-267">This property is read-only.</span></span>|
|<span data-ttu-id="81204-268">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="81204-268">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="81204-269">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81204-269">DateTimeOffset</span></span>|<span data-ttu-id="81204-270">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="81204-270">Last time the device contacted Exchange.</span></span> <span data-ttu-id="81204-271">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-271">This property is read-only.</span></span>|
|<span data-ttu-id="81204-272">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="81204-272">exchangeAccessState</span></span>|[<span data-ttu-id="81204-273">девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="81204-273">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="81204-274">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="81204-274">The Access State of the device in Exchange.</span></span> <span data-ttu-id="81204-275">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-275">This property is read-only.</span></span> <span data-ttu-id="81204-276">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="81204-276">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="81204-277">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="81204-277">exchangeAccessStateReason</span></span>|[<span data-ttu-id="81204-278">девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="81204-278">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="81204-279">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="81204-279">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="81204-280">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-280">This property is read-only.</span></span> <span data-ttu-id="81204-281">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="81204-281">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="81204-282">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="81204-282">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="81204-283">String.</span><span class="sxs-lookup"><span data-stu-id="81204-283">String</span></span>|<span data-ttu-id="81204-284">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="81204-284">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="81204-285">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-285">This property is read-only.</span></span>|
|<span data-ttu-id="81204-286">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="81204-286">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="81204-287">String</span><span class="sxs-lookup"><span data-stu-id="81204-287">String</span></span>|<span data-ttu-id="81204-288">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="81204-288">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="81204-289">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-289">This property is read-only.</span></span>|
|<span data-ttu-id="81204-290">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="81204-290">isEncrypted</span></span>|<span data-ttu-id="81204-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="81204-291">Boolean</span></span>|<span data-ttu-id="81204-292">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-292">Device encryption status.</span></span> <span data-ttu-id="81204-293">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-293">This property is read-only.</span></span>|
|<span data-ttu-id="81204-294">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="81204-294">userPrincipalName</span></span>|<span data-ttu-id="81204-295">String</span><span class="sxs-lookup"><span data-stu-id="81204-295">String</span></span>|<span data-ttu-id="81204-296">Имя участника пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-296">Device user principal name.</span></span> <span data-ttu-id="81204-297">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-297">This property is read-only.</span></span>|
|<span data-ttu-id="81204-298">model</span><span class="sxs-lookup"><span data-stu-id="81204-298">model</span></span>|<span data-ttu-id="81204-299">String.</span><span class="sxs-lookup"><span data-stu-id="81204-299">String</span></span>|<span data-ttu-id="81204-300">Модель устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-300">Model of the device.</span></span> <span data-ttu-id="81204-301">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-301">This property is read-only.</span></span>|
|<span data-ttu-id="81204-302">manufacturer</span><span class="sxs-lookup"><span data-stu-id="81204-302">manufacturer</span></span>|<span data-ttu-id="81204-303">String.</span><span class="sxs-lookup"><span data-stu-id="81204-303">String</span></span>|<span data-ttu-id="81204-304">Производитель устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-304">Manufacturer of the device.</span></span> <span data-ttu-id="81204-305">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-305">This property is read-only.</span></span>|
|<span data-ttu-id="81204-306">imei</span><span class="sxs-lookup"><span data-stu-id="81204-306">imei</span></span>|<span data-ttu-id="81204-307">String.</span><span class="sxs-lookup"><span data-stu-id="81204-307">String</span></span>|<span data-ttu-id="81204-308">IMEI.</span><span class="sxs-lookup"><span data-stu-id="81204-308">IMEI.</span></span> <span data-ttu-id="81204-309">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-309">This property is read-only.</span></span>|
|<span data-ttu-id="81204-310">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="81204-310">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="81204-311">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81204-311">DateTimeOffset</span></span>|<span data-ttu-id="81204-312">Дата и время истечения льготного периода соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="81204-312">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="81204-313">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-313">This property is read-only.</span></span>|
|<span data-ttu-id="81204-314">serialNumber</span><span class="sxs-lookup"><span data-stu-id="81204-314">serialNumber</span></span>|<span data-ttu-id="81204-315">Строка</span><span class="sxs-lookup"><span data-stu-id="81204-315">String</span></span>|<span data-ttu-id="81204-316">Серийный.</span><span class="sxs-lookup"><span data-stu-id="81204-316">SerialNumber.</span></span> <span data-ttu-id="81204-317">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-317">This property is read-only.</span></span>|
|<span data-ttu-id="81204-318">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="81204-318">phoneNumber</span></span>|<span data-ttu-id="81204-319">String</span><span class="sxs-lookup"><span data-stu-id="81204-319">String</span></span>|<span data-ttu-id="81204-320">Номер телефона устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-320">Phone number of the device.</span></span> <span data-ttu-id="81204-321">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-321">This property is read-only.</span></span>|
|<span data-ttu-id="81204-322">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="81204-322">androidSecurityPatchLevel</span></span>|<span data-ttu-id="81204-323">String.</span><span class="sxs-lookup"><span data-stu-id="81204-323">String</span></span>|<span data-ttu-id="81204-324">Уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="81204-324">Android security patch level.</span></span> <span data-ttu-id="81204-325">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-325">This property is read-only.</span></span>|
|<span data-ttu-id="81204-326">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="81204-326">userDisplayName</span></span>|<span data-ttu-id="81204-327">String</span><span class="sxs-lookup"><span data-stu-id="81204-327">String</span></span>|<span data-ttu-id="81204-328">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="81204-328">User display name.</span></span> <span data-ttu-id="81204-329">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-329">This property is read-only.</span></span>|
|<span data-ttu-id="81204-330">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="81204-330">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="81204-331">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="81204-331">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="81204-332">Функции, поддерживающие клиент Конфигрмгр.</span><span class="sxs-lookup"><span data-stu-id="81204-332">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="81204-333">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-333">This property is read-only.</span></span>|
|<span data-ttu-id="81204-334">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="81204-334">wiFiMacAddress</span></span>|<span data-ttu-id="81204-335">String.</span><span class="sxs-lookup"><span data-stu-id="81204-335">String</span></span>|<span data-ttu-id="81204-336">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="81204-336">Wi-Fi MAC.</span></span> <span data-ttu-id="81204-337">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-337">This property is read-only.</span></span>|
|<span data-ttu-id="81204-338">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="81204-338">deviceHealthAttestationState</span></span>|[<span data-ttu-id="81204-339">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="81204-339">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="81204-340">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-340">The device health attestation state.</span></span> <span data-ttu-id="81204-341">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-341">This property is read-only.</span></span>|
|<span data-ttu-id="81204-342">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="81204-342">subscriberCarrier</span></span>|<span data-ttu-id="81204-343">String.</span><span class="sxs-lookup"><span data-stu-id="81204-343">String</span></span>|<span data-ttu-id="81204-344">Перевозчик абонента.</span><span class="sxs-lookup"><span data-stu-id="81204-344">Subscriber Carrier.</span></span> <span data-ttu-id="81204-345">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-345">This property is read-only.</span></span>|
|<span data-ttu-id="81204-346">meid</span><span class="sxs-lookup"><span data-stu-id="81204-346">meid</span></span>|<span data-ttu-id="81204-347">String.</span><span class="sxs-lookup"><span data-stu-id="81204-347">String</span></span>|<span data-ttu-id="81204-348">MEID.</span><span class="sxs-lookup"><span data-stu-id="81204-348">MEID.</span></span> <span data-ttu-id="81204-349">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-349">This property is read-only.</span></span>|
|<span data-ttu-id="81204-350">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="81204-350">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="81204-351">Int64</span><span class="sxs-lookup"><span data-stu-id="81204-351">Int64</span></span>|<span data-ttu-id="81204-352">Общий объем хранилища в байтах.</span><span class="sxs-lookup"><span data-stu-id="81204-352">Total Storage in Bytes.</span></span> <span data-ttu-id="81204-353">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-353">This property is read-only.</span></span>|
|<span data-ttu-id="81204-354">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="81204-354">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="81204-355">Int64</span><span class="sxs-lookup"><span data-stu-id="81204-355">Int64</span></span>|<span data-ttu-id="81204-356">Свободное хранилище в байтах.</span><span class="sxs-lookup"><span data-stu-id="81204-356">Free Storage in Bytes.</span></span> <span data-ttu-id="81204-357">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-357">This property is read-only.</span></span>|
|<span data-ttu-id="81204-358">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="81204-358">managedDeviceName</span></span>|<span data-ttu-id="81204-359">String</span><span class="sxs-lookup"><span data-stu-id="81204-359">String</span></span>|<span data-ttu-id="81204-360">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-360">Automatically generated name to identify a device.</span></span> <span data-ttu-id="81204-361">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="81204-361">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="81204-362">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="81204-362">partnerReportedThreatState</span></span>|[<span data-ttu-id="81204-363">манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="81204-363">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="81204-364">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="81204-364">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="81204-365">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-365">Read Only.</span></span> <span data-ttu-id="81204-366">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-366">This property is read-only.</span></span> <span data-ttu-id="81204-367">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="81204-367">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="81204-368">ретиреафтердатетиме</span><span class="sxs-lookup"><span data-stu-id="81204-368">retireAfterDateTime</span></span>|<span data-ttu-id="81204-369">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81204-369">DateTimeOffset</span></span>|<span data-ttu-id="81204-370">Указывает время, по истечении которого устройство будет автоматически снято из-за запланированного действия.</span><span class="sxs-lookup"><span data-stu-id="81204-370">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="81204-371">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-371">This property is read-only.</span></span>|
|<span data-ttu-id="81204-372">усерслогжедон</span><span class="sxs-lookup"><span data-stu-id="81204-372">usersLoggedOn</span></span>|<span data-ttu-id="81204-373">Коллекция [логжедонусер](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="81204-373">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="81204-374">Указывает последнего вошедшего в систему пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-374">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="81204-375">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-375">This property is read-only.</span></span>|
|<span data-ttu-id="81204-376">префермдмоверграупполициапплиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="81204-376">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="81204-377">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81204-377">DateTimeOffset</span></span>|<span data-ttu-id="81204-378">Сообщает о значении DateTime, заданном параметром Префермдмоверграупполици.</span><span class="sxs-lookup"><span data-stu-id="81204-378">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="81204-379">Если этот параметр установлен, параметры групповой политики в случае конфликта будут переопределяться параметрами групповой политики.</span><span class="sxs-lookup"><span data-stu-id="81204-379">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="81204-380">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-380">Read Only.</span></span> <span data-ttu-id="81204-381">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-381">This property is read-only.</span></span>|
|<span data-ttu-id="81204-382">аутопилотенроллед</span><span class="sxs-lookup"><span data-stu-id="81204-382">autopilotEnrolled</span></span>|<span data-ttu-id="81204-383">Boolean.</span><span class="sxs-lookup"><span data-stu-id="81204-383">Boolean</span></span>|<span data-ttu-id="81204-384">Сообщает, зарегистрировано ли управляемое устройство через Автоматический пилот.</span><span class="sxs-lookup"><span data-stu-id="81204-384">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="81204-385">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-385">This property is read-only.</span></span>|
|<span data-ttu-id="81204-386">рекуиреусеренроллментаппровал</span><span class="sxs-lookup"><span data-stu-id="81204-386">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="81204-387">Boolean.</span><span class="sxs-lookup"><span data-stu-id="81204-387">Boolean</span></span>|<span data-ttu-id="81204-388">Указывает, является ли управляемое устройство iOS регистрацией на утверждение пользователя.</span><span class="sxs-lookup"><span data-stu-id="81204-388">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="81204-389">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-389">This property is read-only.</span></span>|
|<span data-ttu-id="81204-390">манажементцертификатикспиратиондате</span><span class="sxs-lookup"><span data-stu-id="81204-390">managementCertificateExpirationDate</span></span>|<span data-ttu-id="81204-391">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81204-391">DateTimeOffset</span></span>|<span data-ttu-id="81204-392">Дата окончания срока действия сертификата управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="81204-392">Reports device management certificate expiration date.</span></span> <span data-ttu-id="81204-393">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-393">This property is read-only.</span></span>|
|<span data-ttu-id="81204-394">икЦид</span><span class="sxs-lookup"><span data-stu-id="81204-394">iccid</span></span>|<span data-ttu-id="81204-395">String.</span><span class="sxs-lookup"><span data-stu-id="81204-395">String</span></span>|<span data-ttu-id="81204-396">Идентификатор встроенной карты — это уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="81204-396">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="81204-397">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-397">This property is read-only.</span></span>|
|<span data-ttu-id="81204-398">удид</span><span class="sxs-lookup"><span data-stu-id="81204-398">udid</span></span>|<span data-ttu-id="81204-399">String.</span><span class="sxs-lookup"><span data-stu-id="81204-399">String</span></span>|<span data-ttu-id="81204-400">Уникальный идентификатор устройства для устройств iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="81204-400">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="81204-401">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-401">This property is read-only.</span></span>|
|<span data-ttu-id="81204-402">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="81204-402">roleScopeTagIds</span></span>|<span data-ttu-id="81204-403">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="81204-403">String collection</span></span>|<span data-ttu-id="81204-404">Список идентификаторов тегов области для этого экземпляра устройства.</span><span class="sxs-lookup"><span data-stu-id="81204-404">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="81204-405">виндовсактивемалварекаунт</span><span class="sxs-lookup"><span data-stu-id="81204-405">windowsActiveMalwareCount</span></span>|<span data-ttu-id="81204-406">Int32</span><span class="sxs-lookup"><span data-stu-id="81204-406">Int32</span></span>|<span data-ttu-id="81204-407">Количество активных вредоносных программ для этого устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="81204-407">Count of active malware for this windows device.</span></span> <span data-ttu-id="81204-408">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-408">This property is read-only.</span></span>|
|<span data-ttu-id="81204-409">виндовсремедиатедмалварекаунт</span><span class="sxs-lookup"><span data-stu-id="81204-409">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="81204-410">Int32</span><span class="sxs-lookup"><span data-stu-id="81204-410">Int32</span></span>|<span data-ttu-id="81204-411">Количество исправленных вредоносных программ для этого устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="81204-411">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="81204-412">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81204-412">This property is read-only.</span></span>|
|<span data-ttu-id="81204-413">notes</span><span class="sxs-lookup"><span data-stu-id="81204-413">notes</span></span>|<span data-ttu-id="81204-414">String.</span><span class="sxs-lookup"><span data-stu-id="81204-414">String</span></span>|<span data-ttu-id="81204-415">Примечания к устройству, созданному ИТ ИТ Admin</span><span class="sxs-lookup"><span data-stu-id="81204-415">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="81204-416">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="81204-416">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="81204-417">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="81204-417">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="81204-418">Состояние работоспособности клиента Configuration Manager, действительно только для устройств под управлением агентов MDM/ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="81204-418">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="81204-419">конфигуратионманажерклиентинформатион</span><span class="sxs-lookup"><span data-stu-id="81204-419">configurationManagerClientInformation</span></span>|[<span data-ttu-id="81204-420">конфигуратионманажерклиентинформатион</span><span class="sxs-lookup"><span data-stu-id="81204-420">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="81204-421">Сведения о клиенте Configuration Manager, действительные только для управляемых устройств, управляемых дуел или управляемых с помощью агентов ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="81204-421">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="81204-422">Отклик</span><span class="sxs-lookup"><span data-stu-id="81204-422">Response</span></span>
<span data-ttu-id="81204-423">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDevice](../resources/intune-devices-manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="81204-423">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81204-424">Пример</span><span class="sxs-lookup"><span data-stu-id="81204-424">Example</span></span>

### <a name="request"></a><span data-ttu-id="81204-425">Запрос</span><span class="sxs-lookup"><span data-stu-id="81204-425">Request</span></span>
<span data-ttu-id="81204-426">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81204-426">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7513

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
  }
}
```

### <a name="response"></a><span data-ttu-id="81204-427">Отклик</span><span class="sxs-lookup"><span data-stu-id="81204-427">Response</span></span>
<span data-ttu-id="81204-p167">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="81204-p167">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7562

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
  }
}
```




