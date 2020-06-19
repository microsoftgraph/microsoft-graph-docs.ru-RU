---
title: Создание Виндовсманажеддевице
description: Создание нового объекта Виндовсманажеддевице.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4bcb2ef375a1cb84f4dd6ba9f24237654b5033e7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792122"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="25452-103">Создание Виндовсманажеддевице</span><span class="sxs-lookup"><span data-stu-id="25452-103">Create windowsManagedDevice</span></span>

<span data-ttu-id="25452-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25452-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25452-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25452-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25452-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25452-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25452-107">Создание нового объекта [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="25452-107">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25452-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="25452-108">Prerequisites</span></span>
<span data-ttu-id="25452-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="25452-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="25452-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25452-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25452-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25452-111">Permission type</span></span>|<span data-ttu-id="25452-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="25452-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25452-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25452-113">Delegated (work or school account)</span></span>|<span data-ttu-id="25452-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25452-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="25452-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25452-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25452-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25452-116">Not supported.</span></span>|
|<span data-ttu-id="25452-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25452-117">Application</span></span>|<span data-ttu-id="25452-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25452-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25452-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25452-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="25452-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="25452-120">Request headers</span></span>
|<span data-ttu-id="25452-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25452-121">Header</span></span>|<span data-ttu-id="25452-122">Значение</span><span class="sxs-lookup"><span data-stu-id="25452-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25452-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25452-123">Authorization</span></span>|<span data-ttu-id="25452-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25452-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25452-125">Accept</span><span class="sxs-lookup"><span data-stu-id="25452-125">Accept</span></span>|<span data-ttu-id="25452-126">application/json</span><span class="sxs-lookup"><span data-stu-id="25452-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25452-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25452-127">Request body</span></span>
<span data-ttu-id="25452-128">В тексте запроса добавьте представление объекта Виндовсманажеддевице в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25452-128">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="25452-129">В следующей таблице приведены свойства, необходимые при создании Виндовсманажеддевице.</span><span class="sxs-lookup"><span data-stu-id="25452-129">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="25452-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="25452-130">Property</span></span>|<span data-ttu-id="25452-131">Тип</span><span class="sxs-lookup"><span data-stu-id="25452-131">Type</span></span>|<span data-ttu-id="25452-132">Описание</span><span class="sxs-lookup"><span data-stu-id="25452-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25452-133">id</span><span class="sxs-lookup"><span data-stu-id="25452-133">id</span></span>|<span data-ttu-id="25452-134">Строка</span><span class="sxs-lookup"><span data-stu-id="25452-134">String</span></span>|<span data-ttu-id="25452-135">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-135">Unique Identifier for the device.</span></span> <span data-ttu-id="25452-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-136">This property is read-only.</span></span> <span data-ttu-id="25452-137">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-137">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-138">userId</span><span class="sxs-lookup"><span data-stu-id="25452-138">userId</span></span>|<span data-ttu-id="25452-139">String</span><span class="sxs-lookup"><span data-stu-id="25452-139">String</span></span>|<span data-ttu-id="25452-140">Уникальный идентификатор пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="25452-140">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="25452-141">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-141">This property is read-only.</span></span> <span data-ttu-id="25452-142">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-142">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="25452-143">deviceName</span></span>|<span data-ttu-id="25452-144">String</span><span class="sxs-lookup"><span data-stu-id="25452-144">String</span></span>|<span data-ttu-id="25452-145">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-145">Name of the device.</span></span> <span data-ttu-id="25452-146">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-146">This property is read-only.</span></span> <span data-ttu-id="25452-147">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-147">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-148">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="25452-148">hardwareInformation</span></span>|[<span data-ttu-id="25452-149">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="25452-149">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="25452-150">Сведения о хардвард для устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-150">The hardward details for the device.</span></span>  <span data-ttu-id="25452-151">Включает такие сведения, как место хранения, производитель, серийный номер и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-151">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="25452-152">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-152">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="25452-153">ownerType</span></span>|[<span data-ttu-id="25452-154">ownerType</span><span class="sxs-lookup"><span data-stu-id="25452-154">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="25452-155">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="25452-155">Ownership of the device.</span></span> <span data-ttu-id="25452-156">Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25452-156">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="25452-157">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="25452-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="25452-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="25452-158">managedDeviceOwnerType</span></span>|[<span data-ttu-id="25452-159">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="25452-159">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="25452-160">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="25452-160">Ownership of the device.</span></span> <span data-ttu-id="25452-161">Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25452-161">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="25452-162">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="25452-162">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="25452-163">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="25452-163">deviceActionResults</span></span>|<span data-ttu-id="25452-164">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="25452-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="25452-165">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="25452-165">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="25452-166">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-166">This property is read-only.</span></span> <span data-ttu-id="25452-167">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-168">манажементстате</span><span class="sxs-lookup"><span data-stu-id="25452-168">managementState</span></span>|[<span data-ttu-id="25452-169">манажементстате</span><span class="sxs-lookup"><span data-stu-id="25452-169">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="25452-170">Состояние управления для устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-170">Management state of the device.</span></span> <span data-ttu-id="25452-171">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-171">This property is read-only.</span></span> <span data-ttu-id="25452-172">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25452-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="25452-173">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="25452-173">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="25452-174">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="25452-174">enrolledDateTime</span></span>|<span data-ttu-id="25452-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25452-175">DateTimeOffset</span></span>|<span data-ttu-id="25452-176">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-176">Enrollment time of the device.</span></span> <span data-ttu-id="25452-177">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-177">This property is read-only.</span></span> <span data-ttu-id="25452-178">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-178">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-179">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="25452-179">lastSyncDateTime</span></span>|<span data-ttu-id="25452-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25452-180">DateTimeOffset</span></span>|<span data-ttu-id="25452-181">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="25452-181">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="25452-182">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-182">This property is read-only.</span></span> <span data-ttu-id="25452-183">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-183">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-184">чассистипе</span><span class="sxs-lookup"><span data-stu-id="25452-184">chassisType</span></span>|[<span data-ttu-id="25452-185">чассистипе</span><span class="sxs-lookup"><span data-stu-id="25452-185">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="25452-186">Тип корпуса устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-186">Chassis type of the device.</span></span> <span data-ttu-id="25452-187">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-187">This property is read-only.</span></span> <span data-ttu-id="25452-188">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25452-188">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="25452-189">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="25452-189">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="25452-190">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="25452-190">operatingSystem</span></span>|<span data-ttu-id="25452-191">String</span><span class="sxs-lookup"><span data-stu-id="25452-191">String</span></span>|<span data-ttu-id="25452-192">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-192">Operating system of the device.</span></span> <span data-ttu-id="25452-193">Windows, iOS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-193">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="25452-194">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="25452-195">deviceType</span></span>|[<span data-ttu-id="25452-196">deviceType</span><span class="sxs-lookup"><span data-stu-id="25452-196">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="25452-197">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-197">Platform of the device.</span></span> <span data-ttu-id="25452-198">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-198">This property is read-only.</span></span> <span data-ttu-id="25452-199">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25452-199">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="25452-200">Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` , `macMDM` , `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `blackberry` `palm` `unknown` ,,,,,,,,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="25452-200">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="25452-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="25452-201">complianceState</span></span>|[<span data-ttu-id="25452-202">complianceState</span><span class="sxs-lookup"><span data-stu-id="25452-202">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="25452-203">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="25452-203">Compliance state of the device.</span></span> <span data-ttu-id="25452-204">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-204">This property is read-only.</span></span> <span data-ttu-id="25452-205">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25452-205">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="25452-206">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="25452-206">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="25452-207">jailBroken</span><span class="sxs-lookup"><span data-stu-id="25452-207">jailBroken</span></span>|<span data-ttu-id="25452-208">String</span><span class="sxs-lookup"><span data-stu-id="25452-208">String</span></span>|<span data-ttu-id="25452-209">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="25452-209">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="25452-210">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-210">This property is read-only.</span></span> <span data-ttu-id="25452-211">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-212">managementAgent</span><span class="sxs-lookup"><span data-stu-id="25452-212">managementAgent</span></span>|[<span data-ttu-id="25452-213">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="25452-213">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="25452-214">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="25452-214">Management channel of the device.</span></span> <span data-ttu-id="25452-215">Intune, EAS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-215">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="25452-216">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25452-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="25452-217">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="25452-217">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="25452-218">osVersion</span><span class="sxs-lookup"><span data-stu-id="25452-218">osVersion</span></span>|<span data-ttu-id="25452-219">String</span><span class="sxs-lookup"><span data-stu-id="25452-219">String</span></span>|<span data-ttu-id="25452-220">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-220">Operating system version of the device.</span></span> <span data-ttu-id="25452-221">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-221">This property is read-only.</span></span> <span data-ttu-id="25452-222">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-222">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-223">easActivated</span><span class="sxs-lookup"><span data-stu-id="25452-223">easActivated</span></span>|<span data-ttu-id="25452-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="25452-224">Boolean</span></span>|<span data-ttu-id="25452-225">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="25452-225">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="25452-226">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-226">This property is read-only.</span></span> <span data-ttu-id="25452-227">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="25452-228">easDeviceId</span></span>|<span data-ttu-id="25452-229">String</span><span class="sxs-lookup"><span data-stu-id="25452-229">String</span></span>|<span data-ttu-id="25452-230">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="25452-230">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="25452-231">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-231">This property is read-only.</span></span> <span data-ttu-id="25452-232">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-232">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-233">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="25452-233">easActivationDateTime</span></span>|<span data-ttu-id="25452-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25452-234">DateTimeOffset</span></span>|<span data-ttu-id="25452-235">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="25452-235">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="25452-236">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-236">This property is read-only.</span></span> <span data-ttu-id="25452-237">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-238">аадрегистеред</span><span class="sxs-lookup"><span data-stu-id="25452-238">aadRegistered</span></span>|<span data-ttu-id="25452-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="25452-239">Boolean</span></span>|<span data-ttu-id="25452-240">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="25452-240">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="25452-241">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-241">This property is read-only.</span></span> <span data-ttu-id="25452-242">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-242">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-243">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="25452-243">azureADRegistered</span></span>|<span data-ttu-id="25452-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="25452-244">Boolean</span></span>|<span data-ttu-id="25452-245">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="25452-245">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="25452-246">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-246">This property is read-only.</span></span> <span data-ttu-id="25452-247">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-247">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="25452-248">deviceEnrollmentType</span></span>|[<span data-ttu-id="25452-249">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="25452-249">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="25452-250">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-250">Enrollment type of the device.</span></span> <span data-ttu-id="25452-251">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-251">This property is read-only.</span></span> <span data-ttu-id="25452-252">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25452-252">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="25452-253">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="25452-253">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="25452-254">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="25452-254">lostModeState</span></span>|[<span data-ttu-id="25452-255">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="25452-255">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="25452-256">Указывает, включен ли режим потерянных или отключенных.</span><span class="sxs-lookup"><span data-stu-id="25452-256">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="25452-257">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-257">This property is read-only.</span></span> <span data-ttu-id="25452-258">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25452-258">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="25452-259">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="25452-259">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="25452-260">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="25452-260">activationLockBypassCode</span></span>|<span data-ttu-id="25452-261">String</span><span class="sxs-lookup"><span data-stu-id="25452-261">String</span></span>|<span data-ttu-id="25452-262">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="25452-262">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="25452-263">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-263">This property is read-only.</span></span> <span data-ttu-id="25452-264">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-265">emailAddress</span><span class="sxs-lookup"><span data-stu-id="25452-265">emailAddress</span></span>|<span data-ttu-id="25452-266">String</span><span class="sxs-lookup"><span data-stu-id="25452-266">String</span></span>|<span data-ttu-id="25452-267">Сообщения электронной почты пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="25452-267">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="25452-268">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-268">This property is read-only.</span></span> <span data-ttu-id="25452-269">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-270">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="25452-270">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="25452-271">String</span><span class="sxs-lookup"><span data-stu-id="25452-271">String</span></span>|<span data-ttu-id="25452-272">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="25452-272">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="25452-273">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-273">Read only.</span></span> <span data-ttu-id="25452-274">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-274">This property is read-only.</span></span> <span data-ttu-id="25452-275">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-275">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-276">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="25452-276">azureADDeviceId</span></span>|<span data-ttu-id="25452-277">String</span><span class="sxs-lookup"><span data-stu-id="25452-277">String</span></span>|<span data-ttu-id="25452-278">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="25452-278">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="25452-279">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-279">Read only.</span></span> <span data-ttu-id="25452-280">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-280">This property is read-only.</span></span> <span data-ttu-id="25452-281">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-281">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="25452-282">deviceRegistrationState</span></span>|[<span data-ttu-id="25452-283">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="25452-283">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="25452-284">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-284">Device registration state.</span></span> <span data-ttu-id="25452-285">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-285">This property is read-only.</span></span> <span data-ttu-id="25452-286">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25452-286">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="25452-287">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="25452-287">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="25452-288">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="25452-288">deviceCategoryDisplayName</span></span>|<span data-ttu-id="25452-289">String</span><span class="sxs-lookup"><span data-stu-id="25452-289">String</span></span>|<span data-ttu-id="25452-290">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="25452-290">Device category display name.</span></span> <span data-ttu-id="25452-291">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-291">This property is read-only.</span></span> <span data-ttu-id="25452-292">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-292">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-293">isSupervised</span><span class="sxs-lookup"><span data-stu-id="25452-293">isSupervised</span></span>|<span data-ttu-id="25452-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="25452-294">Boolean</span></span>|<span data-ttu-id="25452-295">Состояние контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-295">Device supervised status.</span></span> <span data-ttu-id="25452-296">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-296">This property is read-only.</span></span> <span data-ttu-id="25452-297">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-297">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-298">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="25452-298">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="25452-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25452-299">DateTimeOffset</span></span>|<span data-ttu-id="25452-300">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="25452-300">Last time the device contacted Exchange.</span></span> <span data-ttu-id="25452-301">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-301">This property is read-only.</span></span> <span data-ttu-id="25452-302">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-302">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="25452-303">exchangeAccessState</span></span>|[<span data-ttu-id="25452-304">девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="25452-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="25452-305">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="25452-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="25452-306">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-306">This property is read-only.</span></span> <span data-ttu-id="25452-307">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25452-307">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="25452-308">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="25452-308">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="25452-309">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="25452-309">exchangeAccessStateReason</span></span>|[<span data-ttu-id="25452-310">девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="25452-310">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="25452-311">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="25452-311">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="25452-312">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-312">This property is read-only.</span></span> <span data-ttu-id="25452-313">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25452-313">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="25452-314">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="25452-314">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="25452-315">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="25452-315">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="25452-316">String</span><span class="sxs-lookup"><span data-stu-id="25452-316">String</span></span>|<span data-ttu-id="25452-317">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="25452-317">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="25452-318">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-318">This property is read-only.</span></span> <span data-ttu-id="25452-319">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-319">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-320">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="25452-320">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="25452-321">String</span><span class="sxs-lookup"><span data-stu-id="25452-321">String</span></span>|<span data-ttu-id="25452-322">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="25452-322">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="25452-323">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-323">This property is read-only.</span></span> <span data-ttu-id="25452-324">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-324">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="25452-325">isEncrypted</span></span>|<span data-ttu-id="25452-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="25452-326">Boolean</span></span>|<span data-ttu-id="25452-327">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-327">Device encryption status.</span></span> <span data-ttu-id="25452-328">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-328">This property is read-only.</span></span> <span data-ttu-id="25452-329">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-329">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-330">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="25452-330">userPrincipalName</span></span>|<span data-ttu-id="25452-331">String</span><span class="sxs-lookup"><span data-stu-id="25452-331">String</span></span>|<span data-ttu-id="25452-332">Имя участника пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-332">Device user principal name.</span></span> <span data-ttu-id="25452-333">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-333">This property is read-only.</span></span> <span data-ttu-id="25452-334">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-334">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-335">model</span><span class="sxs-lookup"><span data-stu-id="25452-335">model</span></span>|<span data-ttu-id="25452-336">String</span><span class="sxs-lookup"><span data-stu-id="25452-336">String</span></span>|<span data-ttu-id="25452-337">Модель устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-337">Model of the device.</span></span> <span data-ttu-id="25452-338">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-338">This property is read-only.</span></span> <span data-ttu-id="25452-339">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-340">manufacturer</span><span class="sxs-lookup"><span data-stu-id="25452-340">manufacturer</span></span>|<span data-ttu-id="25452-341">String</span><span class="sxs-lookup"><span data-stu-id="25452-341">String</span></span>|<span data-ttu-id="25452-342">Производитель устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-342">Manufacturer of the device.</span></span> <span data-ttu-id="25452-343">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-343">This property is read-only.</span></span> <span data-ttu-id="25452-344">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-345">imei</span><span class="sxs-lookup"><span data-stu-id="25452-345">imei</span></span>|<span data-ttu-id="25452-346">String</span><span class="sxs-lookup"><span data-stu-id="25452-346">String</span></span>|<span data-ttu-id="25452-347">IMEI.</span><span class="sxs-lookup"><span data-stu-id="25452-347">IMEI.</span></span> <span data-ttu-id="25452-348">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-348">This property is read-only.</span></span> <span data-ttu-id="25452-349">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-349">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-350">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="25452-350">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="25452-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25452-351">DateTimeOffset</span></span>|<span data-ttu-id="25452-352">Дата и время истечения льготного периода соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="25452-352">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="25452-353">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-353">This property is read-only.</span></span> <span data-ttu-id="25452-354">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-355">serialNumber</span><span class="sxs-lookup"><span data-stu-id="25452-355">serialNumber</span></span>|<span data-ttu-id="25452-356">Строка</span><span class="sxs-lookup"><span data-stu-id="25452-356">String</span></span>|<span data-ttu-id="25452-357">Серийный.</span><span class="sxs-lookup"><span data-stu-id="25452-357">SerialNumber.</span></span> <span data-ttu-id="25452-358">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-358">This property is read-only.</span></span> <span data-ttu-id="25452-359">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-360">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="25452-360">phoneNumber</span></span>|<span data-ttu-id="25452-361">String</span><span class="sxs-lookup"><span data-stu-id="25452-361">String</span></span>|<span data-ttu-id="25452-362">Номер телефона устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-362">Phone number of the device.</span></span> <span data-ttu-id="25452-363">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-363">This property is read-only.</span></span> <span data-ttu-id="25452-364">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-364">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-365">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="25452-365">androidSecurityPatchLevel</span></span>|<span data-ttu-id="25452-366">String</span><span class="sxs-lookup"><span data-stu-id="25452-366">String</span></span>|<span data-ttu-id="25452-367">Уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="25452-367">Android security patch level.</span></span> <span data-ttu-id="25452-368">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-368">This property is read-only.</span></span> <span data-ttu-id="25452-369">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-370">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="25452-370">userDisplayName</span></span>|<span data-ttu-id="25452-371">String</span><span class="sxs-lookup"><span data-stu-id="25452-371">String</span></span>|<span data-ttu-id="25452-372">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="25452-372">User display name.</span></span> <span data-ttu-id="25452-373">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-373">This property is read-only.</span></span> <span data-ttu-id="25452-374">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="25452-375">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="25452-376">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="25452-376">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="25452-377">Функции, поддерживающие клиент Конфигрмгр.</span><span class="sxs-lookup"><span data-stu-id="25452-377">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="25452-378">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-378">This property is read-only.</span></span> <span data-ttu-id="25452-379">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-379">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-380">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="25452-380">wiFiMacAddress</span></span>|<span data-ttu-id="25452-381">String</span><span class="sxs-lookup"><span data-stu-id="25452-381">String</span></span>|<span data-ttu-id="25452-382">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="25452-382">Wi-Fi MAC.</span></span> <span data-ttu-id="25452-383">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-383">This property is read-only.</span></span> <span data-ttu-id="25452-384">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-384">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="25452-385">deviceHealthAttestationState</span></span>|[<span data-ttu-id="25452-386">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="25452-386">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="25452-387">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-387">The device health attestation state.</span></span> <span data-ttu-id="25452-388">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-388">This property is read-only.</span></span> <span data-ttu-id="25452-389">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-389">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-390">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="25452-390">subscriberCarrier</span></span>|<span data-ttu-id="25452-391">String</span><span class="sxs-lookup"><span data-stu-id="25452-391">String</span></span>|<span data-ttu-id="25452-392">Перевозчик абонента.</span><span class="sxs-lookup"><span data-stu-id="25452-392">Subscriber Carrier.</span></span> <span data-ttu-id="25452-393">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-393">This property is read-only.</span></span> <span data-ttu-id="25452-394">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-394">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-395">meid</span><span class="sxs-lookup"><span data-stu-id="25452-395">meid</span></span>|<span data-ttu-id="25452-396">String</span><span class="sxs-lookup"><span data-stu-id="25452-396">String</span></span>|<span data-ttu-id="25452-397">MEID.</span><span class="sxs-lookup"><span data-stu-id="25452-397">MEID.</span></span> <span data-ttu-id="25452-398">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-398">This property is read-only.</span></span> <span data-ttu-id="25452-399">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-399">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-400">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="25452-400">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="25452-401">Int64</span><span class="sxs-lookup"><span data-stu-id="25452-401">Int64</span></span>|<span data-ttu-id="25452-402">Общий объем хранилища в байтах.</span><span class="sxs-lookup"><span data-stu-id="25452-402">Total Storage in Bytes.</span></span> <span data-ttu-id="25452-403">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-403">This property is read-only.</span></span> <span data-ttu-id="25452-404">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-404">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-405">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="25452-405">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="25452-406">Int64</span><span class="sxs-lookup"><span data-stu-id="25452-406">Int64</span></span>|<span data-ttu-id="25452-407">Свободное хранилище в байтах.</span><span class="sxs-lookup"><span data-stu-id="25452-407">Free Storage in Bytes.</span></span> <span data-ttu-id="25452-408">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-408">This property is read-only.</span></span> <span data-ttu-id="25452-409">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-409">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-410">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="25452-410">managedDeviceName</span></span>|<span data-ttu-id="25452-411">String</span><span class="sxs-lookup"><span data-stu-id="25452-411">String</span></span>|<span data-ttu-id="25452-412">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-412">Automatically generated name to identify a device.</span></span> <span data-ttu-id="25452-413">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="25452-413">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="25452-414">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-414">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-415">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="25452-415">partnerReportedThreatState</span></span>|[<span data-ttu-id="25452-416">манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="25452-416">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="25452-417">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="25452-417">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="25452-418">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-418">Read Only.</span></span> <span data-ttu-id="25452-419">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-419">This property is read-only.</span></span> <span data-ttu-id="25452-420">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25452-420">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="25452-421">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="25452-421">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="25452-422">ретиреафтердатетиме</span><span class="sxs-lookup"><span data-stu-id="25452-422">retireAfterDateTime</span></span>|<span data-ttu-id="25452-423">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25452-423">DateTimeOffset</span></span>|<span data-ttu-id="25452-424">Указывает время, по истечении которого устройство будет автоматически снято из-за запланированного действия.</span><span class="sxs-lookup"><span data-stu-id="25452-424">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="25452-425">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-425">This property is read-only.</span></span> <span data-ttu-id="25452-426">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-426">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-427">усерслогжедон</span><span class="sxs-lookup"><span data-stu-id="25452-427">usersLoggedOn</span></span>|<span data-ttu-id="25452-428">Коллекция [логжедонусер](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="25452-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="25452-429">Указывает последнего вошедшего в систему пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-429">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="25452-430">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-430">This property is read-only.</span></span> <span data-ttu-id="25452-431">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-431">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-432">префермдмоверграупполициапплиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="25452-432">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="25452-433">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25452-433">DateTimeOffset</span></span>|<span data-ttu-id="25452-434">Сообщает о значении DateTime, заданном параметром Префермдмоверграупполици.</span><span class="sxs-lookup"><span data-stu-id="25452-434">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="25452-435">Если этот параметр установлен, параметры групповой политики в случае конфликта будут переопределяться параметрами групповой политики.</span><span class="sxs-lookup"><span data-stu-id="25452-435">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="25452-436">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-436">Read Only.</span></span> <span data-ttu-id="25452-437">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-437">This property is read-only.</span></span> <span data-ttu-id="25452-438">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-438">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-439">аутопилотенроллед</span><span class="sxs-lookup"><span data-stu-id="25452-439">autopilotEnrolled</span></span>|<span data-ttu-id="25452-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="25452-440">Boolean</span></span>|<span data-ttu-id="25452-441">Сообщает, зарегистрировано ли управляемое устройство через Автоматический пилот.</span><span class="sxs-lookup"><span data-stu-id="25452-441">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="25452-442">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-442">This property is read-only.</span></span> <span data-ttu-id="25452-443">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-443">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-444">рекуиреусеренроллментаппровал</span><span class="sxs-lookup"><span data-stu-id="25452-444">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="25452-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="25452-445">Boolean</span></span>|<span data-ttu-id="25452-446">Указывает, является ли управляемое устройство iOS регистрацией на утверждение пользователя.</span><span class="sxs-lookup"><span data-stu-id="25452-446">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="25452-447">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-447">This property is read-only.</span></span> <span data-ttu-id="25452-448">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-448">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-449">манажементцертификатикспиратиондате</span><span class="sxs-lookup"><span data-stu-id="25452-449">managementCertificateExpirationDate</span></span>|<span data-ttu-id="25452-450">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25452-450">DateTimeOffset</span></span>|<span data-ttu-id="25452-451">Дата окончания срока действия сертификата управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="25452-451">Reports device management certificate expiration date.</span></span> <span data-ttu-id="25452-452">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-452">This property is read-only.</span></span> <span data-ttu-id="25452-453">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-453">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-454">икЦид</span><span class="sxs-lookup"><span data-stu-id="25452-454">iccid</span></span>|<span data-ttu-id="25452-455">String</span><span class="sxs-lookup"><span data-stu-id="25452-455">String</span></span>|<span data-ttu-id="25452-456">Идентификатор встроенной карты — это уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="25452-456">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="25452-457">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-457">This property is read-only.</span></span> <span data-ttu-id="25452-458">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-458">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-459">удид</span><span class="sxs-lookup"><span data-stu-id="25452-459">udid</span></span>|<span data-ttu-id="25452-460">String</span><span class="sxs-lookup"><span data-stu-id="25452-460">String</span></span>|<span data-ttu-id="25452-461">Уникальный идентификатор устройства для устройств iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="25452-461">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="25452-462">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-462">This property is read-only.</span></span> <span data-ttu-id="25452-463">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-463">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-464">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="25452-464">roleScopeTagIds</span></span>|<span data-ttu-id="25452-465">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="25452-465">String collection</span></span>|<span data-ttu-id="25452-466">Список идентификаторов тегов области для этого экземпляра устройства.</span><span class="sxs-lookup"><span data-stu-id="25452-466">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="25452-467">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-467">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-468">виндовсактивемалварекаунт</span><span class="sxs-lookup"><span data-stu-id="25452-468">windowsActiveMalwareCount</span></span>|<span data-ttu-id="25452-469">Int32</span><span class="sxs-lookup"><span data-stu-id="25452-469">Int32</span></span>|<span data-ttu-id="25452-470">Количество активных вредоносных программ для этого устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="25452-470">Count of active malware for this windows device.</span></span> <span data-ttu-id="25452-471">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-471">This property is read-only.</span></span> <span data-ttu-id="25452-472">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-472">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-473">виндовсремедиатедмалварекаунт</span><span class="sxs-lookup"><span data-stu-id="25452-473">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="25452-474">Int32</span><span class="sxs-lookup"><span data-stu-id="25452-474">Int32</span></span>|<span data-ttu-id="25452-475">Количество исправленных вредоносных программ для этого устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="25452-475">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="25452-476">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-476">This property is read-only.</span></span> <span data-ttu-id="25452-477">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-477">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-478">notes</span><span class="sxs-lookup"><span data-stu-id="25452-478">notes</span></span>|<span data-ttu-id="25452-479">String</span><span class="sxs-lookup"><span data-stu-id="25452-479">String</span></span>|<span data-ttu-id="25452-480">Примечания на устройстве, созданном администратором ИТ, унаследованном от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-480">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="25452-481">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="25452-482">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="25452-482">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="25452-483">Состояние работоспособности клиента Configuration Manager, действующее только для устройств под управлением агентов MDM/ConfigMgr, наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-483">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="25452-484">configurationManagerClientInformation</span></span>|[<span data-ttu-id="25452-485">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="25452-485">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="25452-486">Сведения о клиенте Configuration Manager, действительные только для управляемых устройств, управляемых дуел и управляемых с помощью агента Configuration Manager, наследуемого от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-486">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-487">есернетмакаддресс</span><span class="sxs-lookup"><span data-stu-id="25452-487">ethernetMacAddress</span></span>|<span data-ttu-id="25452-488">String</span><span class="sxs-lookup"><span data-stu-id="25452-488">String</span></span>|<span data-ttu-id="25452-489">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="25452-489">Ethernet MAC.</span></span> <span data-ttu-id="25452-490">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-490">This property is read-only.</span></span> <span data-ttu-id="25452-491">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-491">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-492">фисикалмеморинбитес</span><span class="sxs-lookup"><span data-stu-id="25452-492">physicalMemoryInBytes</span></span>|<span data-ttu-id="25452-493">Int64</span><span class="sxs-lookup"><span data-stu-id="25452-493">Int64</span></span>|<span data-ttu-id="25452-494">Общий объем памяти в байтах.</span><span class="sxs-lookup"><span data-stu-id="25452-494">Total Memory in Bytes.</span></span> <span data-ttu-id="25452-495">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-495">This property is read-only.</span></span> <span data-ttu-id="25452-496">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-496">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-497">процессорарчитектуре</span><span class="sxs-lookup"><span data-stu-id="25452-497">processorArchitecture</span></span>|[<span data-ttu-id="25452-498">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="25452-498">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="25452-499">Архитектура процессора.</span><span class="sxs-lookup"><span data-stu-id="25452-499">Processor architecture.</span></span> <span data-ttu-id="25452-500">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-500">This property is read-only.</span></span> <span data-ttu-id="25452-501">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25452-501">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="25452-502">Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="25452-502">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="25452-503">спеЦификатионверсион</span><span class="sxs-lookup"><span data-stu-id="25452-503">specificationVersion</span></span>|<span data-ttu-id="25452-504">String</span><span class="sxs-lookup"><span data-stu-id="25452-504">String</span></span>|<span data-ttu-id="25452-505">Версия спецификации.</span><span class="sxs-lookup"><span data-stu-id="25452-505">Specification version.</span></span> <span data-ttu-id="25452-506">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25452-506">This property is read-only.</span></span> <span data-ttu-id="25452-507">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-507">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="25452-508">joinType</span><span class="sxs-lookup"><span data-stu-id="25452-508">joinType</span></span>|[<span data-ttu-id="25452-509">joinType</span><span class="sxs-lookup"><span data-stu-id="25452-509">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="25452-510">Тип присоединения устройств наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25452-510">Device join type Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="25452-511">Возможные значения: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span><span class="sxs-lookup"><span data-stu-id="25452-511">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="25452-512">скуфамили</span><span class="sxs-lookup"><span data-stu-id="25452-512">skuFamily</span></span>|<span data-ttu-id="25452-513">String</span><span class="sxs-lookup"><span data-stu-id="25452-513">String</span></span>|<span data-ttu-id="25452-514">Семейство конфигураций устройств, унаследованное от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="25452-514">Device sku family Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="25452-515">Отклик</span><span class="sxs-lookup"><span data-stu-id="25452-515">Response</span></span>
<span data-ttu-id="25452-516">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="25452-516">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25452-517">Пример</span><span class="sxs-lookup"><span data-stu-id="25452-517">Example</span></span>

### <a name="request"></a><span data-ttu-id="25452-518">Запрос</span><span class="sxs-lookup"><span data-stu-id="25452-518">Request</span></span>
<span data-ttu-id="25452-519">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25452-519">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 7830

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

### <a name="response"></a><span data-ttu-id="25452-520">Отклик</span><span class="sxs-lookup"><span data-stu-id="25452-520">Response</span></span>
<span data-ttu-id="25452-521">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="25452-521">Here is an example of the response.</span></span> <span data-ttu-id="25452-522">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="25452-522">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="25452-523">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="25452-523">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7879

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



