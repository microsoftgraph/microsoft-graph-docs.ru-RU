---
title: Создание Виндовсманажеддевице
description: Создание нового объекта Виндовсманажеддевице.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fdc1c7c142e0c00a5eb8b9129018d1ee4e434e6f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525308"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="c0ee9-103">Создание Виндовсманажеддевице</span><span class="sxs-lookup"><span data-stu-id="c0ee9-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="c0ee9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0ee9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0ee9-106">Создание нового объекта [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="c0ee9-106">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0ee9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c0ee9-107">Prerequisites</span></span>
<span data-ttu-id="c0ee9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0ee9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0ee9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0ee9-110">Permission type</span></span>|<span data-ttu-id="c0ee9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0ee9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0ee9-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0ee9-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c0ee9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0ee9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-115">Not supported.</span></span>|
|<span data-ttu-id="c0ee9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0ee9-116">Application</span></span>|<span data-ttu-id="c0ee9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0ee9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0ee9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="c0ee9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0ee9-119">Request headers</span></span>
|<span data-ttu-id="c0ee9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0ee9-120">Header</span></span>|<span data-ttu-id="c0ee9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c0ee9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0ee9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0ee9-122">Authorization</span></span>|<span data-ttu-id="c0ee9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0ee9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c0ee9-124">Accept</span></span>|<span data-ttu-id="c0ee9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0ee9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0ee9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0ee9-126">Request body</span></span>
<span data-ttu-id="c0ee9-127">В тексте запроса добавьте представление объекта Виндовсманажеддевице в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-127">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="c0ee9-128">В следующей таблице приведены свойства, необходимые при создании Виндовсманажеддевице.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-128">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="c0ee9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0ee9-129">Property</span></span>|<span data-ttu-id="c0ee9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c0ee9-130">Type</span></span>|<span data-ttu-id="c0ee9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c0ee9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0ee9-132">id</span><span class="sxs-lookup"><span data-stu-id="c0ee9-132">id</span></span>|<span data-ttu-id="c0ee9-133">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-133">String</span></span>|<span data-ttu-id="c0ee9-134">Уникальный идентификатор устройства, наСледуемого от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-134">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-135">userId</span><span class="sxs-lookup"><span data-stu-id="c0ee9-135">userId</span></span>|<span data-ttu-id="c0ee9-136">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-136">String</span></span>|<span data-ttu-id="c0ee9-137">Уникальный идентификатор пользователя, связанного с устройством, унаследованным от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-137">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="c0ee9-138">deviceName</span></span>|<span data-ttu-id="c0ee9-139">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-139">String</span></span>|<span data-ttu-id="c0ee9-140">Имя устройства, унаследованного от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-140">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-141">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-141">hardwareInformation</span></span>|[<span data-ttu-id="c0ee9-142">Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="c0ee9-143">Сведения о хардвард для устройства.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-143">The hardward details for the device.</span></span>  <span data-ttu-id="c0ee9-144">Включает такие сведения, как место хранения, производитель, серийный номер и т. д. НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-144">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-145">ownerType</span><span class="sxs-lookup"><span data-stu-id="c0ee9-145">ownerType</span></span>|[<span data-ttu-id="c0ee9-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="c0ee9-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="c0ee9-147">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-147">Ownership of the device.</span></span> <span data-ttu-id="c0ee9-148">Может быть "Company" или "Personal", наСледуемых от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="c0ee9-148">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="c0ee9-149">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="c0ee9-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="c0ee9-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="c0ee9-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="c0ee9-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="c0ee9-152">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-152">Ownership of the device.</span></span> <span data-ttu-id="c0ee9-153">Может быть "Company" или "Personal", наСледуемых от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="c0ee9-153">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="c0ee9-154">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="c0ee9-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="c0ee9-155">deviceActionResults</span></span>|<span data-ttu-id="c0ee9-156">Коллекция [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="c0ee9-157">Список объектов deviceActionResult сложного типа.
</span><span class="sxs-lookup"><span data-stu-id="c0ee9-157">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="c0ee9-158">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-158">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-159">Манажементстате</span><span class="sxs-lookup"><span data-stu-id="c0ee9-159">managementState</span></span>|[<span data-ttu-id="c0ee9-160">Манажементстате</span><span class="sxs-lookup"><span data-stu-id="c0ee9-160">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="c0ee9-161">Состояние управления для устройства.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-161">Management state of the device.</span></span> <span data-ttu-id="c0ee9-162">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="c0ee9-162">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="c0ee9-163">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-163">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="c0ee9-164">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="c0ee9-164">enrolledDateTime</span></span>|<span data-ttu-id="c0ee9-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0ee9-165">DateTimeOffset</span></span>|<span data-ttu-id="c0ee9-166">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-166">Enrollment time of the device.</span></span> <span data-ttu-id="c0ee9-167">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-168">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c0ee9-168">lastSyncDateTime</span></span>|<span data-ttu-id="c0ee9-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0ee9-169">DateTimeOffset</span></span>|<span data-ttu-id="c0ee9-170">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-170">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="c0ee9-171">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-172">Чассистипе</span><span class="sxs-lookup"><span data-stu-id="c0ee9-172">chassisType</span></span>|[<span data-ttu-id="c0ee9-173">Чассистипе</span><span class="sxs-lookup"><span data-stu-id="c0ee9-173">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="c0ee9-174">Тип корпуса устройства.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-174">Chassis type of the device.</span></span> <span data-ttu-id="c0ee9-175">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="c0ee9-175">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="c0ee9-176">Возможные значения: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-176">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="c0ee9-177">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="c0ee9-177">operatingSystem</span></span>|<span data-ttu-id="c0ee9-178">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-178">String</span></span>|<span data-ttu-id="c0ee9-179">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-179">Operating system of the device.</span></span> <span data-ttu-id="c0ee9-180">Windows, iOS и т. д. НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-180">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-181">deviceType</span><span class="sxs-lookup"><span data-stu-id="c0ee9-181">deviceType</span></span>|[<span data-ttu-id="c0ee9-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="c0ee9-182">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="c0ee9-183">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-183">Platform of the device.</span></span> <span data-ttu-id="c0ee9-184">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="c0ee9-184">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="c0ee9-185">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `android` `iSocConsumer`,,,,,,,,,,,,,,,,,,,,, `winEmbedded` `iPhone` `iPad` `iPod` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-185">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="c0ee9-186">complianceState</span><span class="sxs-lookup"><span data-stu-id="c0ee9-186">complianceState</span></span>|[<span data-ttu-id="c0ee9-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="c0ee9-187">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="c0ee9-188">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-188">Compliance state of the device.</span></span> <span data-ttu-id="c0ee9-189">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="c0ee9-189">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="c0ee9-190">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-190">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="c0ee9-191">jailBroken</span><span class="sxs-lookup"><span data-stu-id="c0ee9-191">jailBroken</span></span>|<span data-ttu-id="c0ee9-192">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-192">String</span></span>|<span data-ttu-id="c0ee9-193">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-193">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="c0ee9-194">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-195">managementAgent</span><span class="sxs-lookup"><span data-stu-id="c0ee9-195">managementAgent</span></span>|[<span data-ttu-id="c0ee9-196">Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="c0ee9-196">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="c0ee9-197">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-197">Management channel of the device.</span></span> <span data-ttu-id="c0ee9-198">Intune, EAS и т. д. НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="c0ee9-198">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="c0ee9-199">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-199">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="c0ee9-200">osVersion</span><span class="sxs-lookup"><span data-stu-id="c0ee9-200">osVersion</span></span>|<span data-ttu-id="c0ee9-201">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-201">String</span></span>|<span data-ttu-id="c0ee9-202">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-202">Operating system version of the device.</span></span> <span data-ttu-id="c0ee9-203">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-203">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-204">easActivated</span><span class="sxs-lookup"><span data-stu-id="c0ee9-204">easActivated</span></span>|<span data-ttu-id="c0ee9-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0ee9-205">Boolean</span></span>|<span data-ttu-id="c0ee9-206">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-206">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="c0ee9-207">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-207">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-208">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="c0ee9-208">easDeviceId</span></span>|<span data-ttu-id="c0ee9-209">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-209">String</span></span>|<span data-ttu-id="c0ee9-210">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-210">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="c0ee9-211">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-212">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="c0ee9-212">easActivationDateTime</span></span>|<span data-ttu-id="c0ee9-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0ee9-213">DateTimeOffset</span></span>|<span data-ttu-id="c0ee9-214">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-214">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="c0ee9-215">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-216">Аадрегистеред</span><span class="sxs-lookup"><span data-stu-id="c0ee9-216">aadRegistered</span></span>|<span data-ttu-id="c0ee9-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0ee9-217">Boolean</span></span>|<span data-ttu-id="c0ee9-218">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-218">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="c0ee9-219">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-219">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-220">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="c0ee9-220">azureADRegistered</span></span>|<span data-ttu-id="c0ee9-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0ee9-221">Boolean</span></span>|<span data-ttu-id="c0ee9-222">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="c0ee9-223">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-223">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-224">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="c0ee9-224">deviceEnrollmentType</span></span>|[<span data-ttu-id="c0ee9-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="c0ee9-225">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="c0ee9-226">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-226">Enrollment type of the device.</span></span> <span data-ttu-id="c0ee9-227">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="c0ee9-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="c0ee9-228">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-228">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="c0ee9-229">Лостмодестате</span><span class="sxs-lookup"><span data-stu-id="c0ee9-229">lostModeState</span></span>|[<span data-ttu-id="c0ee9-230">Лостмодестате</span><span class="sxs-lookup"><span data-stu-id="c0ee9-230">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="c0ee9-231">Указывает, включен ли режим потерянных или отключенных наСледуемых от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="c0ee9-231">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="c0ee9-232">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-232">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="c0ee9-233">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="c0ee9-233">activationLockBypassCode</span></span>|<span data-ttu-id="c0ee9-234">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-234">String</span></span>|<span data-ttu-id="c0ee9-235">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-235">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="c0ee9-236">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-237">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c0ee9-237">emailAddress</span></span>|<span data-ttu-id="c0ee9-238">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-238">String</span></span>|<span data-ttu-id="c0ee9-239">Сообщения электронной почты пользователя, связанного с устройством, унаследованным из [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-239">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-240">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="c0ee9-240">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="c0ee9-241">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-241">String</span></span>|<span data-ttu-id="c0ee9-242">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-242">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="c0ee9-243">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-243">Read only.</span></span> <span data-ttu-id="c0ee9-244">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-244">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-245">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="c0ee9-245">azureADDeviceId</span></span>|<span data-ttu-id="c0ee9-246">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-246">String</span></span>|<span data-ttu-id="c0ee9-247">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="c0ee9-248">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-248">Read only.</span></span> <span data-ttu-id="c0ee9-249">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-249">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-250">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="c0ee9-250">deviceRegistrationState</span></span>|[<span data-ttu-id="c0ee9-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="c0ee9-251">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="c0ee9-252">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-252">Device registration state.</span></span> <span data-ttu-id="c0ee9-253">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="c0ee9-253">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="c0ee9-254">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-254">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="c0ee9-255">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="c0ee9-255">deviceCategoryDisplayName</span></span>|<span data-ttu-id="c0ee9-256">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-256">String</span></span>|<span data-ttu-id="c0ee9-257">Отображаемое имя категории устройств, унаследованное от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-257">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-258">isSupervised</span><span class="sxs-lookup"><span data-stu-id="c0ee9-258">isSupervised</span></span>|<span data-ttu-id="c0ee9-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0ee9-259">Boolean</span></span>|<span data-ttu-id="c0ee9-260">Защищенное состояние устройства унаследовано от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-260">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-261">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c0ee9-261">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="c0ee9-262">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0ee9-262">DateTimeOffset</span></span>|<span data-ttu-id="c0ee9-263">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-263">Last time the device contacted Exchange.</span></span> <span data-ttu-id="c0ee9-264">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-265">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="c0ee9-265">exchangeAccessState</span></span>|[<span data-ttu-id="c0ee9-266">Девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="c0ee9-266">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="c0ee9-267">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-267">The Access State of the device in Exchange.</span></span> <span data-ttu-id="c0ee9-268">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="c0ee9-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="c0ee9-269">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-269">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="c0ee9-270">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="c0ee9-270">exchangeAccessStateReason</span></span>|[<span data-ttu-id="c0ee9-271">Девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="c0ee9-271">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="c0ee9-272">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-272">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="c0ee9-273">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="c0ee9-273">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="c0ee9-274">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-274">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="c0ee9-275">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="c0ee9-275">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="c0ee9-276">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-276">String</span></span>|<span data-ttu-id="c0ee9-277">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-277">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="c0ee9-278">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-278">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-279">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c0ee9-279">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="c0ee9-280">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-280">String</span></span>|<span data-ttu-id="c0ee9-281">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-281">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="c0ee9-282">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-282">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-283">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="c0ee9-283">isEncrypted</span></span>|<span data-ttu-id="c0ee9-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0ee9-284">Boolean</span></span>|<span data-ttu-id="c0ee9-285">Состояние шифрования устройства, унаследованное от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-285">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-286">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c0ee9-286">userPrincipalName</span></span>|<span data-ttu-id="c0ee9-287">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-287">String</span></span>|<span data-ttu-id="c0ee9-288">Имя участника пользователя устройства, унаследованное от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-288">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-289">model</span><span class="sxs-lookup"><span data-stu-id="c0ee9-289">model</span></span>|<span data-ttu-id="c0ee9-290">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-290">String</span></span>|<span data-ttu-id="c0ee9-291">Модель устройства, унаследованного от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-291">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-292">manufacturer</span><span class="sxs-lookup"><span data-stu-id="c0ee9-292">manufacturer</span></span>|<span data-ttu-id="c0ee9-293">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-293">String</span></span>|<span data-ttu-id="c0ee9-294">Производитель устройства, унаследованного от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-294">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-295">imei</span><span class="sxs-lookup"><span data-stu-id="c0ee9-295">imei</span></span>|<span data-ttu-id="c0ee9-296">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-296">String</span></span>|<span data-ttu-id="c0ee9-297">IMEI унаследованы от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-297">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-298">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c0ee9-298">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="c0ee9-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0ee9-299">DateTimeOffset</span></span>|<span data-ttu-id="c0ee9-300">Дата и время истечения льготного периода соответствия устройства, наСледуемого от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-300">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-301">serialNumber</span><span class="sxs-lookup"><span data-stu-id="c0ee9-301">serialNumber</span></span>|<span data-ttu-id="c0ee9-302">Строка</span><span class="sxs-lookup"><span data-stu-id="c0ee9-302">String</span></span>|<span data-ttu-id="c0ee9-303">SerialNumber, наСледуемый от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-303">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-304">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="c0ee9-304">phoneNumber</span></span>|<span data-ttu-id="c0ee9-305">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-305">String</span></span>|<span data-ttu-id="c0ee9-306">Номер телефона устройства, унаследованного от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-306">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-307">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="c0ee9-307">androidSecurityPatchLevel</span></span>|<span data-ttu-id="c0ee9-308">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-308">String</span></span>|<span data-ttu-id="c0ee9-309">Уровень обновления для системы безопасности Android, наСледуемый от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-309">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-310">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c0ee9-310">userDisplayName</span></span>|<span data-ttu-id="c0ee9-311">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-311">String</span></span>|<span data-ttu-id="c0ee9-312">Отображаемое имя пользователя, унаследованное от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-312">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-313">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="c0ee9-313">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="c0ee9-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="c0ee9-314">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="c0ee9-315">Функции, поддерживающие клиент Конфигрмгр, унаследованные от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-315">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-316">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="c0ee9-316">wiFiMacAddress</span></span>|<span data-ttu-id="c0ee9-317">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-317">String</span></span>|<span data-ttu-id="c0ee9-318">MAC-адрес сети Wi-Fi, наСледуемый от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-318">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-319">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="c0ee9-319">deviceHealthAttestationState</span></span>|[<span data-ttu-id="c0ee9-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="c0ee9-320">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="c0ee9-321">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-321">The device health attestation state.</span></span> <span data-ttu-id="c0ee9-322">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-322">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-323">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="c0ee9-323">subscriberCarrier</span></span>|<span data-ttu-id="c0ee9-324">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-324">String</span></span>|<span data-ttu-id="c0ee9-325">Оператор перевозчика абонента, наСледуемый от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-325">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-326">meid</span><span class="sxs-lookup"><span data-stu-id="c0ee9-326">meid</span></span>|<span data-ttu-id="c0ee9-327">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-327">String</span></span>|<span data-ttu-id="c0ee9-328">MEID наСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-328">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-329">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="c0ee9-329">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="c0ee9-330">Int64</span><span class="sxs-lookup"><span data-stu-id="c0ee9-330">Int64</span></span>|<span data-ttu-id="c0ee9-331">Общий объем хранилища в байтах, наСледуемых от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-331">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-332">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="c0ee9-332">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="c0ee9-333">Int64</span><span class="sxs-lookup"><span data-stu-id="c0ee9-333">Int64</span></span>|<span data-ttu-id="c0ee9-334">Свободное хранилище в байтах, наСледуемых от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-334">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-335">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="c0ee9-335">managedDeviceName</span></span>|<span data-ttu-id="c0ee9-336">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-336">String</span></span>|<span data-ttu-id="c0ee9-337">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-337">Automatically generated name to identify a device.</span></span> <span data-ttu-id="c0ee9-338">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-338">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="c0ee9-339">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-340">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="c0ee9-340">partnerReportedThreatState</span></span>|[<span data-ttu-id="c0ee9-341">Манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="c0ee9-341">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="c0ee9-342">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).
</span><span class="sxs-lookup"><span data-stu-id="c0ee9-342">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="c0ee9-343">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-343">Read Only.</span></span> <span data-ttu-id="c0ee9-344">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="c0ee9-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="c0ee9-345">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-345">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="c0ee9-346">Усерслогжедон</span><span class="sxs-lookup"><span data-stu-id="c0ee9-346">usersLoggedOn</span></span>|<span data-ttu-id="c0ee9-347">Коллекция [логжедонусер](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-347">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="c0ee9-348">Указывает последнего вошедшего в систему пользователей устройства, унаследованного от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-348">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-349">Префермдмоверграупполициапплиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="c0ee9-349">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="c0ee9-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0ee9-350">DateTimeOffset</span></span>|<span data-ttu-id="c0ee9-351">Сообщает о значении DateTime, заданном параметром Префермдмоверграупполици.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-351">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="c0ee9-352">Если этот параметр установлен, параметры групповой политики в случае конфликта будут переопределяться параметрами групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-352">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="c0ee9-353">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-353">Read Only.</span></span> <span data-ttu-id="c0ee9-354">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-355">Аутопилотенроллед</span><span class="sxs-lookup"><span data-stu-id="c0ee9-355">autopilotEnrolled</span></span>|<span data-ttu-id="c0ee9-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0ee9-356">Boolean</span></span>|<span data-ttu-id="c0ee9-357">Сообщает, зарегистрировано ли управляемое устройство через Автоматический пилот.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-357">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="c0ee9-358">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-359">Рекуиреусеренроллментаппровал</span><span class="sxs-lookup"><span data-stu-id="c0ee9-359">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="c0ee9-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0ee9-360">Boolean</span></span>|<span data-ttu-id="c0ee9-361">Указывает, является ли управляемое устройство iOS регистрацией на утверждение пользователя.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-361">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="c0ee9-362">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-362">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-363">Манажементцертификатикспиратиондате</span><span class="sxs-lookup"><span data-stu-id="c0ee9-363">managementCertificateExpirationDate</span></span>|<span data-ttu-id="c0ee9-364">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0ee9-364">DateTimeOffset</span></span>|<span data-ttu-id="c0ee9-365">Дата окончания срока действия сертификата управления устройствами наСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-365">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-366">икЦид</span><span class="sxs-lookup"><span data-stu-id="c0ee9-366">iccid</span></span>|<span data-ttu-id="c0ee9-367">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-367">String</span></span>|<span data-ttu-id="c0ee9-368">Идентификатор встроенной карты — это уникальный идентификационный номер SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-368">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="c0ee9-369">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-370">удид</span><span class="sxs-lookup"><span data-stu-id="c0ee9-370">udid</span></span>|<span data-ttu-id="c0ee9-371">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-371">String</span></span>|<span data-ttu-id="c0ee9-372">Уникальный идентификатор устройства для устройств iOS и macOS.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-372">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="c0ee9-373">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-374">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c0ee9-374">roleScopeTagIds</span></span>|<span data-ttu-id="c0ee9-375">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c0ee9-375">String collection</span></span>|<span data-ttu-id="c0ee9-376">Список идентификаторов тегов области для этого экземпляра устройства.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-376">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="c0ee9-377">НаСледуется от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-377">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-378">Виндовсактивемалварекаунт</span><span class="sxs-lookup"><span data-stu-id="c0ee9-378">windowsActiveMalwareCount</span></span>|<span data-ttu-id="c0ee9-379">Int32</span><span class="sxs-lookup"><span data-stu-id="c0ee9-379">Int32</span></span>|<span data-ttu-id="c0ee9-380">Число активных вредоносных программ для этого устройства Windows, унаследованных из [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-380">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-381">Виндовсремедиатедмалварекаунт</span><span class="sxs-lookup"><span data-stu-id="c0ee9-381">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="c0ee9-382">Int32</span><span class="sxs-lookup"><span data-stu-id="c0ee9-382">Int32</span></span>|<span data-ttu-id="c0ee9-383">Количество исправленных вредоносных программ для этого устройства Windows, унаследованных из [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-383">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-384">notes</span><span class="sxs-lookup"><span data-stu-id="c0ee9-384">notes</span></span>|<span data-ttu-id="c0ee9-385">String</span><span class="sxs-lookup"><span data-stu-id="c0ee9-385">String</span></span>|<span data-ttu-id="c0ee9-386">Примечания на устройстве, созданном администратором ИТ, унаследованном от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-386">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="c0ee9-387">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="c0ee9-387">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="c0ee9-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="c0ee9-388">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="c0ee9-389">Состояние работоспособности клиента Configuration Manager, действующее только для устройств под управлением агентов MDM/ConfigMgr, наСледуемых от [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c0ee9-389">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c0ee9-390">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0ee9-390">Response</span></span>
<span data-ttu-id="c0ee9-391">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-391">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0ee9-392">Пример</span><span class="sxs-lookup"><span data-stu-id="c0ee9-392">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0ee9-393">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0ee9-393">Request</span></span>
<span data-ttu-id="c0ee9-394">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-394">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 7231

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

### <a name="response"></a><span data-ttu-id="c0ee9-395">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0ee9-395">Response</span></span>
<span data-ttu-id="c0ee9-p141">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0ee9-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7280

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





