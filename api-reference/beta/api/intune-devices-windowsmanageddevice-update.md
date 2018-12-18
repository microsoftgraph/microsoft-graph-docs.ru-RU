---
title: Обновление windowsManagedDevice
description: Обновление свойства объекта windowsManagedDevice.
author: tfitzmac
ms.openlocfilehash: d1aa637a513d45ad33a1a5990399cf35f4cb21ae
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347637"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="4c24d-103">Обновление windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="4c24d-103">Update windowsManagedDevice</span></span>

> <span data-ttu-id="4c24d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4c24d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c24d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c24d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c24d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4c24d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c24d-107">Обновление свойства объекта [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="4c24d-107">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c24d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4c24d-108">Prerequisites</span></span>
<span data-ttu-id="4c24d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c24d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c24d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c24d-111">Permission type</span></span>|<span data-ttu-id="4c24d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c24d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c24d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c24d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c24d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c24d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4c24d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c24d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c24d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c24d-116">Not supported.</span></span>|
|<span data-ttu-id="4c24d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c24d-117">Application</span></span>|<span data-ttu-id="4c24d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c24d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c24d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c24d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="4c24d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c24d-120">Request headers</span></span>
|<span data-ttu-id="4c24d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c24d-121">Header</span></span>|<span data-ttu-id="4c24d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4c24d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c24d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c24d-123">Authorization</span></span>|<span data-ttu-id="4c24d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4c24d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c24d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4c24d-125">Accept</span></span>|<span data-ttu-id="4c24d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c24d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c24d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c24d-127">Request body</span></span>
<span data-ttu-id="4c24d-128">В тексте запроса укажите представление JSON для объекта [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="4c24d-128">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="4c24d-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4c24d-129">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="4c24d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c24d-130">Property</span></span>|<span data-ttu-id="4c24d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4c24d-131">Type</span></span>|<span data-ttu-id="4c24d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4c24d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c24d-133">id</span><span class="sxs-lookup"><span data-stu-id="4c24d-133">id</span></span>|<span data-ttu-id="4c24d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4c24d-134">String</span></span>|<span data-ttu-id="4c24d-135">Уникальный идентификатор для устройства унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-135">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-136">userId</span><span class="sxs-lookup"><span data-stu-id="4c24d-136">userId</span></span>|<span data-ttu-id="4c24d-137">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-137">String</span></span>|<span data-ttu-id="4c24d-138">Уникальный идентификатор для пользователя, связанного с устройством унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-138">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="4c24d-139">deviceName</span></span>|<span data-ttu-id="4c24d-140">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-140">String</span></span>|<span data-ttu-id="4c24d-141">Имя устройства, унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-141">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="4c24d-142">hardwareInformation</span></span>|[<span data-ttu-id="4c24d-143">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="4c24d-143">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="4c24d-144">Сведения о объектами для устройства.</span><span class="sxs-lookup"><span data-stu-id="4c24d-144">The hardward details for the device.</span></span>  <span data-ttu-id="4c24d-145">Содержит сведения, такие как дисковое пространство, производителя, серийный номер, и т.д. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-145">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="4c24d-146">ownerType</span></span>|[<span data-ttu-id="4c24d-147">ownerType</span><span class="sxs-lookup"><span data-stu-id="4c24d-147">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="4c24d-148">Владельцем устройства.</span><span class="sxs-lookup"><span data-stu-id="4c24d-148">Ownership of the device.</span></span> <span data-ttu-id="4c24d-149">Может быть «компания» или «личные» унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4c24d-149">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4c24d-150">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="4c24d-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="4c24d-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="4c24d-151">managedDeviceOwnerType</span></span>|[<span data-ttu-id="4c24d-152">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="4c24d-152">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="4c24d-153">Владельцем устройства.</span><span class="sxs-lookup"><span data-stu-id="4c24d-153">Ownership of the device.</span></span> <span data-ttu-id="4c24d-154">Может быть «компания» или «личные» унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4c24d-154">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4c24d-155">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="4c24d-155">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="4c24d-156">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="4c24d-156">deviceActionResults</span></span>|<span data-ttu-id="4c24d-157">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="4c24d-158">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="4c24d-158">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="4c24d-159">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-159">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-160">managementState</span><span class="sxs-lookup"><span data-stu-id="4c24d-160">managementState</span></span>|[<span data-ttu-id="4c24d-161">managementState</span><span class="sxs-lookup"><span data-stu-id="4c24d-161">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="4c24d-162">Состояние управления устройства.</span><span class="sxs-lookup"><span data-stu-id="4c24d-162">Management state of the device.</span></span> <span data-ttu-id="4c24d-163">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4c24d-163">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4c24d-164">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="4c24d-164">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="4c24d-165">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="4c24d-165">enrolledDateTime</span></span>|<span data-ttu-id="4c24d-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c24d-166">DateTimeOffset</span></span>|<span data-ttu-id="4c24d-167">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="4c24d-167">Enrollment time of the device.</span></span> <span data-ttu-id="4c24d-168">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-168">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-169">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4c24d-169">lastSyncDateTime</span></span>|<span data-ttu-id="4c24d-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c24d-170">DateTimeOffset</span></span>|<span data-ttu-id="4c24d-171">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="4c24d-171">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="4c24d-172">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-173">Тип корпуса</span><span class="sxs-lookup"><span data-stu-id="4c24d-173">chassisType</span></span>|[<span data-ttu-id="4c24d-174">Тип корпуса</span><span class="sxs-lookup"><span data-stu-id="4c24d-174">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="4c24d-175">Тип корпуса устройства.</span><span class="sxs-lookup"><span data-stu-id="4c24d-175">Chassis type of the device.</span></span> <span data-ttu-id="4c24d-176">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4c24d-176">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4c24d-177">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="4c24d-177">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="4c24d-178">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="4c24d-178">operatingSystem</span></span>|<span data-ttu-id="4c24d-179">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-179">String</span></span>|<span data-ttu-id="4c24d-180">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="4c24d-180">Operating system of the device.</span></span> <span data-ttu-id="4c24d-181">Windows, iOS и т.д. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-181">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="4c24d-182">deviceType</span></span>|[<span data-ttu-id="4c24d-183">deviceType</span><span class="sxs-lookup"><span data-stu-id="4c24d-183">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="4c24d-184">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="4c24d-184">Platform of the device.</span></span> <span data-ttu-id="4c24d-185">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4c24d-185">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4c24d-186">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4c24d-186">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="4c24d-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="4c24d-187">complianceState</span></span>|[<span data-ttu-id="4c24d-188">complianceState</span><span class="sxs-lookup"><span data-stu-id="4c24d-188">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="4c24d-189">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="4c24d-189">Compliance state of the device.</span></span> <span data-ttu-id="4c24d-190">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4c24d-190">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4c24d-191">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="4c24d-191">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="4c24d-192">jailBroken</span><span class="sxs-lookup"><span data-stu-id="4c24d-192">jailBroken</span></span>|<span data-ttu-id="4c24d-193">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-193">String</span></span>|<span data-ttu-id="4c24d-194">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="4c24d-194">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="4c24d-195">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-195">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-196">managementAgent</span><span class="sxs-lookup"><span data-stu-id="4c24d-196">managementAgent</span></span>|[<span data-ttu-id="4c24d-197">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="4c24d-197">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="4c24d-198">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="4c24d-198">Management channel of the device.</span></span> <span data-ttu-id="4c24d-199">Intune, EAS, и т.д. Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4c24d-199">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4c24d-200">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="4c24d-200">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="4c24d-201">osVersion</span><span class="sxs-lookup"><span data-stu-id="4c24d-201">osVersion</span></span>|<span data-ttu-id="4c24d-202">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-202">String</span></span>|<span data-ttu-id="4c24d-203">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="4c24d-203">Operating system version of the device.</span></span> <span data-ttu-id="4c24d-204">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-205">easActivated</span><span class="sxs-lookup"><span data-stu-id="4c24d-205">easActivated</span></span>|<span data-ttu-id="4c24d-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c24d-206">Boolean</span></span>|<span data-ttu-id="4c24d-207">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="4c24d-207">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="4c24d-208">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-208">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-209">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="4c24d-209">easDeviceId</span></span>|<span data-ttu-id="4c24d-210">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-210">String</span></span>|<span data-ttu-id="4c24d-211">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="4c24d-211">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="4c24d-212">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-212">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-213">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="4c24d-213">easActivationDateTime</span></span>|<span data-ttu-id="4c24d-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c24d-214">DateTimeOffset</span></span>|<span data-ttu-id="4c24d-215">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="4c24d-215">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="4c24d-216">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-217">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="4c24d-217">aadRegistered</span></span>|<span data-ttu-id="4c24d-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c24d-218">Boolean</span></span>|<span data-ttu-id="4c24d-219">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4c24d-219">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="4c24d-220">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-220">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-221">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="4c24d-221">azureADRegistered</span></span>|<span data-ttu-id="4c24d-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c24d-222">Boolean</span></span>|<span data-ttu-id="4c24d-223">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4c24d-223">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="4c24d-224">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-224">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="4c24d-225">deviceEnrollmentType</span></span>|[<span data-ttu-id="4c24d-226">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="4c24d-226">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="4c24d-227">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="4c24d-227">Enrollment type of the device.</span></span> <span data-ttu-id="4c24d-228">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4c24d-228">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4c24d-229">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="4c24d-229">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="4c24d-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="4c24d-230">lostModeState</span></span>|[<span data-ttu-id="4c24d-231">lostModeState</span><span class="sxs-lookup"><span data-stu-id="4c24d-231">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="4c24d-232">Указывает, если потеряны режим — это включен или отключен унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4c24d-232">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4c24d-233">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="4c24d-233">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="4c24d-234">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="4c24d-234">activationLockBypassCode</span></span>|<span data-ttu-id="4c24d-235">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-235">String</span></span>|<span data-ttu-id="4c24d-236">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4c24d-236">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="4c24d-237">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-238">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4c24d-238">emailAddress</span></span>|<span data-ttu-id="4c24d-239">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-239">String</span></span>|<span data-ttu-id="4c24d-240">Email(s) для пользователя, связанного с устройством унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-240">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-241">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="4c24d-241">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="4c24d-242">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-242">String</span></span>|<span data-ttu-id="4c24d-243">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4c24d-243">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="4c24d-244">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c24d-244">Read only.</span></span> <span data-ttu-id="4c24d-245">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-245">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-246">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="4c24d-246">azureADDeviceId</span></span>|<span data-ttu-id="4c24d-247">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-247">String</span></span>|<span data-ttu-id="4c24d-248">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4c24d-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="4c24d-249">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c24d-249">Read only.</span></span> <span data-ttu-id="4c24d-250">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-250">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="4c24d-251">deviceRegistrationState</span></span>|[<span data-ttu-id="4c24d-252">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="4c24d-252">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="4c24d-253">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="4c24d-253">Device registration state.</span></span> <span data-ttu-id="4c24d-254">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4c24d-254">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4c24d-255">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4c24d-255">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="4c24d-256">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="4c24d-256">deviceCategoryDisplayName</span></span>|<span data-ttu-id="4c24d-257">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-257">String</span></span>|<span data-ttu-id="4c24d-258">Категории устройств отображаемое имя унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-258">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-259">isSupervised</span><span class="sxs-lookup"><span data-stu-id="4c24d-259">isSupervised</span></span>|<span data-ttu-id="4c24d-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c24d-260">Boolean</span></span>|<span data-ttu-id="4c24d-261">Состояние устройства управляет унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-261">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-262">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4c24d-262">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="4c24d-263">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c24d-263">DateTimeOffset</span></span>|<span data-ttu-id="4c24d-264">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="4c24d-264">Last time the device contacted Exchange.</span></span> <span data-ttu-id="4c24d-265">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-265">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-266">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="4c24d-266">exchangeAccessState</span></span>|[<span data-ttu-id="4c24d-267">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="4c24d-267">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="4c24d-268">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="4c24d-268">The Access State of the device in Exchange.</span></span> <span data-ttu-id="4c24d-269">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4c24d-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4c24d-270">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="4c24d-270">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="4c24d-271">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="4c24d-271">exchangeAccessStateReason</span></span>|[<span data-ttu-id="4c24d-272">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="4c24d-272">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="4c24d-273">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="4c24d-273">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="4c24d-274">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4c24d-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4c24d-275">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="4c24d-275">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="4c24d-276">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="4c24d-276">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="4c24d-277">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-277">String</span></span>|<span data-ttu-id="4c24d-278">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="4c24d-278">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="4c24d-279">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-279">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-280">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="4c24d-280">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="4c24d-281">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-281">String</span></span>|<span data-ttu-id="4c24d-282">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="4c24d-282">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="4c24d-283">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-283">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-284">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="4c24d-284">isEncrypted</span></span>|<span data-ttu-id="4c24d-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c24d-285">Boolean</span></span>|<span data-ttu-id="4c24d-286">Состояние шифрование устройства унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-286">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-287">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4c24d-287">userPrincipalName</span></span>|<span data-ttu-id="4c24d-288">Строка</span><span class="sxs-lookup"><span data-stu-id="4c24d-288">String</span></span>|<span data-ttu-id="4c24d-289">Устройство имя участника-пользователя унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-289">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-290">model</span><span class="sxs-lookup"><span data-stu-id="4c24d-290">model</span></span>|<span data-ttu-id="4c24d-291">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-291">String</span></span>|<span data-ttu-id="4c24d-292">Модели устройства, унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-292">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-293">manufacturer</span><span class="sxs-lookup"><span data-stu-id="4c24d-293">manufacturer</span></span>|<span data-ttu-id="4c24d-294">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-294">String</span></span>|<span data-ttu-id="4c24d-295">Производителя устройства унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-295">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-296">imei</span><span class="sxs-lookup"><span data-stu-id="4c24d-296">imei</span></span>|<span data-ttu-id="4c24d-297">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-297">String</span></span>|<span data-ttu-id="4c24d-298">IMEI наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-298">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-299">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4c24d-299">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="4c24d-300">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c24d-300">DateTimeOffset</span></span>|<span data-ttu-id="4c24d-301">Дата и время по истечении устройства соответствия льготный период унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-301">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-302">serialNumber</span><span class="sxs-lookup"><span data-stu-id="4c24d-302">serialNumber</span></span>|<span data-ttu-id="4c24d-303">Строка</span><span class="sxs-lookup"><span data-stu-id="4c24d-303">String</span></span>|<span data-ttu-id="4c24d-304">SerialNumber наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-304">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-305">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="4c24d-305">phoneNumber</span></span>|<span data-ttu-id="4c24d-306">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-306">String</span></span>|<span data-ttu-id="4c24d-307">Номер телефона устройства, унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-307">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-308">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="4c24d-308">androidSecurityPatchLevel</span></span>|<span data-ttu-id="4c24d-309">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-309">String</span></span>|<span data-ttu-id="4c24d-310">Уровень исправлений безопасности Android унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-310">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-311">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4c24d-311">userDisplayName</span></span>|<span data-ttu-id="4c24d-312">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-312">String</span></span>|<span data-ttu-id="4c24d-313">Отображаемое имя пользователя унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-313">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="4c24d-314">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="4c24d-315">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="4c24d-315">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="4c24d-316">Клиент ConfigrMgr включенные компоненты унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-316">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-317">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="4c24d-317">wiFiMacAddress</span></span>|<span data-ttu-id="4c24d-318">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-318">String</span></span>|<span data-ttu-id="4c24d-319">Wi-Fi MAC наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-319">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="4c24d-320">deviceHealthAttestationState</span></span>|[<span data-ttu-id="4c24d-321">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="4c24d-321">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="4c24d-322">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="4c24d-322">The device health attestation state.</span></span> <span data-ttu-id="4c24d-323">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-324">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="4c24d-324">subscriberCarrier</span></span>|<span data-ttu-id="4c24d-325">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-325">String</span></span>|<span data-ttu-id="4c24d-326">Подписчик на поставщика наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-326">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-327">meid</span><span class="sxs-lookup"><span data-stu-id="4c24d-327">meid</span></span>|<span data-ttu-id="4c24d-328">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-328">String</span></span>|<span data-ttu-id="4c24d-329">MEID наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-329">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-330">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="4c24d-330">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="4c24d-331">Int64</span><span class="sxs-lookup"><span data-stu-id="4c24d-331">Int64</span></span>|<span data-ttu-id="4c24d-332">Общий объем хранилища в байтах наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-332">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-333">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="4c24d-333">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="4c24d-334">Int64</span><span class="sxs-lookup"><span data-stu-id="4c24d-334">Int64</span></span>|<span data-ttu-id="4c24d-335">Бесплатная хранилища в байтах наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-335">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-336">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="4c24d-336">managedDeviceName</span></span>|<span data-ttu-id="4c24d-337">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-337">String</span></span>|<span data-ttu-id="4c24d-338">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="4c24d-338">Automatically generated name to identify a device.</span></span> <span data-ttu-id="4c24d-339">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="4c24d-339">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="4c24d-340">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-340">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-341">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="4c24d-341">partnerReportedThreatState</span></span>|[<span data-ttu-id="4c24d-342">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="4c24d-342">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="4c24d-343">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="4c24d-343">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="4c24d-344">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c24d-344">Read Only.</span></span> <span data-ttu-id="4c24d-345">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4c24d-345">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4c24d-346">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="4c24d-346">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="4c24d-347">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="4c24d-347">usersLoggedOn</span></span>|<span data-ttu-id="4c24d-348">[loggedOnUser](../resources/intune-devices-loggedonuser.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4c24d-348">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="4c24d-349">Указывает последний вход в систему пользователи устройства унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-349">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-350">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c24d-350">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="4c24d-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c24d-351">DateTimeOffset</span></span>|<span data-ttu-id="4c24d-352">Отчеты о DateTime параметр preferMdmOverGroupPolicy имеет значение.</span><span class="sxs-lookup"><span data-stu-id="4c24d-352">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="4c24d-353">Если задано, параметры Intune MDM переопределяет параметры групповой политики в случае конфликта.</span><span class="sxs-lookup"><span data-stu-id="4c24d-353">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="4c24d-354">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c24d-354">Read Only.</span></span> <span data-ttu-id="4c24d-355">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-355">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-356">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="4c24d-356">autopilotEnrolled</span></span>|<span data-ttu-id="4c24d-357">Boolean.</span><span class="sxs-lookup"><span data-stu-id="4c24d-357">Boolean</span></span>|<span data-ttu-id="4c24d-358">Отчеты при регистрации управляемой устройство через автопилот.</span><span class="sxs-lookup"><span data-stu-id="4c24d-358">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="4c24d-359">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-360">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="4c24d-360">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="4c24d-361">Boolean.</span><span class="sxs-lookup"><span data-stu-id="4c24d-361">Boolean</span></span>|<span data-ttu-id="4c24d-362">Отчеты, если устройство управляемых iOS утверждения регистрации пользователя.</span><span class="sxs-lookup"><span data-stu-id="4c24d-362">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="4c24d-363">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-364">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="4c24d-364">managementCertificateExpirationDate</span></span>|<span data-ttu-id="4c24d-365">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c24d-365">DateTimeOffset</span></span>|<span data-ttu-id="4c24d-366">Отчеты устройства управления срок действия сертификата унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-366">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-367">iccid</span><span class="sxs-lookup"><span data-stu-id="4c24d-367">iccid</span></span>|<span data-ttu-id="4c24d-368">String.</span><span class="sxs-lookup"><span data-stu-id="4c24d-368">String</span></span>|<span data-ttu-id="4c24d-369">Идентификатор карты интегральной, это уникальный идентификационный номер карты диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="4c24d-369">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="4c24d-370">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-370">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-371">UDID</span><span class="sxs-lookup"><span data-stu-id="4c24d-371">udid</span></span>|<span data-ttu-id="4c24d-372">String.</span><span class="sxs-lookup"><span data-stu-id="4c24d-372">String</span></span>|<span data-ttu-id="4c24d-373">Уникальный идентификатор устройства для операций ввода-вывода и macOS устройств.</span><span class="sxs-lookup"><span data-stu-id="4c24d-373">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="4c24d-374">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-375">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4c24d-375">roleScopeTagIds</span></span>|<span data-ttu-id="4c24d-376">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4c24d-376">String collection</span></span>|<span data-ttu-id="4c24d-377">Список идентификаторов тег области для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="4c24d-377">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="4c24d-378">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-379">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="4c24d-379">windowsActiveMalwareCount</span></span>|<span data-ttu-id="4c24d-380">Int32</span><span class="sxs-lookup"><span data-stu-id="4c24d-380">Int32</span></span>|<span data-ttu-id="4c24d-381">Число активных вредоносных программ для этого устройства windows унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-381">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-382">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="4c24d-382">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="4c24d-383">Int32</span><span class="sxs-lookup"><span data-stu-id="4c24d-383">Int32</span></span>|<span data-ttu-id="4c24d-384">Число проверка вредоносных программ для этого устройства windows унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-384">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-385">notes</span><span class="sxs-lookup"><span data-stu-id="4c24d-385">notes</span></span>|<span data-ttu-id="4c24d-386">String</span><span class="sxs-lookup"><span data-stu-id="4c24d-386">String</span></span>|<span data-ttu-id="4c24d-387">Заметки на устройстве, созданные ИТ Admin наследуется из [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-387">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4c24d-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="4c24d-388">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="4c24d-389">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="4c24d-389">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="4c24d-390">Конфигурация диспетчера состоянием работоспособности клиента, только для устройств, управляемых MDM/ConfigMgr агента наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4c24d-390">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4c24d-391">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c24d-391">Response</span></span>
<span data-ttu-id="4c24d-392">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4c24d-392">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c24d-393">Пример</span><span class="sxs-lookup"><span data-stu-id="4c24d-393">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c24d-394">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c24d-394">Request</span></span>
<span data-ttu-id="4c24d-395">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c24d-395">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7114

{
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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
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
    "windowsUpdateForBusiness": true
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
  }
}
```

### <a name="response"></a><span data-ttu-id="4c24d-396">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c24d-396">Response</span></span>
<span data-ttu-id="4c24d-p142">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4c24d-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7222

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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
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
    "windowsUpdateForBusiness": true
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
  }
}
```





