---
title: Создание windowsManagedDevice
description: Создайте новый объект WindowsManagedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b1d8bd8e1651a2549777e0c668420f229305e4c
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611771"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="ab691-103">Создание windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="ab691-103">Create windowsManagedDevice</span></span>

<span data-ttu-id="ab691-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab691-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab691-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab691-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab691-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab691-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab691-107">Создайте [новый объект WindowsManagedDevice.](../resources/intune-devices-windowsmanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-107">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab691-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ab691-108">Prerequisites</span></span>
<span data-ttu-id="ab691-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab691-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab691-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab691-111">Permission type</span></span>|<span data-ttu-id="ab691-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab691-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab691-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab691-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab691-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab691-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ab691-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab691-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab691-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab691-116">Not supported.</span></span>|
|<span data-ttu-id="ab691-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ab691-117">Application</span></span>|<span data-ttu-id="ab691-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab691-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab691-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab691-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/comanagedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="ab691-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ab691-120">Request headers</span></span>
|<span data-ttu-id="ab691-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab691-121">Header</span></span>|<span data-ttu-id="ab691-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ab691-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab691-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab691-123">Authorization</span></span>|<span data-ttu-id="ab691-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab691-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab691-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab691-125">Accept</span></span>|<span data-ttu-id="ab691-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab691-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab691-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab691-127">Request body</span></span>
<span data-ttu-id="ab691-128">В теле запроса поставляем представление JSON для объекта WindowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="ab691-128">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="ab691-129">В следующей таблице показаны свойства, необходимые при создании windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="ab691-129">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="ab691-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab691-130">Property</span></span>|<span data-ttu-id="ab691-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ab691-131">Type</span></span>|<span data-ttu-id="ab691-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ab691-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab691-133">id</span><span class="sxs-lookup"><span data-stu-id="ab691-133">id</span></span>|<span data-ttu-id="ab691-134">String</span><span class="sxs-lookup"><span data-stu-id="ab691-134">String</span></span>|<span data-ttu-id="ab691-135">Уникальный идентификатор для устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-135">Unique Identifier for the device.</span></span> <span data-ttu-id="ab691-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-136">This property is read-only.</span></span> <span data-ttu-id="ab691-137">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-137">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-138">userId</span><span class="sxs-lookup"><span data-stu-id="ab691-138">userId</span></span>|<span data-ttu-id="ab691-139">String</span><span class="sxs-lookup"><span data-stu-id="ab691-139">String</span></span>|<span data-ttu-id="ab691-140">Уникальный идентификатор для пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="ab691-140">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="ab691-141">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-141">This property is read-only.</span></span> <span data-ttu-id="ab691-142">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-142">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="ab691-143">deviceName</span></span>|<span data-ttu-id="ab691-144">String</span><span class="sxs-lookup"><span data-stu-id="ab691-144">String</span></span>|<span data-ttu-id="ab691-145">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-145">Name of the device.</span></span> <span data-ttu-id="ab691-146">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-146">This property is read-only.</span></span> <span data-ttu-id="ab691-147">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-147">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="ab691-148">hardwareInformation</span></span>|[<span data-ttu-id="ab691-149">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="ab691-149">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="ab691-150">Подробные сведения для устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-150">The hardward details for the device.</span></span>  <span data-ttu-id="ab691-151">Включает такие сведения, как пространство для хранения, производитель, серийный номер и т.д. Это свойство только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-151">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="ab691-152">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-152">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="ab691-153">ownerType</span></span>|[<span data-ttu-id="ab691-154">ownerType</span><span class="sxs-lookup"><span data-stu-id="ab691-154">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="ab691-155">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="ab691-155">Ownership of the device.</span></span> <span data-ttu-id="ab691-156">Может быть "company" или "personal" Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab691-156">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-157">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="ab691-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ab691-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ab691-158">managedDeviceOwnerType</span></span>|[<span data-ttu-id="ab691-159">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ab691-159">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="ab691-160">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="ab691-160">Ownership of the device.</span></span> <span data-ttu-id="ab691-161">Может быть "company" или "personal" Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab691-161">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-162">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="ab691-162">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ab691-163">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="ab691-163">deviceActionResults</span></span>|<span data-ttu-id="ab691-164">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="ab691-165">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="ab691-165">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="ab691-166">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-166">This property is read-only.</span></span> <span data-ttu-id="ab691-167">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-168">managementState</span><span class="sxs-lookup"><span data-stu-id="ab691-168">managementState</span></span>|[<span data-ttu-id="ab691-169">managementState</span><span class="sxs-lookup"><span data-stu-id="ab691-169">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="ab691-170">Состояние управления устройством.</span><span class="sxs-lookup"><span data-stu-id="ab691-170">Management state of the device.</span></span> <span data-ttu-id="ab691-171">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-171">This property is read-only.</span></span> <span data-ttu-id="ab691-172">Унаследовано от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab691-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-173">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="ab691-173">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="ab691-174">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="ab691-174">enrolledDateTime</span></span>|<span data-ttu-id="ab691-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab691-175">DateTimeOffset</span></span>|<span data-ttu-id="ab691-176">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-176">Enrollment time of the device.</span></span> <span data-ttu-id="ab691-177">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-177">This property is read-only.</span></span> <span data-ttu-id="ab691-178">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-178">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-179">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ab691-179">lastSyncDateTime</span></span>|<span data-ttu-id="ab691-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab691-180">DateTimeOffset</span></span>|<span data-ttu-id="ab691-181">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="ab691-181">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="ab691-182">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-182">This property is read-only.</span></span> <span data-ttu-id="ab691-183">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-183">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="ab691-184">chassisType</span></span>|[<span data-ttu-id="ab691-185">chassisType</span><span class="sxs-lookup"><span data-stu-id="ab691-185">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="ab691-186">Тип шасси устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-186">Chassis type of the device.</span></span> <span data-ttu-id="ab691-187">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-187">This property is read-only.</span></span> <span data-ttu-id="ab691-188">Унаследовано от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab691-188">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-189">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="ab691-189">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="ab691-190">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="ab691-190">operatingSystem</span></span>|<span data-ttu-id="ab691-191">String</span><span class="sxs-lookup"><span data-stu-id="ab691-191">String</span></span>|<span data-ttu-id="ab691-192">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-192">Operating system of the device.</span></span> <span data-ttu-id="ab691-193">Windows, iOS и т. д. Это свойство только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-193">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="ab691-194">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="ab691-195">deviceType</span></span>|[<span data-ttu-id="ab691-196">deviceType</span><span class="sxs-lookup"><span data-stu-id="ab691-196">deviceType</span></span>](../resources/intune-devices-devicetype.md)|<span data-ttu-id="ab691-197">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-197">Platform of the device.</span></span> <span data-ttu-id="ab691-198">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-198">This property is read-only.</span></span> <span data-ttu-id="ab691-199">Унаследовано от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab691-199">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-200">Возможные значения: `desktop` `windowsRT` , `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `chromeOS` `linux` `blackberry` `palm` , `unknown` `cloudPC` , .</span><span class="sxs-lookup"><span data-stu-id="ab691-200">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `chromeOS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="ab691-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="ab691-201">complianceState</span></span>|[<span data-ttu-id="ab691-202">complianceState</span><span class="sxs-lookup"><span data-stu-id="ab691-202">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="ab691-203">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="ab691-203">Compliance state of the device.</span></span> <span data-ttu-id="ab691-204">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-204">This property is read-only.</span></span> <span data-ttu-id="ab691-205">Унаследовано от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab691-205">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-206">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="ab691-206">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="ab691-207">jailBroken</span><span class="sxs-lookup"><span data-stu-id="ab691-207">jailBroken</span></span>|<span data-ttu-id="ab691-208">String</span><span class="sxs-lookup"><span data-stu-id="ab691-208">String</span></span>|<span data-ttu-id="ab691-209">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="ab691-209">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="ab691-210">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-210">This property is read-only.</span></span> <span data-ttu-id="ab691-211">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-212">managementAgent</span><span class="sxs-lookup"><span data-stu-id="ab691-212">managementAgent</span></span>|[<span data-ttu-id="ab691-213">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="ab691-213">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="ab691-214">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="ab691-214">Management channel of the device.</span></span> <span data-ttu-id="ab691-215">Intune, EAS и т. д. Это свойство только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-215">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="ab691-216">Унаследовано от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab691-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-217">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="ab691-217">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="ab691-218">osVersion</span><span class="sxs-lookup"><span data-stu-id="ab691-218">osVersion</span></span>|<span data-ttu-id="ab691-219">String</span><span class="sxs-lookup"><span data-stu-id="ab691-219">String</span></span>|<span data-ttu-id="ab691-220">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-220">Operating system version of the device.</span></span> <span data-ttu-id="ab691-221">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-221">This property is read-only.</span></span> <span data-ttu-id="ab691-222">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-222">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-223">easActivated</span><span class="sxs-lookup"><span data-stu-id="ab691-223">easActivated</span></span>|<span data-ttu-id="ab691-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab691-224">Boolean</span></span>|<span data-ttu-id="ab691-225">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="ab691-225">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="ab691-226">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-226">This property is read-only.</span></span> <span data-ttu-id="ab691-227">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="ab691-228">easDeviceId</span></span>|<span data-ttu-id="ab691-229">String</span><span class="sxs-lookup"><span data-stu-id="ab691-229">String</span></span>|<span data-ttu-id="ab691-230">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="ab691-230">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="ab691-231">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-231">This property is read-only.</span></span> <span data-ttu-id="ab691-232">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-232">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-233">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="ab691-233">easActivationDateTime</span></span>|<span data-ttu-id="ab691-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab691-234">DateTimeOffset</span></span>|<span data-ttu-id="ab691-235">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="ab691-235">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="ab691-236">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-236">This property is read-only.</span></span> <span data-ttu-id="ab691-237">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-238">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="ab691-238">aadRegistered</span></span>|<span data-ttu-id="ab691-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab691-239">Boolean</span></span>|<span data-ttu-id="ab691-240">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ab691-240">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="ab691-241">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-241">This property is read-only.</span></span> <span data-ttu-id="ab691-242">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-242">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-243">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="ab691-243">azureADRegistered</span></span>|<span data-ttu-id="ab691-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab691-244">Boolean</span></span>|<span data-ttu-id="ab691-245">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ab691-245">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="ab691-246">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-246">This property is read-only.</span></span> <span data-ttu-id="ab691-247">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-247">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ab691-248">deviceEnrollmentType</span></span>|[<span data-ttu-id="ab691-249">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ab691-249">deviceEnrollmentType</span></span>](../resources/intune-devices-deviceenrollmenttype.md)|<span data-ttu-id="ab691-250">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-250">Enrollment type of the device.</span></span> <span data-ttu-id="ab691-251">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-251">This property is read-only.</span></span> <span data-ttu-id="ab691-252">Унаследовано от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab691-252">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-253">Возможные значения: `unknown` `userEnrollment` , , , , , `deviceEnrollmentManager` , , `appleBulkWithUser` , `appleBulkWithoutUser` `windowsAzureADJoin` `windowsBulkUserless` `windowsAutoEnrollment` `windowsBulkAzureDomainJoin` `windowsCoManagement` `windowsAzureADJoinUsingDeviceAuth` `appleUserEnrollment` `appleUserEnrollmentWithServiceAccount` `azureAdJoinUsingAzureVmExtension` `androidEnterpriseDedicatedDevice` `androidEnterpriseFullyManaged` `androidEnterpriseCorporateWorkProfile` .</span><span class="sxs-lookup"><span data-stu-id="ab691-253">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="ab691-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="ab691-254">lostModeState</span></span>|[<span data-ttu-id="ab691-255">lostModeState</span><span class="sxs-lookup"><span data-stu-id="ab691-255">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="ab691-256">Указывает, включен или отключен режим Lost.</span><span class="sxs-lookup"><span data-stu-id="ab691-256">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="ab691-257">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-257">This property is read-only.</span></span> <span data-ttu-id="ab691-258">Унаследовано от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab691-258">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-259">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="ab691-259">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="ab691-260">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="ab691-260">activationLockBypassCode</span></span>|<span data-ttu-id="ab691-261">String</span><span class="sxs-lookup"><span data-stu-id="ab691-261">String</span></span>|<span data-ttu-id="ab691-262">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="ab691-262">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="ab691-263">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-263">This property is read-only.</span></span> <span data-ttu-id="ab691-264">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-265">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ab691-265">emailAddress</span></span>|<span data-ttu-id="ab691-266">String</span><span class="sxs-lookup"><span data-stu-id="ab691-266">String</span></span>|<span data-ttu-id="ab691-267">Электронная почта (ы) для пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="ab691-267">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="ab691-268">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-268">This property is read-only.</span></span> <span data-ttu-id="ab691-269">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-270">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="ab691-270">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="ab691-271">String</span><span class="sxs-lookup"><span data-stu-id="ab691-271">String</span></span>|<span data-ttu-id="ab691-272">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ab691-272">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="ab691-273">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-273">Read only.</span></span> <span data-ttu-id="ab691-274">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-274">This property is read-only.</span></span> <span data-ttu-id="ab691-275">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-275">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-276">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="ab691-276">azureADDeviceId</span></span>|<span data-ttu-id="ab691-277">String</span><span class="sxs-lookup"><span data-stu-id="ab691-277">String</span></span>|<span data-ttu-id="ab691-278">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ab691-278">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="ab691-279">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-279">Read only.</span></span> <span data-ttu-id="ab691-280">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-280">This property is read-only.</span></span> <span data-ttu-id="ab691-281">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-281">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ab691-282">deviceRegistrationState</span></span>|[<span data-ttu-id="ab691-283">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ab691-283">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="ab691-284">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-284">Device registration state.</span></span> <span data-ttu-id="ab691-285">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-285">This property is read-only.</span></span> <span data-ttu-id="ab691-286">Унаследовано от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab691-286">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-287">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ab691-287">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="ab691-288">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="ab691-288">deviceCategoryDisplayName</span></span>|<span data-ttu-id="ab691-289">String</span><span class="sxs-lookup"><span data-stu-id="ab691-289">String</span></span>|<span data-ttu-id="ab691-290">Имя отображения категории устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-290">Device category display name.</span></span> <span data-ttu-id="ab691-291">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-291">This property is read-only.</span></span> <span data-ttu-id="ab691-292">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-292">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-293">isSupervised</span><span class="sxs-lookup"><span data-stu-id="ab691-293">isSupervised</span></span>|<span data-ttu-id="ab691-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab691-294">Boolean</span></span>|<span data-ttu-id="ab691-295">Состояние под контролем устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-295">Device supervised status.</span></span> <span data-ttu-id="ab691-296">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-296">This property is read-only.</span></span> <span data-ttu-id="ab691-297">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-297">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-298">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ab691-298">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="ab691-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab691-299">DateTimeOffset</span></span>|<span data-ttu-id="ab691-300">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab691-300">Last time the device contacted Exchange.</span></span> <span data-ttu-id="ab691-301">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-301">This property is read-only.</span></span> <span data-ttu-id="ab691-302">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-302">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="ab691-303">exchangeAccessState</span></span>|[<span data-ttu-id="ab691-304">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="ab691-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="ab691-305">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab691-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="ab691-306">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-306">This property is read-only.</span></span> <span data-ttu-id="ab691-307">Унаследовано от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab691-307">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-308">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="ab691-308">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="ab691-309">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="ab691-309">exchangeAccessStateReason</span></span>|[<span data-ttu-id="ab691-310">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="ab691-310">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="ab691-311">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab691-311">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="ab691-312">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-312">This property is read-only.</span></span> <span data-ttu-id="ab691-313">Унаследовано от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab691-313">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-314">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="ab691-314">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="ab691-315">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="ab691-315">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="ab691-316">String</span><span class="sxs-lookup"><span data-stu-id="ab691-316">String</span></span>|<span data-ttu-id="ab691-317">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="ab691-317">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="ab691-318">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-318">This property is read-only.</span></span> <span data-ttu-id="ab691-319">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-319">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-320">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ab691-320">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="ab691-321">String</span><span class="sxs-lookup"><span data-stu-id="ab691-321">String</span></span>|<span data-ttu-id="ab691-322">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="ab691-322">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="ab691-323">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-323">This property is read-only.</span></span> <span data-ttu-id="ab691-324">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-324">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="ab691-325">isEncrypted</span></span>|<span data-ttu-id="ab691-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab691-326">Boolean</span></span>|<span data-ttu-id="ab691-327">Состояние шифрования устройств.</span><span class="sxs-lookup"><span data-stu-id="ab691-327">Device encryption status.</span></span> <span data-ttu-id="ab691-328">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-328">This property is read-only.</span></span> <span data-ttu-id="ab691-329">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-329">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-330">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ab691-330">userPrincipalName</span></span>|<span data-ttu-id="ab691-331">String</span><span class="sxs-lookup"><span data-stu-id="ab691-331">String</span></span>|<span data-ttu-id="ab691-332">Имя основного пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-332">Device user principal name.</span></span> <span data-ttu-id="ab691-333">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-333">This property is read-only.</span></span> <span data-ttu-id="ab691-334">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-334">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-335">model</span><span class="sxs-lookup"><span data-stu-id="ab691-335">model</span></span>|<span data-ttu-id="ab691-336">String</span><span class="sxs-lookup"><span data-stu-id="ab691-336">String</span></span>|<span data-ttu-id="ab691-337">Модель устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-337">Model of the device.</span></span> <span data-ttu-id="ab691-338">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-338">This property is read-only.</span></span> <span data-ttu-id="ab691-339">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-340">manufacturer</span><span class="sxs-lookup"><span data-stu-id="ab691-340">manufacturer</span></span>|<span data-ttu-id="ab691-341">String</span><span class="sxs-lookup"><span data-stu-id="ab691-341">String</span></span>|<span data-ttu-id="ab691-342">Производитель устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-342">Manufacturer of the device.</span></span> <span data-ttu-id="ab691-343">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-343">This property is read-only.</span></span> <span data-ttu-id="ab691-344">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-345">imei</span><span class="sxs-lookup"><span data-stu-id="ab691-345">imei</span></span>|<span data-ttu-id="ab691-346">String</span><span class="sxs-lookup"><span data-stu-id="ab691-346">String</span></span>|<span data-ttu-id="ab691-347">IMEI.</span><span class="sxs-lookup"><span data-stu-id="ab691-347">IMEI.</span></span> <span data-ttu-id="ab691-348">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-348">This property is read-only.</span></span> <span data-ttu-id="ab691-349">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-349">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-350">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ab691-350">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ab691-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab691-351">DateTimeOffset</span></span>|<span data-ttu-id="ab691-352">DateTime, когда истекает срок действия льготного периода соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-352">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="ab691-353">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-353">This property is read-only.</span></span> <span data-ttu-id="ab691-354">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-355">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ab691-355">serialNumber</span></span>|<span data-ttu-id="ab691-356">String</span><span class="sxs-lookup"><span data-stu-id="ab691-356">String</span></span>|<span data-ttu-id="ab691-357">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="ab691-357">SerialNumber.</span></span> <span data-ttu-id="ab691-358">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-358">This property is read-only.</span></span> <span data-ttu-id="ab691-359">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-360">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="ab691-360">phoneNumber</span></span>|<span data-ttu-id="ab691-361">String</span><span class="sxs-lookup"><span data-stu-id="ab691-361">String</span></span>|<span data-ttu-id="ab691-362">Номер телефона устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-362">Phone number of the device.</span></span> <span data-ttu-id="ab691-363">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-363">This property is read-only.</span></span> <span data-ttu-id="ab691-364">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-364">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-365">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="ab691-365">androidSecurityPatchLevel</span></span>|<span data-ttu-id="ab691-366">String</span><span class="sxs-lookup"><span data-stu-id="ab691-366">String</span></span>|<span data-ttu-id="ab691-367">Уровень исправления безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="ab691-367">Android security patch level.</span></span> <span data-ttu-id="ab691-368">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-368">This property is read-only.</span></span> <span data-ttu-id="ab691-369">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-370">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ab691-370">userDisplayName</span></span>|<span data-ttu-id="ab691-371">String</span><span class="sxs-lookup"><span data-stu-id="ab691-371">String</span></span>|<span data-ttu-id="ab691-372">Имя отображения пользователя.</span><span class="sxs-lookup"><span data-stu-id="ab691-372">User display name.</span></span> <span data-ttu-id="ab691-373">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-373">This property is read-only.</span></span> <span data-ttu-id="ab691-374">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="ab691-375">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="ab691-376">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="ab691-376">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="ab691-377">Функции с включенной поддержкой клиента ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="ab691-377">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="ab691-378">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-378">This property is read-only.</span></span> <span data-ttu-id="ab691-379">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-379">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-380">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="ab691-380">wiFiMacAddress</span></span>|<span data-ttu-id="ab691-381">String</span><span class="sxs-lookup"><span data-stu-id="ab691-381">String</span></span>|<span data-ttu-id="ab691-382">Wi-Fi MAC.</span><span class="sxs-lookup"><span data-stu-id="ab691-382">Wi-Fi MAC.</span></span> <span data-ttu-id="ab691-383">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-383">This property is read-only.</span></span> <span data-ttu-id="ab691-384">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-384">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="ab691-385">deviceHealthAttestationState</span></span>|[<span data-ttu-id="ab691-386">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="ab691-386">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="ab691-387">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-387">The device health attestation state.</span></span> <span data-ttu-id="ab691-388">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-388">This property is read-only.</span></span> <span data-ttu-id="ab691-389">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-389">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-390">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="ab691-390">subscriberCarrier</span></span>|<span data-ttu-id="ab691-391">String</span><span class="sxs-lookup"><span data-stu-id="ab691-391">String</span></span>|<span data-ttu-id="ab691-392">Оператор абонентов.</span><span class="sxs-lookup"><span data-stu-id="ab691-392">Subscriber Carrier.</span></span> <span data-ttu-id="ab691-393">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-393">This property is read-only.</span></span> <span data-ttu-id="ab691-394">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-394">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-395">meid</span><span class="sxs-lookup"><span data-stu-id="ab691-395">meid</span></span>|<span data-ttu-id="ab691-396">String</span><span class="sxs-lookup"><span data-stu-id="ab691-396">String</span></span>|<span data-ttu-id="ab691-397">MEID.</span><span class="sxs-lookup"><span data-stu-id="ab691-397">MEID.</span></span> <span data-ttu-id="ab691-398">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-398">This property is read-only.</span></span> <span data-ttu-id="ab691-399">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-399">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-400">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="ab691-400">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="ab691-401">Int64</span><span class="sxs-lookup"><span data-stu-id="ab691-401">Int64</span></span>|<span data-ttu-id="ab691-402">Общее хранилище в bytes.</span><span class="sxs-lookup"><span data-stu-id="ab691-402">Total Storage in Bytes.</span></span> <span data-ttu-id="ab691-403">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-403">This property is read-only.</span></span> <span data-ttu-id="ab691-404">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-404">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-405">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="ab691-405">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="ab691-406">Int64</span><span class="sxs-lookup"><span data-stu-id="ab691-406">Int64</span></span>|<span data-ttu-id="ab691-407">Бесплатное хранение в bytes.</span><span class="sxs-lookup"><span data-stu-id="ab691-407">Free Storage in Bytes.</span></span> <span data-ttu-id="ab691-408">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-408">This property is read-only.</span></span> <span data-ttu-id="ab691-409">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-409">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-410">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="ab691-410">managedDeviceName</span></span>|<span data-ttu-id="ab691-411">String</span><span class="sxs-lookup"><span data-stu-id="ab691-411">String</span></span>|<span data-ttu-id="ab691-412">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-412">Automatically generated name to identify a device.</span></span> <span data-ttu-id="ab691-413">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="ab691-413">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="ab691-414">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-414">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-415">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="ab691-415">partnerReportedThreatState</span></span>|[<span data-ttu-id="ab691-416">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="ab691-416">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="ab691-417">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="ab691-417">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="ab691-418">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-418">Read Only.</span></span> <span data-ttu-id="ab691-419">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-419">This property is read-only.</span></span> <span data-ttu-id="ab691-420">Унаследовано от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab691-420">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-421">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="ab691-421">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="ab691-422">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="ab691-422">retireAfterDateTime</span></span>|<span data-ttu-id="ab691-423">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab691-423">DateTimeOffset</span></span>|<span data-ttu-id="ab691-424">Указывает время после автоматической отставку устройства из-за запланированных действий.</span><span class="sxs-lookup"><span data-stu-id="ab691-424">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="ab691-425">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-425">This property is read-only.</span></span> <span data-ttu-id="ab691-426">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-426">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-427">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="ab691-427">usersLoggedOn</span></span>|<span data-ttu-id="ab691-428">[коллекция loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="ab691-429">Указывает последний вход в систему для пользователей устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-429">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="ab691-430">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-430">This property is read-only.</span></span> <span data-ttu-id="ab691-431">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-431">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-432">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab691-432">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="ab691-433">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab691-433">DateTimeOffset</span></span>|<span data-ttu-id="ab691-434">Сообщает dateTime, задав параметр preferMdmOverGroupPolicy.</span><span class="sxs-lookup"><span data-stu-id="ab691-434">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="ab691-435">При задании параметры MDM Intune переопределяют параметры групповой политики в случае конфликта.</span><span class="sxs-lookup"><span data-stu-id="ab691-435">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="ab691-436">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-436">Read Only.</span></span> <span data-ttu-id="ab691-437">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-437">This property is read-only.</span></span> <span data-ttu-id="ab691-438">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-438">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-439">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="ab691-439">autopilotEnrolled</span></span>|<span data-ttu-id="ab691-440">Логический</span><span class="sxs-lookup"><span data-stu-id="ab691-440">Boolean</span></span>|<span data-ttu-id="ab691-441">Отчеты о регистрации управляемого устройства с помощью автопилотирования.</span><span class="sxs-lookup"><span data-stu-id="ab691-441">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="ab691-442">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-442">This property is read-only.</span></span> <span data-ttu-id="ab691-443">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-443">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-444">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="ab691-444">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="ab691-445">Логический</span><span class="sxs-lookup"><span data-stu-id="ab691-445">Boolean</span></span>|<span data-ttu-id="ab691-446">Отчеты о том, является ли управляемое устройство iOS регистрацией пользователя.</span><span class="sxs-lookup"><span data-stu-id="ab691-446">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="ab691-447">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-447">This property is read-only.</span></span> <span data-ttu-id="ab691-448">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-448">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-449">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="ab691-449">managementCertificateExpirationDate</span></span>|<span data-ttu-id="ab691-450">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab691-450">DateTimeOffset</span></span>|<span data-ttu-id="ab691-451">Отчеты о сроках действия сертификата управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="ab691-451">Reports device management certificate expiration date.</span></span> <span data-ttu-id="ab691-452">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-452">This property is read-only.</span></span> <span data-ttu-id="ab691-453">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-453">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-454">iccid</span><span class="sxs-lookup"><span data-stu-id="ab691-454">iccid</span></span>|<span data-ttu-id="ab691-455">String</span><span class="sxs-lookup"><span data-stu-id="ab691-455">String</span></span>|<span data-ttu-id="ab691-456">Интегрированный идентификатор карты схемы — уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="ab691-456">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="ab691-457">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-457">This property is read-only.</span></span> <span data-ttu-id="ab691-458">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-458">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-459">udid</span><span class="sxs-lookup"><span data-stu-id="ab691-459">udid</span></span>|<span data-ttu-id="ab691-460">String</span><span class="sxs-lookup"><span data-stu-id="ab691-460">String</span></span>|<span data-ttu-id="ab691-461">Уникальный идентификатор устройства для устройств с iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="ab691-461">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="ab691-462">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-462">This property is read-only.</span></span> <span data-ttu-id="ab691-463">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-463">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-464">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ab691-464">roleScopeTagIds</span></span>|<span data-ttu-id="ab691-465">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ab691-465">String collection</span></span>|<span data-ttu-id="ab691-466">Список ID-тегов области для этого экземпляра устройства.</span><span class="sxs-lookup"><span data-stu-id="ab691-466">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="ab691-467">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-467">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-468">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="ab691-468">windowsActiveMalwareCount</span></span>|<span data-ttu-id="ab691-469">Int32</span><span class="sxs-lookup"><span data-stu-id="ab691-469">Int32</span></span>|<span data-ttu-id="ab691-470">Количество активных вредоносных программ для этого устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="ab691-470">Count of active malware for this windows device.</span></span> <span data-ttu-id="ab691-471">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-471">This property is read-only.</span></span> <span data-ttu-id="ab691-472">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-472">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-473">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="ab691-473">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="ab691-474">Int32</span><span class="sxs-lookup"><span data-stu-id="ab691-474">Int32</span></span>|<span data-ttu-id="ab691-475">Количество исправленных вредоносных программ для этого устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="ab691-475">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="ab691-476">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-476">This property is read-only.</span></span> <span data-ttu-id="ab691-477">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-477">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-478">notes</span><span class="sxs-lookup"><span data-stu-id="ab691-478">notes</span></span>|<span data-ttu-id="ab691-479">String</span><span class="sxs-lookup"><span data-stu-id="ab691-479">String</span></span>|<span data-ttu-id="ab691-480">Заметки на устройстве, созданном ИТ-администратором, унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-480">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="ab691-481">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="ab691-482">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="ab691-482">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="ab691-483">Состояние здоровья клиента диспетчера конфигурации, допустимо только для устройств, управляемых агентом MDM/ConfigMgr, унаследованных от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-483">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="ab691-484">configurationManagerClientInformation</span></span>|[<span data-ttu-id="ab691-485">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="ab691-485">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="ab691-486">Сведения о клиенте диспетчера конфигурации, действительные только для устройств, управляемых, управляемых дуэлями или трехуправленных агентом ConfigMgr, унаследованных от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-486">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-487">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="ab691-487">ethernetMacAddress</span></span>|<span data-ttu-id="ab691-488">String</span><span class="sxs-lookup"><span data-stu-id="ab691-488">String</span></span>|<span data-ttu-id="ab691-489">Mac Ethernet.</span><span class="sxs-lookup"><span data-stu-id="ab691-489">Ethernet MAC.</span></span> <span data-ttu-id="ab691-490">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-490">This property is read-only.</span></span> <span data-ttu-id="ab691-491">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-491">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-492">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="ab691-492">physicalMemoryInBytes</span></span>|<span data-ttu-id="ab691-493">Int64</span><span class="sxs-lookup"><span data-stu-id="ab691-493">Int64</span></span>|<span data-ttu-id="ab691-494">Общая память в bytes.</span><span class="sxs-lookup"><span data-stu-id="ab691-494">Total Memory in Bytes.</span></span> <span data-ttu-id="ab691-495">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-495">This property is read-only.</span></span> <span data-ttu-id="ab691-496">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-496">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-497">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="ab691-497">processorArchitecture</span></span>|[<span data-ttu-id="ab691-498">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="ab691-498">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="ab691-499">Архитектура процессора.</span><span class="sxs-lookup"><span data-stu-id="ab691-499">Processor architecture.</span></span> <span data-ttu-id="ab691-500">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-500">This property is read-only.</span></span> <span data-ttu-id="ab691-501">Унаследовано от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab691-501">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-502">Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="ab691-502">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="ab691-503">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="ab691-503">specificationVersion</span></span>|<span data-ttu-id="ab691-504">String</span><span class="sxs-lookup"><span data-stu-id="ab691-504">String</span></span>|<span data-ttu-id="ab691-505">Версия спецификации.</span><span class="sxs-lookup"><span data-stu-id="ab691-505">Specification version.</span></span> <span data-ttu-id="ab691-506">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-506">This property is read-only.</span></span> <span data-ttu-id="ab691-507">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-507">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-508">joinType</span><span class="sxs-lookup"><span data-stu-id="ab691-508">joinType</span></span>|[<span data-ttu-id="ab691-509">joinType</span><span class="sxs-lookup"><span data-stu-id="ab691-509">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="ab691-510">Тип присоединиться к устройству, унаследованный от [managedDevice.](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-510">Device join type Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-511">Возможные значения: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span><span class="sxs-lookup"><span data-stu-id="ab691-511">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="ab691-512">skuFamily</span><span class="sxs-lookup"><span data-stu-id="ab691-512">skuFamily</span></span>|<span data-ttu-id="ab691-513">String</span><span class="sxs-lookup"><span data-stu-id="ab691-513">String</span></span>|<span data-ttu-id="ab691-514">Семейство устройств sku, унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-514">Device sku family Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-515">skuNumber</span><span class="sxs-lookup"><span data-stu-id="ab691-515">skuNumber</span></span>|<span data-ttu-id="ab691-516">Int32</span><span class="sxs-lookup"><span data-stu-id="ab691-516">Int32</span></span>|<span data-ttu-id="ab691-517">Номер sku устройства см. также: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo .</span><span class="sxs-lookup"><span data-stu-id="ab691-517">Device sku number, see also: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo.</span></span> <span data-ttu-id="ab691-518">Допустимые значения от 0 до 2147483647.</span><span class="sxs-lookup"><span data-stu-id="ab691-518">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="ab691-519">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab691-519">This property is read-only.</span></span> <span data-ttu-id="ab691-520">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-520">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="ab691-521">managementFeatures</span><span class="sxs-lookup"><span data-stu-id="ab691-521">managementFeatures</span></span>|[<span data-ttu-id="ab691-522">managedDeviceManagementFeatures</span><span class="sxs-lookup"><span data-stu-id="ab691-522">managedDeviceManagementFeatures</span></span>](../resources/intune-devices-manageddevicemanagementfeatures.md)|<span data-ttu-id="ab691-523">Функции управления устройствами, унаследованные [от managedDevice.](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-523">Device management features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="ab691-524">Возможные значения: `none`, `microsoftManagedDesktop`.</span><span class="sxs-lookup"><span data-stu-id="ab691-524">Possible values are: `none`, `microsoftManagedDesktop`.</span></span>|
|<span data-ttu-id="ab691-525">chromeOSDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="ab691-525">chromeOSDeviceInfo</span></span>|<span data-ttu-id="ab691-526">[коллекция chromeOSDeviceProperty](../resources/intune-devices-chromeosdeviceproperty.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-526">[chromeOSDeviceProperty](../resources/intune-devices-chromeosdeviceproperty.md) collection</span></span>|<span data-ttu-id="ab691-527">Список свойств устройства ChromeOS.</span><span class="sxs-lookup"><span data-stu-id="ab691-527">List of properties of the ChromeOS Device.</span></span> <span data-ttu-id="ab691-528">Унаследованный от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ab691-528">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ab691-529">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab691-529">Response</span></span>
<span data-ttu-id="ab691-530">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab691-530">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab691-531">Пример</span><span class="sxs-lookup"><span data-stu-id="ab691-531">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab691-532">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab691-532">Request</span></span>
<span data-ttu-id="ab691-533">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab691-533">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 8351

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
  "managementFeatures": "microsoftManagedDesktop",
  "chromeOSDeviceInfo": [
    {
      "@odata.type": "microsoft.graph.chromeOSDeviceProperty",
      "name": "Name value",
      "value": "Value value",
      "valueType": "Value Type value",
      "updatable": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ab691-534">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab691-534">Response</span></span>
<span data-ttu-id="ab691-p176">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab691-p176">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 8400

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
  "managementFeatures": "microsoftManagedDesktop",
  "chromeOSDeviceInfo": [
    {
      "@odata.type": "microsoft.graph.chromeOSDeviceProperty",
      "name": "Name value",
      "value": "Value value",
      "valueType": "Value Type value",
      "updatable": true
    }
  ]
}
```




