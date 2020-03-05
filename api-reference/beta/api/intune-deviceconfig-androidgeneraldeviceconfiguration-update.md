---
title: Update androidGeneralDeviceConfiguration
description: Обновление свойств объекта androidGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 34bbf29bfb67f3266973844f1ea8d652e85ce39e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443722"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="aa507-103">Update androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="aa507-103">Update androidGeneralDeviceConfiguration</span></span>

<span data-ttu-id="aa507-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="aa507-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa507-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa507-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa507-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa507-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa507-107">Обновление свойств объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa507-107">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa507-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="aa507-108">Prerequisites</span></span>
<span data-ttu-id="aa507-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa507-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa507-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa507-111">Permission type</span></span>|<span data-ttu-id="aa507-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa507-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa507-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa507-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa507-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa507-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aa507-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa507-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa507-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa507-116">Not supported.</span></span>|
|<span data-ttu-id="aa507-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa507-117">Application</span></span>|<span data-ttu-id="aa507-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa507-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa507-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa507-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aa507-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aa507-120">Request headers</span></span>
|<span data-ttu-id="aa507-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aa507-121">Header</span></span>|<span data-ttu-id="aa507-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aa507-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa507-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa507-123">Authorization</span></span>|<span data-ttu-id="aa507-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa507-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa507-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aa507-125">Accept</span></span>|<span data-ttu-id="aa507-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa507-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa507-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa507-127">Request body</span></span>
<span data-ttu-id="aa507-128">В тексте запроса добавьте представление объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa507-128">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="aa507-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa507-129">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="aa507-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa507-130">Property</span></span>|<span data-ttu-id="aa507-131">Тип</span><span class="sxs-lookup"><span data-stu-id="aa507-131">Type</span></span>|<span data-ttu-id="aa507-132">Описание</span><span class="sxs-lookup"><span data-stu-id="aa507-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa507-133">id</span><span class="sxs-lookup"><span data-stu-id="aa507-133">id</span></span>|<span data-ttu-id="aa507-134">String</span><span class="sxs-lookup"><span data-stu-id="aa507-134">String</span></span>|<span data-ttu-id="aa507-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="aa507-135">Key of the entity.</span></span> <span data-ttu-id="aa507-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa507-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa507-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa507-137">lastModifiedDateTime</span></span>|<span data-ttu-id="aa507-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa507-138">DateTimeOffset</span></span>|<span data-ttu-id="aa507-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="aa507-139">DateTime the object was last modified.</span></span> <span data-ttu-id="aa507-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa507-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa507-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aa507-141">roleScopeTagIds</span></span>|<span data-ttu-id="aa507-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="aa507-142">String collection</span></span>|<span data-ttu-id="aa507-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="aa507-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aa507-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa507-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa507-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="aa507-145">supportsScopeTags</span></span>|<span data-ttu-id="aa507-146">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-146">Boolean</span></span>|<span data-ttu-id="aa507-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="aa507-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aa507-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="aa507-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aa507-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="aa507-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aa507-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aa507-150">This property is read-only.</span></span> <span data-ttu-id="aa507-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa507-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa507-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aa507-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="aa507-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aa507-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="aa507-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="aa507-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="aa507-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa507-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa507-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aa507-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="aa507-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aa507-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="aa507-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="aa507-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="aa507-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa507-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa507-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aa507-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="aa507-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aa507-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="aa507-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="aa507-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="aa507-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa507-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa507-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa507-164">createdDateTime</span></span>|<span data-ttu-id="aa507-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa507-165">DateTimeOffset</span></span>|<span data-ttu-id="aa507-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="aa507-166">DateTime the object was created.</span></span> <span data-ttu-id="aa507-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa507-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa507-168">description</span><span class="sxs-lookup"><span data-stu-id="aa507-168">description</span></span>|<span data-ttu-id="aa507-169">String</span><span class="sxs-lookup"><span data-stu-id="aa507-169">String</span></span>|<span data-ttu-id="aa507-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aa507-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aa507-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa507-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa507-172">displayName</span><span class="sxs-lookup"><span data-stu-id="aa507-172">displayName</span></span>|<span data-ttu-id="aa507-173">Строка</span><span class="sxs-lookup"><span data-stu-id="aa507-173">String</span></span>|<span data-ttu-id="aa507-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aa507-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aa507-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa507-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa507-176">version</span><span class="sxs-lookup"><span data-stu-id="aa507-176">version</span></span>|<span data-ttu-id="aa507-177">Int32</span><span class="sxs-lookup"><span data-stu-id="aa507-177">Int32</span></span>|<span data-ttu-id="aa507-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aa507-178">Version of the device configuration.</span></span> <span data-ttu-id="aa507-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa507-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa507-180">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="aa507-180">appsBlockClipboardSharing</span></span>|<span data-ttu-id="aa507-181">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-181">Boolean</span></span>|<span data-ttu-id="aa507-182">Указывает, следует ли запретить совместное использование буфера обмена для копирования данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="aa507-182">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="aa507-183">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="aa507-183">appsBlockCopyPaste</span></span>|<span data-ttu-id="aa507-184">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-184">Boolean</span></span>|<span data-ttu-id="aa507-185">Указывает, следует ли запретить копирование данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="aa507-185">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="aa507-186">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="aa507-186">appsBlockYouTube</span></span>|<span data-ttu-id="aa507-187">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-187">Boolean</span></span>|<span data-ttu-id="aa507-188">Указывает, следует ли заблокировать приложение YouTube.</span><span class="sxs-lookup"><span data-stu-id="aa507-188">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="aa507-189">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="aa507-189">bluetoothBlocked</span></span>|<span data-ttu-id="aa507-190">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-190">Boolean</span></span>|<span data-ttu-id="aa507-191">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="aa507-191">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="aa507-192">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="aa507-192">cameraBlocked</span></span>|<span data-ttu-id="aa507-193">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-193">Boolean</span></span>|<span data-ttu-id="aa507-194">Указывает, следует ли запретить использовать камеру.</span><span class="sxs-lookup"><span data-stu-id="aa507-194">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="aa507-195">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="aa507-195">cellularBlockDataRoaming</span></span>|<span data-ttu-id="aa507-196">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-196">Boolean</span></span>|<span data-ttu-id="aa507-197">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="aa507-197">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="aa507-198">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="aa507-198">cellularBlockMessaging</span></span>|<span data-ttu-id="aa507-199">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-199">Boolean</span></span>|<span data-ttu-id="aa507-200">Указывает, следует ли запретить обмениваться SMS и MMS.</span><span class="sxs-lookup"><span data-stu-id="aa507-200">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="aa507-201">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="aa507-201">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="aa507-202">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-202">Boolean</span></span>|<span data-ttu-id="aa507-203">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="aa507-203">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="aa507-204">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="aa507-204">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="aa507-205">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-205">Boolean</span></span>|<span data-ttu-id="aa507-206">Указывает, следует ли блокировать синхронизацию модема Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="aa507-206">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="aa507-207">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="aa507-207">compliantAppsList</span></span>|<span data-ttu-id="aa507-208">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="aa507-208">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="aa507-209">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="aa507-209">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="aa507-210">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="aa507-210">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="aa507-211">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="aa507-211">compliantAppListType</span></span>|[<span data-ttu-id="aa507-212">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="aa507-212">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="aa507-213">Тип списка, определенного свойством CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="aa507-213">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="aa507-214">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="aa507-214">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="aa507-215">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="aa507-215">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="aa507-216">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-216">Boolean</span></span>|<span data-ttu-id="aa507-217">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="aa507-217">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="aa507-218">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="aa507-218">locationServicesBlocked</span></span>|<span data-ttu-id="aa507-219">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-219">Boolean</span></span>|<span data-ttu-id="aa507-220">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="aa507-220">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="aa507-221">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="aa507-221">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="aa507-222">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-222">Boolean</span></span>|<span data-ttu-id="aa507-223">Указывает, следует ли блокировать автоматическую синхронизацию учетной записи Google.</span><span class="sxs-lookup"><span data-stu-id="aa507-223">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="aa507-224">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="aa507-224">googlePlayStoreBlocked</span></span>|<span data-ttu-id="aa507-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa507-225">Boolean</span></span>|<span data-ttu-id="aa507-226">Указывает, следует ли блокировать Google Play Маркет.</span><span class="sxs-lookup"><span data-stu-id="aa507-226">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="aa507-227">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="aa507-227">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="aa507-228">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-228">Boolean</span></span>|<span data-ttu-id="aa507-229">Указывает, следует ли блокировать кнопку спящего режима экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="aa507-229">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="aa507-230">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="aa507-230">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="aa507-231">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-231">Boolean</span></span>|<span data-ttu-id="aa507-232">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="aa507-232">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="aa507-233">датеандтимеблоккчанжес</span><span class="sxs-lookup"><span data-stu-id="aa507-233">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="aa507-234">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-234">Boolean</span></span>|<span data-ttu-id="aa507-235">Указывает, следует ли заблокировать изменение даты и времени в режиме KNOX.</span><span class="sxs-lookup"><span data-stu-id="aa507-235">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="aa507-236">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="aa507-236">kioskModeApps</span></span>|<span data-ttu-id="aa507-237">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="aa507-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="aa507-238">Список разрешенных приложений в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="aa507-238">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="aa507-239">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="aa507-239">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="aa507-240">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="aa507-240">nfcBlocked</span></span>|<span data-ttu-id="aa507-241">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-241">Boolean</span></span>|<span data-ttu-id="aa507-242">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="aa507-242">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="aa507-243">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="aa507-243">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="aa507-244">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-244">Boolean</span></span>|<span data-ttu-id="aa507-245">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="aa507-245">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="aa507-246">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="aa507-246">passwordBlockTrustAgents</span></span>|<span data-ttu-id="aa507-247">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-247">Boolean</span></span>|<span data-ttu-id="aa507-248">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="aa507-248">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="aa507-249">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="aa507-249">passwordExpirationDays</span></span>|<span data-ttu-id="aa507-250">Int32</span><span class="sxs-lookup"><span data-stu-id="aa507-250">Int32</span></span>|<span data-ttu-id="aa507-251">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="aa507-251">Number of days before the password expires.</span></span> <span data-ttu-id="aa507-252">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="aa507-252">Valid values 1 to 365</span></span>|
|<span data-ttu-id="aa507-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="aa507-253">passwordMinimumLength</span></span>|<span data-ttu-id="aa507-254">Int32</span><span class="sxs-lookup"><span data-stu-id="aa507-254">Int32</span></span>|<span data-ttu-id="aa507-255">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="aa507-255">Minimum length of passwords.</span></span> <span data-ttu-id="aa507-256">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="aa507-256">Valid values 4 to 16</span></span>|
|<span data-ttu-id="aa507-257">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="aa507-257">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="aa507-258">Int32</span><span class="sxs-lookup"><span data-stu-id="aa507-258">Int32</span></span>|<span data-ttu-id="aa507-259">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="aa507-259">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="aa507-260">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="aa507-260">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="aa507-261">Int32</span><span class="sxs-lookup"><span data-stu-id="aa507-261">Int32</span></span>|<span data-ttu-id="aa507-262">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="aa507-262">Number of previous passwords to block.</span></span> <span data-ttu-id="aa507-263">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="aa507-263">Valid values 0 to 24</span></span>|
|<span data-ttu-id="aa507-264">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="aa507-264">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="aa507-265">Int32</span><span class="sxs-lookup"><span data-stu-id="aa507-265">Int32</span></span>|<span data-ttu-id="aa507-266">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="aa507-266">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="aa507-267">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="aa507-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="aa507-268">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="aa507-268">passwordRequiredType</span></span>|[<span data-ttu-id="aa507-269">андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="aa507-269">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="aa507-270">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="aa507-270">Type of password that is required.</span></span> <span data-ttu-id="aa507-271">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="aa507-271">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="aa507-272">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="aa507-272">passwordRequired</span></span>|<span data-ttu-id="aa507-273">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-273">Boolean</span></span>|<span data-ttu-id="aa507-274">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="aa507-274">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="aa507-275">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="aa507-275">powerOffBlocked</span></span>|<span data-ttu-id="aa507-276">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-276">Boolean</span></span>|<span data-ttu-id="aa507-277">Указывает, следует ли блокировать отключение устройства.</span><span class="sxs-lookup"><span data-stu-id="aa507-277">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="aa507-278">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="aa507-278">factoryResetBlocked</span></span>|<span data-ttu-id="aa507-279">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-279">Boolean</span></span>|<span data-ttu-id="aa507-280">Указывает, следует ли запретить пользователю восстанавливать заводские настройки.</span><span class="sxs-lookup"><span data-stu-id="aa507-280">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="aa507-281">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="aa507-281">screenCaptureBlocked</span></span>|<span data-ttu-id="aa507-282">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-282">Boolean</span></span>|<span data-ttu-id="aa507-283">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="aa507-283">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="aa507-284">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="aa507-284">deviceSharingAllowed</span></span>|<span data-ttu-id="aa507-285">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-285">Boolean</span></span>|<span data-ttu-id="aa507-286">Указывает, следует ли разрешить режим совместного доступа к устройству.</span><span class="sxs-lookup"><span data-stu-id="aa507-286">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="aa507-287">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="aa507-287">storageBlockGoogleBackup</span></span>|<span data-ttu-id="aa507-288">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-288">Boolean</span></span>|<span data-ttu-id="aa507-289">Указывает, следует ли блокировать резервное копирование Google.</span><span class="sxs-lookup"><span data-stu-id="aa507-289">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="aa507-290">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="aa507-290">storageBlockRemovableStorage</span></span>|<span data-ttu-id="aa507-291">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-291">Boolean</span></span>|<span data-ttu-id="aa507-292">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="aa507-292">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="aa507-293">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="aa507-293">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="aa507-294">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-294">Boolean</span></span>|<span data-ttu-id="aa507-295">Указывает, обязательно ли шифрование устройства.</span><span class="sxs-lookup"><span data-stu-id="aa507-295">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="aa507-296">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="aa507-296">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="aa507-297">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-297">Boolean</span></span>|<span data-ttu-id="aa507-298">Указывает, обязательно ли шифрование съемных носителей.</span><span class="sxs-lookup"><span data-stu-id="aa507-298">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="aa507-299">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="aa507-299">voiceAssistantBlocked</span></span>|<span data-ttu-id="aa507-300">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-300">Boolean</span></span>|<span data-ttu-id="aa507-301">Указывает, следует ли блокировать использование голосового помощника.</span><span class="sxs-lookup"><span data-stu-id="aa507-301">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="aa507-302">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="aa507-302">voiceDialingBlocked</span></span>|<span data-ttu-id="aa507-303">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-303">Boolean</span></span>|<span data-ttu-id="aa507-304">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="aa507-304">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="aa507-305">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="aa507-305">webBrowserBlockPopups</span></span>|<span data-ttu-id="aa507-306">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-306">Boolean</span></span>|<span data-ttu-id="aa507-307">Указывает, следует ли блокировать всплывающие окна в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="aa507-307">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="aa507-308">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="aa507-308">webBrowserBlockAutofill</span></span>|<span data-ttu-id="aa507-309">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-309">Boolean</span></span>|<span data-ttu-id="aa507-310">Указывает, следует ли заблокировать функцию автозаполнения в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="aa507-310">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="aa507-311">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="aa507-311">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="aa507-312">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-312">Boolean</span></span>|<span data-ttu-id="aa507-313">Указывает, следует ли заблокировать JavaScript в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="aa507-313">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="aa507-314">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="aa507-314">webBrowserBlocked</span></span>|<span data-ttu-id="aa507-315">Логический</span><span class="sxs-lookup"><span data-stu-id="aa507-315">Boolean</span></span>|<span data-ttu-id="aa507-316">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="aa507-316">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="aa507-317">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="aa507-317">webBrowserCookieSettings</span></span>|[<span data-ttu-id="aa507-318">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="aa507-318">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="aa507-319">Настройки файлов cookie в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="aa507-319">Cookie settings within the web browser.</span></span> <span data-ttu-id="aa507-320">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="aa507-320">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="aa507-321">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="aa507-321">wiFiBlocked</span></span>|<span data-ttu-id="aa507-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa507-322">Boolean</span></span>|<span data-ttu-id="aa507-323">Указывает, следует ли заблокировать синхронизацию Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="aa507-323">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="aa507-324">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="aa507-324">appsInstallAllowList</span></span>|<span data-ttu-id="aa507-325">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="aa507-325">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="aa507-326">Список приложений, которые можно установить на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="aa507-326">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="aa507-327">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="aa507-327">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="aa507-328">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="aa507-328">appsLaunchBlockList</span></span>|<span data-ttu-id="aa507-329">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="aa507-329">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="aa507-330">Список приложений, которые запрещено запускать на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="aa507-330">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="aa507-331">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="aa507-331">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="aa507-332">appsHideList</span><span class="sxs-lookup"><span data-stu-id="aa507-332">appsHideList</span></span>|<span data-ttu-id="aa507-333">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="aa507-333">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="aa507-334">Список приложений, которые следует скрыть на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="aa507-334">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="aa507-335">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="aa507-335">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="aa507-336">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="aa507-336">securityRequireVerifyApps</span></span>|<span data-ttu-id="aa507-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa507-337">Boolean</span></span>|<span data-ttu-id="aa507-338">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="aa507-338">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="aa507-339">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa507-339">Response</span></span>
<span data-ttu-id="aa507-340">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="aa507-340">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa507-341">Пример</span><span class="sxs-lookup"><span data-stu-id="aa507-341">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa507-342">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa507-342">Request</span></span>
<span data-ttu-id="aa507-343">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa507-343">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aa507-344">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa507-344">Response</span></span>
<span data-ttu-id="aa507-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa507-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





