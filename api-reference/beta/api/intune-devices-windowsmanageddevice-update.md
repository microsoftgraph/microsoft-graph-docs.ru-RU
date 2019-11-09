---
title: Обновление Виндовсманажеддевице
description: Обновление свойств объекта Виндовсманажеддевице.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 347589686718054f5dbd0c143ade0ecb66aef481
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087392"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="f0069-103">Обновление Виндовсманажеддевице</span><span class="sxs-lookup"><span data-stu-id="f0069-103">Update windowsManagedDevice</span></span>

> <span data-ttu-id="f0069-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0069-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0069-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0069-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0069-106">Обновление свойств объекта [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="f0069-106">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0069-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f0069-107">Prerequisites</span></span>
<span data-ttu-id="f0069-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0069-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0069-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0069-110">Permission type</span></span>|<span data-ttu-id="f0069-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0069-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0069-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0069-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f0069-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0069-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f0069-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0069-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0069-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0069-115">Not supported.</span></span>|
|<span data-ttu-id="f0069-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0069-116">Application</span></span>|<span data-ttu-id="f0069-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0069-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0069-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0069-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f0069-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f0069-119">Request headers</span></span>
|<span data-ttu-id="f0069-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0069-120">Header</span></span>|<span data-ttu-id="f0069-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f0069-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0069-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0069-122">Authorization</span></span>|<span data-ttu-id="f0069-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0069-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0069-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f0069-124">Accept</span></span>|<span data-ttu-id="f0069-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f0069-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0069-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0069-126">Request body</span></span>
<span data-ttu-id="f0069-127">В тексте запроса добавьте представление объекта [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0069-127">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="f0069-128">В следующей таблице приведены свойства, необходимые при создании [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f0069-128">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="f0069-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0069-129">Property</span></span>|<span data-ttu-id="f0069-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f0069-130">Type</span></span>|<span data-ttu-id="f0069-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f0069-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0069-132">id</span><span class="sxs-lookup"><span data-stu-id="f0069-132">id</span></span>|<span data-ttu-id="f0069-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f0069-133">String</span></span>|<span data-ttu-id="f0069-134">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-134">Unique Identifier for the device.</span></span> <span data-ttu-id="f0069-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-135">This property is read-only.</span></span> <span data-ttu-id="f0069-136">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-136">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-137">userId</span><span class="sxs-lookup"><span data-stu-id="f0069-137">userId</span></span>|<span data-ttu-id="f0069-138">String</span><span class="sxs-lookup"><span data-stu-id="f0069-138">String</span></span>|<span data-ttu-id="f0069-139">Уникальный идентификатор пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="f0069-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="f0069-140">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-140">This property is read-only.</span></span> <span data-ttu-id="f0069-141">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-141">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="f0069-142">deviceName</span></span>|<span data-ttu-id="f0069-143">String</span><span class="sxs-lookup"><span data-stu-id="f0069-143">String</span></span>|<span data-ttu-id="f0069-144">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-144">Name of the device.</span></span> <span data-ttu-id="f0069-145">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-145">This property is read-only.</span></span> <span data-ttu-id="f0069-146">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-146">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-147">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="f0069-147">hardwareInformation</span></span>|[<span data-ttu-id="f0069-148">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="f0069-148">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="f0069-149">Сведения о хардвард для устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-149">The hardward details for the device.</span></span>  <span data-ttu-id="f0069-150">Включает такие сведения, как место хранения, производитель, серийный номер и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-150">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="f0069-151">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-151">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-152">ownerType</span><span class="sxs-lookup"><span data-stu-id="f0069-152">ownerType</span></span>|[<span data-ttu-id="f0069-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="f0069-153">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="f0069-154">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="f0069-154">Ownership of the device.</span></span> <span data-ttu-id="f0069-155">Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f0069-155">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f0069-156">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="f0069-156">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="f0069-157">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="f0069-157">managedDeviceOwnerType</span></span>|[<span data-ttu-id="f0069-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="f0069-158">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="f0069-159">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="f0069-159">Ownership of the device.</span></span> <span data-ttu-id="f0069-160">Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f0069-160">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f0069-161">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="f0069-161">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="f0069-162">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="f0069-162">deviceActionResults</span></span>|<span data-ttu-id="f0069-163">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-163">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="f0069-164">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="f0069-164">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="f0069-165">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-165">This property is read-only.</span></span> <span data-ttu-id="f0069-166">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-166">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-167">манажементстате</span><span class="sxs-lookup"><span data-stu-id="f0069-167">managementState</span></span>|[<span data-ttu-id="f0069-168">манажементстате</span><span class="sxs-lookup"><span data-stu-id="f0069-168">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="f0069-169">Состояние управления для устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-169">Management state of the device.</span></span> <span data-ttu-id="f0069-170">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-170">This property is read-only.</span></span> <span data-ttu-id="f0069-171">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f0069-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f0069-172">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="f0069-172">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="f0069-173">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="f0069-173">enrolledDateTime</span></span>|<span data-ttu-id="f0069-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0069-174">DateTimeOffset</span></span>|<span data-ttu-id="f0069-175">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-175">Enrollment time of the device.</span></span> <span data-ttu-id="f0069-176">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-176">This property is read-only.</span></span> <span data-ttu-id="f0069-177">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-177">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-178">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f0069-178">lastSyncDateTime</span></span>|<span data-ttu-id="f0069-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0069-179">DateTimeOffset</span></span>|<span data-ttu-id="f0069-180">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="f0069-180">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="f0069-181">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-181">This property is read-only.</span></span> <span data-ttu-id="f0069-182">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-182">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-183">чассистипе</span><span class="sxs-lookup"><span data-stu-id="f0069-183">chassisType</span></span>|[<span data-ttu-id="f0069-184">чассистипе</span><span class="sxs-lookup"><span data-stu-id="f0069-184">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="f0069-185">Тип корпуса устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-185">Chassis type of the device.</span></span> <span data-ttu-id="f0069-186">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-186">This property is read-only.</span></span> <span data-ttu-id="f0069-187">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f0069-187">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f0069-188">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="f0069-188">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="f0069-189">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="f0069-189">operatingSystem</span></span>|<span data-ttu-id="f0069-190">String</span><span class="sxs-lookup"><span data-stu-id="f0069-190">String</span></span>|<span data-ttu-id="f0069-191">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-191">Operating system of the device.</span></span> <span data-ttu-id="f0069-192">Windows, iOS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-192">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="f0069-193">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-193">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-194">deviceType</span><span class="sxs-lookup"><span data-stu-id="f0069-194">deviceType</span></span>|[<span data-ttu-id="f0069-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="f0069-195">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="f0069-196">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-196">Platform of the device.</span></span> <span data-ttu-id="f0069-197">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-197">This property is read-only.</span></span> <span data-ttu-id="f0069-198">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f0069-198">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f0069-199">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `iSocConsumer` `unknown`,,,,,,,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`</span><span class="sxs-lookup"><span data-stu-id="f0069-199">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="f0069-200">complianceState</span><span class="sxs-lookup"><span data-stu-id="f0069-200">complianceState</span></span>|[<span data-ttu-id="f0069-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="f0069-201">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="f0069-202">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="f0069-202">Compliance state of the device.</span></span> <span data-ttu-id="f0069-203">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-203">This property is read-only.</span></span> <span data-ttu-id="f0069-204">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f0069-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f0069-205">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="f0069-205">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="f0069-206">jailBroken</span><span class="sxs-lookup"><span data-stu-id="f0069-206">jailBroken</span></span>|<span data-ttu-id="f0069-207">String</span><span class="sxs-lookup"><span data-stu-id="f0069-207">String</span></span>|<span data-ttu-id="f0069-208">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="f0069-208">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="f0069-209">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-209">This property is read-only.</span></span> <span data-ttu-id="f0069-210">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-210">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-211">managementAgent</span><span class="sxs-lookup"><span data-stu-id="f0069-211">managementAgent</span></span>|[<span data-ttu-id="f0069-212">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="f0069-212">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="f0069-213">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="f0069-213">Management channel of the device.</span></span> <span data-ttu-id="f0069-214">Intune, EAS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-214">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="f0069-215">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f0069-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f0069-216">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="f0069-216">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="f0069-217">osVersion</span><span class="sxs-lookup"><span data-stu-id="f0069-217">osVersion</span></span>|<span data-ttu-id="f0069-218">String</span><span class="sxs-lookup"><span data-stu-id="f0069-218">String</span></span>|<span data-ttu-id="f0069-219">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-219">Operating system version of the device.</span></span> <span data-ttu-id="f0069-220">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-220">This property is read-only.</span></span> <span data-ttu-id="f0069-221">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-221">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-222">easActivated</span><span class="sxs-lookup"><span data-stu-id="f0069-222">easActivated</span></span>|<span data-ttu-id="f0069-223">Логический</span><span class="sxs-lookup"><span data-stu-id="f0069-223">Boolean</span></span>|<span data-ttu-id="f0069-224">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="f0069-224">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="f0069-225">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-225">This property is read-only.</span></span> <span data-ttu-id="f0069-226">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-226">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-227">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="f0069-227">easDeviceId</span></span>|<span data-ttu-id="f0069-228">String</span><span class="sxs-lookup"><span data-stu-id="f0069-228">String</span></span>|<span data-ttu-id="f0069-229">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="f0069-229">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="f0069-230">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-230">This property is read-only.</span></span> <span data-ttu-id="f0069-231">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-231">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-232">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="f0069-232">easActivationDateTime</span></span>|<span data-ttu-id="f0069-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0069-233">DateTimeOffset</span></span>|<span data-ttu-id="f0069-234">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="f0069-234">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="f0069-235">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-235">This property is read-only.</span></span> <span data-ttu-id="f0069-236">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-237">аадрегистеред</span><span class="sxs-lookup"><span data-stu-id="f0069-237">aadRegistered</span></span>|<span data-ttu-id="f0069-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0069-238">Boolean</span></span>|<span data-ttu-id="f0069-239">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f0069-239">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="f0069-240">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-240">This property is read-only.</span></span> <span data-ttu-id="f0069-241">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-241">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-242">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="f0069-242">azureADRegistered</span></span>|<span data-ttu-id="f0069-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0069-243">Boolean</span></span>|<span data-ttu-id="f0069-244">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f0069-244">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="f0069-245">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-245">This property is read-only.</span></span> <span data-ttu-id="f0069-246">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-246">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-247">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f0069-247">deviceEnrollmentType</span></span>|[<span data-ttu-id="f0069-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f0069-248">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="f0069-249">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-249">Enrollment type of the device.</span></span> <span data-ttu-id="f0069-250">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-250">This property is read-only.</span></span> <span data-ttu-id="f0069-251">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f0069-251">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f0069-252">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="f0069-252">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="f0069-253">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="f0069-253">lostModeState</span></span>|[<span data-ttu-id="f0069-254">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="f0069-254">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="f0069-255">Указывает, включен ли режим потерянных или отключенных.</span><span class="sxs-lookup"><span data-stu-id="f0069-255">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="f0069-256">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-256">This property is read-only.</span></span> <span data-ttu-id="f0069-257">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f0069-257">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f0069-258">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="f0069-258">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="f0069-259">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="f0069-259">activationLockBypassCode</span></span>|<span data-ttu-id="f0069-260">String</span><span class="sxs-lookup"><span data-stu-id="f0069-260">String</span></span>|<span data-ttu-id="f0069-261">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f0069-261">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="f0069-262">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-262">This property is read-only.</span></span> <span data-ttu-id="f0069-263">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-263">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-264">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f0069-264">emailAddress</span></span>|<span data-ttu-id="f0069-265">String</span><span class="sxs-lookup"><span data-stu-id="f0069-265">String</span></span>|<span data-ttu-id="f0069-266">Сообщения электронной почты пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="f0069-266">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="f0069-267">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-267">This property is read-only.</span></span> <span data-ttu-id="f0069-268">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-269">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="f0069-269">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="f0069-270">String</span><span class="sxs-lookup"><span data-stu-id="f0069-270">String</span></span>|<span data-ttu-id="f0069-271">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f0069-271">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="f0069-272">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-272">Read only.</span></span> <span data-ttu-id="f0069-273">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-273">This property is read-only.</span></span> <span data-ttu-id="f0069-274">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-275">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="f0069-275">azureADDeviceId</span></span>|<span data-ttu-id="f0069-276">String</span><span class="sxs-lookup"><span data-stu-id="f0069-276">String</span></span>|<span data-ttu-id="f0069-277">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f0069-277">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="f0069-278">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-278">Read only.</span></span> <span data-ttu-id="f0069-279">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-279">This property is read-only.</span></span> <span data-ttu-id="f0069-280">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-280">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-281">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="f0069-281">deviceRegistrationState</span></span>|[<span data-ttu-id="f0069-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="f0069-282">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="f0069-283">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-283">Device registration state.</span></span> <span data-ttu-id="f0069-284">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-284">This property is read-only.</span></span> <span data-ttu-id="f0069-285">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f0069-285">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f0069-286">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f0069-286">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="f0069-287">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="f0069-287">deviceCategoryDisplayName</span></span>|<span data-ttu-id="f0069-288">String</span><span class="sxs-lookup"><span data-stu-id="f0069-288">String</span></span>|<span data-ttu-id="f0069-289">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="f0069-289">Device category display name.</span></span> <span data-ttu-id="f0069-290">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-290">This property is read-only.</span></span> <span data-ttu-id="f0069-291">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-291">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-292">isSupervised</span><span class="sxs-lookup"><span data-stu-id="f0069-292">isSupervised</span></span>|<span data-ttu-id="f0069-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0069-293">Boolean</span></span>|<span data-ttu-id="f0069-294">Состояние контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-294">Device supervised status.</span></span> <span data-ttu-id="f0069-295">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-295">This property is read-only.</span></span> <span data-ttu-id="f0069-296">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-296">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-297">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f0069-297">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="f0069-298">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0069-298">DateTimeOffset</span></span>|<span data-ttu-id="f0069-299">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="f0069-299">Last time the device contacted Exchange.</span></span> <span data-ttu-id="f0069-300">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-300">This property is read-only.</span></span> <span data-ttu-id="f0069-301">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-301">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-302">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="f0069-302">exchangeAccessState</span></span>|[<span data-ttu-id="f0069-303">девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="f0069-303">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="f0069-304">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="f0069-304">The Access State of the device in Exchange.</span></span> <span data-ttu-id="f0069-305">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-305">This property is read-only.</span></span> <span data-ttu-id="f0069-306">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f0069-306">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f0069-307">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="f0069-307">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="f0069-308">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="f0069-308">exchangeAccessStateReason</span></span>|[<span data-ttu-id="f0069-309">девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="f0069-309">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="f0069-310">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="f0069-310">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="f0069-311">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-311">This property is read-only.</span></span> <span data-ttu-id="f0069-312">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f0069-312">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f0069-313">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="f0069-313">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="f0069-314">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="f0069-314">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="f0069-315">String</span><span class="sxs-lookup"><span data-stu-id="f0069-315">String</span></span>|<span data-ttu-id="f0069-316">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="f0069-316">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="f0069-317">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-317">This property is read-only.</span></span> <span data-ttu-id="f0069-318">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-318">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-319">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f0069-319">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="f0069-320">String</span><span class="sxs-lookup"><span data-stu-id="f0069-320">String</span></span>|<span data-ttu-id="f0069-321">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="f0069-321">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="f0069-322">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-322">This property is read-only.</span></span> <span data-ttu-id="f0069-323">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-324">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="f0069-324">isEncrypted</span></span>|<span data-ttu-id="f0069-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0069-325">Boolean</span></span>|<span data-ttu-id="f0069-326">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-326">Device encryption status.</span></span> <span data-ttu-id="f0069-327">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-327">This property is read-only.</span></span> <span data-ttu-id="f0069-328">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-328">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-329">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f0069-329">userPrincipalName</span></span>|<span data-ttu-id="f0069-330">String</span><span class="sxs-lookup"><span data-stu-id="f0069-330">String</span></span>|<span data-ttu-id="f0069-331">Имя участника пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-331">Device user principal name.</span></span> <span data-ttu-id="f0069-332">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-332">This property is read-only.</span></span> <span data-ttu-id="f0069-333">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-333">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-334">model</span><span class="sxs-lookup"><span data-stu-id="f0069-334">model</span></span>|<span data-ttu-id="f0069-335">String</span><span class="sxs-lookup"><span data-stu-id="f0069-335">String</span></span>|<span data-ttu-id="f0069-336">Модель устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-336">Model of the device.</span></span> <span data-ttu-id="f0069-337">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-337">This property is read-only.</span></span> <span data-ttu-id="f0069-338">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-338">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-339">manufacturer</span><span class="sxs-lookup"><span data-stu-id="f0069-339">manufacturer</span></span>|<span data-ttu-id="f0069-340">String</span><span class="sxs-lookup"><span data-stu-id="f0069-340">String</span></span>|<span data-ttu-id="f0069-341">Производитель устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-341">Manufacturer of the device.</span></span> <span data-ttu-id="f0069-342">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-342">This property is read-only.</span></span> <span data-ttu-id="f0069-343">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-343">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-344">imei</span><span class="sxs-lookup"><span data-stu-id="f0069-344">imei</span></span>|<span data-ttu-id="f0069-345">String</span><span class="sxs-lookup"><span data-stu-id="f0069-345">String</span></span>|<span data-ttu-id="f0069-346">IMEI.</span><span class="sxs-lookup"><span data-stu-id="f0069-346">IMEI.</span></span> <span data-ttu-id="f0069-347">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-347">This property is read-only.</span></span> <span data-ttu-id="f0069-348">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-348">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-349">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f0069-349">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f0069-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0069-350">DateTimeOffset</span></span>|<span data-ttu-id="f0069-351">Дата и время истечения льготного периода соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="f0069-351">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="f0069-352">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-352">This property is read-only.</span></span> <span data-ttu-id="f0069-353">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-353">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-354">serialNumber</span><span class="sxs-lookup"><span data-stu-id="f0069-354">serialNumber</span></span>|<span data-ttu-id="f0069-355">Строка</span><span class="sxs-lookup"><span data-stu-id="f0069-355">String</span></span>|<span data-ttu-id="f0069-356">Серийный.</span><span class="sxs-lookup"><span data-stu-id="f0069-356">SerialNumber.</span></span> <span data-ttu-id="f0069-357">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-357">This property is read-only.</span></span> <span data-ttu-id="f0069-358">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-359">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="f0069-359">phoneNumber</span></span>|<span data-ttu-id="f0069-360">String</span><span class="sxs-lookup"><span data-stu-id="f0069-360">String</span></span>|<span data-ttu-id="f0069-361">Номер телефона устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-361">Phone number of the device.</span></span> <span data-ttu-id="f0069-362">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-362">This property is read-only.</span></span> <span data-ttu-id="f0069-363">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-364">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="f0069-364">androidSecurityPatchLevel</span></span>|<span data-ttu-id="f0069-365">String</span><span class="sxs-lookup"><span data-stu-id="f0069-365">String</span></span>|<span data-ttu-id="f0069-366">Уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="f0069-366">Android security patch level.</span></span> <span data-ttu-id="f0069-367">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-367">This property is read-only.</span></span> <span data-ttu-id="f0069-368">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-368">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-369">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f0069-369">userDisplayName</span></span>|<span data-ttu-id="f0069-370">String</span><span class="sxs-lookup"><span data-stu-id="f0069-370">String</span></span>|<span data-ttu-id="f0069-371">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="f0069-371">User display name.</span></span> <span data-ttu-id="f0069-372">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-372">This property is read-only.</span></span> <span data-ttu-id="f0069-373">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-374">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="f0069-374">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="f0069-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="f0069-375">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="f0069-376">Функции, поддерживающие клиент Конфигрмгр.</span><span class="sxs-lookup"><span data-stu-id="f0069-376">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="f0069-377">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-377">This property is read-only.</span></span> <span data-ttu-id="f0069-378">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-379">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="f0069-379">wiFiMacAddress</span></span>|<span data-ttu-id="f0069-380">String</span><span class="sxs-lookup"><span data-stu-id="f0069-380">String</span></span>|<span data-ttu-id="f0069-381">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f0069-381">Wi-Fi MAC.</span></span> <span data-ttu-id="f0069-382">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-382">This property is read-only.</span></span> <span data-ttu-id="f0069-383">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-383">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-384">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="f0069-384">deviceHealthAttestationState</span></span>|[<span data-ttu-id="f0069-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="f0069-385">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="f0069-386">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-386">The device health attestation state.</span></span> <span data-ttu-id="f0069-387">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-387">This property is read-only.</span></span> <span data-ttu-id="f0069-388">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-388">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-389">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="f0069-389">subscriberCarrier</span></span>|<span data-ttu-id="f0069-390">String</span><span class="sxs-lookup"><span data-stu-id="f0069-390">String</span></span>|<span data-ttu-id="f0069-391">Перевозчик абонента.</span><span class="sxs-lookup"><span data-stu-id="f0069-391">Subscriber Carrier.</span></span> <span data-ttu-id="f0069-392">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-392">This property is read-only.</span></span> <span data-ttu-id="f0069-393">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-393">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-394">meid</span><span class="sxs-lookup"><span data-stu-id="f0069-394">meid</span></span>|<span data-ttu-id="f0069-395">String</span><span class="sxs-lookup"><span data-stu-id="f0069-395">String</span></span>|<span data-ttu-id="f0069-396">MEID.</span><span class="sxs-lookup"><span data-stu-id="f0069-396">MEID.</span></span> <span data-ttu-id="f0069-397">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-397">This property is read-only.</span></span> <span data-ttu-id="f0069-398">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-398">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-399">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="f0069-399">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="f0069-400">Int64</span><span class="sxs-lookup"><span data-stu-id="f0069-400">Int64</span></span>|<span data-ttu-id="f0069-401">Общий объем хранилища в байтах.</span><span class="sxs-lookup"><span data-stu-id="f0069-401">Total Storage in Bytes.</span></span> <span data-ttu-id="f0069-402">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-402">This property is read-only.</span></span> <span data-ttu-id="f0069-403">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-403">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-404">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="f0069-404">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="f0069-405">Int64</span><span class="sxs-lookup"><span data-stu-id="f0069-405">Int64</span></span>|<span data-ttu-id="f0069-406">Свободное хранилище в байтах.</span><span class="sxs-lookup"><span data-stu-id="f0069-406">Free Storage in Bytes.</span></span> <span data-ttu-id="f0069-407">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-407">This property is read-only.</span></span> <span data-ttu-id="f0069-408">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-408">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-409">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="f0069-409">managedDeviceName</span></span>|<span data-ttu-id="f0069-410">String</span><span class="sxs-lookup"><span data-stu-id="f0069-410">String</span></span>|<span data-ttu-id="f0069-411">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-411">Automatically generated name to identify a device.</span></span> <span data-ttu-id="f0069-412">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="f0069-412">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="f0069-413">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-413">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-414">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="f0069-414">partnerReportedThreatState</span></span>|[<span data-ttu-id="f0069-415">манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="f0069-415">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="f0069-416">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="f0069-416">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="f0069-417">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-417">Read Only.</span></span> <span data-ttu-id="f0069-418">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-418">This property is read-only.</span></span> <span data-ttu-id="f0069-419">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f0069-419">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f0069-420">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="f0069-420">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="f0069-421">ретиреафтердатетиме</span><span class="sxs-lookup"><span data-stu-id="f0069-421">retireAfterDateTime</span></span>|<span data-ttu-id="f0069-422">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0069-422">DateTimeOffset</span></span>|<span data-ttu-id="f0069-423">Указывает время, по истечении которого устройство будет автоматически снято из-за запланированного действия.</span><span class="sxs-lookup"><span data-stu-id="f0069-423">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="f0069-424">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-424">This property is read-only.</span></span> <span data-ttu-id="f0069-425">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-425">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-426">усерслогжедон</span><span class="sxs-lookup"><span data-stu-id="f0069-426">usersLoggedOn</span></span>|<span data-ttu-id="f0069-427">Коллекция [логжедонусер](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-427">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="f0069-428">Указывает последнего вошедшего в систему пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-428">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="f0069-429">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-429">This property is read-only.</span></span> <span data-ttu-id="f0069-430">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-430">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-431">префермдмоверграупполициапплиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="f0069-431">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="f0069-432">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0069-432">DateTimeOffset</span></span>|<span data-ttu-id="f0069-433">Сообщает о значении DateTime, заданном параметром Префермдмоверграупполици.</span><span class="sxs-lookup"><span data-stu-id="f0069-433">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="f0069-434">Если этот параметр установлен, параметры групповой политики в случае конфликта будут переопределяться параметрами групповой политики.</span><span class="sxs-lookup"><span data-stu-id="f0069-434">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="f0069-435">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-435">Read Only.</span></span> <span data-ttu-id="f0069-436">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-436">This property is read-only.</span></span> <span data-ttu-id="f0069-437">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-437">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-438">аутопилотенроллед</span><span class="sxs-lookup"><span data-stu-id="f0069-438">autopilotEnrolled</span></span>|<span data-ttu-id="f0069-439">Логический</span><span class="sxs-lookup"><span data-stu-id="f0069-439">Boolean</span></span>|<span data-ttu-id="f0069-440">Сообщает, зарегистрировано ли управляемое устройство через Автоматический пилот.</span><span class="sxs-lookup"><span data-stu-id="f0069-440">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="f0069-441">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-441">This property is read-only.</span></span> <span data-ttu-id="f0069-442">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-442">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-443">рекуиреусеренроллментаппровал</span><span class="sxs-lookup"><span data-stu-id="f0069-443">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="f0069-444">Логический</span><span class="sxs-lookup"><span data-stu-id="f0069-444">Boolean</span></span>|<span data-ttu-id="f0069-445">Указывает, является ли управляемое устройство iOS регистрацией на утверждение пользователя.</span><span class="sxs-lookup"><span data-stu-id="f0069-445">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="f0069-446">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-446">This property is read-only.</span></span> <span data-ttu-id="f0069-447">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-447">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-448">манажементцертификатикспиратиондате</span><span class="sxs-lookup"><span data-stu-id="f0069-448">managementCertificateExpirationDate</span></span>|<span data-ttu-id="f0069-449">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0069-449">DateTimeOffset</span></span>|<span data-ttu-id="f0069-450">Дата окончания срока действия сертификата управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="f0069-450">Reports device management certificate expiration date.</span></span> <span data-ttu-id="f0069-451">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-451">This property is read-only.</span></span> <span data-ttu-id="f0069-452">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-452">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-453">икЦид</span><span class="sxs-lookup"><span data-stu-id="f0069-453">iccid</span></span>|<span data-ttu-id="f0069-454">String</span><span class="sxs-lookup"><span data-stu-id="f0069-454">String</span></span>|<span data-ttu-id="f0069-455">Идентификатор встроенной карты — это уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="f0069-455">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="f0069-456">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-456">This property is read-only.</span></span> <span data-ttu-id="f0069-457">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-457">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-458">удид</span><span class="sxs-lookup"><span data-stu-id="f0069-458">udid</span></span>|<span data-ttu-id="f0069-459">String</span><span class="sxs-lookup"><span data-stu-id="f0069-459">String</span></span>|<span data-ttu-id="f0069-460">Уникальный идентификатор устройства для устройств iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="f0069-460">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="f0069-461">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-461">This property is read-only.</span></span> <span data-ttu-id="f0069-462">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-462">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-463">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f0069-463">roleScopeTagIds</span></span>|<span data-ttu-id="f0069-464">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f0069-464">String collection</span></span>|<span data-ttu-id="f0069-465">Список идентификаторов тегов области для этого экземпляра устройства.</span><span class="sxs-lookup"><span data-stu-id="f0069-465">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="f0069-466">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-466">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-467">виндовсактивемалварекаунт</span><span class="sxs-lookup"><span data-stu-id="f0069-467">windowsActiveMalwareCount</span></span>|<span data-ttu-id="f0069-468">Int32</span><span class="sxs-lookup"><span data-stu-id="f0069-468">Int32</span></span>|<span data-ttu-id="f0069-469">Количество активных вредоносных программ для этого устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="f0069-469">Count of active malware for this windows device.</span></span> <span data-ttu-id="f0069-470">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-470">This property is read-only.</span></span> <span data-ttu-id="f0069-471">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-471">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-472">виндовсремедиатедмалварекаунт</span><span class="sxs-lookup"><span data-stu-id="f0069-472">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="f0069-473">Int32</span><span class="sxs-lookup"><span data-stu-id="f0069-473">Int32</span></span>|<span data-ttu-id="f0069-474">Количество исправленных вредоносных программ для этого устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="f0069-474">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="f0069-475">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-475">This property is read-only.</span></span> <span data-ttu-id="f0069-476">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-476">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-477">notes</span><span class="sxs-lookup"><span data-stu-id="f0069-477">notes</span></span>|<span data-ttu-id="f0069-478">String</span><span class="sxs-lookup"><span data-stu-id="f0069-478">String</span></span>|<span data-ttu-id="f0069-479">Примечания на устройстве, созданном администратором ИТ, унаследованном от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-479">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-480">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="f0069-480">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="f0069-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="f0069-481">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="f0069-482">Состояние работоспособности клиента Configuration Manager, действующее только для устройств под управлением агентов MDM/ConfigMgr, наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-482">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-483">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="f0069-483">configurationManagerClientInformation</span></span>|[<span data-ttu-id="f0069-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="f0069-484">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="f0069-485">Сведения о клиенте Configuration Manager, действительные только для управляемых устройств, управляемых дуел и управляемых с помощью агента Configuration Manager, наследуемого от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-485">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f0069-486">есернетмакаддресс</span><span class="sxs-lookup"><span data-stu-id="f0069-486">ethernetMacAddress</span></span>|<span data-ttu-id="f0069-487">String</span><span class="sxs-lookup"><span data-stu-id="f0069-487">String</span></span>|<span data-ttu-id="f0069-488">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="f0069-488">Ethernet MAC.</span></span> <span data-ttu-id="f0069-489">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0069-489">This property is read-only.</span></span> <span data-ttu-id="f0069-490">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f0069-490">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f0069-491">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0069-491">Response</span></span>
<span data-ttu-id="f0069-492">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0069-492">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0069-493">Пример</span><span class="sxs-lookup"><span data-stu-id="f0069-493">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0069-494">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0069-494">Request</span></span>
<span data-ttu-id="f0069-495">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0069-495">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7575

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
  "ethernetMacAddress": "Ethernet Mac Address value"
}
```

### <a name="response"></a><span data-ttu-id="f0069-496">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0069-496">Response</span></span>
<span data-ttu-id="f0069-p169">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0069-p169">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7624

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
  "ethernetMacAddress": "Ethernet Mac Address value"
}
```






