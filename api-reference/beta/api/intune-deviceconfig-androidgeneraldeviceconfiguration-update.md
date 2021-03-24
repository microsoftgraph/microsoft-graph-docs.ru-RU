---
title: Update androidGeneralDeviceConfiguration
description: Обновление свойств объекта androidGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8db51e97f79ac6e8dbe32236dd80d3dcff3307b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138038"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="bb595-103">Update androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb595-103">Update androidGeneralDeviceConfiguration</span></span>

<span data-ttu-id="bb595-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb595-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb595-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb595-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb595-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb595-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb595-107">Обновление свойств объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb595-107">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb595-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bb595-108">Prerequisites</span></span>
<span data-ttu-id="bb595-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb595-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb595-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb595-111">Permission type</span></span>|<span data-ttu-id="bb595-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb595-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb595-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb595-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb595-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb595-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb595-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb595-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb595-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb595-116">Not supported.</span></span>|
|<span data-ttu-id="bb595-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bb595-117">Application</span></span>|<span data-ttu-id="bb595-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb595-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb595-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb595-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bb595-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bb595-120">Request headers</span></span>
|<span data-ttu-id="bb595-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb595-121">Header</span></span>|<span data-ttu-id="bb595-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bb595-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb595-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb595-123">Authorization</span></span>|<span data-ttu-id="bb595-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb595-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb595-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bb595-125">Accept</span></span>|<span data-ttu-id="bb595-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb595-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb595-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb595-127">Request body</span></span>
<span data-ttu-id="bb595-128">В тексте запроса добавьте представление объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb595-128">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="bb595-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb595-129">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="bb595-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb595-130">Property</span></span>|<span data-ttu-id="bb595-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bb595-131">Type</span></span>|<span data-ttu-id="bb595-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bb595-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb595-133">id</span><span class="sxs-lookup"><span data-stu-id="bb595-133">id</span></span>|<span data-ttu-id="bb595-134">Строка</span><span class="sxs-lookup"><span data-stu-id="bb595-134">String</span></span>|<span data-ttu-id="bb595-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bb595-135">Key of the entity.</span></span> <span data-ttu-id="bb595-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb595-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb595-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb595-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bb595-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb595-138">DateTimeOffset</span></span>|<span data-ttu-id="bb595-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bb595-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bb595-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb595-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb595-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bb595-141">roleScopeTagIds</span></span>|<span data-ttu-id="bb595-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bb595-142">String collection</span></span>|<span data-ttu-id="bb595-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="bb595-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bb595-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb595-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb595-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bb595-145">supportsScopeTags</span></span>|<span data-ttu-id="bb595-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-146">Boolean</span></span>|<span data-ttu-id="bb595-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="bb595-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bb595-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="bb595-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bb595-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bb595-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bb595-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb595-150">This property is read-only.</span></span> <span data-ttu-id="bb595-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb595-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb595-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bb595-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bb595-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bb595-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bb595-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bb595-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bb595-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb595-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb595-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bb595-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bb595-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bb595-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bb595-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bb595-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bb595-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb595-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb595-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bb595-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bb595-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bb595-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bb595-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bb595-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bb595-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb595-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb595-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb595-164">createdDateTime</span></span>|<span data-ttu-id="bb595-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb595-165">DateTimeOffset</span></span>|<span data-ttu-id="bb595-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bb595-166">DateTime the object was created.</span></span> <span data-ttu-id="bb595-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb595-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb595-168">description</span><span class="sxs-lookup"><span data-stu-id="bb595-168">description</span></span>|<span data-ttu-id="bb595-169">Строка</span><span class="sxs-lookup"><span data-stu-id="bb595-169">String</span></span>|<span data-ttu-id="bb595-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bb595-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bb595-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb595-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb595-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bb595-172">displayName</span></span>|<span data-ttu-id="bb595-173">Строка</span><span class="sxs-lookup"><span data-stu-id="bb595-173">String</span></span>|<span data-ttu-id="bb595-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bb595-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bb595-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb595-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb595-176">version</span><span class="sxs-lookup"><span data-stu-id="bb595-176">version</span></span>|<span data-ttu-id="bb595-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bb595-177">Int32</span></span>|<span data-ttu-id="bb595-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bb595-178">Version of the device configuration.</span></span> <span data-ttu-id="bb595-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb595-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb595-180">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="bb595-180">appsBlockClipboardSharing</span></span>|<span data-ttu-id="bb595-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-181">Boolean</span></span>|<span data-ttu-id="bb595-182">Указывает, следует ли запретить совместное использование буфера обмена для копирования данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="bb595-182">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="bb595-183">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="bb595-183">appsBlockCopyPaste</span></span>|<span data-ttu-id="bb595-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-184">Boolean</span></span>|<span data-ttu-id="bb595-185">Указывает, следует ли запретить копирование данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="bb595-185">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="bb595-186">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="bb595-186">appsBlockYouTube</span></span>|<span data-ttu-id="bb595-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-187">Boolean</span></span>|<span data-ttu-id="bb595-188">Указывает, следует ли заблокировать приложение YouTube.</span><span class="sxs-lookup"><span data-stu-id="bb595-188">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="bb595-189">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="bb595-189">bluetoothBlocked</span></span>|<span data-ttu-id="bb595-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-190">Boolean</span></span>|<span data-ttu-id="bb595-191">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="bb595-191">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="bb595-192">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="bb595-192">cameraBlocked</span></span>|<span data-ttu-id="bb595-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-193">Boolean</span></span>|<span data-ttu-id="bb595-194">Указывает, следует ли запретить использовать камеру.</span><span class="sxs-lookup"><span data-stu-id="bb595-194">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="bb595-195">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="bb595-195">cellularBlockDataRoaming</span></span>|<span data-ttu-id="bb595-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-196">Boolean</span></span>|<span data-ttu-id="bb595-197">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="bb595-197">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="bb595-198">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="bb595-198">cellularBlockMessaging</span></span>|<span data-ttu-id="bb595-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-199">Boolean</span></span>|<span data-ttu-id="bb595-200">Указывает, следует ли запретить обмениваться SMS и MMS.</span><span class="sxs-lookup"><span data-stu-id="bb595-200">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="bb595-201">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="bb595-201">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="bb595-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-202">Boolean</span></span>|<span data-ttu-id="bb595-203">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="bb595-203">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="bb595-204">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="bb595-204">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="bb595-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-205">Boolean</span></span>|<span data-ttu-id="bb595-206">Указывает, следует ли блокировать синхронизацию модема Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="bb595-206">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="bb595-207">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="bb595-207">compliantAppsList</span></span>|<span data-ttu-id="bb595-208">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bb595-208">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bb595-209">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="bb595-209">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="bb595-210">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="bb595-210">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="bb595-211">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="bb595-211">compliantAppListType</span></span>|[<span data-ttu-id="bb595-212">appListType</span><span class="sxs-lookup"><span data-stu-id="bb595-212">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="bb595-213">Тип списка, определенного свойством CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="bb595-213">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="bb595-214">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="bb595-214">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="bb595-215">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="bb595-215">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="bb595-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-216">Boolean</span></span>|<span data-ttu-id="bb595-217">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="bb595-217">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="bb595-218">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="bb595-218">locationServicesBlocked</span></span>|<span data-ttu-id="bb595-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-219">Boolean</span></span>|<span data-ttu-id="bb595-220">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="bb595-220">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="bb595-221">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="bb595-221">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="bb595-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-222">Boolean</span></span>|<span data-ttu-id="bb595-223">Указывает, следует ли блокировать автоматическую синхронизацию учетной записи Google.</span><span class="sxs-lookup"><span data-stu-id="bb595-223">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="bb595-224">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="bb595-224">googlePlayStoreBlocked</span></span>|<span data-ttu-id="bb595-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-225">Boolean</span></span>|<span data-ttu-id="bb595-226">Указывает, следует ли блокировать Google Play Маркет.</span><span class="sxs-lookup"><span data-stu-id="bb595-226">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="bb595-227">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="bb595-227">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="bb595-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-228">Boolean</span></span>|<span data-ttu-id="bb595-229">Указывает, следует ли блокировать кнопку спящего режима экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="bb595-229">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="bb595-230">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="bb595-230">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="bb595-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-231">Boolean</span></span>|<span data-ttu-id="bb595-232">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="bb595-232">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="bb595-233">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="bb595-233">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="bb595-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-234">Boolean</span></span>|<span data-ttu-id="bb595-235">Указывает, следует ли блокировать изменение даты и времени в режиме KNOX.</span><span class="sxs-lookup"><span data-stu-id="bb595-235">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="bb595-236">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="bb595-236">kioskModeApps</span></span>|<span data-ttu-id="bb595-237">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bb595-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bb595-238">Список разрешенных приложений в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="bb595-238">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="bb595-239">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="bb595-239">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="bb595-240">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="bb595-240">nfcBlocked</span></span>|<span data-ttu-id="bb595-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-241">Boolean</span></span>|<span data-ttu-id="bb595-242">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="bb595-242">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="bb595-243">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="bb595-243">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="bb595-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-244">Boolean</span></span>|<span data-ttu-id="bb595-245">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="bb595-245">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="bb595-246">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="bb595-246">passwordBlockTrustAgents</span></span>|<span data-ttu-id="bb595-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-247">Boolean</span></span>|<span data-ttu-id="bb595-248">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="bb595-248">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="bb595-249">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bb595-249">passwordExpirationDays</span></span>|<span data-ttu-id="bb595-250">Int32</span><span class="sxs-lookup"><span data-stu-id="bb595-250">Int32</span></span>|<span data-ttu-id="bb595-251">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="bb595-251">Number of days before the password expires.</span></span> <span data-ttu-id="bb595-252">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="bb595-252">Valid values 1 to 365</span></span>|
|<span data-ttu-id="bb595-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bb595-253">passwordMinimumLength</span></span>|<span data-ttu-id="bb595-254">Int32</span><span class="sxs-lookup"><span data-stu-id="bb595-254">Int32</span></span>|<span data-ttu-id="bb595-255">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="bb595-255">Minimum length of passwords.</span></span> <span data-ttu-id="bb595-256">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="bb595-256">Valid values 4 to 16</span></span>|
|<span data-ttu-id="bb595-257">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="bb595-257">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="bb595-258">Int32</span><span class="sxs-lookup"><span data-stu-id="bb595-258">Int32</span></span>|<span data-ttu-id="bb595-259">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="bb595-259">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="bb595-260">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bb595-260">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bb595-261">Int32</span><span class="sxs-lookup"><span data-stu-id="bb595-261">Int32</span></span>|<span data-ttu-id="bb595-262">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="bb595-262">Number of previous passwords to block.</span></span> <span data-ttu-id="bb595-263">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="bb595-263">Valid values 0 to 24</span></span>|
|<span data-ttu-id="bb595-264">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="bb595-264">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="bb595-265">Int32</span><span class="sxs-lookup"><span data-stu-id="bb595-265">Int32</span></span>|<span data-ttu-id="bb595-266">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="bb595-266">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="bb595-267">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="bb595-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="bb595-268">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bb595-268">passwordRequiredType</span></span>|[<span data-ttu-id="bb595-269">AndroidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bb595-269">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="bb595-270">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="bb595-270">Type of password that is required.</span></span> <span data-ttu-id="bb595-271">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="bb595-271">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="bb595-272">requiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="bb595-272">requiredPasswordComplexity</span></span>|[<span data-ttu-id="bb595-273">androidRequiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="bb595-273">androidRequiredPasswordComplexity</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordcomplexity.md)|<span data-ttu-id="bb595-274">Указывает на требуемую сложность пароля на Android.</span><span class="sxs-lookup"><span data-stu-id="bb595-274">Indicates the required password complexity on Android.</span></span> <span data-ttu-id="bb595-275">Один из: NONE, LOW, MEDIUM, HIGH.</span><span class="sxs-lookup"><span data-stu-id="bb595-275">One of: NONE, LOW, MEDIUM, HIGH.</span></span> <span data-ttu-id="bb595-276">Это API, нацеленный на Android 11+.</span><span class="sxs-lookup"><span data-stu-id="bb595-276">This is an API targeted to Android 11+.</span></span> <span data-ttu-id="bb595-277">Возможные значения: `none`, `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="bb595-277">Possible values are: `none`, `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="bb595-278">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="bb595-278">passwordRequired</span></span>|<span data-ttu-id="bb595-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-279">Boolean</span></span>|<span data-ttu-id="bb595-280">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="bb595-280">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="bb595-281">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="bb595-281">powerOffBlocked</span></span>|<span data-ttu-id="bb595-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-282">Boolean</span></span>|<span data-ttu-id="bb595-283">Указывает, следует ли блокировать отключение устройства.</span><span class="sxs-lookup"><span data-stu-id="bb595-283">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="bb595-284">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="bb595-284">factoryResetBlocked</span></span>|<span data-ttu-id="bb595-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-285">Boolean</span></span>|<span data-ttu-id="bb595-286">Указывает, следует ли запретить пользователю восстанавливать заводские настройки.</span><span class="sxs-lookup"><span data-stu-id="bb595-286">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="bb595-287">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="bb595-287">screenCaptureBlocked</span></span>|<span data-ttu-id="bb595-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-288">Boolean</span></span>|<span data-ttu-id="bb595-289">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="bb595-289">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="bb595-290">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="bb595-290">deviceSharingAllowed</span></span>|<span data-ttu-id="bb595-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-291">Boolean</span></span>|<span data-ttu-id="bb595-292">Указывает, следует ли разрешить режим совместного доступа к устройству.</span><span class="sxs-lookup"><span data-stu-id="bb595-292">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="bb595-293">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="bb595-293">storageBlockGoogleBackup</span></span>|<span data-ttu-id="bb595-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-294">Boolean</span></span>|<span data-ttu-id="bb595-295">Указывает, следует ли блокировать резервное копирование Google.</span><span class="sxs-lookup"><span data-stu-id="bb595-295">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="bb595-296">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="bb595-296">storageBlockRemovableStorage</span></span>|<span data-ttu-id="bb595-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-297">Boolean</span></span>|<span data-ttu-id="bb595-298">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="bb595-298">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="bb595-299">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="bb595-299">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="bb595-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-300">Boolean</span></span>|<span data-ttu-id="bb595-301">Указывает, обязательно ли шифрование устройства.</span><span class="sxs-lookup"><span data-stu-id="bb595-301">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="bb595-302">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="bb595-302">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="bb595-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-303">Boolean</span></span>|<span data-ttu-id="bb595-304">Указывает, обязательно ли шифрование съемных носителей.</span><span class="sxs-lookup"><span data-stu-id="bb595-304">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="bb595-305">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="bb595-305">voiceAssistantBlocked</span></span>|<span data-ttu-id="bb595-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-306">Boolean</span></span>|<span data-ttu-id="bb595-307">Указывает, следует ли блокировать использование голосового помощника.</span><span class="sxs-lookup"><span data-stu-id="bb595-307">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="bb595-308">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="bb595-308">voiceDialingBlocked</span></span>|<span data-ttu-id="bb595-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-309">Boolean</span></span>|<span data-ttu-id="bb595-310">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="bb595-310">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="bb595-311">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="bb595-311">webBrowserBlockPopups</span></span>|<span data-ttu-id="bb595-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-312">Boolean</span></span>|<span data-ttu-id="bb595-313">Указывает, следует ли блокировать всплывающие окна в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="bb595-313">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="bb595-314">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="bb595-314">webBrowserBlockAutofill</span></span>|<span data-ttu-id="bb595-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-315">Boolean</span></span>|<span data-ttu-id="bb595-316">Указывает, следует ли заблокировать функцию автозаполнения в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="bb595-316">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="bb595-317">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="bb595-317">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="bb595-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-318">Boolean</span></span>|<span data-ttu-id="bb595-319">Указывает, следует ли заблокировать JavaScript в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="bb595-319">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="bb595-320">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="bb595-320">webBrowserBlocked</span></span>|<span data-ttu-id="bb595-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-321">Boolean</span></span>|<span data-ttu-id="bb595-322">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="bb595-322">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="bb595-323">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="bb595-323">webBrowserCookieSettings</span></span>|[<span data-ttu-id="bb595-324">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="bb595-324">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="bb595-325">Настройки файлов cookie в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="bb595-325">Cookie settings within the web browser.</span></span> <span data-ttu-id="bb595-326">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="bb595-326">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="bb595-327">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="bb595-327">wiFiBlocked</span></span>|<span data-ttu-id="bb595-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-328">Boolean</span></span>|<span data-ttu-id="bb595-329">Указывает, следует ли заблокировать синхронизацию Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="bb595-329">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="bb595-330">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="bb595-330">appsInstallAllowList</span></span>|<span data-ttu-id="bb595-331">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bb595-331">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bb595-332">Список приложений, которые можно установить на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="bb595-332">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="bb595-333">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="bb595-333">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="bb595-334">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="bb595-334">appsLaunchBlockList</span></span>|<span data-ttu-id="bb595-335">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bb595-335">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bb595-336">Список приложений, которые запрещено запускать на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="bb595-336">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="bb595-337">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="bb595-337">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="bb595-338">appsHideList</span><span class="sxs-lookup"><span data-stu-id="bb595-338">appsHideList</span></span>|<span data-ttu-id="bb595-339">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bb595-339">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bb595-340">Список приложений, которые следует скрыть на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="bb595-340">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="bb595-341">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="bb595-341">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="bb595-342">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="bb595-342">securityRequireVerifyApps</span></span>|<span data-ttu-id="bb595-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb595-343">Boolean</span></span>|<span data-ttu-id="bb595-344">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="bb595-344">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="bb595-345">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb595-345">Response</span></span>
<span data-ttu-id="bb595-346">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bb595-346">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb595-347">Пример</span><span class="sxs-lookup"><span data-stu-id="bb595-347">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb595-348">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb595-348">Request</span></span>
<span data-ttu-id="bb595-349">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb595-349">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3974

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
  "requiredPasswordComplexity": "low",
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

### <a name="response"></a><span data-ttu-id="bb595-350">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb595-350">Response</span></span>
<span data-ttu-id="bb595-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb595-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4146

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
  "requiredPasswordComplexity": "low",
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




