---
title: Создание Виндовсманажеддевице
description: Создание нового объекта Виндовсманажеддевице.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75f6393938d8dfb72fffd4d5afe2698a0fa787fb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813672"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="b8236-103">Создание Виндовсманажеддевице</span><span class="sxs-lookup"><span data-stu-id="b8236-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="b8236-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8236-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8236-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8236-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8236-106">Создание нового объекта [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="b8236-106">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8236-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b8236-107">Prerequisites</span></span>
<span data-ttu-id="b8236-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8236-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8236-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8236-110">Permission type</span></span>|<span data-ttu-id="b8236-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8236-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8236-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8236-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b8236-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8236-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b8236-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8236-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8236-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8236-115">Not supported.</span></span>|
|<span data-ttu-id="b8236-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b8236-116">Application</span></span>|<span data-ttu-id="b8236-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8236-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8236-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8236-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="b8236-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b8236-119">Request headers</span></span>
|<span data-ttu-id="b8236-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8236-120">Header</span></span>|<span data-ttu-id="b8236-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b8236-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8236-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8236-122">Authorization</span></span>|<span data-ttu-id="b8236-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8236-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8236-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b8236-124">Accept</span></span>|<span data-ttu-id="b8236-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b8236-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8236-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8236-126">Request body</span></span>
<span data-ttu-id="b8236-127">В тексте запроса добавьте представление объекта Виндовсманажеддевице в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8236-127">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="b8236-128">В следующей таблице приведены свойства, необходимые при создании Виндовсманажеддевице.</span><span class="sxs-lookup"><span data-stu-id="b8236-128">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="b8236-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8236-129">Property</span></span>|<span data-ttu-id="b8236-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b8236-130">Type</span></span>|<span data-ttu-id="b8236-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b8236-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8236-132">id</span><span class="sxs-lookup"><span data-stu-id="b8236-132">id</span></span>|<span data-ttu-id="b8236-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b8236-133">String</span></span>|<span data-ttu-id="b8236-134">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-134">Unique Identifier for the device.</span></span> <span data-ttu-id="b8236-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-135">This property is read-only.</span></span> <span data-ttu-id="b8236-136">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-136">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-137">userId</span><span class="sxs-lookup"><span data-stu-id="b8236-137">userId</span></span>|<span data-ttu-id="b8236-138">String</span><span class="sxs-lookup"><span data-stu-id="b8236-138">String</span></span>|<span data-ttu-id="b8236-139">Уникальный идентификатор пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="b8236-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="b8236-140">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-140">This property is read-only.</span></span> <span data-ttu-id="b8236-141">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-141">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="b8236-142">deviceName</span></span>|<span data-ttu-id="b8236-143">String</span><span class="sxs-lookup"><span data-stu-id="b8236-143">String</span></span>|<span data-ttu-id="b8236-144">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-144">Name of the device.</span></span> <span data-ttu-id="b8236-145">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-145">This property is read-only.</span></span> <span data-ttu-id="b8236-146">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-146">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-147">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="b8236-147">hardwareInformation</span></span>|[<span data-ttu-id="b8236-148">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="b8236-148">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="b8236-149">Сведения о хардвард для устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-149">The hardward details for the device.</span></span>  <span data-ttu-id="b8236-150">Включает такие сведения, как место хранения, производитель, серийный номер и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-150">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="b8236-151">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-151">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-152">ownerType</span><span class="sxs-lookup"><span data-stu-id="b8236-152">ownerType</span></span>|[<span data-ttu-id="b8236-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="b8236-153">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="b8236-154">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="b8236-154">Ownership of the device.</span></span> <span data-ttu-id="b8236-155">Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b8236-155">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="b8236-156">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="b8236-156">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="b8236-157">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="b8236-157">managedDeviceOwnerType</span></span>|[<span data-ttu-id="b8236-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="b8236-158">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="b8236-159">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="b8236-159">Ownership of the device.</span></span> <span data-ttu-id="b8236-160">Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b8236-160">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="b8236-161">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="b8236-161">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="b8236-162">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="b8236-162">deviceActionResults</span></span>|<span data-ttu-id="b8236-163">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-163">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="b8236-164">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="b8236-164">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="b8236-165">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-165">This property is read-only.</span></span> <span data-ttu-id="b8236-166">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-166">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-167">манажементстате</span><span class="sxs-lookup"><span data-stu-id="b8236-167">managementState</span></span>|[<span data-ttu-id="b8236-168">манажементстате</span><span class="sxs-lookup"><span data-stu-id="b8236-168">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="b8236-169">Состояние управления для устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-169">Management state of the device.</span></span> <span data-ttu-id="b8236-170">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-170">This property is read-only.</span></span> <span data-ttu-id="b8236-171">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b8236-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="b8236-172">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="b8236-172">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="b8236-173">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="b8236-173">enrolledDateTime</span></span>|<span data-ttu-id="b8236-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8236-174">DateTimeOffset</span></span>|<span data-ttu-id="b8236-175">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-175">Enrollment time of the device.</span></span> <span data-ttu-id="b8236-176">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-176">This property is read-only.</span></span> <span data-ttu-id="b8236-177">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-177">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-178">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b8236-178">lastSyncDateTime</span></span>|<span data-ttu-id="b8236-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8236-179">DateTimeOffset</span></span>|<span data-ttu-id="b8236-180">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="b8236-180">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="b8236-181">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-181">This property is read-only.</span></span> <span data-ttu-id="b8236-182">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-182">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-183">чассистипе</span><span class="sxs-lookup"><span data-stu-id="b8236-183">chassisType</span></span>|[<span data-ttu-id="b8236-184">чассистипе</span><span class="sxs-lookup"><span data-stu-id="b8236-184">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="b8236-185">Тип корпуса устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-185">Chassis type of the device.</span></span> <span data-ttu-id="b8236-186">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-186">This property is read-only.</span></span> <span data-ttu-id="b8236-187">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b8236-187">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="b8236-188">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="b8236-188">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="b8236-189">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b8236-189">operatingSystem</span></span>|<span data-ttu-id="b8236-190">String</span><span class="sxs-lookup"><span data-stu-id="b8236-190">String</span></span>|<span data-ttu-id="b8236-191">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-191">Operating system of the device.</span></span> <span data-ttu-id="b8236-192">Windows, iOS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-192">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="b8236-193">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-193">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-194">deviceType</span><span class="sxs-lookup"><span data-stu-id="b8236-194">deviceType</span></span>|[<span data-ttu-id="b8236-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="b8236-195">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="b8236-196">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-196">Platform of the device.</span></span> <span data-ttu-id="b8236-197">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-197">This property is read-only.</span></span> <span data-ttu-id="b8236-198">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b8236-198">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="b8236-199">Возможные `desktop`значения:, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `blackberry` `palm` `unknown`,,,,,,, `iSocConsumer`,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`</span><span class="sxs-lookup"><span data-stu-id="b8236-199">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="b8236-200">complianceState</span><span class="sxs-lookup"><span data-stu-id="b8236-200">complianceState</span></span>|[<span data-ttu-id="b8236-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="b8236-201">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="b8236-202">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="b8236-202">Compliance state of the device.</span></span> <span data-ttu-id="b8236-203">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-203">This property is read-only.</span></span> <span data-ttu-id="b8236-204">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b8236-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="b8236-205">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="b8236-205">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="b8236-206">jailBroken</span><span class="sxs-lookup"><span data-stu-id="b8236-206">jailBroken</span></span>|<span data-ttu-id="b8236-207">String</span><span class="sxs-lookup"><span data-stu-id="b8236-207">String</span></span>|<span data-ttu-id="b8236-208">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="b8236-208">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="b8236-209">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-209">This property is read-only.</span></span> <span data-ttu-id="b8236-210">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-210">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-211">managementAgent</span><span class="sxs-lookup"><span data-stu-id="b8236-211">managementAgent</span></span>|[<span data-ttu-id="b8236-212">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="b8236-212">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="b8236-213">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="b8236-213">Management channel of the device.</span></span> <span data-ttu-id="b8236-214">Intune, EAS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-214">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="b8236-215">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b8236-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="b8236-216">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="b8236-216">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="b8236-217">osVersion</span><span class="sxs-lookup"><span data-stu-id="b8236-217">osVersion</span></span>|<span data-ttu-id="b8236-218">String</span><span class="sxs-lookup"><span data-stu-id="b8236-218">String</span></span>|<span data-ttu-id="b8236-219">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-219">Operating system version of the device.</span></span> <span data-ttu-id="b8236-220">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-220">This property is read-only.</span></span> <span data-ttu-id="b8236-221">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-221">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-222">easActivated</span><span class="sxs-lookup"><span data-stu-id="b8236-222">easActivated</span></span>|<span data-ttu-id="b8236-223">Логический</span><span class="sxs-lookup"><span data-stu-id="b8236-223">Boolean</span></span>|<span data-ttu-id="b8236-224">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="b8236-224">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="b8236-225">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-225">This property is read-only.</span></span> <span data-ttu-id="b8236-226">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-226">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-227">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="b8236-227">easDeviceId</span></span>|<span data-ttu-id="b8236-228">String</span><span class="sxs-lookup"><span data-stu-id="b8236-228">String</span></span>|<span data-ttu-id="b8236-229">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="b8236-229">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="b8236-230">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-230">This property is read-only.</span></span> <span data-ttu-id="b8236-231">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-231">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-232">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="b8236-232">easActivationDateTime</span></span>|<span data-ttu-id="b8236-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8236-233">DateTimeOffset</span></span>|<span data-ttu-id="b8236-234">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="b8236-234">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="b8236-235">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-235">This property is read-only.</span></span> <span data-ttu-id="b8236-236">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-237">аадрегистеред</span><span class="sxs-lookup"><span data-stu-id="b8236-237">aadRegistered</span></span>|<span data-ttu-id="b8236-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8236-238">Boolean</span></span>|<span data-ttu-id="b8236-239">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8236-239">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="b8236-240">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-240">This property is read-only.</span></span> <span data-ttu-id="b8236-241">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-241">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-242">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="b8236-242">azureADRegistered</span></span>|<span data-ttu-id="b8236-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8236-243">Boolean</span></span>|<span data-ttu-id="b8236-244">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8236-244">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="b8236-245">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-245">This property is read-only.</span></span> <span data-ttu-id="b8236-246">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-246">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-247">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="b8236-247">deviceEnrollmentType</span></span>|[<span data-ttu-id="b8236-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="b8236-248">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="b8236-249">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-249">Enrollment type of the device.</span></span> <span data-ttu-id="b8236-250">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-250">This property is read-only.</span></span> <span data-ttu-id="b8236-251">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b8236-251">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="b8236-252">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="b8236-252">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="b8236-253">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="b8236-253">lostModeState</span></span>|[<span data-ttu-id="b8236-254">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="b8236-254">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="b8236-255">Указывает, включен ли режим потерянных или отключенных.</span><span class="sxs-lookup"><span data-stu-id="b8236-255">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="b8236-256">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-256">This property is read-only.</span></span> <span data-ttu-id="b8236-257">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b8236-257">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="b8236-258">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="b8236-258">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="b8236-259">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="b8236-259">activationLockBypassCode</span></span>|<span data-ttu-id="b8236-260">String</span><span class="sxs-lookup"><span data-stu-id="b8236-260">String</span></span>|<span data-ttu-id="b8236-261">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b8236-261">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="b8236-262">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-262">This property is read-only.</span></span> <span data-ttu-id="b8236-263">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-263">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-264">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b8236-264">emailAddress</span></span>|<span data-ttu-id="b8236-265">String</span><span class="sxs-lookup"><span data-stu-id="b8236-265">String</span></span>|<span data-ttu-id="b8236-266">Сообщения электронной почты пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="b8236-266">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="b8236-267">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-267">This property is read-only.</span></span> <span data-ttu-id="b8236-268">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-269">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="b8236-269">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="b8236-270">String</span><span class="sxs-lookup"><span data-stu-id="b8236-270">String</span></span>|<span data-ttu-id="b8236-271">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8236-271">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="b8236-272">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-272">Read only.</span></span> <span data-ttu-id="b8236-273">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-273">This property is read-only.</span></span> <span data-ttu-id="b8236-274">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-275">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="b8236-275">azureADDeviceId</span></span>|<span data-ttu-id="b8236-276">String</span><span class="sxs-lookup"><span data-stu-id="b8236-276">String</span></span>|<span data-ttu-id="b8236-277">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8236-277">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="b8236-278">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-278">Read only.</span></span> <span data-ttu-id="b8236-279">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-279">This property is read-only.</span></span> <span data-ttu-id="b8236-280">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-280">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-281">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="b8236-281">deviceRegistrationState</span></span>|[<span data-ttu-id="b8236-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="b8236-282">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="b8236-283">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-283">Device registration state.</span></span> <span data-ttu-id="b8236-284">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-284">This property is read-only.</span></span> <span data-ttu-id="b8236-285">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b8236-285">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="b8236-286">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b8236-286">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="b8236-287">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="b8236-287">deviceCategoryDisplayName</span></span>|<span data-ttu-id="b8236-288">String</span><span class="sxs-lookup"><span data-stu-id="b8236-288">String</span></span>|<span data-ttu-id="b8236-289">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="b8236-289">Device category display name.</span></span> <span data-ttu-id="b8236-290">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-290">This property is read-only.</span></span> <span data-ttu-id="b8236-291">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-291">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-292">isSupervised</span><span class="sxs-lookup"><span data-stu-id="b8236-292">isSupervised</span></span>|<span data-ttu-id="b8236-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8236-293">Boolean</span></span>|<span data-ttu-id="b8236-294">Состояние контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-294">Device supervised status.</span></span> <span data-ttu-id="b8236-295">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-295">This property is read-only.</span></span> <span data-ttu-id="b8236-296">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-296">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-297">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b8236-297">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="b8236-298">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8236-298">DateTimeOffset</span></span>|<span data-ttu-id="b8236-299">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="b8236-299">Last time the device contacted Exchange.</span></span> <span data-ttu-id="b8236-300">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-300">This property is read-only.</span></span> <span data-ttu-id="b8236-301">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-301">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-302">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="b8236-302">exchangeAccessState</span></span>|[<span data-ttu-id="b8236-303">девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="b8236-303">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="b8236-304">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="b8236-304">The Access State of the device in Exchange.</span></span> <span data-ttu-id="b8236-305">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-305">This property is read-only.</span></span> <span data-ttu-id="b8236-306">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b8236-306">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="b8236-307">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="b8236-307">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="b8236-308">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="b8236-308">exchangeAccessStateReason</span></span>|[<span data-ttu-id="b8236-309">девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="b8236-309">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="b8236-310">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="b8236-310">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="b8236-311">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-311">This property is read-only.</span></span> <span data-ttu-id="b8236-312">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b8236-312">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="b8236-313">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="b8236-313">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="b8236-314">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="b8236-314">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="b8236-315">String</span><span class="sxs-lookup"><span data-stu-id="b8236-315">String</span></span>|<span data-ttu-id="b8236-316">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="b8236-316">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="b8236-317">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-317">This property is read-only.</span></span> <span data-ttu-id="b8236-318">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-318">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-319">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="b8236-319">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="b8236-320">String</span><span class="sxs-lookup"><span data-stu-id="b8236-320">String</span></span>|<span data-ttu-id="b8236-321">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="b8236-321">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="b8236-322">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-322">This property is read-only.</span></span> <span data-ttu-id="b8236-323">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-324">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="b8236-324">isEncrypted</span></span>|<span data-ttu-id="b8236-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8236-325">Boolean</span></span>|<span data-ttu-id="b8236-326">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-326">Device encryption status.</span></span> <span data-ttu-id="b8236-327">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-327">This property is read-only.</span></span> <span data-ttu-id="b8236-328">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-328">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-329">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b8236-329">userPrincipalName</span></span>|<span data-ttu-id="b8236-330">String</span><span class="sxs-lookup"><span data-stu-id="b8236-330">String</span></span>|<span data-ttu-id="b8236-331">Имя участника пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-331">Device user principal name.</span></span> <span data-ttu-id="b8236-332">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-332">This property is read-only.</span></span> <span data-ttu-id="b8236-333">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-333">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-334">model</span><span class="sxs-lookup"><span data-stu-id="b8236-334">model</span></span>|<span data-ttu-id="b8236-335">String</span><span class="sxs-lookup"><span data-stu-id="b8236-335">String</span></span>|<span data-ttu-id="b8236-336">Модель устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-336">Model of the device.</span></span> <span data-ttu-id="b8236-337">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-337">This property is read-only.</span></span> <span data-ttu-id="b8236-338">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-338">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-339">manufacturer</span><span class="sxs-lookup"><span data-stu-id="b8236-339">manufacturer</span></span>|<span data-ttu-id="b8236-340">String</span><span class="sxs-lookup"><span data-stu-id="b8236-340">String</span></span>|<span data-ttu-id="b8236-341">Производитель устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-341">Manufacturer of the device.</span></span> <span data-ttu-id="b8236-342">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-342">This property is read-only.</span></span> <span data-ttu-id="b8236-343">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-343">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-344">imei</span><span class="sxs-lookup"><span data-stu-id="b8236-344">imei</span></span>|<span data-ttu-id="b8236-345">String</span><span class="sxs-lookup"><span data-stu-id="b8236-345">String</span></span>|<span data-ttu-id="b8236-346">IMEI.</span><span class="sxs-lookup"><span data-stu-id="b8236-346">IMEI.</span></span> <span data-ttu-id="b8236-347">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-347">This property is read-only.</span></span> <span data-ttu-id="b8236-348">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-348">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-349">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b8236-349">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b8236-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8236-350">DateTimeOffset</span></span>|<span data-ttu-id="b8236-351">Дата и время истечения льготного периода соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="b8236-351">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="b8236-352">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-352">This property is read-only.</span></span> <span data-ttu-id="b8236-353">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-353">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-354">serialNumber</span><span class="sxs-lookup"><span data-stu-id="b8236-354">serialNumber</span></span>|<span data-ttu-id="b8236-355">Строка</span><span class="sxs-lookup"><span data-stu-id="b8236-355">String</span></span>|<span data-ttu-id="b8236-356">Серийный.</span><span class="sxs-lookup"><span data-stu-id="b8236-356">SerialNumber.</span></span> <span data-ttu-id="b8236-357">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-357">This property is read-only.</span></span> <span data-ttu-id="b8236-358">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-359">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="b8236-359">phoneNumber</span></span>|<span data-ttu-id="b8236-360">String</span><span class="sxs-lookup"><span data-stu-id="b8236-360">String</span></span>|<span data-ttu-id="b8236-361">Номер телефона устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-361">Phone number of the device.</span></span> <span data-ttu-id="b8236-362">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-362">This property is read-only.</span></span> <span data-ttu-id="b8236-363">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-364">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="b8236-364">androidSecurityPatchLevel</span></span>|<span data-ttu-id="b8236-365">String</span><span class="sxs-lookup"><span data-stu-id="b8236-365">String</span></span>|<span data-ttu-id="b8236-366">Уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="b8236-366">Android security patch level.</span></span> <span data-ttu-id="b8236-367">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-367">This property is read-only.</span></span> <span data-ttu-id="b8236-368">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-368">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-369">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b8236-369">userDisplayName</span></span>|<span data-ttu-id="b8236-370">String</span><span class="sxs-lookup"><span data-stu-id="b8236-370">String</span></span>|<span data-ttu-id="b8236-371">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="b8236-371">User display name.</span></span> <span data-ttu-id="b8236-372">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-372">This property is read-only.</span></span> <span data-ttu-id="b8236-373">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-374">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="b8236-374">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="b8236-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="b8236-375">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="b8236-376">Функции, поддерживающие клиент Конфигрмгр.</span><span class="sxs-lookup"><span data-stu-id="b8236-376">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="b8236-377">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-377">This property is read-only.</span></span> <span data-ttu-id="b8236-378">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-379">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="b8236-379">wiFiMacAddress</span></span>|<span data-ttu-id="b8236-380">String</span><span class="sxs-lookup"><span data-stu-id="b8236-380">String</span></span>|<span data-ttu-id="b8236-381">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b8236-381">Wi-Fi MAC.</span></span> <span data-ttu-id="b8236-382">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-382">This property is read-only.</span></span> <span data-ttu-id="b8236-383">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-383">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-384">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="b8236-384">deviceHealthAttestationState</span></span>|[<span data-ttu-id="b8236-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="b8236-385">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="b8236-386">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-386">The device health attestation state.</span></span> <span data-ttu-id="b8236-387">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-387">This property is read-only.</span></span> <span data-ttu-id="b8236-388">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-388">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-389">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="b8236-389">subscriberCarrier</span></span>|<span data-ttu-id="b8236-390">String</span><span class="sxs-lookup"><span data-stu-id="b8236-390">String</span></span>|<span data-ttu-id="b8236-391">Перевозчик абонента.</span><span class="sxs-lookup"><span data-stu-id="b8236-391">Subscriber Carrier.</span></span> <span data-ttu-id="b8236-392">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-392">This property is read-only.</span></span> <span data-ttu-id="b8236-393">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-393">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-394">meid</span><span class="sxs-lookup"><span data-stu-id="b8236-394">meid</span></span>|<span data-ttu-id="b8236-395">String</span><span class="sxs-lookup"><span data-stu-id="b8236-395">String</span></span>|<span data-ttu-id="b8236-396">MEID.</span><span class="sxs-lookup"><span data-stu-id="b8236-396">MEID.</span></span> <span data-ttu-id="b8236-397">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-397">This property is read-only.</span></span> <span data-ttu-id="b8236-398">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-398">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-399">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="b8236-399">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="b8236-400">Int64</span><span class="sxs-lookup"><span data-stu-id="b8236-400">Int64</span></span>|<span data-ttu-id="b8236-401">Общий объем хранилища в байтах.</span><span class="sxs-lookup"><span data-stu-id="b8236-401">Total Storage in Bytes.</span></span> <span data-ttu-id="b8236-402">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-402">This property is read-only.</span></span> <span data-ttu-id="b8236-403">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-403">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-404">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="b8236-404">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="b8236-405">Int64</span><span class="sxs-lookup"><span data-stu-id="b8236-405">Int64</span></span>|<span data-ttu-id="b8236-406">Свободное хранилище в байтах.</span><span class="sxs-lookup"><span data-stu-id="b8236-406">Free Storage in Bytes.</span></span> <span data-ttu-id="b8236-407">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-407">This property is read-only.</span></span> <span data-ttu-id="b8236-408">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-408">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-409">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="b8236-409">managedDeviceName</span></span>|<span data-ttu-id="b8236-410">String</span><span class="sxs-lookup"><span data-stu-id="b8236-410">String</span></span>|<span data-ttu-id="b8236-411">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-411">Automatically generated name to identify a device.</span></span> <span data-ttu-id="b8236-412">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="b8236-412">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="b8236-413">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-413">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-414">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="b8236-414">partnerReportedThreatState</span></span>|[<span data-ttu-id="b8236-415">манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="b8236-415">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="b8236-416">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="b8236-416">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="b8236-417">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-417">Read Only.</span></span> <span data-ttu-id="b8236-418">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-418">This property is read-only.</span></span> <span data-ttu-id="b8236-419">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b8236-419">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="b8236-420">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="b8236-420">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="b8236-421">ретиреафтердатетиме</span><span class="sxs-lookup"><span data-stu-id="b8236-421">retireAfterDateTime</span></span>|<span data-ttu-id="b8236-422">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8236-422">DateTimeOffset</span></span>|<span data-ttu-id="b8236-423">Указывает время, по истечении которого устройство будет автоматически снято из-за запланированного действия.</span><span class="sxs-lookup"><span data-stu-id="b8236-423">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="b8236-424">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-424">This property is read-only.</span></span> <span data-ttu-id="b8236-425">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-425">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-426">усерслогжедон</span><span class="sxs-lookup"><span data-stu-id="b8236-426">usersLoggedOn</span></span>|<span data-ttu-id="b8236-427">Коллекция [логжедонусер](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-427">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="b8236-428">Указывает последнего вошедшего в систему пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-428">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="b8236-429">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-429">This property is read-only.</span></span> <span data-ttu-id="b8236-430">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-430">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-431">префермдмоверграупполициапплиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="b8236-431">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="b8236-432">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8236-432">DateTimeOffset</span></span>|<span data-ttu-id="b8236-433">Сообщает о значении DateTime, заданном параметром Префермдмоверграупполици.</span><span class="sxs-lookup"><span data-stu-id="b8236-433">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="b8236-434">Если этот параметр установлен, параметры групповой политики в случае конфликта будут переопределяться параметрами групповой политики.</span><span class="sxs-lookup"><span data-stu-id="b8236-434">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="b8236-435">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-435">Read Only.</span></span> <span data-ttu-id="b8236-436">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-436">This property is read-only.</span></span> <span data-ttu-id="b8236-437">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-437">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-438">аутопилотенроллед</span><span class="sxs-lookup"><span data-stu-id="b8236-438">autopilotEnrolled</span></span>|<span data-ttu-id="b8236-439">Логический</span><span class="sxs-lookup"><span data-stu-id="b8236-439">Boolean</span></span>|<span data-ttu-id="b8236-440">Сообщает, зарегистрировано ли управляемое устройство через Автоматический пилот.</span><span class="sxs-lookup"><span data-stu-id="b8236-440">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="b8236-441">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-441">This property is read-only.</span></span> <span data-ttu-id="b8236-442">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-442">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-443">рекуиреусеренроллментаппровал</span><span class="sxs-lookup"><span data-stu-id="b8236-443">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="b8236-444">Логический</span><span class="sxs-lookup"><span data-stu-id="b8236-444">Boolean</span></span>|<span data-ttu-id="b8236-445">Указывает, является ли управляемое устройство iOS регистрацией на утверждение пользователя.</span><span class="sxs-lookup"><span data-stu-id="b8236-445">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="b8236-446">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-446">This property is read-only.</span></span> <span data-ttu-id="b8236-447">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-447">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-448">манажементцертификатикспиратиондате</span><span class="sxs-lookup"><span data-stu-id="b8236-448">managementCertificateExpirationDate</span></span>|<span data-ttu-id="b8236-449">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8236-449">DateTimeOffset</span></span>|<span data-ttu-id="b8236-450">Дата окончания срока действия сертификата управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="b8236-450">Reports device management certificate expiration date.</span></span> <span data-ttu-id="b8236-451">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-451">This property is read-only.</span></span> <span data-ttu-id="b8236-452">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-452">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-453">икЦид</span><span class="sxs-lookup"><span data-stu-id="b8236-453">iccid</span></span>|<span data-ttu-id="b8236-454">String</span><span class="sxs-lookup"><span data-stu-id="b8236-454">String</span></span>|<span data-ttu-id="b8236-455">Идентификатор встроенной карты — это уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="b8236-455">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="b8236-456">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-456">This property is read-only.</span></span> <span data-ttu-id="b8236-457">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-457">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-458">удид</span><span class="sxs-lookup"><span data-stu-id="b8236-458">udid</span></span>|<span data-ttu-id="b8236-459">String</span><span class="sxs-lookup"><span data-stu-id="b8236-459">String</span></span>|<span data-ttu-id="b8236-460">Уникальный идентификатор устройства для устройств iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="b8236-460">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="b8236-461">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-461">This property is read-only.</span></span> <span data-ttu-id="b8236-462">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-462">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-463">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b8236-463">roleScopeTagIds</span></span>|<span data-ttu-id="b8236-464">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b8236-464">String collection</span></span>|<span data-ttu-id="b8236-465">Список идентификаторов тегов области для этого экземпляра устройства.</span><span class="sxs-lookup"><span data-stu-id="b8236-465">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="b8236-466">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-466">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-467">виндовсактивемалварекаунт</span><span class="sxs-lookup"><span data-stu-id="b8236-467">windowsActiveMalwareCount</span></span>|<span data-ttu-id="b8236-468">Int32</span><span class="sxs-lookup"><span data-stu-id="b8236-468">Int32</span></span>|<span data-ttu-id="b8236-469">Количество активных вредоносных программ для этого устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="b8236-469">Count of active malware for this windows device.</span></span> <span data-ttu-id="b8236-470">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-470">This property is read-only.</span></span> <span data-ttu-id="b8236-471">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-471">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-472">виндовсремедиатедмалварекаунт</span><span class="sxs-lookup"><span data-stu-id="b8236-472">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="b8236-473">Int32</span><span class="sxs-lookup"><span data-stu-id="b8236-473">Int32</span></span>|<span data-ttu-id="b8236-474">Количество исправленных вредоносных программ для этого устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="b8236-474">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="b8236-475">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-475">This property is read-only.</span></span> <span data-ttu-id="b8236-476">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-476">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-477">notes</span><span class="sxs-lookup"><span data-stu-id="b8236-477">notes</span></span>|<span data-ttu-id="b8236-478">String</span><span class="sxs-lookup"><span data-stu-id="b8236-478">String</span></span>|<span data-ttu-id="b8236-479">Примечания на устройстве, созданном администратором ИТ, унаследованном от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-479">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-480">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="b8236-480">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="b8236-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="b8236-481">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="b8236-482">Состояние работоспособности клиента Configuration Manager, действующее только для устройств под управлением агентов MDM/ConfigMgr, наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-482">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-483">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="b8236-483">configurationManagerClientInformation</span></span>|[<span data-ttu-id="b8236-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="b8236-484">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="b8236-485">Сведения о клиенте Configuration Manager, действительные только для управляемых устройств, управляемых дуел и управляемых с помощью агента Configuration Manager, наследуемого от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-485">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-486">есернетмакаддресс</span><span class="sxs-lookup"><span data-stu-id="b8236-486">ethernetMacAddress</span></span>|<span data-ttu-id="b8236-487">String</span><span class="sxs-lookup"><span data-stu-id="b8236-487">String</span></span>|<span data-ttu-id="b8236-488">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="b8236-488">Ethernet MAC.</span></span> <span data-ttu-id="b8236-489">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-489">This property is read-only.</span></span> <span data-ttu-id="b8236-490">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-490">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-491">фисикалмеморинбитес</span><span class="sxs-lookup"><span data-stu-id="b8236-491">physicalMemoryInBytes</span></span>|<span data-ttu-id="b8236-492">Int64</span><span class="sxs-lookup"><span data-stu-id="b8236-492">Int64</span></span>|<span data-ttu-id="b8236-493">Общий объем памяти в байтах.</span><span class="sxs-lookup"><span data-stu-id="b8236-493">Total Memory in Bytes.</span></span> <span data-ttu-id="b8236-494">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-494">This property is read-only.</span></span> <span data-ttu-id="b8236-495">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b8236-495">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="b8236-496">процессорарчитектуре</span><span class="sxs-lookup"><span data-stu-id="b8236-496">processorArchitecture</span></span>|[<span data-ttu-id="b8236-497">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="b8236-497">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="b8236-498">Архитектура процессора.</span><span class="sxs-lookup"><span data-stu-id="b8236-498">Processor architecture.</span></span> <span data-ttu-id="b8236-499">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8236-499">This property is read-only.</span></span> <span data-ttu-id="b8236-500">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b8236-500">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="b8236-501">Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="b8236-501">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|



## <a name="response"></a><span data-ttu-id="b8236-502">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8236-502">Response</span></span>
<span data-ttu-id="b8236-503">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b8236-503">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8236-504">Пример</span><span class="sxs-lookup"><span data-stu-id="b8236-504">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8236-505">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8236-505">Request</span></span>
<span data-ttu-id="b8236-506">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8236-506">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 7665

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
    "clientIdentifier": "Client Identifier value",
    "isBlocked": true
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86"
}
```

### <a name="response"></a><span data-ttu-id="b8236-507">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8236-507">Response</span></span>
<span data-ttu-id="b8236-p171">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8236-p171">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7714

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
    "clientIdentifier": "Client Identifier value",
    "isBlocked": true
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86"
}
```




