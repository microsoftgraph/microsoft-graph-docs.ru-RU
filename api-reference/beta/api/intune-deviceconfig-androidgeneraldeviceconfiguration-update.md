---
title: Update androidGeneralDeviceConfiguration
description: Обновление свойств объекта androidGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1fc7f6b0681a0b9ddb8f25a182a68c5b4310abe3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34970186"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="50ebd-103">Update androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="50ebd-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="50ebd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50ebd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50ebd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50ebd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50ebd-106">Обновление свойств объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50ebd-106">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50ebd-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="50ebd-107">Prerequisites</span></span>
<span data-ttu-id="50ebd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50ebd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50ebd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50ebd-110">Permission type</span></span>|<span data-ttu-id="50ebd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50ebd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50ebd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50ebd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50ebd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50ebd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50ebd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50ebd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50ebd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50ebd-115">Not supported.</span></span>|
|<span data-ttu-id="50ebd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50ebd-116">Application</span></span>|<span data-ttu-id="50ebd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50ebd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50ebd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50ebd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="50ebd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50ebd-119">Request headers</span></span>
|<span data-ttu-id="50ebd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50ebd-120">Header</span></span>|<span data-ttu-id="50ebd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="50ebd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50ebd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50ebd-122">Authorization</span></span>|<span data-ttu-id="50ebd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50ebd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50ebd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="50ebd-124">Accept</span></span>|<span data-ttu-id="50ebd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="50ebd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50ebd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="50ebd-126">Request body</span></span>
<span data-ttu-id="50ebd-127">В тексте запроса добавьте представление объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50ebd-127">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="50ebd-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50ebd-128">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="50ebd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="50ebd-129">Property</span></span>|<span data-ttu-id="50ebd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="50ebd-130">Type</span></span>|<span data-ttu-id="50ebd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="50ebd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50ebd-132">id</span><span class="sxs-lookup"><span data-stu-id="50ebd-132">id</span></span>|<span data-ttu-id="50ebd-133">String</span><span class="sxs-lookup"><span data-stu-id="50ebd-133">String</span></span>|<span data-ttu-id="50ebd-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="50ebd-134">Key of the entity.</span></span> <span data-ttu-id="50ebd-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50ebd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50ebd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50ebd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="50ebd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50ebd-137">DateTimeOffset</span></span>|<span data-ttu-id="50ebd-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="50ebd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="50ebd-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50ebd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50ebd-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50ebd-140">roleScopeTagIds</span></span>|<span data-ttu-id="50ebd-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="50ebd-141">String collection</span></span>|<span data-ttu-id="50ebd-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="50ebd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="50ebd-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50ebd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50ebd-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="50ebd-144">supportsScopeTags</span></span>|<span data-ttu-id="50ebd-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-145">Boolean</span></span>|<span data-ttu-id="50ebd-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="50ebd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="50ebd-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="50ebd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="50ebd-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="50ebd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="50ebd-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50ebd-149">This property is read-only.</span></span> <span data-ttu-id="50ebd-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50ebd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50ebd-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="50ebd-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="50ebd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="50ebd-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="50ebd-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="50ebd-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="50ebd-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50ebd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50ebd-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="50ebd-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="50ebd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="50ebd-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="50ebd-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="50ebd-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="50ebd-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50ebd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50ebd-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="50ebd-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="50ebd-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="50ebd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="50ebd-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="50ebd-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="50ebd-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50ebd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50ebd-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50ebd-163">createdDateTime</span></span>|<span data-ttu-id="50ebd-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50ebd-164">DateTimeOffset</span></span>|<span data-ttu-id="50ebd-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="50ebd-165">DateTime the object was created.</span></span> <span data-ttu-id="50ebd-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50ebd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50ebd-167">description</span><span class="sxs-lookup"><span data-stu-id="50ebd-167">description</span></span>|<span data-ttu-id="50ebd-168">String</span><span class="sxs-lookup"><span data-stu-id="50ebd-168">String</span></span>|<span data-ttu-id="50ebd-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="50ebd-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="50ebd-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50ebd-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50ebd-171">displayName</span><span class="sxs-lookup"><span data-stu-id="50ebd-171">displayName</span></span>|<span data-ttu-id="50ebd-172">Строка</span><span class="sxs-lookup"><span data-stu-id="50ebd-172">String</span></span>|<span data-ttu-id="50ebd-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="50ebd-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="50ebd-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50ebd-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50ebd-175">version</span><span class="sxs-lookup"><span data-stu-id="50ebd-175">version</span></span>|<span data-ttu-id="50ebd-176">Int32</span><span class="sxs-lookup"><span data-stu-id="50ebd-176">Int32</span></span>|<span data-ttu-id="50ebd-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="50ebd-177">Version of the device configuration.</span></span> <span data-ttu-id="50ebd-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50ebd-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50ebd-179">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="50ebd-179">appsBlockClipboardSharing</span></span>|<span data-ttu-id="50ebd-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-180">Boolean</span></span>|<span data-ttu-id="50ebd-181">Указывает, следует ли запретить совместное использование буфера обмена для копирования данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="50ebd-181">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="50ebd-182">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="50ebd-182">appsBlockCopyPaste</span></span>|<span data-ttu-id="50ebd-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-183">Boolean</span></span>|<span data-ttu-id="50ebd-184">Указывает, следует ли запретить копирование данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="50ebd-184">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="50ebd-185">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="50ebd-185">appsBlockYouTube</span></span>|<span data-ttu-id="50ebd-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-186">Boolean</span></span>|<span data-ttu-id="50ebd-187">Указывает, следует ли заблокировать приложение YouTube.</span><span class="sxs-lookup"><span data-stu-id="50ebd-187">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="50ebd-188">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="50ebd-188">bluetoothBlocked</span></span>|<span data-ttu-id="50ebd-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-189">Boolean</span></span>|<span data-ttu-id="50ebd-190">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="50ebd-190">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="50ebd-191">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="50ebd-191">cameraBlocked</span></span>|<span data-ttu-id="50ebd-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-192">Boolean</span></span>|<span data-ttu-id="50ebd-193">Указывает, следует ли запретить использовать камеру.</span><span class="sxs-lookup"><span data-stu-id="50ebd-193">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="50ebd-194">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="50ebd-194">cellularBlockDataRoaming</span></span>|<span data-ttu-id="50ebd-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-195">Boolean</span></span>|<span data-ttu-id="50ebd-196">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="50ebd-196">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="50ebd-197">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="50ebd-197">cellularBlockMessaging</span></span>|<span data-ttu-id="50ebd-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-198">Boolean</span></span>|<span data-ttu-id="50ebd-199">Указывает, следует ли запретить обмениваться SMS и MMS.</span><span class="sxs-lookup"><span data-stu-id="50ebd-199">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="50ebd-200">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="50ebd-200">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="50ebd-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-201">Boolean</span></span>|<span data-ttu-id="50ebd-202">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="50ebd-202">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="50ebd-203">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="50ebd-203">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="50ebd-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-204">Boolean</span></span>|<span data-ttu-id="50ebd-205">Указывает, следует ли блокировать синхронизацию модема Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="50ebd-205">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="50ebd-206">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="50ebd-206">compliantAppsList</span></span>|<span data-ttu-id="50ebd-207">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="50ebd-207">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="50ebd-208">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="50ebd-208">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="50ebd-209">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="50ebd-209">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="50ebd-210">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="50ebd-210">compliantAppListType</span></span>|[<span data-ttu-id="50ebd-211">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="50ebd-211">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="50ebd-212">Тип списка, определенного свойством CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="50ebd-212">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="50ebd-213">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="50ebd-213">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="50ebd-214">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="50ebd-214">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="50ebd-215">Логический</span><span class="sxs-lookup"><span data-stu-id="50ebd-215">Boolean</span></span>|<span data-ttu-id="50ebd-216">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="50ebd-216">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="50ebd-217">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="50ebd-217">locationServicesBlocked</span></span>|<span data-ttu-id="50ebd-218">Логический</span><span class="sxs-lookup"><span data-stu-id="50ebd-218">Boolean</span></span>|<span data-ttu-id="50ebd-219">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="50ebd-219">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="50ebd-220">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="50ebd-220">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="50ebd-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-221">Boolean</span></span>|<span data-ttu-id="50ebd-222">Указывает, следует ли блокировать автоматическую синхронизацию учетной записи Google.</span><span class="sxs-lookup"><span data-stu-id="50ebd-222">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="50ebd-223">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="50ebd-223">googlePlayStoreBlocked</span></span>|<span data-ttu-id="50ebd-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-224">Boolean</span></span>|<span data-ttu-id="50ebd-225">Указывает, следует ли блокировать Google Play Маркет.</span><span class="sxs-lookup"><span data-stu-id="50ebd-225">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="50ebd-226">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="50ebd-226">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="50ebd-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-227">Boolean</span></span>|<span data-ttu-id="50ebd-228">Указывает, следует ли блокировать кнопку спящего режима экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="50ebd-228">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="50ebd-229">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="50ebd-229">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="50ebd-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-230">Boolean</span></span>|<span data-ttu-id="50ebd-231">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="50ebd-231">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="50ebd-232">Датеандтимеблоккчанжес</span><span class="sxs-lookup"><span data-stu-id="50ebd-232">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="50ebd-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-233">Boolean</span></span>|<span data-ttu-id="50ebd-234">Указывает, следует ли заблокировать изменение даты и времени в режиме KNOX.</span><span class="sxs-lookup"><span data-stu-id="50ebd-234">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="50ebd-235">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="50ebd-235">kioskModeApps</span></span>|<span data-ttu-id="50ebd-236">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="50ebd-236">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="50ebd-237">Список разрешенных приложений в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="50ebd-237">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="50ebd-238">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="50ebd-238">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="50ebd-239">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="50ebd-239">nfcBlocked</span></span>|<span data-ttu-id="50ebd-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-240">Boolean</span></span>|<span data-ttu-id="50ebd-241">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="50ebd-241">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="50ebd-242">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="50ebd-242">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="50ebd-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-243">Boolean</span></span>|<span data-ttu-id="50ebd-244">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="50ebd-244">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="50ebd-245">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="50ebd-245">passwordBlockTrustAgents</span></span>|<span data-ttu-id="50ebd-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-246">Boolean</span></span>|<span data-ttu-id="50ebd-247">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="50ebd-247">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="50ebd-248">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="50ebd-248">passwordExpirationDays</span></span>|<span data-ttu-id="50ebd-249">Int32</span><span class="sxs-lookup"><span data-stu-id="50ebd-249">Int32</span></span>|<span data-ttu-id="50ebd-250">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="50ebd-250">Number of days before the password expires.</span></span> <span data-ttu-id="50ebd-251">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="50ebd-251">Valid values 1 to 365</span></span>|
|<span data-ttu-id="50ebd-252">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="50ebd-252">passwordMinimumLength</span></span>|<span data-ttu-id="50ebd-253">Int32</span><span class="sxs-lookup"><span data-stu-id="50ebd-253">Int32</span></span>|<span data-ttu-id="50ebd-254">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="50ebd-254">Minimum length of passwords.</span></span> <span data-ttu-id="50ebd-255">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="50ebd-255">Valid values 4 to 16</span></span>|
|<span data-ttu-id="50ebd-256">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="50ebd-256">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="50ebd-257">Int32</span><span class="sxs-lookup"><span data-stu-id="50ebd-257">Int32</span></span>|<span data-ttu-id="50ebd-258">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="50ebd-258">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="50ebd-259">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="50ebd-259">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="50ebd-260">Int32</span><span class="sxs-lookup"><span data-stu-id="50ebd-260">Int32</span></span>|<span data-ttu-id="50ebd-261">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="50ebd-261">Number of previous passwords to block.</span></span> <span data-ttu-id="50ebd-262">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="50ebd-262">Valid values 0 to 24</span></span>|
|<span data-ttu-id="50ebd-263">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="50ebd-263">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="50ebd-264">Int32</span><span class="sxs-lookup"><span data-stu-id="50ebd-264">Int32</span></span>|<span data-ttu-id="50ebd-265">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="50ebd-265">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="50ebd-266">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="50ebd-266">Valid values 1 to 16</span></span>|
|<span data-ttu-id="50ebd-267">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="50ebd-267">passwordRequiredType</span></span>|[<span data-ttu-id="50ebd-268">Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="50ebd-268">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="50ebd-269">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="50ebd-269">Type of password that is required.</span></span> <span data-ttu-id="50ebd-270">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="50ebd-270">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="50ebd-271">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="50ebd-271">passwordRequired</span></span>|<span data-ttu-id="50ebd-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-272">Boolean</span></span>|<span data-ttu-id="50ebd-273">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="50ebd-273">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="50ebd-274">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="50ebd-274">powerOffBlocked</span></span>|<span data-ttu-id="50ebd-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-275">Boolean</span></span>|<span data-ttu-id="50ebd-276">Указывает, следует ли блокировать отключение устройства.</span><span class="sxs-lookup"><span data-stu-id="50ebd-276">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="50ebd-277">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="50ebd-277">factoryResetBlocked</span></span>|<span data-ttu-id="50ebd-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-278">Boolean</span></span>|<span data-ttu-id="50ebd-279">Указывает, следует ли запретить пользователю восстанавливать заводские настройки.</span><span class="sxs-lookup"><span data-stu-id="50ebd-279">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="50ebd-280">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="50ebd-280">screenCaptureBlocked</span></span>|<span data-ttu-id="50ebd-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-281">Boolean</span></span>|<span data-ttu-id="50ebd-282">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="50ebd-282">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="50ebd-283">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="50ebd-283">deviceSharingAllowed</span></span>|<span data-ttu-id="50ebd-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-284">Boolean</span></span>|<span data-ttu-id="50ebd-285">Указывает, следует ли разрешить режим совместного доступа к устройству.</span><span class="sxs-lookup"><span data-stu-id="50ebd-285">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="50ebd-286">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="50ebd-286">storageBlockGoogleBackup</span></span>|<span data-ttu-id="50ebd-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-287">Boolean</span></span>|<span data-ttu-id="50ebd-288">Указывает, следует ли блокировать резервное копирование Google.</span><span class="sxs-lookup"><span data-stu-id="50ebd-288">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="50ebd-289">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="50ebd-289">storageBlockRemovableStorage</span></span>|<span data-ttu-id="50ebd-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-290">Boolean</span></span>|<span data-ttu-id="50ebd-291">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="50ebd-291">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="50ebd-292">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="50ebd-292">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="50ebd-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-293">Boolean</span></span>|<span data-ttu-id="50ebd-294">Указывает, обязательно ли шифрование устройства.</span><span class="sxs-lookup"><span data-stu-id="50ebd-294">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="50ebd-295">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="50ebd-295">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="50ebd-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-296">Boolean</span></span>|<span data-ttu-id="50ebd-297">Указывает, обязательно ли шифрование съемных носителей.</span><span class="sxs-lookup"><span data-stu-id="50ebd-297">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="50ebd-298">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="50ebd-298">voiceAssistantBlocked</span></span>|<span data-ttu-id="50ebd-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-299">Boolean</span></span>|<span data-ttu-id="50ebd-300">Указывает, следует ли блокировать использование голосового помощника.</span><span class="sxs-lookup"><span data-stu-id="50ebd-300">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="50ebd-301">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="50ebd-301">voiceDialingBlocked</span></span>|<span data-ttu-id="50ebd-302">Логический</span><span class="sxs-lookup"><span data-stu-id="50ebd-302">Boolean</span></span>|<span data-ttu-id="50ebd-303">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="50ebd-303">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="50ebd-304">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="50ebd-304">webBrowserBlockPopups</span></span>|<span data-ttu-id="50ebd-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-305">Boolean</span></span>|<span data-ttu-id="50ebd-306">Указывает, следует ли блокировать всплывающие окна в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="50ebd-306">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="50ebd-307">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="50ebd-307">webBrowserBlockAutofill</span></span>|<span data-ttu-id="50ebd-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-308">Boolean</span></span>|<span data-ttu-id="50ebd-309">Указывает, следует ли заблокировать функцию автозаполнения в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="50ebd-309">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="50ebd-310">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="50ebd-310">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="50ebd-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-311">Boolean</span></span>|<span data-ttu-id="50ebd-312">Указывает, следует ли заблокировать JavaScript в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="50ebd-312">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="50ebd-313">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="50ebd-313">webBrowserBlocked</span></span>|<span data-ttu-id="50ebd-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-314">Boolean</span></span>|<span data-ttu-id="50ebd-315">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="50ebd-315">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="50ebd-316">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="50ebd-316">webBrowserCookieSettings</span></span>|[<span data-ttu-id="50ebd-317">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="50ebd-317">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="50ebd-318">Настройки файлов cookie в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="50ebd-318">Cookie settings within the web browser.</span></span> <span data-ttu-id="50ebd-319">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="50ebd-319">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="50ebd-320">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="50ebd-320">wiFiBlocked</span></span>|<span data-ttu-id="50ebd-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-321">Boolean</span></span>|<span data-ttu-id="50ebd-322">Указывает, следует ли заблокировать синхронизацию Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="50ebd-322">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="50ebd-323">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="50ebd-323">appsInstallAllowList</span></span>|<span data-ttu-id="50ebd-324">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="50ebd-324">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="50ebd-325">Список приложений, которые можно установить на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="50ebd-325">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="50ebd-326">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="50ebd-326">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="50ebd-327">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="50ebd-327">appsLaunchBlockList</span></span>|<span data-ttu-id="50ebd-328">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="50ebd-328">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="50ebd-329">Список приложений, которые запрещено запускать на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="50ebd-329">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="50ebd-330">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="50ebd-330">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="50ebd-331">appsHideList</span><span class="sxs-lookup"><span data-stu-id="50ebd-331">appsHideList</span></span>|<span data-ttu-id="50ebd-332">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="50ebd-332">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="50ebd-333">Список приложений, которые следует скрыть на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="50ebd-333">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="50ebd-334">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="50ebd-334">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="50ebd-335">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="50ebd-335">securityRequireVerifyApps</span></span>|<span data-ttu-id="50ebd-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="50ebd-336">Boolean</span></span>|<span data-ttu-id="50ebd-337">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="50ebd-337">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="50ebd-338">Ответ</span><span class="sxs-lookup"><span data-stu-id="50ebd-338">Response</span></span>
<span data-ttu-id="50ebd-339">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="50ebd-339">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50ebd-340">Пример</span><span class="sxs-lookup"><span data-stu-id="50ebd-340">Example</span></span>

### <a name="request"></a><span data-ttu-id="50ebd-341">Запрос</span><span class="sxs-lookup"><span data-stu-id="50ebd-341">Request</span></span>
<span data-ttu-id="50ebd-342">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50ebd-342">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3934

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="50ebd-343">Отклик</span><span class="sxs-lookup"><span data-stu-id="50ebd-343">Response</span></span>
<span data-ttu-id="50ebd-p125">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50ebd-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4106

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```





