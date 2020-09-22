---
title: Обновление Виндовсманажеддевице
description: Обновление свойств объекта Виндовсманажеддевице.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 48176886db9e306d2165497539a1f5a00695abb7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972303"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="ef88a-103">Обновление Виндовсманажеддевице</span><span class="sxs-lookup"><span data-stu-id="ef88a-103">Update windowsManagedDevice</span></span>

<span data-ttu-id="ef88a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef88a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef88a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef88a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef88a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef88a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef88a-107">Обновление свойств объекта [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="ef88a-107">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef88a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ef88a-108">Prerequisites</span></span>
<span data-ttu-id="ef88a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef88a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef88a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef88a-111">Permission type</span></span>|<span data-ttu-id="ef88a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef88a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef88a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef88a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef88a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef88a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ef88a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef88a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef88a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef88a-116">Not supported.</span></span>|
|<span data-ttu-id="ef88a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef88a-117">Application</span></span>|<span data-ttu-id="ef88a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef88a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef88a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef88a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="ef88a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ef88a-120">Request headers</span></span>
|<span data-ttu-id="ef88a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef88a-121">Header</span></span>|<span data-ttu-id="ef88a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ef88a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef88a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef88a-123">Authorization</span></span>|<span data-ttu-id="ef88a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef88a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef88a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef88a-125">Accept</span></span>|<span data-ttu-id="ef88a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef88a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef88a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef88a-127">Request body</span></span>
<span data-ttu-id="ef88a-128">В тексте запроса добавьте представление объекта [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef88a-128">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="ef88a-129">В следующей таблице приведены свойства, необходимые при создании [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-129">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="ef88a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef88a-130">Property</span></span>|<span data-ttu-id="ef88a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ef88a-131">Type</span></span>|<span data-ttu-id="ef88a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ef88a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef88a-133">id</span><span class="sxs-lookup"><span data-stu-id="ef88a-133">id</span></span>|<span data-ttu-id="ef88a-134">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-134">String</span></span>|<span data-ttu-id="ef88a-135">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-135">Unique Identifier for the device.</span></span> <span data-ttu-id="ef88a-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-136">This property is read-only.</span></span> <span data-ttu-id="ef88a-137">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-137">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-138">userId</span><span class="sxs-lookup"><span data-stu-id="ef88a-138">userId</span></span>|<span data-ttu-id="ef88a-139">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-139">String</span></span>|<span data-ttu-id="ef88a-140">Уникальный идентификатор пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="ef88a-140">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="ef88a-141">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-141">This property is read-only.</span></span> <span data-ttu-id="ef88a-142">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-142">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="ef88a-143">deviceName</span></span>|<span data-ttu-id="ef88a-144">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-144">String</span></span>|<span data-ttu-id="ef88a-145">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-145">Name of the device.</span></span> <span data-ttu-id="ef88a-146">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-146">This property is read-only.</span></span> <span data-ttu-id="ef88a-147">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-147">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-148">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="ef88a-148">hardwareInformation</span></span>|[<span data-ttu-id="ef88a-149">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="ef88a-149">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="ef88a-150">Сведения о хардвард для устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-150">The hardward details for the device.</span></span>  <span data-ttu-id="ef88a-151">Включает такие сведения, как место хранения, производитель, серийный номер и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-151">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="ef88a-152">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-152">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="ef88a-153">ownerType</span></span>|[<span data-ttu-id="ef88a-154">ownerType</span><span class="sxs-lookup"><span data-stu-id="ef88a-154">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="ef88a-155">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="ef88a-155">Ownership of the device.</span></span> <span data-ttu-id="ef88a-156">Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-156">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-157">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="ef88a-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ef88a-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ef88a-158">managedDeviceOwnerType</span></span>|[<span data-ttu-id="ef88a-159">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ef88a-159">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="ef88a-160">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="ef88a-160">Ownership of the device.</span></span> <span data-ttu-id="ef88a-161">Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-161">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-162">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="ef88a-162">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ef88a-163">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="ef88a-163">deviceActionResults</span></span>|<span data-ttu-id="ef88a-164">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="ef88a-165">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="ef88a-165">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="ef88a-166">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-166">This property is read-only.</span></span> <span data-ttu-id="ef88a-167">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-168">манажементстате</span><span class="sxs-lookup"><span data-stu-id="ef88a-168">managementState</span></span>|[<span data-ttu-id="ef88a-169">манажементстате</span><span class="sxs-lookup"><span data-stu-id="ef88a-169">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="ef88a-170">Состояние управления для устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-170">Management state of the device.</span></span> <span data-ttu-id="ef88a-171">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-171">This property is read-only.</span></span> <span data-ttu-id="ef88a-172">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-173">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="ef88a-173">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="ef88a-174">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="ef88a-174">enrolledDateTime</span></span>|<span data-ttu-id="ef88a-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef88a-175">DateTimeOffset</span></span>|<span data-ttu-id="ef88a-176">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-176">Enrollment time of the device.</span></span> <span data-ttu-id="ef88a-177">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-177">This property is read-only.</span></span> <span data-ttu-id="ef88a-178">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-178">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-179">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ef88a-179">lastSyncDateTime</span></span>|<span data-ttu-id="ef88a-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef88a-180">DateTimeOffset</span></span>|<span data-ttu-id="ef88a-181">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="ef88a-181">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="ef88a-182">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-182">This property is read-only.</span></span> <span data-ttu-id="ef88a-183">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-183">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-184">чассистипе</span><span class="sxs-lookup"><span data-stu-id="ef88a-184">chassisType</span></span>|[<span data-ttu-id="ef88a-185">чассистипе</span><span class="sxs-lookup"><span data-stu-id="ef88a-185">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="ef88a-186">Тип корпуса устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-186">Chassis type of the device.</span></span> <span data-ttu-id="ef88a-187">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-187">This property is read-only.</span></span> <span data-ttu-id="ef88a-188">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-188">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-189">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="ef88a-189">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="ef88a-190">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="ef88a-190">operatingSystem</span></span>|<span data-ttu-id="ef88a-191">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-191">String</span></span>|<span data-ttu-id="ef88a-192">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-192">Operating system of the device.</span></span> <span data-ttu-id="ef88a-193">Windows, iOS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-193">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="ef88a-194">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="ef88a-195">deviceType</span></span>|[<span data-ttu-id="ef88a-196">deviceType</span><span class="sxs-lookup"><span data-stu-id="ef88a-196">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="ef88a-197">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-197">Platform of the device.</span></span> <span data-ttu-id="ef88a-198">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-198">This property is read-only.</span></span> <span data-ttu-id="ef88a-199">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-199">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-200">Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` ,,, `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` ,, `unknown` ,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="ef88a-200">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="ef88a-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="ef88a-201">complianceState</span></span>|[<span data-ttu-id="ef88a-202">complianceState</span><span class="sxs-lookup"><span data-stu-id="ef88a-202">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="ef88a-203">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="ef88a-203">Compliance state of the device.</span></span> <span data-ttu-id="ef88a-204">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-204">This property is read-only.</span></span> <span data-ttu-id="ef88a-205">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-205">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-206">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="ef88a-206">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="ef88a-207">jailBroken</span><span class="sxs-lookup"><span data-stu-id="ef88a-207">jailBroken</span></span>|<span data-ttu-id="ef88a-208">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-208">String</span></span>|<span data-ttu-id="ef88a-209">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="ef88a-209">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="ef88a-210">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-210">This property is read-only.</span></span> <span data-ttu-id="ef88a-211">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-212">managementAgent</span><span class="sxs-lookup"><span data-stu-id="ef88a-212">managementAgent</span></span>|[<span data-ttu-id="ef88a-213">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="ef88a-213">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="ef88a-214">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="ef88a-214">Management channel of the device.</span></span> <span data-ttu-id="ef88a-215">Intune, EAS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-215">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="ef88a-216">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-217">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="ef88a-217">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="ef88a-218">osVersion</span><span class="sxs-lookup"><span data-stu-id="ef88a-218">osVersion</span></span>|<span data-ttu-id="ef88a-219">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-219">String</span></span>|<span data-ttu-id="ef88a-220">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-220">Operating system version of the device.</span></span> <span data-ttu-id="ef88a-221">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-221">This property is read-only.</span></span> <span data-ttu-id="ef88a-222">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-222">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-223">easActivated</span><span class="sxs-lookup"><span data-stu-id="ef88a-223">easActivated</span></span>|<span data-ttu-id="ef88a-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef88a-224">Boolean</span></span>|<span data-ttu-id="ef88a-225">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="ef88a-225">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="ef88a-226">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-226">This property is read-only.</span></span> <span data-ttu-id="ef88a-227">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="ef88a-228">easDeviceId</span></span>|<span data-ttu-id="ef88a-229">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-229">String</span></span>|<span data-ttu-id="ef88a-230">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="ef88a-230">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="ef88a-231">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-231">This property is read-only.</span></span> <span data-ttu-id="ef88a-232">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-232">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-233">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="ef88a-233">easActivationDateTime</span></span>|<span data-ttu-id="ef88a-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef88a-234">DateTimeOffset</span></span>|<span data-ttu-id="ef88a-235">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="ef88a-235">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="ef88a-236">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-236">This property is read-only.</span></span> <span data-ttu-id="ef88a-237">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-238">аадрегистеред</span><span class="sxs-lookup"><span data-stu-id="ef88a-238">aadRegistered</span></span>|<span data-ttu-id="ef88a-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef88a-239">Boolean</span></span>|<span data-ttu-id="ef88a-240">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ef88a-240">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="ef88a-241">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-241">This property is read-only.</span></span> <span data-ttu-id="ef88a-242">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-242">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-243">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="ef88a-243">azureADRegistered</span></span>|<span data-ttu-id="ef88a-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef88a-244">Boolean</span></span>|<span data-ttu-id="ef88a-245">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ef88a-245">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="ef88a-246">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-246">This property is read-only.</span></span> <span data-ttu-id="ef88a-247">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-247">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ef88a-248">deviceEnrollmentType</span></span>|[<span data-ttu-id="ef88a-249">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ef88a-249">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="ef88a-250">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-250">Enrollment type of the device.</span></span> <span data-ttu-id="ef88a-251">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-251">This property is read-only.</span></span> <span data-ttu-id="ef88a-252">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-252">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-253">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="ef88a-253">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="ef88a-254">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="ef88a-254">lostModeState</span></span>|[<span data-ttu-id="ef88a-255">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="ef88a-255">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="ef88a-256">Указывает, включен ли режим потерянных или отключенных.</span><span class="sxs-lookup"><span data-stu-id="ef88a-256">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="ef88a-257">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-257">This property is read-only.</span></span> <span data-ttu-id="ef88a-258">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-258">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-259">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="ef88a-259">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="ef88a-260">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="ef88a-260">activationLockBypassCode</span></span>|<span data-ttu-id="ef88a-261">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-261">String</span></span>|<span data-ttu-id="ef88a-262">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="ef88a-262">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="ef88a-263">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-263">This property is read-only.</span></span> <span data-ttu-id="ef88a-264">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-265">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ef88a-265">emailAddress</span></span>|<span data-ttu-id="ef88a-266">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-266">String</span></span>|<span data-ttu-id="ef88a-267">Сообщения электронной почты пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="ef88a-267">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="ef88a-268">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-268">This property is read-only.</span></span> <span data-ttu-id="ef88a-269">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-270">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="ef88a-270">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="ef88a-271">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-271">String</span></span>|<span data-ttu-id="ef88a-272">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ef88a-272">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="ef88a-273">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-273">Read only.</span></span> <span data-ttu-id="ef88a-274">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-274">This property is read-only.</span></span> <span data-ttu-id="ef88a-275">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-275">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-276">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="ef88a-276">azureADDeviceId</span></span>|<span data-ttu-id="ef88a-277">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-277">String</span></span>|<span data-ttu-id="ef88a-278">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ef88a-278">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="ef88a-279">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-279">Read only.</span></span> <span data-ttu-id="ef88a-280">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-280">This property is read-only.</span></span> <span data-ttu-id="ef88a-281">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-281">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ef88a-282">deviceRegistrationState</span></span>|[<span data-ttu-id="ef88a-283">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ef88a-283">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="ef88a-284">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-284">Device registration state.</span></span> <span data-ttu-id="ef88a-285">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-285">This property is read-only.</span></span> <span data-ttu-id="ef88a-286">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-286">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-287">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ef88a-287">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="ef88a-288">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="ef88a-288">deviceCategoryDisplayName</span></span>|<span data-ttu-id="ef88a-289">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-289">String</span></span>|<span data-ttu-id="ef88a-290">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="ef88a-290">Device category display name.</span></span> <span data-ttu-id="ef88a-291">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-291">This property is read-only.</span></span> <span data-ttu-id="ef88a-292">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-292">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-293">isSupervised</span><span class="sxs-lookup"><span data-stu-id="ef88a-293">isSupervised</span></span>|<span data-ttu-id="ef88a-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef88a-294">Boolean</span></span>|<span data-ttu-id="ef88a-295">Состояние контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-295">Device supervised status.</span></span> <span data-ttu-id="ef88a-296">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-296">This property is read-only.</span></span> <span data-ttu-id="ef88a-297">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-297">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-298">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ef88a-298">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="ef88a-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef88a-299">DateTimeOffset</span></span>|<span data-ttu-id="ef88a-300">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="ef88a-300">Last time the device contacted Exchange.</span></span> <span data-ttu-id="ef88a-301">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-301">This property is read-only.</span></span> <span data-ttu-id="ef88a-302">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-302">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="ef88a-303">exchangeAccessState</span></span>|[<span data-ttu-id="ef88a-304">девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="ef88a-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="ef88a-305">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="ef88a-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="ef88a-306">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-306">This property is read-only.</span></span> <span data-ttu-id="ef88a-307">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-307">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-308">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="ef88a-308">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="ef88a-309">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="ef88a-309">exchangeAccessStateReason</span></span>|[<span data-ttu-id="ef88a-310">девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="ef88a-310">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="ef88a-311">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="ef88a-311">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="ef88a-312">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-312">This property is read-only.</span></span> <span data-ttu-id="ef88a-313">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-313">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-314">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="ef88a-314">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="ef88a-315">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="ef88a-315">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="ef88a-316">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-316">String</span></span>|<span data-ttu-id="ef88a-317">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="ef88a-317">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="ef88a-318">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-318">This property is read-only.</span></span> <span data-ttu-id="ef88a-319">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-319">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-320">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ef88a-320">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="ef88a-321">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-321">String</span></span>|<span data-ttu-id="ef88a-322">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="ef88a-322">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="ef88a-323">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-323">This property is read-only.</span></span> <span data-ttu-id="ef88a-324">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-324">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="ef88a-325">isEncrypted</span></span>|<span data-ttu-id="ef88a-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef88a-326">Boolean</span></span>|<span data-ttu-id="ef88a-327">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-327">Device encryption status.</span></span> <span data-ttu-id="ef88a-328">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-328">This property is read-only.</span></span> <span data-ttu-id="ef88a-329">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-329">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-330">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ef88a-330">userPrincipalName</span></span>|<span data-ttu-id="ef88a-331">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-331">String</span></span>|<span data-ttu-id="ef88a-332">Имя участника пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-332">Device user principal name.</span></span> <span data-ttu-id="ef88a-333">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-333">This property is read-only.</span></span> <span data-ttu-id="ef88a-334">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-334">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-335">model</span><span class="sxs-lookup"><span data-stu-id="ef88a-335">model</span></span>|<span data-ttu-id="ef88a-336">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-336">String</span></span>|<span data-ttu-id="ef88a-337">Модель устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-337">Model of the device.</span></span> <span data-ttu-id="ef88a-338">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-338">This property is read-only.</span></span> <span data-ttu-id="ef88a-339">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-340">manufacturer</span><span class="sxs-lookup"><span data-stu-id="ef88a-340">manufacturer</span></span>|<span data-ttu-id="ef88a-341">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-341">String</span></span>|<span data-ttu-id="ef88a-342">Производитель устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-342">Manufacturer of the device.</span></span> <span data-ttu-id="ef88a-343">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-343">This property is read-only.</span></span> <span data-ttu-id="ef88a-344">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-345">imei</span><span class="sxs-lookup"><span data-stu-id="ef88a-345">imei</span></span>|<span data-ttu-id="ef88a-346">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-346">String</span></span>|<span data-ttu-id="ef88a-347">IMEI.</span><span class="sxs-lookup"><span data-stu-id="ef88a-347">IMEI.</span></span> <span data-ttu-id="ef88a-348">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-348">This property is read-only.</span></span> <span data-ttu-id="ef88a-349">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-349">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-350">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ef88a-350">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ef88a-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef88a-351">DateTimeOffset</span></span>|<span data-ttu-id="ef88a-352">Дата и время истечения льготного периода соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="ef88a-352">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="ef88a-353">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-353">This property is read-only.</span></span> <span data-ttu-id="ef88a-354">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-355">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ef88a-355">serialNumber</span></span>|<span data-ttu-id="ef88a-356">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-356">String</span></span>|<span data-ttu-id="ef88a-357">Серийный.</span><span class="sxs-lookup"><span data-stu-id="ef88a-357">SerialNumber.</span></span> <span data-ttu-id="ef88a-358">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-358">This property is read-only.</span></span> <span data-ttu-id="ef88a-359">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-360">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="ef88a-360">phoneNumber</span></span>|<span data-ttu-id="ef88a-361">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-361">String</span></span>|<span data-ttu-id="ef88a-362">Номер телефона устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-362">Phone number of the device.</span></span> <span data-ttu-id="ef88a-363">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-363">This property is read-only.</span></span> <span data-ttu-id="ef88a-364">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-364">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-365">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="ef88a-365">androidSecurityPatchLevel</span></span>|<span data-ttu-id="ef88a-366">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-366">String</span></span>|<span data-ttu-id="ef88a-367">Уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="ef88a-367">Android security patch level.</span></span> <span data-ttu-id="ef88a-368">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-368">This property is read-only.</span></span> <span data-ttu-id="ef88a-369">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-370">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ef88a-370">userDisplayName</span></span>|<span data-ttu-id="ef88a-371">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-371">String</span></span>|<span data-ttu-id="ef88a-372">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="ef88a-372">User display name.</span></span> <span data-ttu-id="ef88a-373">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-373">This property is read-only.</span></span> <span data-ttu-id="ef88a-374">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="ef88a-375">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="ef88a-376">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="ef88a-376">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="ef88a-377">Функции, поддерживающие клиент Конфигрмгр.</span><span class="sxs-lookup"><span data-stu-id="ef88a-377">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="ef88a-378">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-378">This property is read-only.</span></span> <span data-ttu-id="ef88a-379">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-379">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-380">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="ef88a-380">wiFiMacAddress</span></span>|<span data-ttu-id="ef88a-381">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-381">String</span></span>|<span data-ttu-id="ef88a-382">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="ef88a-382">Wi-Fi MAC.</span></span> <span data-ttu-id="ef88a-383">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-383">This property is read-only.</span></span> <span data-ttu-id="ef88a-384">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-384">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="ef88a-385">deviceHealthAttestationState</span></span>|[<span data-ttu-id="ef88a-386">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="ef88a-386">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="ef88a-387">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-387">The device health attestation state.</span></span> <span data-ttu-id="ef88a-388">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-388">This property is read-only.</span></span> <span data-ttu-id="ef88a-389">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-389">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-390">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="ef88a-390">subscriberCarrier</span></span>|<span data-ttu-id="ef88a-391">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-391">String</span></span>|<span data-ttu-id="ef88a-392">Перевозчик абонента.</span><span class="sxs-lookup"><span data-stu-id="ef88a-392">Subscriber Carrier.</span></span> <span data-ttu-id="ef88a-393">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-393">This property is read-only.</span></span> <span data-ttu-id="ef88a-394">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-394">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-395">meid</span><span class="sxs-lookup"><span data-stu-id="ef88a-395">meid</span></span>|<span data-ttu-id="ef88a-396">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-396">String</span></span>|<span data-ttu-id="ef88a-397">MEID.</span><span class="sxs-lookup"><span data-stu-id="ef88a-397">MEID.</span></span> <span data-ttu-id="ef88a-398">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-398">This property is read-only.</span></span> <span data-ttu-id="ef88a-399">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-399">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-400">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="ef88a-400">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="ef88a-401">Int64</span><span class="sxs-lookup"><span data-stu-id="ef88a-401">Int64</span></span>|<span data-ttu-id="ef88a-402">Общий объем хранилища в байтах.</span><span class="sxs-lookup"><span data-stu-id="ef88a-402">Total Storage in Bytes.</span></span> <span data-ttu-id="ef88a-403">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-403">This property is read-only.</span></span> <span data-ttu-id="ef88a-404">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-404">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-405">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="ef88a-405">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="ef88a-406">Int64</span><span class="sxs-lookup"><span data-stu-id="ef88a-406">Int64</span></span>|<span data-ttu-id="ef88a-407">Свободное хранилище в байтах.</span><span class="sxs-lookup"><span data-stu-id="ef88a-407">Free Storage in Bytes.</span></span> <span data-ttu-id="ef88a-408">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-408">This property is read-only.</span></span> <span data-ttu-id="ef88a-409">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-409">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-410">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="ef88a-410">managedDeviceName</span></span>|<span data-ttu-id="ef88a-411">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-411">String</span></span>|<span data-ttu-id="ef88a-412">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-412">Automatically generated name to identify a device.</span></span> <span data-ttu-id="ef88a-413">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="ef88a-413">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="ef88a-414">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-414">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-415">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="ef88a-415">partnerReportedThreatState</span></span>|[<span data-ttu-id="ef88a-416">манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="ef88a-416">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="ef88a-417">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="ef88a-417">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="ef88a-418">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-418">Read Only.</span></span> <span data-ttu-id="ef88a-419">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-419">This property is read-only.</span></span> <span data-ttu-id="ef88a-420">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-420">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-421">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="ef88a-421">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="ef88a-422">ретиреафтердатетиме</span><span class="sxs-lookup"><span data-stu-id="ef88a-422">retireAfterDateTime</span></span>|<span data-ttu-id="ef88a-423">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef88a-423">DateTimeOffset</span></span>|<span data-ttu-id="ef88a-424">Указывает время, по истечении которого устройство будет автоматически снято из-за запланированного действия.</span><span class="sxs-lookup"><span data-stu-id="ef88a-424">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="ef88a-425">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-425">This property is read-only.</span></span> <span data-ttu-id="ef88a-426">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-426">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-427">усерслогжедон</span><span class="sxs-lookup"><span data-stu-id="ef88a-427">usersLoggedOn</span></span>|<span data-ttu-id="ef88a-428">Коллекция [логжедонусер](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="ef88a-429">Указывает последнего вошедшего в систему пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-429">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="ef88a-430">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-430">This property is read-only.</span></span> <span data-ttu-id="ef88a-431">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-431">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-432">префермдмоверграупполициапплиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="ef88a-432">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="ef88a-433">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef88a-433">DateTimeOffset</span></span>|<span data-ttu-id="ef88a-434">Сообщает о значении DateTime, заданном параметром Префермдмоверграупполици.</span><span class="sxs-lookup"><span data-stu-id="ef88a-434">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="ef88a-435">Если этот параметр установлен, параметры групповой политики в случае конфликта будут переопределяться параметрами групповой политики.</span><span class="sxs-lookup"><span data-stu-id="ef88a-435">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="ef88a-436">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-436">Read Only.</span></span> <span data-ttu-id="ef88a-437">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-437">This property is read-only.</span></span> <span data-ttu-id="ef88a-438">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-438">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-439">аутопилотенроллед</span><span class="sxs-lookup"><span data-stu-id="ef88a-439">autopilotEnrolled</span></span>|<span data-ttu-id="ef88a-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef88a-440">Boolean</span></span>|<span data-ttu-id="ef88a-441">Сообщает, зарегистрировано ли управляемое устройство через Автоматический пилот.</span><span class="sxs-lookup"><span data-stu-id="ef88a-441">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="ef88a-442">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-442">This property is read-only.</span></span> <span data-ttu-id="ef88a-443">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-443">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-444">рекуиреусеренроллментаппровал</span><span class="sxs-lookup"><span data-stu-id="ef88a-444">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="ef88a-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef88a-445">Boolean</span></span>|<span data-ttu-id="ef88a-446">Указывает, является ли управляемое устройство iOS регистрацией на утверждение пользователя.</span><span class="sxs-lookup"><span data-stu-id="ef88a-446">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="ef88a-447">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-447">This property is read-only.</span></span> <span data-ttu-id="ef88a-448">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-448">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-449">манажементцертификатикспиратиондате</span><span class="sxs-lookup"><span data-stu-id="ef88a-449">managementCertificateExpirationDate</span></span>|<span data-ttu-id="ef88a-450">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef88a-450">DateTimeOffset</span></span>|<span data-ttu-id="ef88a-451">Дата окончания срока действия сертификата управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="ef88a-451">Reports device management certificate expiration date.</span></span> <span data-ttu-id="ef88a-452">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-452">This property is read-only.</span></span> <span data-ttu-id="ef88a-453">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-453">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-454">икЦид</span><span class="sxs-lookup"><span data-stu-id="ef88a-454">iccid</span></span>|<span data-ttu-id="ef88a-455">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-455">String</span></span>|<span data-ttu-id="ef88a-456">Идентификатор встроенной карты — это уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="ef88a-456">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="ef88a-457">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-457">This property is read-only.</span></span> <span data-ttu-id="ef88a-458">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-458">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-459">удид</span><span class="sxs-lookup"><span data-stu-id="ef88a-459">udid</span></span>|<span data-ttu-id="ef88a-460">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-460">String</span></span>|<span data-ttu-id="ef88a-461">Уникальный идентификатор устройства для устройств iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="ef88a-461">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="ef88a-462">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-462">This property is read-only.</span></span> <span data-ttu-id="ef88a-463">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-463">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-464">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ef88a-464">roleScopeTagIds</span></span>|<span data-ttu-id="ef88a-465">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ef88a-465">String collection</span></span>|<span data-ttu-id="ef88a-466">Список идентификаторов тегов области для этого экземпляра устройства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-466">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="ef88a-467">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-467">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-468">виндовсактивемалварекаунт</span><span class="sxs-lookup"><span data-stu-id="ef88a-468">windowsActiveMalwareCount</span></span>|<span data-ttu-id="ef88a-469">Int32</span><span class="sxs-lookup"><span data-stu-id="ef88a-469">Int32</span></span>|<span data-ttu-id="ef88a-470">Количество активных вредоносных программ для этого устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="ef88a-470">Count of active malware for this windows device.</span></span> <span data-ttu-id="ef88a-471">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-471">This property is read-only.</span></span> <span data-ttu-id="ef88a-472">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-472">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-473">виндовсремедиатедмалварекаунт</span><span class="sxs-lookup"><span data-stu-id="ef88a-473">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="ef88a-474">Int32</span><span class="sxs-lookup"><span data-stu-id="ef88a-474">Int32</span></span>|<span data-ttu-id="ef88a-475">Количество исправленных вредоносных программ для этого устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="ef88a-475">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="ef88a-476">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-476">This property is read-only.</span></span> <span data-ttu-id="ef88a-477">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-477">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-478">notes</span><span class="sxs-lookup"><span data-stu-id="ef88a-478">notes</span></span>|<span data-ttu-id="ef88a-479">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-479">String</span></span>|<span data-ttu-id="ef88a-480">Примечания на устройстве, созданном администратором ИТ, унаследованном от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-480">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="ef88a-481">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="ef88a-482">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="ef88a-482">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="ef88a-483">Состояние работоспособности клиента Configuration Manager, действующее только для устройств под управлением агентов MDM/ConfigMgr, наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-483">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="ef88a-484">configurationManagerClientInformation</span></span>|[<span data-ttu-id="ef88a-485">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="ef88a-485">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="ef88a-486">Сведения о клиенте Configuration Manager, действительные только для управляемых устройств, управляемых дуел и управляемых с помощью агента Configuration Manager, наследуемого от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-486">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-487">есернетмакаддресс</span><span class="sxs-lookup"><span data-stu-id="ef88a-487">ethernetMacAddress</span></span>|<span data-ttu-id="ef88a-488">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-488">String</span></span>|<span data-ttu-id="ef88a-489">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="ef88a-489">Ethernet MAC.</span></span> <span data-ttu-id="ef88a-490">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-490">This property is read-only.</span></span> <span data-ttu-id="ef88a-491">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-491">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-492">фисикалмеморинбитес</span><span class="sxs-lookup"><span data-stu-id="ef88a-492">physicalMemoryInBytes</span></span>|<span data-ttu-id="ef88a-493">Int64</span><span class="sxs-lookup"><span data-stu-id="ef88a-493">Int64</span></span>|<span data-ttu-id="ef88a-494">Общий объем памяти в байтах.</span><span class="sxs-lookup"><span data-stu-id="ef88a-494">Total Memory in Bytes.</span></span> <span data-ttu-id="ef88a-495">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-495">This property is read-only.</span></span> <span data-ttu-id="ef88a-496">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-496">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-497">процессорарчитектуре</span><span class="sxs-lookup"><span data-stu-id="ef88a-497">processorArchitecture</span></span>|[<span data-ttu-id="ef88a-498">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="ef88a-498">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="ef88a-499">Архитектура процессора.</span><span class="sxs-lookup"><span data-stu-id="ef88a-499">Processor architecture.</span></span> <span data-ttu-id="ef88a-500">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-500">This property is read-only.</span></span> <span data-ttu-id="ef88a-501">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-501">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-502">Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="ef88a-502">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="ef88a-503">спеЦификатионверсион</span><span class="sxs-lookup"><span data-stu-id="ef88a-503">specificationVersion</span></span>|<span data-ttu-id="ef88a-504">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-504">String</span></span>|<span data-ttu-id="ef88a-505">Версия спецификации.</span><span class="sxs-lookup"><span data-stu-id="ef88a-505">Specification version.</span></span> <span data-ttu-id="ef88a-506">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-506">This property is read-only.</span></span> <span data-ttu-id="ef88a-507">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-507">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-508">joinType</span><span class="sxs-lookup"><span data-stu-id="ef88a-508">joinType</span></span>|[<span data-ttu-id="ef88a-509">joinType</span><span class="sxs-lookup"><span data-stu-id="ef88a-509">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="ef88a-510">Тип присоединения устройств наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-510">Device join type Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-511">Возможные значения: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span><span class="sxs-lookup"><span data-stu-id="ef88a-511">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="ef88a-512">скуфамили</span><span class="sxs-lookup"><span data-stu-id="ef88a-512">skuFamily</span></span>|<span data-ttu-id="ef88a-513">String</span><span class="sxs-lookup"><span data-stu-id="ef88a-513">String</span></span>|<span data-ttu-id="ef88a-514">Семейство конфигураций устройств, унаследованное от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-514">Device sku family Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-515">скунумбер</span><span class="sxs-lookup"><span data-stu-id="ef88a-515">skuNumber</span></span>|<span data-ttu-id="ef88a-516">Int32</span><span class="sxs-lookup"><span data-stu-id="ef88a-516">Int32</span></span>|<span data-ttu-id="ef88a-517">Номер SKU устройства https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo см.</span><span class="sxs-lookup"><span data-stu-id="ef88a-517">Device sku number, see also: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo.</span></span> <span data-ttu-id="ef88a-518">Допустимые значения: от 0 до 2147483647.</span><span class="sxs-lookup"><span data-stu-id="ef88a-518">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="ef88a-519">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef88a-519">This property is read-only.</span></span> <span data-ttu-id="ef88a-520">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ef88a-520">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ef88a-521">манажементфеатурес</span><span class="sxs-lookup"><span data-stu-id="ef88a-521">managementFeatures</span></span>|[<span data-ttu-id="ef88a-522">манажеддевицеманажементфеатурес</span><span class="sxs-lookup"><span data-stu-id="ef88a-522">managedDeviceManagementFeatures</span></span>](../resources/intune-devices-manageddevicemanagementfeatures.md)|<span data-ttu-id="ef88a-523">Функции управления устройствами, наследуемые от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ef88a-523">Device management features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ef88a-524">Возможные значения: `none`, `microsoftManagedDesktop`.</span><span class="sxs-lookup"><span data-stu-id="ef88a-524">Possible values are: `none`, `microsoftManagedDesktop`.</span></span>|



## <a name="response"></a><span data-ttu-id="ef88a-525">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef88a-525">Response</span></span>
<span data-ttu-id="ef88a-526">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ef88a-526">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef88a-527">Пример</span><span class="sxs-lookup"><span data-stu-id="ef88a-527">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef88a-528">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef88a-528">Request</span></span>
<span data-ttu-id="ef88a-529">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef88a-529">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 8026

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
  "skuFamily": "Sku Family value",
  "skuNumber": 9,
  "managementFeatures": "microsoftManagedDesktop"
}
```

### <a name="response"></a><span data-ttu-id="ef88a-530">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef88a-530">Response</span></span>
<span data-ttu-id="ef88a-p175">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef88a-p175">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8075

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
  "skuFamily": "Sku Family value",
  "skuNumber": 9,
  "managementFeatures": "microsoftManagedDesktop"
}
```






