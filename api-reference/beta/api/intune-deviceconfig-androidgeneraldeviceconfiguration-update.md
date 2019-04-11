---
title: Update androidGeneralDeviceConfiguration
description: Обновление свойств объекта androidGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 511712cb44216f1efbdf0d9154dbf8ed970ee0e0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774920"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="932a1-103">Update androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="932a1-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="932a1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="932a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="932a1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="932a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="932a1-106">Обновление свойств объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="932a1-106">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="932a1-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="932a1-107">Prerequisites</span></span>
<span data-ttu-id="932a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="932a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="932a1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="932a1-110">Permission type</span></span>|<span data-ttu-id="932a1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="932a1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="932a1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="932a1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="932a1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="932a1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="932a1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="932a1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="932a1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="932a1-115">Not supported.</span></span>|
|<span data-ttu-id="932a1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="932a1-116">Application</span></span>|<span data-ttu-id="932a1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="932a1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="932a1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="932a1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="932a1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="932a1-119">Request headers</span></span>
|<span data-ttu-id="932a1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="932a1-120">Header</span></span>|<span data-ttu-id="932a1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="932a1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="932a1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="932a1-122">Authorization</span></span>|<span data-ttu-id="932a1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="932a1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="932a1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="932a1-124">Accept</span></span>|<span data-ttu-id="932a1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="932a1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="932a1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="932a1-126">Request body</span></span>
<span data-ttu-id="932a1-127">В тексте запроса добавьте представление объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="932a1-127">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="932a1-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="932a1-128">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="932a1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="932a1-129">Property</span></span>|<span data-ttu-id="932a1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="932a1-130">Type</span></span>|<span data-ttu-id="932a1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="932a1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="932a1-132">id</span><span class="sxs-lookup"><span data-stu-id="932a1-132">id</span></span>|<span data-ttu-id="932a1-133">Строка</span><span class="sxs-lookup"><span data-stu-id="932a1-133">String</span></span>|<span data-ttu-id="932a1-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="932a1-134">Key of the entity.</span></span> <span data-ttu-id="932a1-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="932a1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="932a1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="932a1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="932a1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="932a1-137">DateTimeOffset</span></span>|<span data-ttu-id="932a1-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="932a1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="932a1-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="932a1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="932a1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="932a1-140">roleScopeTagIds</span></span>|<span data-ttu-id="932a1-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="932a1-141">String collection</span></span>|<span data-ttu-id="932a1-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="932a1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="932a1-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="932a1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="932a1-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="932a1-144">supportsScopeTags</span></span>|<span data-ttu-id="932a1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-145">Boolean</span></span>|<span data-ttu-id="932a1-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="932a1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="932a1-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="932a1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="932a1-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="932a1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="932a1-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="932a1-149">This property is read-only.</span></span> <span data-ttu-id="932a1-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="932a1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="932a1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="932a1-151">createdDateTime</span></span>|<span data-ttu-id="932a1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="932a1-152">DateTimeOffset</span></span>|<span data-ttu-id="932a1-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="932a1-153">DateTime the object was created.</span></span> <span data-ttu-id="932a1-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="932a1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="932a1-155">description</span><span class="sxs-lookup"><span data-stu-id="932a1-155">description</span></span>|<span data-ttu-id="932a1-156">String</span><span class="sxs-lookup"><span data-stu-id="932a1-156">String</span></span>|<span data-ttu-id="932a1-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="932a1-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="932a1-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="932a1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="932a1-159">displayName</span><span class="sxs-lookup"><span data-stu-id="932a1-159">displayName</span></span>|<span data-ttu-id="932a1-160">String</span><span class="sxs-lookup"><span data-stu-id="932a1-160">String</span></span>|<span data-ttu-id="932a1-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="932a1-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="932a1-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="932a1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="932a1-163">version</span><span class="sxs-lookup"><span data-stu-id="932a1-163">version</span></span>|<span data-ttu-id="932a1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="932a1-164">Int32</span></span>|<span data-ttu-id="932a1-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="932a1-165">Version of the device configuration.</span></span> <span data-ttu-id="932a1-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="932a1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="932a1-167">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="932a1-167">appsBlockClipboardSharing</span></span>|<span data-ttu-id="932a1-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-168">Boolean</span></span>|<span data-ttu-id="932a1-169">Указывает, следует ли запретить совместное использование буфера обмена для копирования данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="932a1-169">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="932a1-170">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="932a1-170">appsBlockCopyPaste</span></span>|<span data-ttu-id="932a1-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-171">Boolean</span></span>|<span data-ttu-id="932a1-172">Указывает, следует ли запретить копирование данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="932a1-172">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="932a1-173">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="932a1-173">appsBlockYouTube</span></span>|<span data-ttu-id="932a1-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-174">Boolean</span></span>|<span data-ttu-id="932a1-175">Указывает, следует ли заблокировать приложение YouTube.</span><span class="sxs-lookup"><span data-stu-id="932a1-175">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="932a1-176">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="932a1-176">bluetoothBlocked</span></span>|<span data-ttu-id="932a1-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-177">Boolean</span></span>|<span data-ttu-id="932a1-178">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="932a1-178">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="932a1-179">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="932a1-179">cameraBlocked</span></span>|<span data-ttu-id="932a1-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-180">Boolean</span></span>|<span data-ttu-id="932a1-181">Указывает, следует ли запретить использовать камеру.</span><span class="sxs-lookup"><span data-stu-id="932a1-181">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="932a1-182">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="932a1-182">cellularBlockDataRoaming</span></span>|<span data-ttu-id="932a1-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-183">Boolean</span></span>|<span data-ttu-id="932a1-184">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="932a1-184">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="932a1-185">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="932a1-185">cellularBlockMessaging</span></span>|<span data-ttu-id="932a1-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-186">Boolean</span></span>|<span data-ttu-id="932a1-187">Указывает, следует ли запретить обмениваться SMS и MMS.</span><span class="sxs-lookup"><span data-stu-id="932a1-187">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="932a1-188">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="932a1-188">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="932a1-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-189">Boolean</span></span>|<span data-ttu-id="932a1-190">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="932a1-190">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="932a1-191">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="932a1-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="932a1-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-192">Boolean</span></span>|<span data-ttu-id="932a1-193">Указывает, следует ли блокировать синхронизацию модема Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="932a1-193">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="932a1-194">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="932a1-194">compliantAppsList</span></span>|<span data-ttu-id="932a1-195">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="932a1-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="932a1-196">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="932a1-196">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="932a1-197">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="932a1-197">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="932a1-198">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="932a1-198">compliantAppListType</span></span>|[<span data-ttu-id="932a1-199">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="932a1-199">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="932a1-200">Тип списка, определенного свойством CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="932a1-200">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="932a1-201">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="932a1-201">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="932a1-202">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="932a1-202">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="932a1-203">Логический</span><span class="sxs-lookup"><span data-stu-id="932a1-203">Boolean</span></span>|<span data-ttu-id="932a1-204">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="932a1-204">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="932a1-205">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="932a1-205">locationServicesBlocked</span></span>|<span data-ttu-id="932a1-206">Логический</span><span class="sxs-lookup"><span data-stu-id="932a1-206">Boolean</span></span>|<span data-ttu-id="932a1-207">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="932a1-207">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="932a1-208">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="932a1-208">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="932a1-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-209">Boolean</span></span>|<span data-ttu-id="932a1-210">Указывает, следует ли блокировать автоматическую синхронизацию учетной записи Google.</span><span class="sxs-lookup"><span data-stu-id="932a1-210">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="932a1-211">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="932a1-211">googlePlayStoreBlocked</span></span>|<span data-ttu-id="932a1-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-212">Boolean</span></span>|<span data-ttu-id="932a1-213">Указывает, следует ли блокировать Google Play Маркет.</span><span class="sxs-lookup"><span data-stu-id="932a1-213">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="932a1-214">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="932a1-214">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="932a1-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-215">Boolean</span></span>|<span data-ttu-id="932a1-216">Указывает, следует ли блокировать кнопку спящего режима экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="932a1-216">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="932a1-217">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="932a1-217">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="932a1-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-218">Boolean</span></span>|<span data-ttu-id="932a1-219">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="932a1-219">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="932a1-220">Датеандтимеблоккчанжес</span><span class="sxs-lookup"><span data-stu-id="932a1-220">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="932a1-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-221">Boolean</span></span>|<span data-ttu-id="932a1-222">Указывает, следует ли заблокировать изменение даты и времени в режиме KNOX.</span><span class="sxs-lookup"><span data-stu-id="932a1-222">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="932a1-223">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="932a1-223">kioskModeApps</span></span>|<span data-ttu-id="932a1-224">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="932a1-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="932a1-225">Список разрешенных приложений в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="932a1-225">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="932a1-226">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="932a1-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="932a1-227">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="932a1-227">nfcBlocked</span></span>|<span data-ttu-id="932a1-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-228">Boolean</span></span>|<span data-ttu-id="932a1-229">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="932a1-229">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="932a1-230">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="932a1-230">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="932a1-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-231">Boolean</span></span>|<span data-ttu-id="932a1-232">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="932a1-232">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="932a1-233">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="932a1-233">passwordBlockTrustAgents</span></span>|<span data-ttu-id="932a1-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-234">Boolean</span></span>|<span data-ttu-id="932a1-235">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="932a1-235">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="932a1-236">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="932a1-236">passwordExpirationDays</span></span>|<span data-ttu-id="932a1-237">Int32</span><span class="sxs-lookup"><span data-stu-id="932a1-237">Int32</span></span>|<span data-ttu-id="932a1-238">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="932a1-238">Number of days before the password expires.</span></span> <span data-ttu-id="932a1-239">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="932a1-239">Valid values 1 to 365</span></span>|
|<span data-ttu-id="932a1-240">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="932a1-240">passwordMinimumLength</span></span>|<span data-ttu-id="932a1-241">Int32</span><span class="sxs-lookup"><span data-stu-id="932a1-241">Int32</span></span>|<span data-ttu-id="932a1-242">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="932a1-242">Minimum length of passwords.</span></span> <span data-ttu-id="932a1-243">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="932a1-243">Valid values 4 to 16</span></span>|
|<span data-ttu-id="932a1-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="932a1-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="932a1-245">Int32</span><span class="sxs-lookup"><span data-stu-id="932a1-245">Int32</span></span>|<span data-ttu-id="932a1-246">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="932a1-246">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="932a1-247">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="932a1-247">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="932a1-248">Int32</span><span class="sxs-lookup"><span data-stu-id="932a1-248">Int32</span></span>|<span data-ttu-id="932a1-249">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="932a1-249">Number of previous passwords to block.</span></span> <span data-ttu-id="932a1-250">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="932a1-250">Valid values 0 to 24</span></span>|
|<span data-ttu-id="932a1-251">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="932a1-251">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="932a1-252">Int32</span><span class="sxs-lookup"><span data-stu-id="932a1-252">Int32</span></span>|<span data-ttu-id="932a1-253">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="932a1-253">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="932a1-254">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="932a1-254">Valid values 1 to 16</span></span>|
|<span data-ttu-id="932a1-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="932a1-255">passwordRequiredType</span></span>|[<span data-ttu-id="932a1-256">Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="932a1-256">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="932a1-257">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="932a1-257">Type of password that is required.</span></span> <span data-ttu-id="932a1-258">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="932a1-258">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="932a1-259">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="932a1-259">passwordRequired</span></span>|<span data-ttu-id="932a1-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-260">Boolean</span></span>|<span data-ttu-id="932a1-261">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="932a1-261">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="932a1-262">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="932a1-262">powerOffBlocked</span></span>|<span data-ttu-id="932a1-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-263">Boolean</span></span>|<span data-ttu-id="932a1-264">Указывает, следует ли блокировать отключение устройства.</span><span class="sxs-lookup"><span data-stu-id="932a1-264">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="932a1-265">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="932a1-265">factoryResetBlocked</span></span>|<span data-ttu-id="932a1-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-266">Boolean</span></span>|<span data-ttu-id="932a1-267">Указывает, следует ли запретить пользователю восстанавливать заводские настройки.</span><span class="sxs-lookup"><span data-stu-id="932a1-267">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="932a1-268">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="932a1-268">screenCaptureBlocked</span></span>|<span data-ttu-id="932a1-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-269">Boolean</span></span>|<span data-ttu-id="932a1-270">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="932a1-270">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="932a1-271">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="932a1-271">deviceSharingAllowed</span></span>|<span data-ttu-id="932a1-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-272">Boolean</span></span>|<span data-ttu-id="932a1-273">Указывает, следует ли разрешить режим совместного доступа к устройству.</span><span class="sxs-lookup"><span data-stu-id="932a1-273">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="932a1-274">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="932a1-274">storageBlockGoogleBackup</span></span>|<span data-ttu-id="932a1-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-275">Boolean</span></span>|<span data-ttu-id="932a1-276">Указывает, следует ли блокировать резервное копирование Google.</span><span class="sxs-lookup"><span data-stu-id="932a1-276">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="932a1-277">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="932a1-277">storageBlockRemovableStorage</span></span>|<span data-ttu-id="932a1-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-278">Boolean</span></span>|<span data-ttu-id="932a1-279">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="932a1-279">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="932a1-280">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="932a1-280">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="932a1-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-281">Boolean</span></span>|<span data-ttu-id="932a1-282">Указывает, обязательно ли шифрование устройства.</span><span class="sxs-lookup"><span data-stu-id="932a1-282">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="932a1-283">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="932a1-283">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="932a1-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-284">Boolean</span></span>|<span data-ttu-id="932a1-285">Указывает, обязательно ли шифрование съемных носителей.</span><span class="sxs-lookup"><span data-stu-id="932a1-285">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="932a1-286">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="932a1-286">voiceAssistantBlocked</span></span>|<span data-ttu-id="932a1-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-287">Boolean</span></span>|<span data-ttu-id="932a1-288">Указывает, следует ли блокировать использование голосового помощника.</span><span class="sxs-lookup"><span data-stu-id="932a1-288">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="932a1-289">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="932a1-289">voiceDialingBlocked</span></span>|<span data-ttu-id="932a1-290">Логический</span><span class="sxs-lookup"><span data-stu-id="932a1-290">Boolean</span></span>|<span data-ttu-id="932a1-291">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="932a1-291">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="932a1-292">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="932a1-292">webBrowserBlockPopups</span></span>|<span data-ttu-id="932a1-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-293">Boolean</span></span>|<span data-ttu-id="932a1-294">Указывает, следует ли блокировать всплывающие окна в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="932a1-294">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="932a1-295">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="932a1-295">webBrowserBlockAutofill</span></span>|<span data-ttu-id="932a1-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-296">Boolean</span></span>|<span data-ttu-id="932a1-297">Указывает, следует ли заблокировать функцию автозаполнения в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="932a1-297">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="932a1-298">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="932a1-298">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="932a1-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-299">Boolean</span></span>|<span data-ttu-id="932a1-300">Указывает, следует ли заблокировать JavaScript в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="932a1-300">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="932a1-301">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="932a1-301">webBrowserBlocked</span></span>|<span data-ttu-id="932a1-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-302">Boolean</span></span>|<span data-ttu-id="932a1-303">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="932a1-303">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="932a1-304">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="932a1-304">webBrowserCookieSettings</span></span>|[<span data-ttu-id="932a1-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="932a1-305">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="932a1-306">Настройки файлов cookie в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="932a1-306">Cookie settings within the web browser.</span></span> <span data-ttu-id="932a1-307">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="932a1-307">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="932a1-308">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="932a1-308">wiFiBlocked</span></span>|<span data-ttu-id="932a1-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-309">Boolean</span></span>|<span data-ttu-id="932a1-310">Указывает, следует ли заблокировать синхронизацию Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="932a1-310">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="932a1-311">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="932a1-311">appsInstallAllowList</span></span>|<span data-ttu-id="932a1-312">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="932a1-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="932a1-313">Список приложений, которые можно установить на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="932a1-313">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="932a1-314">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="932a1-314">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="932a1-315">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="932a1-315">appsLaunchBlockList</span></span>|<span data-ttu-id="932a1-316">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="932a1-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="932a1-317">Список приложений, которые запрещено запускать на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="932a1-317">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="932a1-318">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="932a1-318">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="932a1-319">appsHideList</span><span class="sxs-lookup"><span data-stu-id="932a1-319">appsHideList</span></span>|<span data-ttu-id="932a1-320">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="932a1-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="932a1-321">Список приложений, которые следует скрыть на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="932a1-321">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="932a1-322">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="932a1-322">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="932a1-323">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="932a1-323">securityRequireVerifyApps</span></span>|<span data-ttu-id="932a1-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="932a1-324">Boolean</span></span>|<span data-ttu-id="932a1-325">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="932a1-325">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="932a1-326">Ответ</span><span class="sxs-lookup"><span data-stu-id="932a1-326">Response</span></span>
<span data-ttu-id="932a1-327">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="932a1-327">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="932a1-328">Пример</span><span class="sxs-lookup"><span data-stu-id="932a1-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="932a1-329">Запрос</span><span class="sxs-lookup"><span data-stu-id="932a1-329">Request</span></span>
<span data-ttu-id="932a1-330">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="932a1-330">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="932a1-331">Отклик</span><span class="sxs-lookup"><span data-stu-id="932a1-331">Response</span></span>
<span data-ttu-id="932a1-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="932a1-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





