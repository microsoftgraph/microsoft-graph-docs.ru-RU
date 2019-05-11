---
title: Создание androidGeneralDeviceConfiguration
description: Создание объекта androidGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 50cc24d7c3c9852066a23dee1252bc7c05f1afdb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33929674"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="79d55-103">Создание androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="79d55-103">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="79d55-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79d55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79d55-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79d55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79d55-106">Создание объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d55-106">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79d55-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="79d55-107">Prerequisites</span></span>
<span data-ttu-id="79d55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79d55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79d55-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79d55-110">Permission type</span></span>|<span data-ttu-id="79d55-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79d55-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79d55-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79d55-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79d55-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79d55-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79d55-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79d55-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79d55-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79d55-115">Not supported.</span></span>|
|<span data-ttu-id="79d55-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79d55-116">Application</span></span>|<span data-ttu-id="79d55-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79d55-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79d55-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79d55-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="79d55-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79d55-119">Request headers</span></span>
|<span data-ttu-id="79d55-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79d55-120">Header</span></span>|<span data-ttu-id="79d55-121">Значение</span><span class="sxs-lookup"><span data-stu-id="79d55-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79d55-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79d55-122">Authorization</span></span>|<span data-ttu-id="79d55-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79d55-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79d55-124">Accept</span><span class="sxs-lookup"><span data-stu-id="79d55-124">Accept</span></span>|<span data-ttu-id="79d55-125">application/json</span><span class="sxs-lookup"><span data-stu-id="79d55-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79d55-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="79d55-126">Request body</span></span>
<span data-ttu-id="79d55-127">В теле запроса добавьте представление объекта androidGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79d55-127">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="79d55-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта androidGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="79d55-128">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="79d55-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="79d55-129">Property</span></span>|<span data-ttu-id="79d55-130">Тип</span><span class="sxs-lookup"><span data-stu-id="79d55-130">Type</span></span>|<span data-ttu-id="79d55-131">Описание</span><span class="sxs-lookup"><span data-stu-id="79d55-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79d55-132">id</span><span class="sxs-lookup"><span data-stu-id="79d55-132">id</span></span>|<span data-ttu-id="79d55-133">String</span><span class="sxs-lookup"><span data-stu-id="79d55-133">String</span></span>|<span data-ttu-id="79d55-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="79d55-134">Key of the entity.</span></span> <span data-ttu-id="79d55-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d55-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d55-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79d55-136">lastModifiedDateTime</span></span>|<span data-ttu-id="79d55-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79d55-137">DateTimeOffset</span></span>|<span data-ttu-id="79d55-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="79d55-138">DateTime the object was last modified.</span></span> <span data-ttu-id="79d55-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d55-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d55-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="79d55-140">roleScopeTagIds</span></span>|<span data-ttu-id="79d55-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="79d55-141">String collection</span></span>|<span data-ttu-id="79d55-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="79d55-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="79d55-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d55-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d55-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="79d55-144">supportsScopeTags</span></span>|<span data-ttu-id="79d55-145">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-145">Boolean</span></span>|<span data-ttu-id="79d55-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="79d55-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="79d55-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="79d55-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="79d55-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="79d55-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="79d55-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="79d55-149">This property is read-only.</span></span> <span data-ttu-id="79d55-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d55-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d55-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79d55-151">createdDateTime</span></span>|<span data-ttu-id="79d55-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79d55-152">DateTimeOffset</span></span>|<span data-ttu-id="79d55-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="79d55-153">DateTime the object was created.</span></span> <span data-ttu-id="79d55-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d55-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d55-155">description</span><span class="sxs-lookup"><span data-stu-id="79d55-155">description</span></span>|<span data-ttu-id="79d55-156">String</span><span class="sxs-lookup"><span data-stu-id="79d55-156">String</span></span>|<span data-ttu-id="79d55-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="79d55-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="79d55-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d55-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d55-159">displayName</span><span class="sxs-lookup"><span data-stu-id="79d55-159">displayName</span></span>|<span data-ttu-id="79d55-160">Строка</span><span class="sxs-lookup"><span data-stu-id="79d55-160">String</span></span>|<span data-ttu-id="79d55-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="79d55-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="79d55-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d55-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d55-163">version</span><span class="sxs-lookup"><span data-stu-id="79d55-163">version</span></span>|<span data-ttu-id="79d55-164">Int32</span><span class="sxs-lookup"><span data-stu-id="79d55-164">Int32</span></span>|<span data-ttu-id="79d55-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="79d55-165">Version of the device configuration.</span></span> <span data-ttu-id="79d55-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79d55-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d55-167">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="79d55-167">appsBlockClipboardSharing</span></span>|<span data-ttu-id="79d55-168">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-168">Boolean</span></span>|<span data-ttu-id="79d55-169">Указывает, следует ли запретить совместное использование буфера обмена для копирования данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="79d55-169">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="79d55-170">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="79d55-170">appsBlockCopyPaste</span></span>|<span data-ttu-id="79d55-171">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-171">Boolean</span></span>|<span data-ttu-id="79d55-172">Указывает, следует ли запретить копирование данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="79d55-172">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="79d55-173">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="79d55-173">appsBlockYouTube</span></span>|<span data-ttu-id="79d55-174">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-174">Boolean</span></span>|<span data-ttu-id="79d55-175">Указывает, следует ли заблокировать приложение YouTube.</span><span class="sxs-lookup"><span data-stu-id="79d55-175">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="79d55-176">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="79d55-176">bluetoothBlocked</span></span>|<span data-ttu-id="79d55-177">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-177">Boolean</span></span>|<span data-ttu-id="79d55-178">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="79d55-178">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="79d55-179">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="79d55-179">cameraBlocked</span></span>|<span data-ttu-id="79d55-180">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-180">Boolean</span></span>|<span data-ttu-id="79d55-181">Указывает, следует ли запретить использовать камеру.</span><span class="sxs-lookup"><span data-stu-id="79d55-181">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="79d55-182">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="79d55-182">cellularBlockDataRoaming</span></span>|<span data-ttu-id="79d55-183">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-183">Boolean</span></span>|<span data-ttu-id="79d55-184">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="79d55-184">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="79d55-185">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="79d55-185">cellularBlockMessaging</span></span>|<span data-ttu-id="79d55-186">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-186">Boolean</span></span>|<span data-ttu-id="79d55-187">Указывает, следует ли запретить обмениваться SMS и MMS.</span><span class="sxs-lookup"><span data-stu-id="79d55-187">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="79d55-188">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="79d55-188">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="79d55-189">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-189">Boolean</span></span>|<span data-ttu-id="79d55-190">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="79d55-190">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="79d55-191">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="79d55-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="79d55-192">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-192">Boolean</span></span>|<span data-ttu-id="79d55-193">Указывает, следует ли блокировать синхронизацию модема Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="79d55-193">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="79d55-194">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="79d55-194">compliantAppsList</span></span>|<span data-ttu-id="79d55-195">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="79d55-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="79d55-196">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="79d55-196">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="79d55-197">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="79d55-197">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="79d55-198">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="79d55-198">compliantAppListType</span></span>|[<span data-ttu-id="79d55-199">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="79d55-199">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="79d55-200">Тип списка, определенного свойством CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="79d55-200">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="79d55-201">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="79d55-201">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="79d55-202">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="79d55-202">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="79d55-203">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-203">Boolean</span></span>|<span data-ttu-id="79d55-204">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="79d55-204">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="79d55-205">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="79d55-205">locationServicesBlocked</span></span>|<span data-ttu-id="79d55-206">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-206">Boolean</span></span>|<span data-ttu-id="79d55-207">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="79d55-207">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="79d55-208">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="79d55-208">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="79d55-209">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-209">Boolean</span></span>|<span data-ttu-id="79d55-210">Указывает, следует ли блокировать автоматическую синхронизацию учетной записи Google.</span><span class="sxs-lookup"><span data-stu-id="79d55-210">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="79d55-211">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="79d55-211">googlePlayStoreBlocked</span></span>|<span data-ttu-id="79d55-212">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-212">Boolean</span></span>|<span data-ttu-id="79d55-213">Указывает, следует ли блокировать Google Play Маркет.</span><span class="sxs-lookup"><span data-stu-id="79d55-213">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="79d55-214">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="79d55-214">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="79d55-215">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-215">Boolean</span></span>|<span data-ttu-id="79d55-216">Указывает, следует ли блокировать кнопку спящего режима экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="79d55-216">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="79d55-217">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="79d55-217">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="79d55-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d55-218">Boolean</span></span>|<span data-ttu-id="79d55-219">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="79d55-219">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="79d55-220">Датеандтимеблоккчанжес</span><span class="sxs-lookup"><span data-stu-id="79d55-220">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="79d55-221">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-221">Boolean</span></span>|<span data-ttu-id="79d55-222">Указывает, следует ли заблокировать изменение даты и времени в режиме KNOX.</span><span class="sxs-lookup"><span data-stu-id="79d55-222">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="79d55-223">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="79d55-223">kioskModeApps</span></span>|<span data-ttu-id="79d55-224">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="79d55-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="79d55-225">Список разрешенных приложений в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="79d55-225">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="79d55-226">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="79d55-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="79d55-227">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="79d55-227">nfcBlocked</span></span>|<span data-ttu-id="79d55-228">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-228">Boolean</span></span>|<span data-ttu-id="79d55-229">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="79d55-229">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="79d55-230">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="79d55-230">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="79d55-231">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-231">Boolean</span></span>|<span data-ttu-id="79d55-232">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="79d55-232">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="79d55-233">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="79d55-233">passwordBlockTrustAgents</span></span>|<span data-ttu-id="79d55-234">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-234">Boolean</span></span>|<span data-ttu-id="79d55-235">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="79d55-235">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="79d55-236">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="79d55-236">passwordExpirationDays</span></span>|<span data-ttu-id="79d55-237">Int32</span><span class="sxs-lookup"><span data-stu-id="79d55-237">Int32</span></span>|<span data-ttu-id="79d55-238">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="79d55-238">Number of days before the password expires.</span></span> <span data-ttu-id="79d55-239">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="79d55-239">Valid values 1 to 365</span></span>|
|<span data-ttu-id="79d55-240">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="79d55-240">passwordMinimumLength</span></span>|<span data-ttu-id="79d55-241">Int32</span><span class="sxs-lookup"><span data-stu-id="79d55-241">Int32</span></span>|<span data-ttu-id="79d55-242">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="79d55-242">Minimum length of passwords.</span></span> <span data-ttu-id="79d55-243">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="79d55-243">Valid values 4 to 16</span></span>|
|<span data-ttu-id="79d55-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="79d55-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="79d55-245">Int32</span><span class="sxs-lookup"><span data-stu-id="79d55-245">Int32</span></span>|<span data-ttu-id="79d55-246">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="79d55-246">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="79d55-247">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="79d55-247">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="79d55-248">Int32</span><span class="sxs-lookup"><span data-stu-id="79d55-248">Int32</span></span>|<span data-ttu-id="79d55-249">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="79d55-249">Number of previous passwords to block.</span></span> <span data-ttu-id="79d55-250">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="79d55-250">Valid values 0 to 24</span></span>|
|<span data-ttu-id="79d55-251">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="79d55-251">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="79d55-252">Int32</span><span class="sxs-lookup"><span data-stu-id="79d55-252">Int32</span></span>|<span data-ttu-id="79d55-253">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="79d55-253">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="79d55-254">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="79d55-254">Valid values 1 to 16</span></span>|
|<span data-ttu-id="79d55-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="79d55-255">passwordRequiredType</span></span>|[<span data-ttu-id="79d55-256">Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="79d55-256">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="79d55-257">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="79d55-257">Type of password that is required.</span></span> <span data-ttu-id="79d55-258">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="79d55-258">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="79d55-259">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="79d55-259">passwordRequired</span></span>|<span data-ttu-id="79d55-260">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-260">Boolean</span></span>|<span data-ttu-id="79d55-261">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="79d55-261">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="79d55-262">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="79d55-262">powerOffBlocked</span></span>|<span data-ttu-id="79d55-263">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-263">Boolean</span></span>|<span data-ttu-id="79d55-264">Указывает, следует ли блокировать отключение устройства.</span><span class="sxs-lookup"><span data-stu-id="79d55-264">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="79d55-265">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="79d55-265">factoryResetBlocked</span></span>|<span data-ttu-id="79d55-266">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-266">Boolean</span></span>|<span data-ttu-id="79d55-267">Указывает, следует ли запретить пользователю восстанавливать заводские настройки.</span><span class="sxs-lookup"><span data-stu-id="79d55-267">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="79d55-268">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="79d55-268">screenCaptureBlocked</span></span>|<span data-ttu-id="79d55-269">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-269">Boolean</span></span>|<span data-ttu-id="79d55-270">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="79d55-270">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="79d55-271">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="79d55-271">deviceSharingAllowed</span></span>|<span data-ttu-id="79d55-272">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-272">Boolean</span></span>|<span data-ttu-id="79d55-273">Указывает, следует ли разрешить режим совместного доступа к устройству.</span><span class="sxs-lookup"><span data-stu-id="79d55-273">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="79d55-274">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="79d55-274">storageBlockGoogleBackup</span></span>|<span data-ttu-id="79d55-275">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-275">Boolean</span></span>|<span data-ttu-id="79d55-276">Указывает, следует ли блокировать резервное копирование Google.</span><span class="sxs-lookup"><span data-stu-id="79d55-276">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="79d55-277">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="79d55-277">storageBlockRemovableStorage</span></span>|<span data-ttu-id="79d55-278">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-278">Boolean</span></span>|<span data-ttu-id="79d55-279">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="79d55-279">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="79d55-280">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="79d55-280">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="79d55-281">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-281">Boolean</span></span>|<span data-ttu-id="79d55-282">Указывает, обязательно ли шифрование устройства.</span><span class="sxs-lookup"><span data-stu-id="79d55-282">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="79d55-283">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="79d55-283">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="79d55-284">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-284">Boolean</span></span>|<span data-ttu-id="79d55-285">Указывает, обязательно ли шифрование съемных носителей.</span><span class="sxs-lookup"><span data-stu-id="79d55-285">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="79d55-286">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="79d55-286">voiceAssistantBlocked</span></span>|<span data-ttu-id="79d55-287">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-287">Boolean</span></span>|<span data-ttu-id="79d55-288">Указывает, следует ли блокировать использование голосового помощника.</span><span class="sxs-lookup"><span data-stu-id="79d55-288">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="79d55-289">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="79d55-289">voiceDialingBlocked</span></span>|<span data-ttu-id="79d55-290">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-290">Boolean</span></span>|<span data-ttu-id="79d55-291">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="79d55-291">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="79d55-292">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="79d55-292">webBrowserBlockPopups</span></span>|<span data-ttu-id="79d55-293">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-293">Boolean</span></span>|<span data-ttu-id="79d55-294">Указывает, следует ли блокировать всплывающие окна в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="79d55-294">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="79d55-295">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="79d55-295">webBrowserBlockAutofill</span></span>|<span data-ttu-id="79d55-296">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-296">Boolean</span></span>|<span data-ttu-id="79d55-297">Указывает, следует ли заблокировать функцию автозаполнения в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="79d55-297">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="79d55-298">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="79d55-298">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="79d55-299">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-299">Boolean</span></span>|<span data-ttu-id="79d55-300">Указывает, следует ли заблокировать JavaScript в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="79d55-300">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="79d55-301">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="79d55-301">webBrowserBlocked</span></span>|<span data-ttu-id="79d55-302">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-302">Boolean</span></span>|<span data-ttu-id="79d55-303">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="79d55-303">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="79d55-304">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="79d55-304">webBrowserCookieSettings</span></span>|[<span data-ttu-id="79d55-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="79d55-305">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="79d55-306">Настройки файлов cookie в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="79d55-306">Cookie settings within the web browser.</span></span> <span data-ttu-id="79d55-307">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="79d55-307">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="79d55-308">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="79d55-308">wiFiBlocked</span></span>|<span data-ttu-id="79d55-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d55-309">Boolean</span></span>|<span data-ttu-id="79d55-310">Указывает, следует ли заблокировать синхронизацию Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="79d55-310">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="79d55-311">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="79d55-311">appsInstallAllowList</span></span>|<span data-ttu-id="79d55-312">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="79d55-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="79d55-313">Список приложений, которые можно установить на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="79d55-313">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="79d55-314">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="79d55-314">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="79d55-315">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="79d55-315">appsLaunchBlockList</span></span>|<span data-ttu-id="79d55-316">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="79d55-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="79d55-317">Список приложений, которые запрещено запускать на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="79d55-317">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="79d55-318">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="79d55-318">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="79d55-319">appsHideList</span><span class="sxs-lookup"><span data-stu-id="79d55-319">appsHideList</span></span>|<span data-ttu-id="79d55-320">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="79d55-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="79d55-321">Список приложений, которые следует скрыть на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="79d55-321">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="79d55-322">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="79d55-322">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="79d55-323">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="79d55-323">securityRequireVerifyApps</span></span>|<span data-ttu-id="79d55-324">Логический</span><span class="sxs-lookup"><span data-stu-id="79d55-324">Boolean</span></span>|<span data-ttu-id="79d55-325">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="79d55-325">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="79d55-326">Отклик</span><span class="sxs-lookup"><span data-stu-id="79d55-326">Response</span></span>
<span data-ttu-id="79d55-327">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="79d55-327">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79d55-328">Пример</span><span class="sxs-lookup"><span data-stu-id="79d55-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="79d55-329">Запрос</span><span class="sxs-lookup"><span data-stu-id="79d55-329">Request</span></span>
<span data-ttu-id="79d55-330">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79d55-330">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="79d55-331">Отклик</span><span class="sxs-lookup"><span data-stu-id="79d55-331">Response</span></span>
<span data-ttu-id="79d55-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79d55-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




