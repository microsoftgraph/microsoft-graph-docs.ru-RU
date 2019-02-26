---
title: Update androidGeneralDeviceConfiguration
description: Обновление свойств объекта androidGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a96b820670ee86fb425f128d964382df951e70b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143766"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="3e292-103">Update androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e292-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="3e292-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e292-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e292-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e292-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e292-106">Обновление свойств объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e292-106">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e292-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3e292-107">Prerequisites</span></span>
<span data-ttu-id="3e292-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3e292-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3e292-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e292-110">Permission type</span></span>|<span data-ttu-id="3e292-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e292-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e292-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e292-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3e292-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e292-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e292-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e292-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e292-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e292-115">Not supported.</span></span>|
|<span data-ttu-id="3e292-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e292-116">Application</span></span>|<span data-ttu-id="3e292-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e292-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e292-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e292-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3e292-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e292-119">Request headers</span></span>
|<span data-ttu-id="3e292-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e292-120">Header</span></span>|<span data-ttu-id="3e292-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3e292-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e292-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e292-122">Authorization</span></span>|<span data-ttu-id="3e292-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3e292-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e292-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3e292-124">Accept</span></span>|<span data-ttu-id="3e292-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3e292-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e292-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e292-126">Request body</span></span>
<span data-ttu-id="3e292-127">В тексте запроса добавьте представление объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e292-127">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="3e292-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e292-128">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="3e292-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e292-129">Property</span></span>|<span data-ttu-id="3e292-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3e292-130">Type</span></span>|<span data-ttu-id="3e292-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3e292-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e292-132">id</span><span class="sxs-lookup"><span data-stu-id="3e292-132">id</span></span>|<span data-ttu-id="3e292-133">String</span><span class="sxs-lookup"><span data-stu-id="3e292-133">String</span></span>|<span data-ttu-id="3e292-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3e292-134">Key of the entity.</span></span> <span data-ttu-id="3e292-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e292-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e292-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e292-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3e292-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e292-137">DateTimeOffset</span></span>|<span data-ttu-id="3e292-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3e292-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3e292-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e292-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e292-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3e292-140">roleScopeTagIds</span></span>|<span data-ttu-id="3e292-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3e292-141">String collection</span></span>|<span data-ttu-id="3e292-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3e292-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3e292-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e292-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e292-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="3e292-144">supportsScopeTags</span></span>|<span data-ttu-id="3e292-145">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-145">Boolean</span></span>|<span data-ttu-id="3e292-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3e292-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3e292-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="3e292-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3e292-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3e292-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3e292-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e292-149">This property is read-only.</span></span> <span data-ttu-id="3e292-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e292-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e292-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e292-151">createdDateTime</span></span>|<span data-ttu-id="3e292-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e292-152">DateTimeOffset</span></span>|<span data-ttu-id="3e292-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3e292-153">DateTime the object was created.</span></span> <span data-ttu-id="3e292-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e292-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e292-155">description</span><span class="sxs-lookup"><span data-stu-id="3e292-155">description</span></span>|<span data-ttu-id="3e292-156">String</span><span class="sxs-lookup"><span data-stu-id="3e292-156">String</span></span>|<span data-ttu-id="3e292-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3e292-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3e292-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e292-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e292-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3e292-159">displayName</span></span>|<span data-ttu-id="3e292-160">String</span><span class="sxs-lookup"><span data-stu-id="3e292-160">String</span></span>|<span data-ttu-id="3e292-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3e292-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3e292-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e292-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e292-163">version</span><span class="sxs-lookup"><span data-stu-id="3e292-163">version</span></span>|<span data-ttu-id="3e292-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3e292-164">Int32</span></span>|<span data-ttu-id="3e292-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3e292-165">Version of the device configuration.</span></span> <span data-ttu-id="3e292-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e292-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e292-167">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="3e292-167">appsBlockClipboardSharing</span></span>|<span data-ttu-id="3e292-168">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-168">Boolean</span></span>|<span data-ttu-id="3e292-169">Указывает, следует ли запретить совместное использование буфера обмена для копирования данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="3e292-169">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="3e292-170">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="3e292-170">appsBlockCopyPaste</span></span>|<span data-ttu-id="3e292-171">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-171">Boolean</span></span>|<span data-ttu-id="3e292-172">Указывает, следует ли запретить копирование данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="3e292-172">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="3e292-173">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="3e292-173">appsBlockYouTube</span></span>|<span data-ttu-id="3e292-174">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-174">Boolean</span></span>|<span data-ttu-id="3e292-175">Указывает, следует ли заблокировать приложение YouTube.</span><span class="sxs-lookup"><span data-stu-id="3e292-175">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="3e292-176">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="3e292-176">bluetoothBlocked</span></span>|<span data-ttu-id="3e292-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e292-177">Boolean</span></span>|<span data-ttu-id="3e292-178">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="3e292-178">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="3e292-179">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="3e292-179">cameraBlocked</span></span>|<span data-ttu-id="3e292-180">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-180">Boolean</span></span>|<span data-ttu-id="3e292-181">Указывает, следует ли запретить использовать камеру.</span><span class="sxs-lookup"><span data-stu-id="3e292-181">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="3e292-182">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="3e292-182">cellularBlockDataRoaming</span></span>|<span data-ttu-id="3e292-183">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-183">Boolean</span></span>|<span data-ttu-id="3e292-184">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="3e292-184">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="3e292-185">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="3e292-185">cellularBlockMessaging</span></span>|<span data-ttu-id="3e292-186">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-186">Boolean</span></span>|<span data-ttu-id="3e292-187">Указывает, следует ли запретить обмениваться SMS и MMS.</span><span class="sxs-lookup"><span data-stu-id="3e292-187">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="3e292-188">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="3e292-188">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="3e292-189">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-189">Boolean</span></span>|<span data-ttu-id="3e292-190">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="3e292-190">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="3e292-191">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="3e292-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="3e292-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e292-192">Boolean</span></span>|<span data-ttu-id="3e292-193">Указывает, следует ли блокировать синхронизацию модема Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="3e292-193">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="3e292-194">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="3e292-194">compliantAppsList</span></span>|<span data-ttu-id="3e292-195">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="3e292-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3e292-196">Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="3e292-196">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="3e292-197">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="3e292-197">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="3e292-198">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="3e292-198">compliantAppListType</span></span>|[<span data-ttu-id="3e292-199">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="3e292-199">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="3e292-200">Тип списка, определенного свойством CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="3e292-200">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="3e292-201">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="3e292-201">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="3e292-202">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="3e292-202">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="3e292-203">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-203">Boolean</span></span>|<span data-ttu-id="3e292-204">Указывает, следует ли блокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="3e292-204">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="3e292-205">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="3e292-205">locationServicesBlocked</span></span>|<span data-ttu-id="3e292-206">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-206">Boolean</span></span>|<span data-ttu-id="3e292-207">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="3e292-207">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="3e292-208">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="3e292-208">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="3e292-209">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-209">Boolean</span></span>|<span data-ttu-id="3e292-210">Указывает, следует ли блокировать автоматическую синхронизацию учетной записи Google.</span><span class="sxs-lookup"><span data-stu-id="3e292-210">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="3e292-211">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="3e292-211">googlePlayStoreBlocked</span></span>|<span data-ttu-id="3e292-212">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-212">Boolean</span></span>|<span data-ttu-id="3e292-213">Указывает, следует ли блокировать Google Play Маркет.</span><span class="sxs-lookup"><span data-stu-id="3e292-213">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="3e292-214">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="3e292-214">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="3e292-215">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-215">Boolean</span></span>|<span data-ttu-id="3e292-216">Указывает, следует ли блокировать кнопку спящего режима экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="3e292-216">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="3e292-217">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="3e292-217">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="3e292-218">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-218">Boolean</span></span>|<span data-ttu-id="3e292-219">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="3e292-219">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="3e292-220">Датеандтимеблоккчанжес</span><span class="sxs-lookup"><span data-stu-id="3e292-220">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="3e292-221">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-221">Boolean</span></span>|<span data-ttu-id="3e292-222">Указывает, следует ли заблокировать изменение даты и времени в режиме KNOX.</span><span class="sxs-lookup"><span data-stu-id="3e292-222">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="3e292-223">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="3e292-223">kioskModeApps</span></span>|<span data-ttu-id="3e292-224">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="3e292-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3e292-225">Список разрешенных приложений в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="3e292-225">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="3e292-226">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3e292-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3e292-227">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="3e292-227">nfcBlocked</span></span>|<span data-ttu-id="3e292-228">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-228">Boolean</span></span>|<span data-ttu-id="3e292-229">Указывает, следует ли блокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="3e292-229">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="3e292-230">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="3e292-230">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="3e292-231">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-231">Boolean</span></span>|<span data-ttu-id="3e292-232">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="3e292-232">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="3e292-233">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="3e292-233">passwordBlockTrustAgents</span></span>|<span data-ttu-id="3e292-234">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-234">Boolean</span></span>|<span data-ttu-id="3e292-235">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="3e292-235">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="3e292-236">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3e292-236">passwordExpirationDays</span></span>|<span data-ttu-id="3e292-237">Int32</span><span class="sxs-lookup"><span data-stu-id="3e292-237">Int32</span></span>|<span data-ttu-id="3e292-238">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="3e292-238">Number of days before the password expires.</span></span> <span data-ttu-id="3e292-239">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="3e292-239">Valid values 1 to 365</span></span>|
|<span data-ttu-id="3e292-240">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3e292-240">passwordMinimumLength</span></span>|<span data-ttu-id="3e292-241">Int32</span><span class="sxs-lookup"><span data-stu-id="3e292-241">Int32</span></span>|<span data-ttu-id="3e292-242">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="3e292-242">Minimum length of passwords.</span></span> <span data-ttu-id="3e292-243">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="3e292-243">Valid values 4 to 16</span></span>|
|<span data-ttu-id="3e292-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="3e292-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="3e292-245">Int32</span><span class="sxs-lookup"><span data-stu-id="3e292-245">Int32</span></span>|<span data-ttu-id="3e292-246">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="3e292-246">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="3e292-247">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3e292-247">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3e292-248">Int32</span><span class="sxs-lookup"><span data-stu-id="3e292-248">Int32</span></span>|<span data-ttu-id="3e292-249">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="3e292-249">Number of previous passwords to block.</span></span> <span data-ttu-id="3e292-250">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="3e292-250">Valid values 0 to 24</span></span>|
|<span data-ttu-id="3e292-251">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="3e292-251">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="3e292-252">Int32</span><span class="sxs-lookup"><span data-stu-id="3e292-252">Int32</span></span>|<span data-ttu-id="3e292-253">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="3e292-253">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="3e292-254">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="3e292-254">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3e292-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3e292-255">passwordRequiredType</span></span>|[<span data-ttu-id="3e292-256">Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="3e292-256">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="3e292-257">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="3e292-257">Type of password that is required.</span></span> <span data-ttu-id="3e292-258">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="3e292-258">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="3e292-259">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3e292-259">passwordRequired</span></span>|<span data-ttu-id="3e292-260">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-260">Boolean</span></span>|<span data-ttu-id="3e292-261">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="3e292-261">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="3e292-262">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="3e292-262">powerOffBlocked</span></span>|<span data-ttu-id="3e292-263">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-263">Boolean</span></span>|<span data-ttu-id="3e292-264">Указывает, следует ли блокировать отключение устройства.</span><span class="sxs-lookup"><span data-stu-id="3e292-264">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="3e292-265">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="3e292-265">factoryResetBlocked</span></span>|<span data-ttu-id="3e292-266">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-266">Boolean</span></span>|<span data-ttu-id="3e292-267">Указывает, следует ли запретить пользователю восстанавливать заводские настройки.</span><span class="sxs-lookup"><span data-stu-id="3e292-267">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="3e292-268">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="3e292-268">screenCaptureBlocked</span></span>|<span data-ttu-id="3e292-269">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-269">Boolean</span></span>|<span data-ttu-id="3e292-270">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="3e292-270">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="3e292-271">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="3e292-271">deviceSharingAllowed</span></span>|<span data-ttu-id="3e292-272">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-272">Boolean</span></span>|<span data-ttu-id="3e292-273">Указывает, следует ли разрешить режим совместного доступа к устройству.</span><span class="sxs-lookup"><span data-stu-id="3e292-273">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="3e292-274">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="3e292-274">storageBlockGoogleBackup</span></span>|<span data-ttu-id="3e292-275">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-275">Boolean</span></span>|<span data-ttu-id="3e292-276">Указывает, следует ли блокировать резервное копирование Google.</span><span class="sxs-lookup"><span data-stu-id="3e292-276">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="3e292-277">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="3e292-277">storageBlockRemovableStorage</span></span>|<span data-ttu-id="3e292-278">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-278">Boolean</span></span>|<span data-ttu-id="3e292-279">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="3e292-279">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="3e292-280">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="3e292-280">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="3e292-281">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-281">Boolean</span></span>|<span data-ttu-id="3e292-282">Указывает, обязательно ли шифрование устройства.</span><span class="sxs-lookup"><span data-stu-id="3e292-282">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="3e292-283">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="3e292-283">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="3e292-284">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-284">Boolean</span></span>|<span data-ttu-id="3e292-285">Указывает, обязательно ли шифрование съемных носителей.</span><span class="sxs-lookup"><span data-stu-id="3e292-285">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="3e292-286">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="3e292-286">voiceAssistantBlocked</span></span>|<span data-ttu-id="3e292-287">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-287">Boolean</span></span>|<span data-ttu-id="3e292-288">Указывает, следует ли блокировать использование голосового помощника.</span><span class="sxs-lookup"><span data-stu-id="3e292-288">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="3e292-289">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="3e292-289">voiceDialingBlocked</span></span>|<span data-ttu-id="3e292-290">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-290">Boolean</span></span>|<span data-ttu-id="3e292-291">Указывает, следует ли блокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="3e292-291">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="3e292-292">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="3e292-292">webBrowserBlockPopups</span></span>|<span data-ttu-id="3e292-293">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-293">Boolean</span></span>|<span data-ttu-id="3e292-294">Указывает, следует ли блокировать всплывающие окна в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="3e292-294">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="3e292-295">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="3e292-295">webBrowserBlockAutofill</span></span>|<span data-ttu-id="3e292-296">Логический</span><span class="sxs-lookup"><span data-stu-id="3e292-296">Boolean</span></span>|<span data-ttu-id="3e292-297">Указывает, следует ли заблокировать функцию автозаполнения в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="3e292-297">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="3e292-298">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="3e292-298">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="3e292-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e292-299">Boolean</span></span>|<span data-ttu-id="3e292-300">Указывает, следует ли заблокировать JavaScript в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="3e292-300">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="3e292-301">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="3e292-301">webBrowserBlocked</span></span>|<span data-ttu-id="3e292-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e292-302">Boolean</span></span>|<span data-ttu-id="3e292-303">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="3e292-303">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="3e292-304">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="3e292-304">webBrowserCookieSettings</span></span>|[<span data-ttu-id="3e292-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="3e292-305">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="3e292-306">Настройки файлов cookie в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="3e292-306">Cookie settings within the web browser.</span></span> <span data-ttu-id="3e292-307">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="3e292-307">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="3e292-308">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="3e292-308">wiFiBlocked</span></span>|<span data-ttu-id="3e292-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e292-309">Boolean</span></span>|<span data-ttu-id="3e292-310">Указывает, следует ли заблокировать синхронизацию Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="3e292-310">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="3e292-311">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="3e292-311">appsInstallAllowList</span></span>|<span data-ttu-id="3e292-312">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="3e292-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3e292-313">Список приложений, которые можно установить на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="3e292-313">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="3e292-314">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3e292-314">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3e292-315">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="3e292-315">appsLaunchBlockList</span></span>|<span data-ttu-id="3e292-316">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="3e292-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3e292-317">Список приложений, которые запрещено запускать на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="3e292-317">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="3e292-318">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3e292-318">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3e292-319">appsHideList</span><span class="sxs-lookup"><span data-stu-id="3e292-319">appsHideList</span></span>|<span data-ttu-id="3e292-320">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="3e292-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3e292-321">Список приложений, которые следует скрыть на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="3e292-321">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="3e292-322">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3e292-322">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3e292-323">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="3e292-323">securityRequireVerifyApps</span></span>|<span data-ttu-id="3e292-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e292-324">Boolean</span></span>|<span data-ttu-id="3e292-325">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="3e292-325">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="3e292-326">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e292-326">Response</span></span>
<span data-ttu-id="3e292-327">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3e292-327">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e292-328">Пример</span><span class="sxs-lookup"><span data-stu-id="3e292-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e292-329">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e292-329">Request</span></span>
<span data-ttu-id="3e292-330">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e292-330">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3161

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="3e292-331">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e292-331">Response</span></span>
<span data-ttu-id="3e292-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3e292-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3333

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




