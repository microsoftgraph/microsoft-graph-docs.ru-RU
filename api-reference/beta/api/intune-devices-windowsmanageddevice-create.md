---
title: Создание Виндовсманажеддевице
description: Создание нового объекта Виндовсманажеддевице.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f8da966e7219f24ab9f3e907acdbc871d8b5ce8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467825"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="d0e08-103">Создание Виндовсманажеддевице</span><span class="sxs-lookup"><span data-stu-id="d0e08-103">Create windowsManagedDevice</span></span>

<span data-ttu-id="d0e08-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d0e08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0e08-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0e08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0e08-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0e08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0e08-107">Создание нового объекта [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="d0e08-107">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0e08-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d0e08-108">Prerequisites</span></span>
<span data-ttu-id="d0e08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0e08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0e08-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0e08-111">Permission type</span></span>|<span data-ttu-id="d0e08-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0e08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0e08-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0e08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0e08-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0e08-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d0e08-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0e08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0e08-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0e08-116">Not supported.</span></span>|
|<span data-ttu-id="d0e08-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0e08-117">Application</span></span>|<span data-ttu-id="d0e08-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0e08-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0e08-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0e08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="d0e08-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d0e08-120">Request headers</span></span>
|<span data-ttu-id="d0e08-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0e08-121">Header</span></span>|<span data-ttu-id="d0e08-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d0e08-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0e08-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0e08-123">Authorization</span></span>|<span data-ttu-id="d0e08-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0e08-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0e08-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d0e08-125">Accept</span></span>|<span data-ttu-id="d0e08-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0e08-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0e08-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0e08-127">Request body</span></span>
<span data-ttu-id="d0e08-128">В тексте запроса добавьте представление объекта Виндовсманажеддевице в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0e08-128">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="d0e08-129">В следующей таблице приведены свойства, необходимые при создании Виндовсманажеддевице.</span><span class="sxs-lookup"><span data-stu-id="d0e08-129">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="d0e08-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0e08-130">Property</span></span>|<span data-ttu-id="d0e08-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d0e08-131">Type</span></span>|<span data-ttu-id="d0e08-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d0e08-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0e08-133">id</span><span class="sxs-lookup"><span data-stu-id="d0e08-133">id</span></span>|<span data-ttu-id="d0e08-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d0e08-134">String</span></span>|<span data-ttu-id="d0e08-135">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-135">Unique Identifier for the device.</span></span> <span data-ttu-id="d0e08-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-136">This property is read-only.</span></span> <span data-ttu-id="d0e08-137">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-137">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-138">userId</span><span class="sxs-lookup"><span data-stu-id="d0e08-138">userId</span></span>|<span data-ttu-id="d0e08-139">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-139">String</span></span>|<span data-ttu-id="d0e08-140">Уникальный идентификатор пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="d0e08-140">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="d0e08-141">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-141">This property is read-only.</span></span> <span data-ttu-id="d0e08-142">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-142">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="d0e08-143">deviceName</span></span>|<span data-ttu-id="d0e08-144">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-144">String</span></span>|<span data-ttu-id="d0e08-145">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-145">Name of the device.</span></span> <span data-ttu-id="d0e08-146">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-146">This property is read-only.</span></span> <span data-ttu-id="d0e08-147">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-147">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-148">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="d0e08-148">hardwareInformation</span></span>|[<span data-ttu-id="d0e08-149">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="d0e08-149">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="d0e08-150">Сведения о хардвард для устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-150">The hardward details for the device.</span></span>  <span data-ttu-id="d0e08-151">Включает такие сведения, как место хранения, производитель, серийный номер и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-151">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="d0e08-152">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-152">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="d0e08-153">ownerType</span></span>|[<span data-ttu-id="d0e08-154">ownerType</span><span class="sxs-lookup"><span data-stu-id="d0e08-154">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="d0e08-155">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="d0e08-155">Ownership of the device.</span></span> <span data-ttu-id="d0e08-156">Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0e08-156">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d0e08-157">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="d0e08-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="d0e08-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="d0e08-158">managedDeviceOwnerType</span></span>|[<span data-ttu-id="d0e08-159">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="d0e08-159">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="d0e08-160">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="d0e08-160">Ownership of the device.</span></span> <span data-ttu-id="d0e08-161">Может быть "Company" или "Personal", наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0e08-161">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d0e08-162">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="d0e08-162">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="d0e08-163">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="d0e08-163">deviceActionResults</span></span>|<span data-ttu-id="d0e08-164">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="d0e08-165">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="d0e08-165">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="d0e08-166">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-166">This property is read-only.</span></span> <span data-ttu-id="d0e08-167">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-168">манажементстате</span><span class="sxs-lookup"><span data-stu-id="d0e08-168">managementState</span></span>|[<span data-ttu-id="d0e08-169">манажементстате</span><span class="sxs-lookup"><span data-stu-id="d0e08-169">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="d0e08-170">Состояние управления для устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-170">Management state of the device.</span></span> <span data-ttu-id="d0e08-171">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-171">This property is read-only.</span></span> <span data-ttu-id="d0e08-172">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0e08-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d0e08-173">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="d0e08-173">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="d0e08-174">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="d0e08-174">enrolledDateTime</span></span>|<span data-ttu-id="d0e08-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0e08-175">DateTimeOffset</span></span>|<span data-ttu-id="d0e08-176">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-176">Enrollment time of the device.</span></span> <span data-ttu-id="d0e08-177">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-177">This property is read-only.</span></span> <span data-ttu-id="d0e08-178">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-178">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-179">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d0e08-179">lastSyncDateTime</span></span>|<span data-ttu-id="d0e08-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0e08-180">DateTimeOffset</span></span>|<span data-ttu-id="d0e08-181">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="d0e08-181">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="d0e08-182">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-182">This property is read-only.</span></span> <span data-ttu-id="d0e08-183">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-183">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-184">чассистипе</span><span class="sxs-lookup"><span data-stu-id="d0e08-184">chassisType</span></span>|[<span data-ttu-id="d0e08-185">чассистипе</span><span class="sxs-lookup"><span data-stu-id="d0e08-185">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="d0e08-186">Тип корпуса устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-186">Chassis type of the device.</span></span> <span data-ttu-id="d0e08-187">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-187">This property is read-only.</span></span> <span data-ttu-id="d0e08-188">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0e08-188">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d0e08-189">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="d0e08-189">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="d0e08-190">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="d0e08-190">operatingSystem</span></span>|<span data-ttu-id="d0e08-191">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-191">String</span></span>|<span data-ttu-id="d0e08-192">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-192">Operating system of the device.</span></span> <span data-ttu-id="d0e08-193">Windows, iOS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-193">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="d0e08-194">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="d0e08-195">deviceType</span></span>|[<span data-ttu-id="d0e08-196">deviceType</span><span class="sxs-lookup"><span data-stu-id="d0e08-196">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="d0e08-197">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-197">Platform of the device.</span></span> <span data-ttu-id="d0e08-198">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-198">This property is read-only.</span></span> <span data-ttu-id="d0e08-199">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0e08-199">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d0e08-200">Возможные `desktop`значения:, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `blackberry` `palm` `unknown`,,,,,,, `iSocConsumer`,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`</span><span class="sxs-lookup"><span data-stu-id="d0e08-200">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="d0e08-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="d0e08-201">complianceState</span></span>|[<span data-ttu-id="d0e08-202">complianceState</span><span class="sxs-lookup"><span data-stu-id="d0e08-202">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="d0e08-203">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="d0e08-203">Compliance state of the device.</span></span> <span data-ttu-id="d0e08-204">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-204">This property is read-only.</span></span> <span data-ttu-id="d0e08-205">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0e08-205">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d0e08-206">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="d0e08-206">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="d0e08-207">jailBroken</span><span class="sxs-lookup"><span data-stu-id="d0e08-207">jailBroken</span></span>|<span data-ttu-id="d0e08-208">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-208">String</span></span>|<span data-ttu-id="d0e08-209">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="d0e08-209">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="d0e08-210">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-210">This property is read-only.</span></span> <span data-ttu-id="d0e08-211">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-212">managementAgent</span><span class="sxs-lookup"><span data-stu-id="d0e08-212">managementAgent</span></span>|[<span data-ttu-id="d0e08-213">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="d0e08-213">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="d0e08-214">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="d0e08-214">Management channel of the device.</span></span> <span data-ttu-id="d0e08-215">Intune, EAS и т. д. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-215">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="d0e08-216">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0e08-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d0e08-217">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="d0e08-217">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="d0e08-218">osVersion</span><span class="sxs-lookup"><span data-stu-id="d0e08-218">osVersion</span></span>|<span data-ttu-id="d0e08-219">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-219">String</span></span>|<span data-ttu-id="d0e08-220">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-220">Operating system version of the device.</span></span> <span data-ttu-id="d0e08-221">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-221">This property is read-only.</span></span> <span data-ttu-id="d0e08-222">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-222">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-223">easActivated</span><span class="sxs-lookup"><span data-stu-id="d0e08-223">easActivated</span></span>|<span data-ttu-id="d0e08-224">Логический</span><span class="sxs-lookup"><span data-stu-id="d0e08-224">Boolean</span></span>|<span data-ttu-id="d0e08-225">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="d0e08-225">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="d0e08-226">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-226">This property is read-only.</span></span> <span data-ttu-id="d0e08-227">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="d0e08-228">easDeviceId</span></span>|<span data-ttu-id="d0e08-229">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-229">String</span></span>|<span data-ttu-id="d0e08-230">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="d0e08-230">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="d0e08-231">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-231">This property is read-only.</span></span> <span data-ttu-id="d0e08-232">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-232">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-233">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="d0e08-233">easActivationDateTime</span></span>|<span data-ttu-id="d0e08-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0e08-234">DateTimeOffset</span></span>|<span data-ttu-id="d0e08-235">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="d0e08-235">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="d0e08-236">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-236">This property is read-only.</span></span> <span data-ttu-id="d0e08-237">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-238">аадрегистеред</span><span class="sxs-lookup"><span data-stu-id="d0e08-238">aadRegistered</span></span>|<span data-ttu-id="d0e08-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0e08-239">Boolean</span></span>|<span data-ttu-id="d0e08-240">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d0e08-240">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="d0e08-241">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-241">This property is read-only.</span></span> <span data-ttu-id="d0e08-242">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-242">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-243">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="d0e08-243">azureADRegistered</span></span>|<span data-ttu-id="d0e08-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0e08-244">Boolean</span></span>|<span data-ttu-id="d0e08-245">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d0e08-245">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="d0e08-246">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-246">This property is read-only.</span></span> <span data-ttu-id="d0e08-247">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-247">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d0e08-248">deviceEnrollmentType</span></span>|[<span data-ttu-id="d0e08-249">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d0e08-249">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="d0e08-250">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-250">Enrollment type of the device.</span></span> <span data-ttu-id="d0e08-251">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-251">This property is read-only.</span></span> <span data-ttu-id="d0e08-252">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0e08-252">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d0e08-253">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="d0e08-253">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="d0e08-254">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="d0e08-254">lostModeState</span></span>|[<span data-ttu-id="d0e08-255">лостмодестате</span><span class="sxs-lookup"><span data-stu-id="d0e08-255">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="d0e08-256">Указывает, включен ли режим потерянных или отключенных.</span><span class="sxs-lookup"><span data-stu-id="d0e08-256">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="d0e08-257">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-257">This property is read-only.</span></span> <span data-ttu-id="d0e08-258">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0e08-258">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d0e08-259">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="d0e08-259">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="d0e08-260">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="d0e08-260">activationLockBypassCode</span></span>|<span data-ttu-id="d0e08-261">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-261">String</span></span>|<span data-ttu-id="d0e08-262">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d0e08-262">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="d0e08-263">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-263">This property is read-only.</span></span> <span data-ttu-id="d0e08-264">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-265">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d0e08-265">emailAddress</span></span>|<span data-ttu-id="d0e08-266">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-266">String</span></span>|<span data-ttu-id="d0e08-267">Сообщения электронной почты пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="d0e08-267">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="d0e08-268">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-268">This property is read-only.</span></span> <span data-ttu-id="d0e08-269">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-270">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="d0e08-270">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="d0e08-271">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-271">String</span></span>|<span data-ttu-id="d0e08-272">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d0e08-272">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="d0e08-273">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-273">Read only.</span></span> <span data-ttu-id="d0e08-274">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-274">This property is read-only.</span></span> <span data-ttu-id="d0e08-275">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-275">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-276">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="d0e08-276">azureADDeviceId</span></span>|<span data-ttu-id="d0e08-277">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-277">String</span></span>|<span data-ttu-id="d0e08-278">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d0e08-278">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="d0e08-279">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-279">Read only.</span></span> <span data-ttu-id="d0e08-280">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-280">This property is read-only.</span></span> <span data-ttu-id="d0e08-281">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-281">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="d0e08-282">deviceRegistrationState</span></span>|[<span data-ttu-id="d0e08-283">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="d0e08-283">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="d0e08-284">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-284">Device registration state.</span></span> <span data-ttu-id="d0e08-285">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-285">This property is read-only.</span></span> <span data-ttu-id="d0e08-286">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0e08-286">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d0e08-287">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d0e08-287">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="d0e08-288">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="d0e08-288">deviceCategoryDisplayName</span></span>|<span data-ttu-id="d0e08-289">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-289">String</span></span>|<span data-ttu-id="d0e08-290">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="d0e08-290">Device category display name.</span></span> <span data-ttu-id="d0e08-291">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-291">This property is read-only.</span></span> <span data-ttu-id="d0e08-292">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-292">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-293">isSupervised</span><span class="sxs-lookup"><span data-stu-id="d0e08-293">isSupervised</span></span>|<span data-ttu-id="d0e08-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0e08-294">Boolean</span></span>|<span data-ttu-id="d0e08-295">Состояние контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-295">Device supervised status.</span></span> <span data-ttu-id="d0e08-296">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-296">This property is read-only.</span></span> <span data-ttu-id="d0e08-297">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-297">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-298">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d0e08-298">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="d0e08-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0e08-299">DateTimeOffset</span></span>|<span data-ttu-id="d0e08-300">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0e08-300">Last time the device contacted Exchange.</span></span> <span data-ttu-id="d0e08-301">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-301">This property is read-only.</span></span> <span data-ttu-id="d0e08-302">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-302">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="d0e08-303">exchangeAccessState</span></span>|[<span data-ttu-id="d0e08-304">девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="d0e08-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="d0e08-305">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0e08-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="d0e08-306">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-306">This property is read-only.</span></span> <span data-ttu-id="d0e08-307">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0e08-307">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d0e08-308">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="d0e08-308">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="d0e08-309">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="d0e08-309">exchangeAccessStateReason</span></span>|[<span data-ttu-id="d0e08-310">девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="d0e08-310">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="d0e08-311">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0e08-311">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="d0e08-312">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-312">This property is read-only.</span></span> <span data-ttu-id="d0e08-313">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0e08-313">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d0e08-314">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="d0e08-314">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="d0e08-315">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="d0e08-315">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="d0e08-316">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-316">String</span></span>|<span data-ttu-id="d0e08-317">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="d0e08-317">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="d0e08-318">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-318">This property is read-only.</span></span> <span data-ttu-id="d0e08-319">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-319">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-320">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d0e08-320">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="d0e08-321">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-321">String</span></span>|<span data-ttu-id="d0e08-322">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="d0e08-322">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="d0e08-323">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-323">This property is read-only.</span></span> <span data-ttu-id="d0e08-324">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-324">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="d0e08-325">isEncrypted</span></span>|<span data-ttu-id="d0e08-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0e08-326">Boolean</span></span>|<span data-ttu-id="d0e08-327">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-327">Device encryption status.</span></span> <span data-ttu-id="d0e08-328">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-328">This property is read-only.</span></span> <span data-ttu-id="d0e08-329">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-329">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-330">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d0e08-330">userPrincipalName</span></span>|<span data-ttu-id="d0e08-331">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-331">String</span></span>|<span data-ttu-id="d0e08-332">Имя участника пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-332">Device user principal name.</span></span> <span data-ttu-id="d0e08-333">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-333">This property is read-only.</span></span> <span data-ttu-id="d0e08-334">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-334">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-335">model</span><span class="sxs-lookup"><span data-stu-id="d0e08-335">model</span></span>|<span data-ttu-id="d0e08-336">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-336">String</span></span>|<span data-ttu-id="d0e08-337">Модель устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-337">Model of the device.</span></span> <span data-ttu-id="d0e08-338">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-338">This property is read-only.</span></span> <span data-ttu-id="d0e08-339">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-340">manufacturer</span><span class="sxs-lookup"><span data-stu-id="d0e08-340">manufacturer</span></span>|<span data-ttu-id="d0e08-341">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-341">String</span></span>|<span data-ttu-id="d0e08-342">Производитель устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-342">Manufacturer of the device.</span></span> <span data-ttu-id="d0e08-343">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-343">This property is read-only.</span></span> <span data-ttu-id="d0e08-344">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-345">imei</span><span class="sxs-lookup"><span data-stu-id="d0e08-345">imei</span></span>|<span data-ttu-id="d0e08-346">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-346">String</span></span>|<span data-ttu-id="d0e08-347">IMEI.</span><span class="sxs-lookup"><span data-stu-id="d0e08-347">IMEI.</span></span> <span data-ttu-id="d0e08-348">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-348">This property is read-only.</span></span> <span data-ttu-id="d0e08-349">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-349">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-350">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d0e08-350">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d0e08-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0e08-351">DateTimeOffset</span></span>|<span data-ttu-id="d0e08-352">Дата и время истечения льготного периода соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="d0e08-352">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="d0e08-353">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-353">This property is read-only.</span></span> <span data-ttu-id="d0e08-354">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-355">serialNumber</span><span class="sxs-lookup"><span data-stu-id="d0e08-355">serialNumber</span></span>|<span data-ttu-id="d0e08-356">Строка</span><span class="sxs-lookup"><span data-stu-id="d0e08-356">String</span></span>|<span data-ttu-id="d0e08-357">Серийный.</span><span class="sxs-lookup"><span data-stu-id="d0e08-357">SerialNumber.</span></span> <span data-ttu-id="d0e08-358">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-358">This property is read-only.</span></span> <span data-ttu-id="d0e08-359">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-360">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="d0e08-360">phoneNumber</span></span>|<span data-ttu-id="d0e08-361">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-361">String</span></span>|<span data-ttu-id="d0e08-362">Номер телефона устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-362">Phone number of the device.</span></span> <span data-ttu-id="d0e08-363">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-363">This property is read-only.</span></span> <span data-ttu-id="d0e08-364">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-364">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-365">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="d0e08-365">androidSecurityPatchLevel</span></span>|<span data-ttu-id="d0e08-366">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-366">String</span></span>|<span data-ttu-id="d0e08-367">Уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="d0e08-367">Android security patch level.</span></span> <span data-ttu-id="d0e08-368">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-368">This property is read-only.</span></span> <span data-ttu-id="d0e08-369">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-370">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d0e08-370">userDisplayName</span></span>|<span data-ttu-id="d0e08-371">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-371">String</span></span>|<span data-ttu-id="d0e08-372">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="d0e08-372">User display name.</span></span> <span data-ttu-id="d0e08-373">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-373">This property is read-only.</span></span> <span data-ttu-id="d0e08-374">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d0e08-375">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="d0e08-376">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d0e08-376">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="d0e08-377">Функции, поддерживающие клиент Конфигрмгр.</span><span class="sxs-lookup"><span data-stu-id="d0e08-377">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="d0e08-378">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-378">This property is read-only.</span></span> <span data-ttu-id="d0e08-379">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-379">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-380">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="d0e08-380">wiFiMacAddress</span></span>|<span data-ttu-id="d0e08-381">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-381">String</span></span>|<span data-ttu-id="d0e08-382">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="d0e08-382">Wi-Fi MAC.</span></span> <span data-ttu-id="d0e08-383">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-383">This property is read-only.</span></span> <span data-ttu-id="d0e08-384">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-384">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d0e08-385">deviceHealthAttestationState</span></span>|[<span data-ttu-id="d0e08-386">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d0e08-386">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="d0e08-387">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-387">The device health attestation state.</span></span> <span data-ttu-id="d0e08-388">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-388">This property is read-only.</span></span> <span data-ttu-id="d0e08-389">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-389">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-390">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="d0e08-390">subscriberCarrier</span></span>|<span data-ttu-id="d0e08-391">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-391">String</span></span>|<span data-ttu-id="d0e08-392">Перевозчик абонента.</span><span class="sxs-lookup"><span data-stu-id="d0e08-392">Subscriber Carrier.</span></span> <span data-ttu-id="d0e08-393">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-393">This property is read-only.</span></span> <span data-ttu-id="d0e08-394">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-394">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-395">meid</span><span class="sxs-lookup"><span data-stu-id="d0e08-395">meid</span></span>|<span data-ttu-id="d0e08-396">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-396">String</span></span>|<span data-ttu-id="d0e08-397">MEID.</span><span class="sxs-lookup"><span data-stu-id="d0e08-397">MEID.</span></span> <span data-ttu-id="d0e08-398">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-398">This property is read-only.</span></span> <span data-ttu-id="d0e08-399">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-399">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-400">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="d0e08-400">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="d0e08-401">Int64</span><span class="sxs-lookup"><span data-stu-id="d0e08-401">Int64</span></span>|<span data-ttu-id="d0e08-402">Общий объем хранилища в байтах.</span><span class="sxs-lookup"><span data-stu-id="d0e08-402">Total Storage in Bytes.</span></span> <span data-ttu-id="d0e08-403">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-403">This property is read-only.</span></span> <span data-ttu-id="d0e08-404">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-404">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-405">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="d0e08-405">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="d0e08-406">Int64</span><span class="sxs-lookup"><span data-stu-id="d0e08-406">Int64</span></span>|<span data-ttu-id="d0e08-407">Свободное хранилище в байтах.</span><span class="sxs-lookup"><span data-stu-id="d0e08-407">Free Storage in Bytes.</span></span> <span data-ttu-id="d0e08-408">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-408">This property is read-only.</span></span> <span data-ttu-id="d0e08-409">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-409">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-410">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="d0e08-410">managedDeviceName</span></span>|<span data-ttu-id="d0e08-411">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-411">String</span></span>|<span data-ttu-id="d0e08-412">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-412">Automatically generated name to identify a device.</span></span> <span data-ttu-id="d0e08-413">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="d0e08-413">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="d0e08-414">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-414">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-415">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="d0e08-415">partnerReportedThreatState</span></span>|[<span data-ttu-id="d0e08-416">манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="d0e08-416">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="d0e08-417">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="d0e08-417">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="d0e08-418">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-418">Read Only.</span></span> <span data-ttu-id="d0e08-419">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-419">This property is read-only.</span></span> <span data-ttu-id="d0e08-420">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0e08-420">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d0e08-421">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="d0e08-421">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="d0e08-422">ретиреафтердатетиме</span><span class="sxs-lookup"><span data-stu-id="d0e08-422">retireAfterDateTime</span></span>|<span data-ttu-id="d0e08-423">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0e08-423">DateTimeOffset</span></span>|<span data-ttu-id="d0e08-424">Указывает время, по истечении которого устройство будет автоматически снято из-за запланированного действия.</span><span class="sxs-lookup"><span data-stu-id="d0e08-424">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="d0e08-425">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-425">This property is read-only.</span></span> <span data-ttu-id="d0e08-426">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-426">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-427">усерслогжедон</span><span class="sxs-lookup"><span data-stu-id="d0e08-427">usersLoggedOn</span></span>|<span data-ttu-id="d0e08-428">Коллекция [логжедонусер](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="d0e08-429">Указывает последнего вошедшего в систему пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-429">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="d0e08-430">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-430">This property is read-only.</span></span> <span data-ttu-id="d0e08-431">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-431">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-432">префермдмоверграупполициапплиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="d0e08-432">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="d0e08-433">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0e08-433">DateTimeOffset</span></span>|<span data-ttu-id="d0e08-434">Сообщает о значении DateTime, заданном параметром Префермдмоверграупполици.</span><span class="sxs-lookup"><span data-stu-id="d0e08-434">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="d0e08-435">Если этот параметр установлен, параметры групповой политики в случае конфликта будут переопределяться параметрами групповой политики.</span><span class="sxs-lookup"><span data-stu-id="d0e08-435">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="d0e08-436">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-436">Read Only.</span></span> <span data-ttu-id="d0e08-437">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-437">This property is read-only.</span></span> <span data-ttu-id="d0e08-438">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-438">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-439">аутопилотенроллед</span><span class="sxs-lookup"><span data-stu-id="d0e08-439">autopilotEnrolled</span></span>|<span data-ttu-id="d0e08-440">Логический</span><span class="sxs-lookup"><span data-stu-id="d0e08-440">Boolean</span></span>|<span data-ttu-id="d0e08-441">Сообщает, зарегистрировано ли управляемое устройство через Автоматический пилот.</span><span class="sxs-lookup"><span data-stu-id="d0e08-441">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="d0e08-442">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-442">This property is read-only.</span></span> <span data-ttu-id="d0e08-443">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-443">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-444">рекуиреусеренроллментаппровал</span><span class="sxs-lookup"><span data-stu-id="d0e08-444">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="d0e08-445">Логический</span><span class="sxs-lookup"><span data-stu-id="d0e08-445">Boolean</span></span>|<span data-ttu-id="d0e08-446">Указывает, является ли управляемое устройство iOS регистрацией на утверждение пользователя.</span><span class="sxs-lookup"><span data-stu-id="d0e08-446">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="d0e08-447">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-447">This property is read-only.</span></span> <span data-ttu-id="d0e08-448">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-448">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-449">манажементцертификатикспиратиондате</span><span class="sxs-lookup"><span data-stu-id="d0e08-449">managementCertificateExpirationDate</span></span>|<span data-ttu-id="d0e08-450">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0e08-450">DateTimeOffset</span></span>|<span data-ttu-id="d0e08-451">Дата окончания срока действия сертификата управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="d0e08-451">Reports device management certificate expiration date.</span></span> <span data-ttu-id="d0e08-452">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-452">This property is read-only.</span></span> <span data-ttu-id="d0e08-453">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-453">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-454">икЦид</span><span class="sxs-lookup"><span data-stu-id="d0e08-454">iccid</span></span>|<span data-ttu-id="d0e08-455">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-455">String</span></span>|<span data-ttu-id="d0e08-456">Идентификатор встроенной карты — это уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="d0e08-456">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="d0e08-457">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-457">This property is read-only.</span></span> <span data-ttu-id="d0e08-458">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-458">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-459">удид</span><span class="sxs-lookup"><span data-stu-id="d0e08-459">udid</span></span>|<span data-ttu-id="d0e08-460">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-460">String</span></span>|<span data-ttu-id="d0e08-461">Уникальный идентификатор устройства для устройств iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="d0e08-461">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="d0e08-462">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-462">This property is read-only.</span></span> <span data-ttu-id="d0e08-463">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-463">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-464">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d0e08-464">roleScopeTagIds</span></span>|<span data-ttu-id="d0e08-465">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d0e08-465">String collection</span></span>|<span data-ttu-id="d0e08-466">Список идентификаторов тегов области для этого экземпляра устройства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-466">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="d0e08-467">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-467">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-468">виндовсактивемалварекаунт</span><span class="sxs-lookup"><span data-stu-id="d0e08-468">windowsActiveMalwareCount</span></span>|<span data-ttu-id="d0e08-469">Int32</span><span class="sxs-lookup"><span data-stu-id="d0e08-469">Int32</span></span>|<span data-ttu-id="d0e08-470">Количество активных вредоносных программ для этого устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="d0e08-470">Count of active malware for this windows device.</span></span> <span data-ttu-id="d0e08-471">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-471">This property is read-only.</span></span> <span data-ttu-id="d0e08-472">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-472">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-473">виндовсремедиатедмалварекаунт</span><span class="sxs-lookup"><span data-stu-id="d0e08-473">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="d0e08-474">Int32</span><span class="sxs-lookup"><span data-stu-id="d0e08-474">Int32</span></span>|<span data-ttu-id="d0e08-475">Количество исправленных вредоносных программ для этого устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="d0e08-475">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="d0e08-476">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-476">This property is read-only.</span></span> <span data-ttu-id="d0e08-477">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-477">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-478">notes</span><span class="sxs-lookup"><span data-stu-id="d0e08-478">notes</span></span>|<span data-ttu-id="d0e08-479">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-479">String</span></span>|<span data-ttu-id="d0e08-480">Примечания на устройстве, созданном администратором ИТ, унаследованном от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-480">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="d0e08-481">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="d0e08-482">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="d0e08-482">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="d0e08-483">Состояние работоспособности клиента Configuration Manager, действующее только для устройств под управлением агентов MDM/ConfigMgr, наследуемых от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-483">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="d0e08-484">configurationManagerClientInformation</span></span>|[<span data-ttu-id="d0e08-485">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="d0e08-485">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="d0e08-486">Сведения о клиенте Configuration Manager, действительные только для управляемых устройств, управляемых дуел и управляемых с помощью агента Configuration Manager, наследуемого от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-486">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-487">есернетмакаддресс</span><span class="sxs-lookup"><span data-stu-id="d0e08-487">ethernetMacAddress</span></span>|<span data-ttu-id="d0e08-488">String</span><span class="sxs-lookup"><span data-stu-id="d0e08-488">String</span></span>|<span data-ttu-id="d0e08-489">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="d0e08-489">Ethernet MAC.</span></span> <span data-ttu-id="d0e08-490">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-490">This property is read-only.</span></span> <span data-ttu-id="d0e08-491">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-491">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-492">фисикалмеморинбитес</span><span class="sxs-lookup"><span data-stu-id="d0e08-492">physicalMemoryInBytes</span></span>|<span data-ttu-id="d0e08-493">Int64</span><span class="sxs-lookup"><span data-stu-id="d0e08-493">Int64</span></span>|<span data-ttu-id="d0e08-494">Общий объем памяти в байтах.</span><span class="sxs-lookup"><span data-stu-id="d0e08-494">Total Memory in Bytes.</span></span> <span data-ttu-id="d0e08-495">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-495">This property is read-only.</span></span> <span data-ttu-id="d0e08-496">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0e08-496">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d0e08-497">процессорарчитектуре</span><span class="sxs-lookup"><span data-stu-id="d0e08-497">processorArchitecture</span></span>|[<span data-ttu-id="d0e08-498">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="d0e08-498">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="d0e08-499">Архитектура процессора.</span><span class="sxs-lookup"><span data-stu-id="d0e08-499">Processor architecture.</span></span> <span data-ttu-id="d0e08-500">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0e08-500">This property is read-only.</span></span> <span data-ttu-id="d0e08-501">Наследуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0e08-501">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d0e08-502">Возможные значения: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="d0e08-502">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|



## <a name="response"></a><span data-ttu-id="d0e08-503">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0e08-503">Response</span></span>
<span data-ttu-id="d0e08-504">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d0e08-504">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0e08-505">Пример</span><span class="sxs-lookup"><span data-stu-id="d0e08-505">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0e08-506">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0e08-506">Request</span></span>
<span data-ttu-id="d0e08-507">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0e08-507">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 7641

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
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86"
}
```

### <a name="response"></a><span data-ttu-id="d0e08-508">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0e08-508">Response</span></span>
<span data-ttu-id="d0e08-p171">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0e08-p171">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7690

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
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86"
}
```





