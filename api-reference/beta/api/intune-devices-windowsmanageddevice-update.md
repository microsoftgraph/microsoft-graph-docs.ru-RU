---
title: Обновление windowsManagedDevice
description: Обновление свойств объекта windowsManagedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 70bb270f578f26a14e90882f73b6db61604b875a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158816"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="89405-103">Обновление windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="89405-103">Update windowsManagedDevice</span></span>

<span data-ttu-id="89405-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89405-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89405-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89405-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89405-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89405-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89405-107">Обновление свойств объекта [windowsManagedDevice.](../resources/intune-devices-windowsmanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-107">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89405-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="89405-108">Prerequisites</span></span>
<span data-ttu-id="89405-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89405-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89405-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89405-111">Permission type</span></span>|<span data-ttu-id="89405-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89405-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89405-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89405-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89405-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89405-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="89405-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89405-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89405-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89405-116">Not supported.</span></span>|
|<span data-ttu-id="89405-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89405-117">Application</span></span>|<span data-ttu-id="89405-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89405-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89405-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89405-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="89405-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="89405-120">Request headers</span></span>
|<span data-ttu-id="89405-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89405-121">Header</span></span>|<span data-ttu-id="89405-122">Значение</span><span class="sxs-lookup"><span data-stu-id="89405-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89405-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89405-123">Authorization</span></span>|<span data-ttu-id="89405-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89405-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89405-125">Accept</span><span class="sxs-lookup"><span data-stu-id="89405-125">Accept</span></span>|<span data-ttu-id="89405-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89405-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89405-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89405-127">Request body</span></span>
<span data-ttu-id="89405-128">В теле запроса укажу представление объекта [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="89405-128">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="89405-129">В следующей таблице показаны свойства, необходимые при создании [объекта windowsManagedDevice.](../resources/intune-devices-windowsmanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-129">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="89405-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="89405-130">Property</span></span>|<span data-ttu-id="89405-131">Тип</span><span class="sxs-lookup"><span data-stu-id="89405-131">Type</span></span>|<span data-ttu-id="89405-132">Описание</span><span class="sxs-lookup"><span data-stu-id="89405-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89405-133">id</span><span class="sxs-lookup"><span data-stu-id="89405-133">id</span></span>|<span data-ttu-id="89405-134">String</span><span class="sxs-lookup"><span data-stu-id="89405-134">String</span></span>|<span data-ttu-id="89405-135">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-135">Unique Identifier for the device.</span></span> <span data-ttu-id="89405-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-136">This property is read-only.</span></span> <span data-ttu-id="89405-137">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-137">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-138">userId</span><span class="sxs-lookup"><span data-stu-id="89405-138">userId</span></span>|<span data-ttu-id="89405-139">String</span><span class="sxs-lookup"><span data-stu-id="89405-139">String</span></span>|<span data-ttu-id="89405-140">Уникальный идентификатор пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="89405-140">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="89405-141">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-141">This property is read-only.</span></span> <span data-ttu-id="89405-142">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-142">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="89405-143">deviceName</span></span>|<span data-ttu-id="89405-144">String</span><span class="sxs-lookup"><span data-stu-id="89405-144">String</span></span>|<span data-ttu-id="89405-145">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-145">Name of the device.</span></span> <span data-ttu-id="89405-146">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-146">This property is read-only.</span></span> <span data-ttu-id="89405-147">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-147">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="89405-148">hardwareInformation</span></span>|[<span data-ttu-id="89405-149">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="89405-149">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="89405-150">Подробные сведения об устройстве.</span><span class="sxs-lookup"><span data-stu-id="89405-150">The hardward details for the device.</span></span>  <span data-ttu-id="89405-151">Включает такие сведения, как место в хранилище, изготовитель, серийный номер и т. д. Это свойство находится только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-151">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="89405-152">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-152">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="89405-153">ownerType</span></span>|[<span data-ttu-id="89405-154">ownerType</span><span class="sxs-lookup"><span data-stu-id="89405-154">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="89405-155">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="89405-155">Ownership of the device.</span></span> <span data-ttu-id="89405-156">Может быть "company" или "personal". Наследуется от [managedDevice.](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-156">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-157">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="89405-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="89405-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="89405-158">managedDeviceOwnerType</span></span>|[<span data-ttu-id="89405-159">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="89405-159">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="89405-160">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="89405-160">Ownership of the device.</span></span> <span data-ttu-id="89405-161">Может быть "company" или "personal". Наследуется от [managedDevice.](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-161">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-162">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="89405-162">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="89405-163">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="89405-163">deviceActionResults</span></span>|<span data-ttu-id="89405-164">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="89405-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="89405-165">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="89405-165">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="89405-166">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-166">This property is read-only.</span></span> <span data-ttu-id="89405-167">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-167">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-168">managementState</span><span class="sxs-lookup"><span data-stu-id="89405-168">managementState</span></span>|[<span data-ttu-id="89405-169">managementState</span><span class="sxs-lookup"><span data-stu-id="89405-169">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="89405-170">Состояние управления устройством.</span><span class="sxs-lookup"><span data-stu-id="89405-170">Management state of the device.</span></span> <span data-ttu-id="89405-171">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-171">This property is read-only.</span></span> <span data-ttu-id="89405-172">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="89405-172">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-173">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="89405-173">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="89405-174">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="89405-174">enrolledDateTime</span></span>|<span data-ttu-id="89405-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89405-175">DateTimeOffset</span></span>|<span data-ttu-id="89405-176">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-176">Enrollment time of the device.</span></span> <span data-ttu-id="89405-177">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-177">This property is read-only.</span></span> <span data-ttu-id="89405-178">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-178">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-179">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="89405-179">lastSyncDateTime</span></span>|<span data-ttu-id="89405-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89405-180">DateTimeOffset</span></span>|<span data-ttu-id="89405-181">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="89405-181">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="89405-182">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-182">This property is read-only.</span></span> <span data-ttu-id="89405-183">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-183">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="89405-184">chassisType</span></span>|[<span data-ttu-id="89405-185">chassisType</span><span class="sxs-lookup"><span data-stu-id="89405-185">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="89405-186">Тип корпусов устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-186">Chassis type of the device.</span></span> <span data-ttu-id="89405-187">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-187">This property is read-only.</span></span> <span data-ttu-id="89405-188">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="89405-188">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-189">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="89405-189">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="89405-190">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="89405-190">operatingSystem</span></span>|<span data-ttu-id="89405-191">String</span><span class="sxs-lookup"><span data-stu-id="89405-191">String</span></span>|<span data-ttu-id="89405-192">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-192">Operating system of the device.</span></span> <span data-ttu-id="89405-193">Windows, iOS и т. д. Это свойство является свойством только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-193">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="89405-194">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-194">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="89405-195">deviceType</span></span>|[<span data-ttu-id="89405-196">deviceType</span><span class="sxs-lookup"><span data-stu-id="89405-196">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="89405-197">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-197">Platform of the device.</span></span> <span data-ttu-id="89405-198">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-198">This property is read-only.</span></span> <span data-ttu-id="89405-199">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="89405-199">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-200">Возможные значения: `desktop` , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` , `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` `cloudPC` .</span><span class="sxs-lookup"><span data-stu-id="89405-200">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="89405-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="89405-201">complianceState</span></span>|[<span data-ttu-id="89405-202">complianceState</span><span class="sxs-lookup"><span data-stu-id="89405-202">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="89405-203">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="89405-203">Compliance state of the device.</span></span> <span data-ttu-id="89405-204">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-204">This property is read-only.</span></span> <span data-ttu-id="89405-205">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="89405-205">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-206">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="89405-206">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="89405-207">jailBroken</span><span class="sxs-lookup"><span data-stu-id="89405-207">jailBroken</span></span>|<span data-ttu-id="89405-208">String</span><span class="sxs-lookup"><span data-stu-id="89405-208">String</span></span>|<span data-ttu-id="89405-209">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="89405-209">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="89405-210">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-210">This property is read-only.</span></span> <span data-ttu-id="89405-211">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-211">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-212">managementAgent</span><span class="sxs-lookup"><span data-stu-id="89405-212">managementAgent</span></span>|[<span data-ttu-id="89405-213">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="89405-213">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="89405-214">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="89405-214">Management channel of the device.</span></span> <span data-ttu-id="89405-215">Intune, EAS и т. д. Это свойство находится только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-215">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="89405-216">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="89405-216">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-217">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="89405-217">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="89405-218">osVersion</span><span class="sxs-lookup"><span data-stu-id="89405-218">osVersion</span></span>|<span data-ttu-id="89405-219">String</span><span class="sxs-lookup"><span data-stu-id="89405-219">String</span></span>|<span data-ttu-id="89405-220">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-220">Operating system version of the device.</span></span> <span data-ttu-id="89405-221">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-221">This property is read-only.</span></span> <span data-ttu-id="89405-222">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-222">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-223">easActivated</span><span class="sxs-lookup"><span data-stu-id="89405-223">easActivated</span></span>|<span data-ttu-id="89405-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="89405-224">Boolean</span></span>|<span data-ttu-id="89405-225">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="89405-225">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="89405-226">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-226">This property is read-only.</span></span> <span data-ttu-id="89405-227">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-227">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="89405-228">easDeviceId</span></span>|<span data-ttu-id="89405-229">String</span><span class="sxs-lookup"><span data-stu-id="89405-229">String</span></span>|<span data-ttu-id="89405-230">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="89405-230">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="89405-231">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-231">This property is read-only.</span></span> <span data-ttu-id="89405-232">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-232">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-233">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="89405-233">easActivationDateTime</span></span>|<span data-ttu-id="89405-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89405-234">DateTimeOffset</span></span>|<span data-ttu-id="89405-235">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="89405-235">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="89405-236">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-236">This property is read-only.</span></span> <span data-ttu-id="89405-237">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-237">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-238">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="89405-238">aadRegistered</span></span>|<span data-ttu-id="89405-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="89405-239">Boolean</span></span>|<span data-ttu-id="89405-240">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="89405-240">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="89405-241">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-241">This property is read-only.</span></span> <span data-ttu-id="89405-242">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-242">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-243">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="89405-243">azureADRegistered</span></span>|<span data-ttu-id="89405-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="89405-244">Boolean</span></span>|<span data-ttu-id="89405-245">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="89405-245">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="89405-246">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-246">This property is read-only.</span></span> <span data-ttu-id="89405-247">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-247">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="89405-248">deviceEnrollmentType</span></span>|[<span data-ttu-id="89405-249">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="89405-249">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="89405-250">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-250">Enrollment type of the device.</span></span> <span data-ttu-id="89405-251">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-251">This property is read-only.</span></span> <span data-ttu-id="89405-252">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="89405-252">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-253">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="89405-253">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="89405-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="89405-254">lostModeState</span></span>|[<span data-ttu-id="89405-255">lostModeState</span><span class="sxs-lookup"><span data-stu-id="89405-255">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="89405-256">Указывает, включен ли режим потери.</span><span class="sxs-lookup"><span data-stu-id="89405-256">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="89405-257">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-257">This property is read-only.</span></span> <span data-ttu-id="89405-258">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="89405-258">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-259">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="89405-259">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="89405-260">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="89405-260">activationLockBypassCode</span></span>|<span data-ttu-id="89405-261">String</span><span class="sxs-lookup"><span data-stu-id="89405-261">String</span></span>|<span data-ttu-id="89405-262">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="89405-262">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="89405-263">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-263">This property is read-only.</span></span> <span data-ttu-id="89405-264">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-264">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-265">emailAddress</span><span class="sxs-lookup"><span data-stu-id="89405-265">emailAddress</span></span>|<span data-ttu-id="89405-266">String</span><span class="sxs-lookup"><span data-stu-id="89405-266">String</span></span>|<span data-ttu-id="89405-267">Электронная почта пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="89405-267">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="89405-268">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-268">This property is read-only.</span></span> <span data-ttu-id="89405-269">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-269">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-270">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="89405-270">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="89405-271">String</span><span class="sxs-lookup"><span data-stu-id="89405-271">String</span></span>|<span data-ttu-id="89405-272">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="89405-272">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="89405-273">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-273">Read only.</span></span> <span data-ttu-id="89405-274">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-274">This property is read-only.</span></span> <span data-ttu-id="89405-275">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-275">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-276">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="89405-276">azureADDeviceId</span></span>|<span data-ttu-id="89405-277">String</span><span class="sxs-lookup"><span data-stu-id="89405-277">String</span></span>|<span data-ttu-id="89405-278">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="89405-278">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="89405-279">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-279">Read only.</span></span> <span data-ttu-id="89405-280">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-280">This property is read-only.</span></span> <span data-ttu-id="89405-281">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-281">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="89405-282">deviceRegistrationState</span></span>|[<span data-ttu-id="89405-283">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="89405-283">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="89405-284">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-284">Device registration state.</span></span> <span data-ttu-id="89405-285">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-285">This property is read-only.</span></span> <span data-ttu-id="89405-286">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="89405-286">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-287">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="89405-287">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="89405-288">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="89405-288">deviceCategoryDisplayName</span></span>|<span data-ttu-id="89405-289">String</span><span class="sxs-lookup"><span data-stu-id="89405-289">String</span></span>|<span data-ttu-id="89405-290">Отображаемая имя категории устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-290">Device category display name.</span></span> <span data-ttu-id="89405-291">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-291">This property is read-only.</span></span> <span data-ttu-id="89405-292">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-292">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-293">isSupervised</span><span class="sxs-lookup"><span data-stu-id="89405-293">isSupervised</span></span>|<span data-ttu-id="89405-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="89405-294">Boolean</span></span>|<span data-ttu-id="89405-295">Состояние устройства под контролем.</span><span class="sxs-lookup"><span data-stu-id="89405-295">Device supervised status.</span></span> <span data-ttu-id="89405-296">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-296">This property is read-only.</span></span> <span data-ttu-id="89405-297">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-297">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-298">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="89405-298">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="89405-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89405-299">DateTimeOffset</span></span>|<span data-ttu-id="89405-300">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="89405-300">Last time the device contacted Exchange.</span></span> <span data-ttu-id="89405-301">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-301">This property is read-only.</span></span> <span data-ttu-id="89405-302">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-302">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="89405-303">exchangeAccessState</span></span>|[<span data-ttu-id="89405-304">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="89405-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="89405-305">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="89405-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="89405-306">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-306">This property is read-only.</span></span> <span data-ttu-id="89405-307">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="89405-307">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-308">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="89405-308">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="89405-309">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="89405-309">exchangeAccessStateReason</span></span>|[<span data-ttu-id="89405-310">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="89405-310">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="89405-311">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="89405-311">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="89405-312">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-312">This property is read-only.</span></span> <span data-ttu-id="89405-313">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="89405-313">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-314">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="89405-314">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="89405-315">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="89405-315">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="89405-316">String</span><span class="sxs-lookup"><span data-stu-id="89405-316">String</span></span>|<span data-ttu-id="89405-317">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="89405-317">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="89405-318">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-318">This property is read-only.</span></span> <span data-ttu-id="89405-319">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-319">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-320">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="89405-320">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="89405-321">String</span><span class="sxs-lookup"><span data-stu-id="89405-321">String</span></span>|<span data-ttu-id="89405-322">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="89405-322">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="89405-323">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-323">This property is read-only.</span></span> <span data-ttu-id="89405-324">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-324">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="89405-325">isEncrypted</span></span>|<span data-ttu-id="89405-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="89405-326">Boolean</span></span>|<span data-ttu-id="89405-327">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-327">Device encryption status.</span></span> <span data-ttu-id="89405-328">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-328">This property is read-only.</span></span> <span data-ttu-id="89405-329">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-329">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-330">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="89405-330">userPrincipalName</span></span>|<span data-ttu-id="89405-331">String</span><span class="sxs-lookup"><span data-stu-id="89405-331">String</span></span>|<span data-ttu-id="89405-332">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-332">Device user principal name.</span></span> <span data-ttu-id="89405-333">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-333">This property is read-only.</span></span> <span data-ttu-id="89405-334">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-334">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-335">model</span><span class="sxs-lookup"><span data-stu-id="89405-335">model</span></span>|<span data-ttu-id="89405-336">String</span><span class="sxs-lookup"><span data-stu-id="89405-336">String</span></span>|<span data-ttu-id="89405-337">Модель устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-337">Model of the device.</span></span> <span data-ttu-id="89405-338">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-338">This property is read-only.</span></span> <span data-ttu-id="89405-339">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-339">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-340">manufacturer</span><span class="sxs-lookup"><span data-stu-id="89405-340">manufacturer</span></span>|<span data-ttu-id="89405-341">String</span><span class="sxs-lookup"><span data-stu-id="89405-341">String</span></span>|<span data-ttu-id="89405-342">Производитель устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-342">Manufacturer of the device.</span></span> <span data-ttu-id="89405-343">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-343">This property is read-only.</span></span> <span data-ttu-id="89405-344">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-344">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-345">imei</span><span class="sxs-lookup"><span data-stu-id="89405-345">imei</span></span>|<span data-ttu-id="89405-346">String</span><span class="sxs-lookup"><span data-stu-id="89405-346">String</span></span>|<span data-ttu-id="89405-347">IMEI.</span><span class="sxs-lookup"><span data-stu-id="89405-347">IMEI.</span></span> <span data-ttu-id="89405-348">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-348">This property is read-only.</span></span> <span data-ttu-id="89405-349">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-349">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-350">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="89405-350">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="89405-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89405-351">DateTimeOffset</span></span>|<span data-ttu-id="89405-352">Дата и время истечения льготного периода соответствия устройств требованиям.</span><span class="sxs-lookup"><span data-stu-id="89405-352">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="89405-353">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-353">This property is read-only.</span></span> <span data-ttu-id="89405-354">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-354">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-355">serialNumber</span><span class="sxs-lookup"><span data-stu-id="89405-355">serialNumber</span></span>|<span data-ttu-id="89405-356">String</span><span class="sxs-lookup"><span data-stu-id="89405-356">String</span></span>|<span data-ttu-id="89405-357">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="89405-357">SerialNumber.</span></span> <span data-ttu-id="89405-358">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-358">This property is read-only.</span></span> <span data-ttu-id="89405-359">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-359">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-360">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="89405-360">phoneNumber</span></span>|<span data-ttu-id="89405-361">String</span><span class="sxs-lookup"><span data-stu-id="89405-361">String</span></span>|<span data-ttu-id="89405-362">Номер телефона устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-362">Phone number of the device.</span></span> <span data-ttu-id="89405-363">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-363">This property is read-only.</span></span> <span data-ttu-id="89405-364">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-364">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-365">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="89405-365">androidSecurityPatchLevel</span></span>|<span data-ttu-id="89405-366">String</span><span class="sxs-lookup"><span data-stu-id="89405-366">String</span></span>|<span data-ttu-id="89405-367">Уровень исправлений для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="89405-367">Android security patch level.</span></span> <span data-ttu-id="89405-368">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-368">This property is read-only.</span></span> <span data-ttu-id="89405-369">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-369">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-370">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="89405-370">userDisplayName</span></span>|<span data-ttu-id="89405-371">String</span><span class="sxs-lookup"><span data-stu-id="89405-371">String</span></span>|<span data-ttu-id="89405-372">Отображаемая имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="89405-372">User display name.</span></span> <span data-ttu-id="89405-373">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-373">This property is read-only.</span></span> <span data-ttu-id="89405-374">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-374">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="89405-375">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="89405-376">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="89405-376">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="89405-377">Функции, включенные клиентом ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="89405-377">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="89405-378">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-378">This property is read-only.</span></span> <span data-ttu-id="89405-379">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-379">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-380">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="89405-380">wiFiMacAddress</span></span>|<span data-ttu-id="89405-381">String</span><span class="sxs-lookup"><span data-stu-id="89405-381">String</span></span>|<span data-ttu-id="89405-382">Wi-Fi MAC.</span><span class="sxs-lookup"><span data-stu-id="89405-382">Wi-Fi MAC.</span></span> <span data-ttu-id="89405-383">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-383">This property is read-only.</span></span> <span data-ttu-id="89405-384">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-384">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="89405-385">deviceHealthAttestationState</span></span>|[<span data-ttu-id="89405-386">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="89405-386">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="89405-387">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-387">The device health attestation state.</span></span> <span data-ttu-id="89405-388">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-388">This property is read-only.</span></span> <span data-ttu-id="89405-389">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-389">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-390">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="89405-390">subscriberCarrier</span></span>|<span data-ttu-id="89405-391">String</span><span class="sxs-lookup"><span data-stu-id="89405-391">String</span></span>|<span data-ttu-id="89405-392">Оператор абонента.</span><span class="sxs-lookup"><span data-stu-id="89405-392">Subscriber Carrier.</span></span> <span data-ttu-id="89405-393">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-393">This property is read-only.</span></span> <span data-ttu-id="89405-394">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-394">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-395">meid</span><span class="sxs-lookup"><span data-stu-id="89405-395">meid</span></span>|<span data-ttu-id="89405-396">String</span><span class="sxs-lookup"><span data-stu-id="89405-396">String</span></span>|<span data-ttu-id="89405-397">MEID.</span><span class="sxs-lookup"><span data-stu-id="89405-397">MEID.</span></span> <span data-ttu-id="89405-398">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-398">This property is read-only.</span></span> <span data-ttu-id="89405-399">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-399">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-400">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="89405-400">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="89405-401">Int64</span><span class="sxs-lookup"><span data-stu-id="89405-401">Int64</span></span>|<span data-ttu-id="89405-402">Общее хранилище в bytes.</span><span class="sxs-lookup"><span data-stu-id="89405-402">Total Storage in Bytes.</span></span> <span data-ttu-id="89405-403">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-403">This property is read-only.</span></span> <span data-ttu-id="89405-404">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-404">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-405">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="89405-405">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="89405-406">Int64</span><span class="sxs-lookup"><span data-stu-id="89405-406">Int64</span></span>|<span data-ttu-id="89405-407">Бесплатное хранилище в вайтах.</span><span class="sxs-lookup"><span data-stu-id="89405-407">Free Storage in Bytes.</span></span> <span data-ttu-id="89405-408">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-408">This property is read-only.</span></span> <span data-ttu-id="89405-409">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-409">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-410">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="89405-410">managedDeviceName</span></span>|<span data-ttu-id="89405-411">String</span><span class="sxs-lookup"><span data-stu-id="89405-411">String</span></span>|<span data-ttu-id="89405-412">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-412">Automatically generated name to identify a device.</span></span> <span data-ttu-id="89405-413">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="89405-413">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="89405-414">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-414">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-415">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="89405-415">partnerReportedThreatState</span></span>|[<span data-ttu-id="89405-416">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="89405-416">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="89405-417">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="89405-417">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="89405-418">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-418">Read Only.</span></span> <span data-ttu-id="89405-419">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-419">This property is read-only.</span></span> <span data-ttu-id="89405-420">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="89405-420">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-421">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="89405-421">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="89405-422">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="89405-422">retireAfterDateTime</span></span>|<span data-ttu-id="89405-423">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89405-423">DateTimeOffset</span></span>|<span data-ttu-id="89405-424">Указывает время после автоматического выхода устройства из-за запланированного действия.</span><span class="sxs-lookup"><span data-stu-id="89405-424">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="89405-425">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-425">This property is read-only.</span></span> <span data-ttu-id="89405-426">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-426">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-427">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="89405-427">usersLoggedOn</span></span>|<span data-ttu-id="89405-428">[коллекция loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="89405-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="89405-429">Указывает последнего во время входа пользователей устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-429">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="89405-430">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-430">This property is read-only.</span></span> <span data-ttu-id="89405-431">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-431">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-432">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="89405-432">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="89405-433">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89405-433">DateTimeOffset</span></span>|<span data-ttu-id="89405-434">Сообщает dateTime, задав параметр preferMdmOverGroupPolicy.</span><span class="sxs-lookup"><span data-stu-id="89405-434">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="89405-435">Если этот параметр задан, параметры MDM Intune переопредят параметры групповой политики в случае конфликта.</span><span class="sxs-lookup"><span data-stu-id="89405-435">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="89405-436">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-436">Read Only.</span></span> <span data-ttu-id="89405-437">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-437">This property is read-only.</span></span> <span data-ttu-id="89405-438">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-438">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-439">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="89405-439">autopilotEnrolled</span></span>|<span data-ttu-id="89405-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="89405-440">Boolean</span></span>|<span data-ttu-id="89405-441">Сообщает, зарегистрировать ли управляемое устройство с помощью автоматического пилотного проекта.</span><span class="sxs-lookup"><span data-stu-id="89405-441">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="89405-442">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-442">This property is read-only.</span></span> <span data-ttu-id="89405-443">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-443">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-444">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="89405-444">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="89405-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="89405-445">Boolean</span></span>|<span data-ttu-id="89405-446">Сообщает, является ли управляемое устройство iOS зарегистрированным пользователем.</span><span class="sxs-lookup"><span data-stu-id="89405-446">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="89405-447">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-447">This property is read-only.</span></span> <span data-ttu-id="89405-448">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-448">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-449">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="89405-449">managementCertificateExpirationDate</span></span>|<span data-ttu-id="89405-450">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89405-450">DateTimeOffset</span></span>|<span data-ttu-id="89405-451">Сообщает дату окончания срока действия сертификата управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="89405-451">Reports device management certificate expiration date.</span></span> <span data-ttu-id="89405-452">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-452">This property is read-only.</span></span> <span data-ttu-id="89405-453">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-453">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-454">iccid</span><span class="sxs-lookup"><span data-stu-id="89405-454">iccid</span></span>|<span data-ttu-id="89405-455">String</span><span class="sxs-lookup"><span data-stu-id="89405-455">String</span></span>|<span data-ttu-id="89405-456">Интегрированный идентификатор схемной карты — это уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="89405-456">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="89405-457">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-457">This property is read-only.</span></span> <span data-ttu-id="89405-458">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-458">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-459">udid</span><span class="sxs-lookup"><span data-stu-id="89405-459">udid</span></span>|<span data-ttu-id="89405-460">String</span><span class="sxs-lookup"><span data-stu-id="89405-460">String</span></span>|<span data-ttu-id="89405-461">Уникальный идентификатор устройства для устройств с iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="89405-461">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="89405-462">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-462">This property is read-only.</span></span> <span data-ttu-id="89405-463">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-463">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-464">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="89405-464">roleScopeTagIds</span></span>|<span data-ttu-id="89405-465">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="89405-465">String collection</span></span>|<span data-ttu-id="89405-466">Список ИД тегов области для этого экземпляра устройства.</span><span class="sxs-lookup"><span data-stu-id="89405-466">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="89405-467">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-467">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-468">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="89405-468">windowsActiveMalwareCount</span></span>|<span data-ttu-id="89405-469">Int32</span><span class="sxs-lookup"><span data-stu-id="89405-469">Int32</span></span>|<span data-ttu-id="89405-470">Количество активных вредоносных программ для этого устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="89405-470">Count of active malware for this windows device.</span></span> <span data-ttu-id="89405-471">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-471">This property is read-only.</span></span> <span data-ttu-id="89405-472">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-472">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-473">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="89405-473">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="89405-474">Int32</span><span class="sxs-lookup"><span data-stu-id="89405-474">Int32</span></span>|<span data-ttu-id="89405-475">Количество исправленных вредоносных программ для этого устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="89405-475">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="89405-476">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-476">This property is read-only.</span></span> <span data-ttu-id="89405-477">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-477">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-478">notes</span><span class="sxs-lookup"><span data-stu-id="89405-478">notes</span></span>|<span data-ttu-id="89405-479">String</span><span class="sxs-lookup"><span data-stu-id="89405-479">String</span></span>|<span data-ttu-id="89405-480">Примечания на устройстве, созданном ИТ-администратором. [Наследуется от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-480">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="89405-481">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="89405-482">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="89405-482">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="89405-483">Состояние состояния клиента Configuration Manager, действительное только для устройств, управляемых агентом MDM/ConfigMgr. Наследуется от [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-483">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="89405-484">configurationManagerClientInformation</span></span>|[<span data-ttu-id="89405-485">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="89405-485">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="89405-486">Сведения о клиенте configuration manager, действительные только для устройств, управляемых, управляемых duel или триуправленных агентом ConfigMgr. Наследуется от [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-486">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-487">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="89405-487">ethernetMacAddress</span></span>|<span data-ttu-id="89405-488">String</span><span class="sxs-lookup"><span data-stu-id="89405-488">String</span></span>|<span data-ttu-id="89405-489">Ethernet MAC.</span><span class="sxs-lookup"><span data-stu-id="89405-489">Ethernet MAC.</span></span> <span data-ttu-id="89405-490">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-490">This property is read-only.</span></span> <span data-ttu-id="89405-491">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-491">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-492">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="89405-492">physicalMemoryInBytes</span></span>|<span data-ttu-id="89405-493">Int64</span><span class="sxs-lookup"><span data-stu-id="89405-493">Int64</span></span>|<span data-ttu-id="89405-494">Общий объем памяти в ветвях.</span><span class="sxs-lookup"><span data-stu-id="89405-494">Total Memory in Bytes.</span></span> <span data-ttu-id="89405-495">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-495">This property is read-only.</span></span> <span data-ttu-id="89405-496">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-496">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-497">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="89405-497">processorArchitecture</span></span>|[<span data-ttu-id="89405-498">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="89405-498">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="89405-499">Архитектура процессора.</span><span class="sxs-lookup"><span data-stu-id="89405-499">Processor architecture.</span></span> <span data-ttu-id="89405-500">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-500">This property is read-only.</span></span> <span data-ttu-id="89405-501">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="89405-501">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-502">Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="89405-502">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="89405-503">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="89405-503">specificationVersion</span></span>|<span data-ttu-id="89405-504">String</span><span class="sxs-lookup"><span data-stu-id="89405-504">String</span></span>|<span data-ttu-id="89405-505">Версия спецификации.</span><span class="sxs-lookup"><span data-stu-id="89405-505">Specification version.</span></span> <span data-ttu-id="89405-506">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-506">This property is read-only.</span></span> <span data-ttu-id="89405-507">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-507">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-508">joinType</span><span class="sxs-lookup"><span data-stu-id="89405-508">joinType</span></span>|[<span data-ttu-id="89405-509">joinType</span><span class="sxs-lookup"><span data-stu-id="89405-509">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="89405-510">Тип следования устройства [Наследуется от managedDevice.](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-510">Device join type Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-511">Возможные значения: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span><span class="sxs-lookup"><span data-stu-id="89405-511">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="89405-512">skuFamily</span><span class="sxs-lookup"><span data-stu-id="89405-512">skuFamily</span></span>|<span data-ttu-id="89405-513">String</span><span class="sxs-lookup"><span data-stu-id="89405-513">String</span></span>|<span data-ttu-id="89405-514">Семейство SKU устройства Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-514">Device sku family Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-515">skuNumber</span><span class="sxs-lookup"><span data-stu-id="89405-515">skuNumber</span></span>|<span data-ttu-id="89405-516">Int32</span><span class="sxs-lookup"><span data-stu-id="89405-516">Int32</span></span>|<span data-ttu-id="89405-517">Номер SKU устройства, см. также: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo .</span><span class="sxs-lookup"><span data-stu-id="89405-517">Device sku number, see also: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo.</span></span> <span data-ttu-id="89405-518">Допустимые значения: от 0 до 2 147 483 647.</span><span class="sxs-lookup"><span data-stu-id="89405-518">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="89405-519">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89405-519">This property is read-only.</span></span> <span data-ttu-id="89405-520">Наследуется [от managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-520">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="89405-521">managementFeatures</span><span class="sxs-lookup"><span data-stu-id="89405-521">managementFeatures</span></span>|[<span data-ttu-id="89405-522">managedDeviceManagementFeatures</span><span class="sxs-lookup"><span data-stu-id="89405-522">managedDeviceManagementFeatures</span></span>](../resources/intune-devices-manageddevicemanagementfeatures.md)|<span data-ttu-id="89405-523">Функции управления устройствами. [Наследуется от managedDevice.](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="89405-523">Device management features Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="89405-524">Возможные значения: `none`, `microsoftManagedDesktop`.</span><span class="sxs-lookup"><span data-stu-id="89405-524">Possible values are: `none`, `microsoftManagedDesktop`.</span></span>|



## <a name="response"></a><span data-ttu-id="89405-525">Отклик</span><span class="sxs-lookup"><span data-stu-id="89405-525">Response</span></span>
<span data-ttu-id="89405-526">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89405-526">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89405-527">Пример</span><span class="sxs-lookup"><span data-stu-id="89405-527">Example</span></span>

### <a name="request"></a><span data-ttu-id="89405-528">Запрос</span><span class="sxs-lookup"><span data-stu-id="89405-528">Request</span></span>
<span data-ttu-id="89405-529">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89405-529">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 8115

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
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

### <a name="response"></a><span data-ttu-id="89405-530">Отклик</span><span class="sxs-lookup"><span data-stu-id="89405-530">Response</span></span>
<span data-ttu-id="89405-p175">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89405-p175">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8164

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "id": "97842b67-2b67-9784-672b-8497672b8497",
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




