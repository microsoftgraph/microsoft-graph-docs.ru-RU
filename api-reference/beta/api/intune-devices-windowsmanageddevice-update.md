---
title: Обновление Виндовсманажеддевице
description: Обновление свойств объекта Виндовсманажеддевице.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f9964304f08a5013c8e03c80c8e79fb44e5e89ca
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708181"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="4649b-103">Обновление Виндовсманажеддевице</span><span class="sxs-lookup"><span data-stu-id="4649b-103">Update windowsManagedDevice</span></span>

<span data-ttu-id="4649b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4649b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4649b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4649b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4649b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4649b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4649b-107">Обновление свойств объекта [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="4649b-107">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4649b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4649b-108">Prerequisites</span></span>
<span data-ttu-id="4649b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4649b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4649b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4649b-111">Permission type</span></span>|<span data-ttu-id="4649b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4649b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4649b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4649b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4649b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4649b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4649b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4649b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4649b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4649b-116">Not supported.</span></span>|
|<span data-ttu-id="4649b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4649b-117">Application</span></span>|<span data-ttu-id="4649b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4649b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4649b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4649b-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4649b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4649b-120">Request headers</span></span>
|<span data-ttu-id="4649b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4649b-121">Header</span></span>|<span data-ttu-id="4649b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4649b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4649b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4649b-123">Authorization</span></span>|<span data-ttu-id="4649b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4649b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4649b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4649b-125">Accept</span></span>|<span data-ttu-id="4649b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4649b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4649b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4649b-127">Request body</span></span>
<span data-ttu-id="4649b-128">В тексте запроса добавьте представление объекта [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4649b-128">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="4649b-129">В следующей таблице приведены свойства, необходимые при создании [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-129">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="4649b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4649b-130">Property</span></span>|<span data-ttu-id="4649b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4649b-131">Type</span></span>|<span data-ttu-id="4649b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4649b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4649b-133">id</span><span class="sxs-lookup"><span data-stu-id="4649b-133">id</span></span>|<span data-ttu-id="4649b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4649b-134">String</span></span>|<span data-ttu-id="4649b-135">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-135">Unique Identifier for the device.</span></span> <span data-ttu-id="4649b-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-136">This property is read-only.</span></span> <span data-ttu-id="4649b-137">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-137">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-138">userId</span><span class="sxs-lookup"><span data-stu-id="4649b-138">userId</span></span>|<span data-ttu-id="4649b-139">String</span><span class="sxs-lookup"><span data-stu-id="4649b-139">String</span></span>|<span data-ttu-id="4649b-140">Уникальный идентификатор пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="4649b-140">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="4649b-141">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-141">This property is read-only.</span></span> <span data-ttu-id="4649b-142">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-142">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="4649b-143">deviceName</span></span>|<span data-ttu-id="4649b-144">String</span><span class="sxs-lookup"><span data-stu-id="4649b-144">String</span></span>|<span data-ttu-id="4649b-145">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-145">Name of the device.</span></span> <span data-ttu-id="4649b-146">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-146">This property is read-only.</span></span> <span data-ttu-id="4649b-147">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-147">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-148">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="4649b-148">hardwareInformation</span></span>|[<span data-ttu-id="4649b-149">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="4649b-149">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="4649b-150">Сведения о хардвард для устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-150">The hardward details for the device.</span></span>  <span data-ttu-id="4649b-151">Включает такие сведения, как место хранения, производитель, серийный номер и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-151">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="4649b-152">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-152">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="4649b-153">ownerType</span></span>|[<span data-ttu-id="4649b-154">ownerType</span><span class="sxs-lookup"><span data-stu-id="4649b-154">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="4649b-155">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="4649b-155">Ownership of the device.</span></span> <span data-ttu-id="4649b-156">Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-156">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-157">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="4649b-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="4649b-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="4649b-158">managedDeviceOwnerType</span></span>|[<span data-ttu-id="4649b-159">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="4649b-159">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="4649b-160">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="4649b-160">Ownership of the device.</span></span> <span data-ttu-id="4649b-161">Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-161">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-162">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="4649b-162">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="4649b-163">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="4649b-163">deviceActionResults</span></span>|<span data-ttu-id="4649b-164">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="4649b-165">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="4649b-165">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="4649b-166">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-166">This property is read-only.</span></span> <span data-ttu-id="4649b-167">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-168">манажементстате</span><span class="sxs-lookup"><span data-stu-id="4649b-168">managementState</span></span>|[<span data-ttu-id="4649b-169">манажементстате</span><span class="sxs-lookup"><span data-stu-id="4649b-169">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="4649b-170">Состояние управления для устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-170">Management state of the device.</span></span> <span data-ttu-id="4649b-171">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-171">This property is read-only.</span></span> <span data-ttu-id="4649b-172">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-173">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="4649b-173">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="4649b-174">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="4649b-174">enrolledDateTime</span></span>|<span data-ttu-id="4649b-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4649b-175">DateTimeOffset</span></span>|<span data-ttu-id="4649b-176">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-176">Enrollment time of the device.</span></span> <span data-ttu-id="4649b-177">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-177">This property is read-only.</span></span> <span data-ttu-id="4649b-178">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-178">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-179">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4649b-179">lastSyncDateTime</span></span>|<span data-ttu-id="4649b-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4649b-180">DateTimeOffset</span></span>|<span data-ttu-id="4649b-181">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="4649b-181">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="4649b-182">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-182">This property is read-only.</span></span> <span data-ttu-id="4649b-183">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-183">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-184">чассистипе</span><span class="sxs-lookup"><span data-stu-id="4649b-184">chassisType</span></span>|[<span data-ttu-id="4649b-185">чассистипе</span><span class="sxs-lookup"><span data-stu-id="4649b-185">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="4649b-186">Тип корпуса устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-186">Chassis type of the device.</span></span> <span data-ttu-id="4649b-187">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-187">This property is read-only.</span></span> <span data-ttu-id="4649b-188">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-188">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-189">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="4649b-189">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="4649b-190">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="4649b-190">operatingSystem</span></span>|<span data-ttu-id="4649b-191">String</span><span class="sxs-lookup"><span data-stu-id="4649b-191">String</span></span>|<span data-ttu-id="4649b-192">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-192">Operating system of the device.</span></span> <span data-ttu-id="4649b-193">Windows, iOS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-193">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="4649b-194">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="4649b-195">deviceType</span></span>|[<span data-ttu-id="4649b-196">deviceType</span><span class="sxs-lookup"><span data-stu-id="4649b-196">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="4649b-197">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-197">Platform of the device.</span></span> <span data-ttu-id="4649b-198">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-198">This property is read-only.</span></span> <span data-ttu-id="4649b-199">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-199">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-200">Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` ,,, `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` ,, `unknown` ,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="4649b-200">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="4649b-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="4649b-201">complianceState</span></span>|[<span data-ttu-id="4649b-202">complianceState</span><span class="sxs-lookup"><span data-stu-id="4649b-202">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="4649b-203">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="4649b-203">Compliance state of the device.</span></span> <span data-ttu-id="4649b-204">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-204">This property is read-only.</span></span> <span data-ttu-id="4649b-205">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-205">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-206">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="4649b-206">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="4649b-207">jailBroken</span><span class="sxs-lookup"><span data-stu-id="4649b-207">jailBroken</span></span>|<span data-ttu-id="4649b-208">String</span><span class="sxs-lookup"><span data-stu-id="4649b-208">String</span></span>|<span data-ttu-id="4649b-209">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="4649b-209">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="4649b-210">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-210">This property is read-only.</span></span> <span data-ttu-id="4649b-211">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-212">managementAgent</span><span class="sxs-lookup"><span data-stu-id="4649b-212">managementAgent</span></span>|[<span data-ttu-id="4649b-213">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="4649b-213">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="4649b-214">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="4649b-214">Management channel of the device.</span></span> <span data-ttu-id="4649b-215">Intune, EAS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-215">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="4649b-216">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-217">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="4649b-217">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="4649b-218">osVersion</span><span class="sxs-lookup"><span data-stu-id="4649b-218">osVersion</span></span>|<span data-ttu-id="4649b-219">String</span><span class="sxs-lookup"><span data-stu-id="4649b-219">String</span></span>|<span data-ttu-id="4649b-220">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-220">Operating system version of the device.</span></span> <span data-ttu-id="4649b-221">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-221">This property is read-only.</span></span> <span data-ttu-id="4649b-222">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-222">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-223">easActivated</span><span class="sxs-lookup"><span data-stu-id="4649b-223">easActivated</span></span>|<span data-ttu-id="4649b-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="4649b-224">Boolean</span></span>|<span data-ttu-id="4649b-225">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="4649b-225">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="4649b-226">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-226">This property is read-only.</span></span> <span data-ttu-id="4649b-227">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="4649b-228">easDeviceId</span></span>|<span data-ttu-id="4649b-229">String</span><span class="sxs-lookup"><span data-stu-id="4649b-229">String</span></span>|<span data-ttu-id="4649b-230">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="4649b-230">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="4649b-231">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-231">This property is read-only.</span></span> <span data-ttu-id="4649b-232">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-232">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-233">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="4649b-233">easActivationDateTime</span></span>|<span data-ttu-id="4649b-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4649b-234">DateTimeOffset</span></span>|<span data-ttu-id="4649b-235">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="4649b-235">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="4649b-236">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-236">This property is read-only.</span></span> <span data-ttu-id="4649b-237">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-238">аадрегистеред</span><span class="sxs-lookup"><span data-stu-id="4649b-238">aadRegistered</span></span>|<span data-ttu-id="4649b-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="4649b-239">Boolean</span></span>|<span data-ttu-id="4649b-240">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4649b-240">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="4649b-241">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-241">This property is read-only.</span></span> <span data-ttu-id="4649b-242">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-242">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-243">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="4649b-243">azureADRegistered</span></span>|<span data-ttu-id="4649b-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="4649b-244">Boolean</span></span>|<span data-ttu-id="4649b-245">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4649b-245">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="4649b-246">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-246">This property is read-only.</span></span> <span data-ttu-id="4649b-247">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-247">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="4649b-248">deviceEnrollmentType</span></span>|[<span data-ttu-id="4649b-249">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="4649b-249">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="4649b-250">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-250">Enrollment type of the device.</span></span> <span data-ttu-id="4649b-251">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-251">This property is read-only.</span></span> <span data-ttu-id="4649b-252">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-252">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-253">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="4649b-253">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="4649b-254">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="4649b-254">lostModeState</span></span>|[<span data-ttu-id="4649b-255">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="4649b-255">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="4649b-256">Указывает, включен ли режим потерянных или отключенных.</span><span class="sxs-lookup"><span data-stu-id="4649b-256">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="4649b-257">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-257">This property is read-only.</span></span> <span data-ttu-id="4649b-258">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-258">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-259">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="4649b-259">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="4649b-260">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="4649b-260">activationLockBypassCode</span></span>|<span data-ttu-id="4649b-261">String</span><span class="sxs-lookup"><span data-stu-id="4649b-261">String</span></span>|<span data-ttu-id="4649b-262">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4649b-262">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="4649b-263">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-263">This property is read-only.</span></span> <span data-ttu-id="4649b-264">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-265">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4649b-265">emailAddress</span></span>|<span data-ttu-id="4649b-266">String</span><span class="sxs-lookup"><span data-stu-id="4649b-266">String</span></span>|<span data-ttu-id="4649b-267">Сообщения электронной почты пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="4649b-267">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="4649b-268">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-268">This property is read-only.</span></span> <span data-ttu-id="4649b-269">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-270">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="4649b-270">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="4649b-271">String</span><span class="sxs-lookup"><span data-stu-id="4649b-271">String</span></span>|<span data-ttu-id="4649b-272">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4649b-272">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="4649b-273">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-273">Read only.</span></span> <span data-ttu-id="4649b-274">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-274">This property is read-only.</span></span> <span data-ttu-id="4649b-275">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-275">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-276">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="4649b-276">azureADDeviceId</span></span>|<span data-ttu-id="4649b-277">String</span><span class="sxs-lookup"><span data-stu-id="4649b-277">String</span></span>|<span data-ttu-id="4649b-278">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4649b-278">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="4649b-279">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-279">Read only.</span></span> <span data-ttu-id="4649b-280">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-280">This property is read-only.</span></span> <span data-ttu-id="4649b-281">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-281">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="4649b-282">deviceRegistrationState</span></span>|[<span data-ttu-id="4649b-283">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="4649b-283">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="4649b-284">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-284">Device registration state.</span></span> <span data-ttu-id="4649b-285">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-285">This property is read-only.</span></span> <span data-ttu-id="4649b-286">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-286">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-287">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4649b-287">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="4649b-288">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="4649b-288">deviceCategoryDisplayName</span></span>|<span data-ttu-id="4649b-289">String</span><span class="sxs-lookup"><span data-stu-id="4649b-289">String</span></span>|<span data-ttu-id="4649b-290">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="4649b-290">Device category display name.</span></span> <span data-ttu-id="4649b-291">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-291">This property is read-only.</span></span> <span data-ttu-id="4649b-292">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-292">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-293">isSupervised</span><span class="sxs-lookup"><span data-stu-id="4649b-293">isSupervised</span></span>|<span data-ttu-id="4649b-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="4649b-294">Boolean</span></span>|<span data-ttu-id="4649b-295">Состояние контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-295">Device supervised status.</span></span> <span data-ttu-id="4649b-296">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-296">This property is read-only.</span></span> <span data-ttu-id="4649b-297">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-297">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-298">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4649b-298">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="4649b-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4649b-299">DateTimeOffset</span></span>|<span data-ttu-id="4649b-300">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="4649b-300">Last time the device contacted Exchange.</span></span> <span data-ttu-id="4649b-301">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-301">This property is read-only.</span></span> <span data-ttu-id="4649b-302">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-302">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="4649b-303">exchangeAccessState</span></span>|[<span data-ttu-id="4649b-304">девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="4649b-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="4649b-305">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="4649b-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="4649b-306">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-306">This property is read-only.</span></span> <span data-ttu-id="4649b-307">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-307">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-308">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="4649b-308">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="4649b-309">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="4649b-309">exchangeAccessStateReason</span></span>|[<span data-ttu-id="4649b-310">девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="4649b-310">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="4649b-311">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="4649b-311">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="4649b-312">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-312">This property is read-only.</span></span> <span data-ttu-id="4649b-313">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-313">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-314">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="4649b-314">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="4649b-315">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="4649b-315">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="4649b-316">String</span><span class="sxs-lookup"><span data-stu-id="4649b-316">String</span></span>|<span data-ttu-id="4649b-317">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="4649b-317">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="4649b-318">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-318">This property is read-only.</span></span> <span data-ttu-id="4649b-319">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-319">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-320">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="4649b-320">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="4649b-321">String</span><span class="sxs-lookup"><span data-stu-id="4649b-321">String</span></span>|<span data-ttu-id="4649b-322">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="4649b-322">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="4649b-323">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-323">This property is read-only.</span></span> <span data-ttu-id="4649b-324">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-324">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="4649b-325">isEncrypted</span></span>|<span data-ttu-id="4649b-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="4649b-326">Boolean</span></span>|<span data-ttu-id="4649b-327">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-327">Device encryption status.</span></span> <span data-ttu-id="4649b-328">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-328">This property is read-only.</span></span> <span data-ttu-id="4649b-329">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-329">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-330">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4649b-330">userPrincipalName</span></span>|<span data-ttu-id="4649b-331">String</span><span class="sxs-lookup"><span data-stu-id="4649b-331">String</span></span>|<span data-ttu-id="4649b-332">Имя участника пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-332">Device user principal name.</span></span> <span data-ttu-id="4649b-333">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-333">This property is read-only.</span></span> <span data-ttu-id="4649b-334">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-334">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-335">model</span><span class="sxs-lookup"><span data-stu-id="4649b-335">model</span></span>|<span data-ttu-id="4649b-336">String</span><span class="sxs-lookup"><span data-stu-id="4649b-336">String</span></span>|<span data-ttu-id="4649b-337">Модель устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-337">Model of the device.</span></span> <span data-ttu-id="4649b-338">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-338">This property is read-only.</span></span> <span data-ttu-id="4649b-339">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-340">manufacturer</span><span class="sxs-lookup"><span data-stu-id="4649b-340">manufacturer</span></span>|<span data-ttu-id="4649b-341">String</span><span class="sxs-lookup"><span data-stu-id="4649b-341">String</span></span>|<span data-ttu-id="4649b-342">Производитель устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-342">Manufacturer of the device.</span></span> <span data-ttu-id="4649b-343">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-343">This property is read-only.</span></span> <span data-ttu-id="4649b-344">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-345">imei</span><span class="sxs-lookup"><span data-stu-id="4649b-345">imei</span></span>|<span data-ttu-id="4649b-346">String</span><span class="sxs-lookup"><span data-stu-id="4649b-346">String</span></span>|<span data-ttu-id="4649b-347">IMEI.</span><span class="sxs-lookup"><span data-stu-id="4649b-347">IMEI.</span></span> <span data-ttu-id="4649b-348">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-348">This property is read-only.</span></span> <span data-ttu-id="4649b-349">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-349">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-350">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4649b-350">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="4649b-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4649b-351">DateTimeOffset</span></span>|<span data-ttu-id="4649b-352">Дата и время истечения льготного периода соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="4649b-352">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="4649b-353">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-353">This property is read-only.</span></span> <span data-ttu-id="4649b-354">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-355">serialNumber</span><span class="sxs-lookup"><span data-stu-id="4649b-355">serialNumber</span></span>|<span data-ttu-id="4649b-356">String</span><span class="sxs-lookup"><span data-stu-id="4649b-356">String</span></span>|<span data-ttu-id="4649b-357">Серийный.</span><span class="sxs-lookup"><span data-stu-id="4649b-357">SerialNumber.</span></span> <span data-ttu-id="4649b-358">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-358">This property is read-only.</span></span> <span data-ttu-id="4649b-359">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-360">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="4649b-360">phoneNumber</span></span>|<span data-ttu-id="4649b-361">String</span><span class="sxs-lookup"><span data-stu-id="4649b-361">String</span></span>|<span data-ttu-id="4649b-362">Номер телефона устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-362">Phone number of the device.</span></span> <span data-ttu-id="4649b-363">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-363">This property is read-only.</span></span> <span data-ttu-id="4649b-364">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-364">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-365">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="4649b-365">androidSecurityPatchLevel</span></span>|<span data-ttu-id="4649b-366">String</span><span class="sxs-lookup"><span data-stu-id="4649b-366">String</span></span>|<span data-ttu-id="4649b-367">Уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="4649b-367">Android security patch level.</span></span> <span data-ttu-id="4649b-368">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-368">This property is read-only.</span></span> <span data-ttu-id="4649b-369">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-370">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4649b-370">userDisplayName</span></span>|<span data-ttu-id="4649b-371">String</span><span class="sxs-lookup"><span data-stu-id="4649b-371">String</span></span>|<span data-ttu-id="4649b-372">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="4649b-372">User display name.</span></span> <span data-ttu-id="4649b-373">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-373">This property is read-only.</span></span> <span data-ttu-id="4649b-374">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="4649b-375">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="4649b-376">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="4649b-376">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="4649b-377">Функции, поддерживающие клиент Конфигрмгр.</span><span class="sxs-lookup"><span data-stu-id="4649b-377">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="4649b-378">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-378">This property is read-only.</span></span> <span data-ttu-id="4649b-379">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-379">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-380">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="4649b-380">wiFiMacAddress</span></span>|<span data-ttu-id="4649b-381">String</span><span class="sxs-lookup"><span data-stu-id="4649b-381">String</span></span>|<span data-ttu-id="4649b-382">Wi-Fi MAC.</span><span class="sxs-lookup"><span data-stu-id="4649b-382">Wi-Fi MAC.</span></span> <span data-ttu-id="4649b-383">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-383">This property is read-only.</span></span> <span data-ttu-id="4649b-384">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-384">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="4649b-385">deviceHealthAttestationState</span></span>|[<span data-ttu-id="4649b-386">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="4649b-386">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="4649b-387">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-387">The device health attestation state.</span></span> <span data-ttu-id="4649b-388">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-388">This property is read-only.</span></span> <span data-ttu-id="4649b-389">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-389">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-390">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="4649b-390">subscriberCarrier</span></span>|<span data-ttu-id="4649b-391">String</span><span class="sxs-lookup"><span data-stu-id="4649b-391">String</span></span>|<span data-ttu-id="4649b-392">Перевозчик абонента.</span><span class="sxs-lookup"><span data-stu-id="4649b-392">Subscriber Carrier.</span></span> <span data-ttu-id="4649b-393">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-393">This property is read-only.</span></span> <span data-ttu-id="4649b-394">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-394">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-395">meid</span><span class="sxs-lookup"><span data-stu-id="4649b-395">meid</span></span>|<span data-ttu-id="4649b-396">String</span><span class="sxs-lookup"><span data-stu-id="4649b-396">String</span></span>|<span data-ttu-id="4649b-397">MEID.</span><span class="sxs-lookup"><span data-stu-id="4649b-397">MEID.</span></span> <span data-ttu-id="4649b-398">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-398">This property is read-only.</span></span> <span data-ttu-id="4649b-399">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-399">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-400">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="4649b-400">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="4649b-401">Int64</span><span class="sxs-lookup"><span data-stu-id="4649b-401">Int64</span></span>|<span data-ttu-id="4649b-402">Общий объем хранилища в байтах.</span><span class="sxs-lookup"><span data-stu-id="4649b-402">Total Storage in Bytes.</span></span> <span data-ttu-id="4649b-403">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-403">This property is read-only.</span></span> <span data-ttu-id="4649b-404">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-404">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-405">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="4649b-405">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="4649b-406">Int64</span><span class="sxs-lookup"><span data-stu-id="4649b-406">Int64</span></span>|<span data-ttu-id="4649b-407">Свободное хранилище в байтах.</span><span class="sxs-lookup"><span data-stu-id="4649b-407">Free Storage in Bytes.</span></span> <span data-ttu-id="4649b-408">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-408">This property is read-only.</span></span> <span data-ttu-id="4649b-409">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-409">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-410">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="4649b-410">managedDeviceName</span></span>|<span data-ttu-id="4649b-411">String</span><span class="sxs-lookup"><span data-stu-id="4649b-411">String</span></span>|<span data-ttu-id="4649b-412">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-412">Automatically generated name to identify a device.</span></span> <span data-ttu-id="4649b-413">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="4649b-413">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="4649b-414">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-414">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-415">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="4649b-415">partnerReportedThreatState</span></span>|[<span data-ttu-id="4649b-416">манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="4649b-416">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="4649b-417">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="4649b-417">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="4649b-418">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-418">Read Only.</span></span> <span data-ttu-id="4649b-419">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-419">This property is read-only.</span></span> <span data-ttu-id="4649b-420">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-420">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-421">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="4649b-421">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="4649b-422">ретиреафтердатетиме</span><span class="sxs-lookup"><span data-stu-id="4649b-422">retireAfterDateTime</span></span>|<span data-ttu-id="4649b-423">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4649b-423">DateTimeOffset</span></span>|<span data-ttu-id="4649b-424">Указывает время, по истечении которого устройство будет автоматически снято из-за запланированного действия.</span><span class="sxs-lookup"><span data-stu-id="4649b-424">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="4649b-425">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-425">This property is read-only.</span></span> <span data-ttu-id="4649b-426">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-426">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-427">усерслогжедон</span><span class="sxs-lookup"><span data-stu-id="4649b-427">usersLoggedOn</span></span>|<span data-ttu-id="4649b-428">Коллекция [логжедонусер](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="4649b-429">Указывает последнего вошедшего в систему пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-429">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="4649b-430">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-430">This property is read-only.</span></span> <span data-ttu-id="4649b-431">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-431">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-432">префермдмоверграупполициапплиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="4649b-432">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="4649b-433">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4649b-433">DateTimeOffset</span></span>|<span data-ttu-id="4649b-434">Сообщает о значении DateTime, заданном параметром Префермдмоверграупполици.</span><span class="sxs-lookup"><span data-stu-id="4649b-434">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="4649b-435">Если этот параметр установлен, параметры групповой политики в случае конфликта будут переопределяться параметрами групповой политики.</span><span class="sxs-lookup"><span data-stu-id="4649b-435">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="4649b-436">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-436">Read Only.</span></span> <span data-ttu-id="4649b-437">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-437">This property is read-only.</span></span> <span data-ttu-id="4649b-438">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-438">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-439">аутопилотенроллед</span><span class="sxs-lookup"><span data-stu-id="4649b-439">autopilotEnrolled</span></span>|<span data-ttu-id="4649b-440">Логический</span><span class="sxs-lookup"><span data-stu-id="4649b-440">Boolean</span></span>|<span data-ttu-id="4649b-441">Сообщает, зарегистрировано ли управляемое устройство через Автоматический пилот.</span><span class="sxs-lookup"><span data-stu-id="4649b-441">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="4649b-442">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-442">This property is read-only.</span></span> <span data-ttu-id="4649b-443">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-443">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-444">рекуиреусеренроллментаппровал</span><span class="sxs-lookup"><span data-stu-id="4649b-444">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="4649b-445">Логический</span><span class="sxs-lookup"><span data-stu-id="4649b-445">Boolean</span></span>|<span data-ttu-id="4649b-446">Указывает, является ли управляемое устройство iOS регистрацией на утверждение пользователя.</span><span class="sxs-lookup"><span data-stu-id="4649b-446">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="4649b-447">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-447">This property is read-only.</span></span> <span data-ttu-id="4649b-448">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-448">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-449">манажементцертификатикспиратиондате</span><span class="sxs-lookup"><span data-stu-id="4649b-449">managementCertificateExpirationDate</span></span>|<span data-ttu-id="4649b-450">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4649b-450">DateTimeOffset</span></span>|<span data-ttu-id="4649b-451">Дата окончания срока действия сертификата управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="4649b-451">Reports device management certificate expiration date.</span></span> <span data-ttu-id="4649b-452">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-452">This property is read-only.</span></span> <span data-ttu-id="4649b-453">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-453">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-454">икЦид</span><span class="sxs-lookup"><span data-stu-id="4649b-454">iccid</span></span>|<span data-ttu-id="4649b-455">Строка</span><span class="sxs-lookup"><span data-stu-id="4649b-455">String</span></span>|<span data-ttu-id="4649b-456">Идентификатор встроенной карты — это уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="4649b-456">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="4649b-457">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-457">This property is read-only.</span></span> <span data-ttu-id="4649b-458">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-458">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-459">удид</span><span class="sxs-lookup"><span data-stu-id="4649b-459">udid</span></span>|<span data-ttu-id="4649b-460">Строка</span><span class="sxs-lookup"><span data-stu-id="4649b-460">String</span></span>|<span data-ttu-id="4649b-461">Уникальный идентификатор устройства для устройств iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="4649b-461">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="4649b-462">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-462">This property is read-only.</span></span> <span data-ttu-id="4649b-463">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-463">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-464">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4649b-464">roleScopeTagIds</span></span>|<span data-ttu-id="4649b-465">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4649b-465">String collection</span></span>|<span data-ttu-id="4649b-466">Список идентификаторов тегов области для этого экземпляра устройства.</span><span class="sxs-lookup"><span data-stu-id="4649b-466">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="4649b-467">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-467">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-468">виндовсактивемалварекаунт</span><span class="sxs-lookup"><span data-stu-id="4649b-468">windowsActiveMalwareCount</span></span>|<span data-ttu-id="4649b-469">Int32</span><span class="sxs-lookup"><span data-stu-id="4649b-469">Int32</span></span>|<span data-ttu-id="4649b-470">Количество активных вредоносных программ для этого устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="4649b-470">Count of active malware for this windows device.</span></span> <span data-ttu-id="4649b-471">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-471">This property is read-only.</span></span> <span data-ttu-id="4649b-472">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-472">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-473">виндовсремедиатедмалварекаунт</span><span class="sxs-lookup"><span data-stu-id="4649b-473">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="4649b-474">Int32</span><span class="sxs-lookup"><span data-stu-id="4649b-474">Int32</span></span>|<span data-ttu-id="4649b-475">Количество исправленных вредоносных программ для этого устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="4649b-475">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="4649b-476">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-476">This property is read-only.</span></span> <span data-ttu-id="4649b-477">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-477">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-478">notes</span><span class="sxs-lookup"><span data-stu-id="4649b-478">notes</span></span>|<span data-ttu-id="4649b-479">String</span><span class="sxs-lookup"><span data-stu-id="4649b-479">String</span></span>|<span data-ttu-id="4649b-480">Примечания на устройстве, созданном администратором ИТ, унаследованном от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-480">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="4649b-481">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="4649b-482">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="4649b-482">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="4649b-483">Состояние работоспособности клиента Configuration Manager, действующее только для устройств под управлением агентов MDM/ConfigMgr, наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-483">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="4649b-484">configurationManagerClientInformation</span></span>|[<span data-ttu-id="4649b-485">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="4649b-485">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="4649b-486">Сведения о клиенте Configuration Manager, действительные только для управляемых устройств, управляемых дуел и управляемых с помощью агента Configuration Manager, наследуемого от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-486">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-487">есернетмакаддресс</span><span class="sxs-lookup"><span data-stu-id="4649b-487">ethernetMacAddress</span></span>|<span data-ttu-id="4649b-488">Строка</span><span class="sxs-lookup"><span data-stu-id="4649b-488">String</span></span>|<span data-ttu-id="4649b-489">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="4649b-489">Ethernet MAC.</span></span> <span data-ttu-id="4649b-490">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-490">This property is read-only.</span></span> <span data-ttu-id="4649b-491">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-491">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-492">фисикалмеморинбитес</span><span class="sxs-lookup"><span data-stu-id="4649b-492">physicalMemoryInBytes</span></span>|<span data-ttu-id="4649b-493">Int64</span><span class="sxs-lookup"><span data-stu-id="4649b-493">Int64</span></span>|<span data-ttu-id="4649b-494">Общий объем памяти в байтах.</span><span class="sxs-lookup"><span data-stu-id="4649b-494">Total Memory in Bytes.</span></span> <span data-ttu-id="4649b-495">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-495">This property is read-only.</span></span> <span data-ttu-id="4649b-496">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-496">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-497">процессорарчитектуре</span><span class="sxs-lookup"><span data-stu-id="4649b-497">processorArchitecture</span></span>|[<span data-ttu-id="4649b-498">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="4649b-498">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="4649b-499">Архитектура процессора.</span><span class="sxs-lookup"><span data-stu-id="4649b-499">Processor architecture.</span></span> <span data-ttu-id="4649b-500">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-500">This property is read-only.</span></span> <span data-ttu-id="4649b-501">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-501">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-502">Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="4649b-502">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="4649b-503">спеЦификатионверсион</span><span class="sxs-lookup"><span data-stu-id="4649b-503">specificationVersion</span></span>|<span data-ttu-id="4649b-504">Строка</span><span class="sxs-lookup"><span data-stu-id="4649b-504">String</span></span>|<span data-ttu-id="4649b-505">Версия спецификации.</span><span class="sxs-lookup"><span data-stu-id="4649b-505">Specification version.</span></span> <span data-ttu-id="4649b-506">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-506">This property is read-only.</span></span> <span data-ttu-id="4649b-507">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-507">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-508">joinType</span><span class="sxs-lookup"><span data-stu-id="4649b-508">joinType</span></span>|[<span data-ttu-id="4649b-509">joinType</span><span class="sxs-lookup"><span data-stu-id="4649b-509">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="4649b-510">Тип присоединения устройств наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-510">Device join type Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-511">Возможные значения: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span><span class="sxs-lookup"><span data-stu-id="4649b-511">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="4649b-512">скуфамили</span><span class="sxs-lookup"><span data-stu-id="4649b-512">skuFamily</span></span>|<span data-ttu-id="4649b-513">Строка</span><span class="sxs-lookup"><span data-stu-id="4649b-513">String</span></span>|<span data-ttu-id="4649b-514">Семейство конфигураций устройств, унаследованное от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-514">Device sku family Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-515">скунумбер</span><span class="sxs-lookup"><span data-stu-id="4649b-515">skuNumber</span></span>|<span data-ttu-id="4649b-516">Int32</span><span class="sxs-lookup"><span data-stu-id="4649b-516">Int32</span></span>|<span data-ttu-id="4649b-517">Номер SKU устройства https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo см.</span><span class="sxs-lookup"><span data-stu-id="4649b-517">Device sku number, see also: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo.</span></span> <span data-ttu-id="4649b-518">Допустимые значения: от 0 до 2147483647.</span><span class="sxs-lookup"><span data-stu-id="4649b-518">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="4649b-519">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4649b-519">This property is read-only.</span></span> <span data-ttu-id="4649b-520">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4649b-520">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4649b-521">манажементфеатурес</span><span class="sxs-lookup"><span data-stu-id="4649b-521">managementFeatures</span></span>|[<span data-ttu-id="4649b-522">managedDeviceManagementFeatures</span><span class="sxs-lookup"><span data-stu-id="4649b-522">managedDeviceManagementFeatures</span></span>](../resources/intune-devices-manageddevicemanagementfeatures.md)|<span data-ttu-id="4649b-523">Функции управления устройствами, наследуемые от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4649b-523">Device management features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4649b-524">Возможные значения: `none`, `microsoftManagedDesktop`.</span><span class="sxs-lookup"><span data-stu-id="4649b-524">Possible values are: `none`, `microsoftManagedDesktop`.</span></span>|



## <a name="response"></a><span data-ttu-id="4649b-525">Отклик</span><span class="sxs-lookup"><span data-stu-id="4649b-525">Response</span></span>
<span data-ttu-id="4649b-526">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4649b-526">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4649b-527">Пример</span><span class="sxs-lookup"><span data-stu-id="4649b-527">Example</span></span>

### <a name="request"></a><span data-ttu-id="4649b-528">Запрос</span><span class="sxs-lookup"><span data-stu-id="4649b-528">Request</span></span>
<span data-ttu-id="4649b-529">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4649b-529">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4649b-530">Отклик</span><span class="sxs-lookup"><span data-stu-id="4649b-530">Response</span></span>
<span data-ttu-id="4649b-p175">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4649b-p175">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





