---
title: Update androidGeneralDeviceConfiguration
description: Обновление свойств объекта androidGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ce4bbbe2074bba753d32a7aa8d293282cd320ded
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757222"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="c0894-103">Update androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0894-103">Update androidGeneralDeviceConfiguration</span></span>

<span data-ttu-id="c0894-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0894-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0894-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0894-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0894-106">Обновление свойств объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0894-106">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0894-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c0894-107">Prerequisites</span></span>
<span data-ttu-id="c0894-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0894-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0894-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0894-110">Permission type</span></span>|<span data-ttu-id="c0894-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0894-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0894-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0894-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0894-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0894-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0894-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0894-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0894-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0894-115">Not supported.</span></span>|
|<span data-ttu-id="c0894-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c0894-116">Application</span></span>|<span data-ttu-id="c0894-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0894-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0894-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0894-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c0894-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c0894-119">Request headers</span></span>
|<span data-ttu-id="c0894-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0894-120">Header</span></span>|<span data-ttu-id="c0894-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c0894-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0894-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0894-122">Authorization</span></span>|<span data-ttu-id="c0894-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0894-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0894-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c0894-124">Accept</span></span>|<span data-ttu-id="c0894-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0894-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0894-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0894-126">Request body</span></span>
<span data-ttu-id="c0894-127">В тексте запроса добавьте представление объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0894-127">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="c0894-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0894-128">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="c0894-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0894-129">Property</span></span>|<span data-ttu-id="c0894-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c0894-130">Type</span></span>|<span data-ttu-id="c0894-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c0894-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0894-132">id</span><span class="sxs-lookup"><span data-stu-id="c0894-132">id</span></span>|<span data-ttu-id="c0894-133">String</span><span class="sxs-lookup"><span data-stu-id="c0894-133">String</span></span>|<span data-ttu-id="c0894-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c0894-134">Key of the entity.</span></span> <span data-ttu-id="c0894-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0894-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0894-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0894-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c0894-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0894-137">DateTimeOffset</span></span>|<span data-ttu-id="c0894-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c0894-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c0894-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0894-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0894-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0894-140">createdDateTime</span></span>|<span data-ttu-id="c0894-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0894-141">DateTimeOffset</span></span>|<span data-ttu-id="c0894-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c0894-142">DateTime the object was created.</span></span> <span data-ttu-id="c0894-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0894-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0894-144">description</span><span class="sxs-lookup"><span data-stu-id="c0894-144">description</span></span>|<span data-ttu-id="c0894-145">String</span><span class="sxs-lookup"><span data-stu-id="c0894-145">String</span></span>|<span data-ttu-id="c0894-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c0894-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c0894-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0894-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0894-148">displayName</span><span class="sxs-lookup"><span data-stu-id="c0894-148">displayName</span></span>|<span data-ttu-id="c0894-149">String</span><span class="sxs-lookup"><span data-stu-id="c0894-149">String</span></span>|<span data-ttu-id="c0894-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c0894-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c0894-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0894-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0894-152">version</span><span class="sxs-lookup"><span data-stu-id="c0894-152">version</span></span>|<span data-ttu-id="c0894-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c0894-153">Int32</span></span>|<span data-ttu-id="c0894-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c0894-154">Version of the device configuration.</span></span> <span data-ttu-id="c0894-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0894-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0894-156">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="c0894-156">appsBlockClipboardSharing</span></span>|<span data-ttu-id="c0894-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-157">Boolean</span></span>|<span data-ttu-id="c0894-158">Указывает, следует ли запретить совместное использование буфера обмена для копирования данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="c0894-158">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="c0894-159">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="c0894-159">appsBlockCopyPaste</span></span>|<span data-ttu-id="c0894-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-160">Boolean</span></span>|<span data-ttu-id="c0894-161">Указывает, следует ли запретить копирование данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="c0894-161">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="c0894-162">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="c0894-162">appsBlockYouTube</span></span>|<span data-ttu-id="c0894-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-163">Boolean</span></span>|<span data-ttu-id="c0894-164">Указывает, следует ли заблокировать приложение YouTube.</span><span class="sxs-lookup"><span data-stu-id="c0894-164">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="c0894-165">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="c0894-165">bluetoothBlocked</span></span>|<span data-ttu-id="c0894-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-166">Boolean</span></span>|<span data-ttu-id="c0894-167">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="c0894-167">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="c0894-168">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="c0894-168">cameraBlocked</span></span>|<span data-ttu-id="c0894-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-169">Boolean</span></span>|<span data-ttu-id="c0894-170">Указывает, следует ли запретить использовать камеру.</span><span class="sxs-lookup"><span data-stu-id="c0894-170">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="c0894-171">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="c0894-171">cellularBlockDataRoaming</span></span>|<span data-ttu-id="c0894-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-172">Boolean</span></span>|<span data-ttu-id="c0894-173">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="c0894-173">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="c0894-174">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="c0894-174">cellularBlockMessaging</span></span>|<span data-ttu-id="c0894-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-175">Boolean</span></span>|<span data-ttu-id="c0894-176">Указывает, следует ли запретить обмениваться SMS и MMS.</span><span class="sxs-lookup"><span data-stu-id="c0894-176">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="c0894-177">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="c0894-177">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="c0894-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-178">Boolean</span></span>|<span data-ttu-id="c0894-179">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="c0894-179">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="c0894-180">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="c0894-180">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="c0894-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-181">Boolean</span></span>|<span data-ttu-id="c0894-182">Указывает, следует ли блокировать синхронизацию модема Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="c0894-182">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="c0894-183">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="c0894-183">compliantAppsList</span></span>|<span data-ttu-id="c0894-184">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c0894-184">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c0894-185">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="c0894-185">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="c0894-186">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="c0894-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c0894-187">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="c0894-187">compliantAppListType</span></span>|[<span data-ttu-id="c0894-188">appListType</span><span class="sxs-lookup"><span data-stu-id="c0894-188">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="c0894-189">Тип списка, определенного свойством CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="c0894-189">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="c0894-190">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="c0894-190">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="c0894-191">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="c0894-191">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="c0894-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-192">Boolean</span></span>|<span data-ttu-id="c0894-193">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="c0894-193">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="c0894-194">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="c0894-194">locationServicesBlocked</span></span>|<span data-ttu-id="c0894-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-195">Boolean</span></span>|<span data-ttu-id="c0894-196">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="c0894-196">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="c0894-197">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="c0894-197">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="c0894-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-198">Boolean</span></span>|<span data-ttu-id="c0894-199">Указывает, следует ли блокировать автоматическую синхронизацию учетной записи Google.</span><span class="sxs-lookup"><span data-stu-id="c0894-199">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="c0894-200">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="c0894-200">googlePlayStoreBlocked</span></span>|<span data-ttu-id="c0894-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-201">Boolean</span></span>|<span data-ttu-id="c0894-202">Указывает, следует ли блокировать Google Play Маркет.</span><span class="sxs-lookup"><span data-stu-id="c0894-202">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="c0894-203">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="c0894-203">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="c0894-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-204">Boolean</span></span>|<span data-ttu-id="c0894-205">Указывает, следует ли блокировать кнопку спящего режима экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="c0894-205">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0894-206">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="c0894-206">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="c0894-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-207">Boolean</span></span>|<span data-ttu-id="c0894-208">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="c0894-208">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0894-209">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="c0894-209">kioskModeApps</span></span>|<span data-ttu-id="c0894-210">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c0894-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c0894-211">Список разрешенных приложений в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="c0894-211">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="c0894-212">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c0894-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c0894-213">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="c0894-213">nfcBlocked</span></span>|<span data-ttu-id="c0894-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-214">Boolean</span></span>|<span data-ttu-id="c0894-215">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="c0894-215">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="c0894-216">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="c0894-216">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="c0894-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-217">Boolean</span></span>|<span data-ttu-id="c0894-218">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="c0894-218">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="c0894-219">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="c0894-219">passwordBlockTrustAgents</span></span>|<span data-ttu-id="c0894-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-220">Boolean</span></span>|<span data-ttu-id="c0894-221">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="c0894-221">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="c0894-222">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c0894-222">passwordExpirationDays</span></span>|<span data-ttu-id="c0894-223">Int32</span><span class="sxs-lookup"><span data-stu-id="c0894-223">Int32</span></span>|<span data-ttu-id="c0894-224">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="c0894-224">Number of days before the password expires.</span></span> <span data-ttu-id="c0894-225">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="c0894-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c0894-226">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c0894-226">passwordMinimumLength</span></span>|<span data-ttu-id="c0894-227">Int32</span><span class="sxs-lookup"><span data-stu-id="c0894-227">Int32</span></span>|<span data-ttu-id="c0894-228">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="c0894-228">Minimum length of passwords.</span></span> <span data-ttu-id="c0894-229">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="c0894-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c0894-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c0894-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c0894-231">Int32</span><span class="sxs-lookup"><span data-stu-id="c0894-231">Int32</span></span>|<span data-ttu-id="c0894-232">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="c0894-232">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c0894-233">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c0894-233">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c0894-234">Int32</span><span class="sxs-lookup"><span data-stu-id="c0894-234">Int32</span></span>|<span data-ttu-id="c0894-235">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="c0894-235">Number of previous passwords to block.</span></span> <span data-ttu-id="c0894-236">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="c0894-236">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c0894-237">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c0894-237">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c0894-238">Int32</span><span class="sxs-lookup"><span data-stu-id="c0894-238">Int32</span></span>|<span data-ttu-id="c0894-239">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="c0894-239">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="c0894-240">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="c0894-240">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c0894-241">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c0894-241">passwordRequiredType</span></span>|[<span data-ttu-id="c0894-242">AndroidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c0894-242">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="c0894-243">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="c0894-243">Type of password that is required.</span></span> <span data-ttu-id="c0894-244">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="c0894-244">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="c0894-245">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c0894-245">passwordRequired</span></span>|<span data-ttu-id="c0894-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-246">Boolean</span></span>|<span data-ttu-id="c0894-247">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="c0894-247">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="c0894-248">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="c0894-248">powerOffBlocked</span></span>|<span data-ttu-id="c0894-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-249">Boolean</span></span>|<span data-ttu-id="c0894-250">Указывает, следует ли блокировать отключение устройства.</span><span class="sxs-lookup"><span data-stu-id="c0894-250">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="c0894-251">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="c0894-251">factoryResetBlocked</span></span>|<span data-ttu-id="c0894-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-252">Boolean</span></span>|<span data-ttu-id="c0894-253">Указывает, следует ли запретить пользователю восстанавливать заводские настройки.</span><span class="sxs-lookup"><span data-stu-id="c0894-253">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="c0894-254">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="c0894-254">screenCaptureBlocked</span></span>|<span data-ttu-id="c0894-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-255">Boolean</span></span>|<span data-ttu-id="c0894-256">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="c0894-256">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="c0894-257">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="c0894-257">deviceSharingAllowed</span></span>|<span data-ttu-id="c0894-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-258">Boolean</span></span>|<span data-ttu-id="c0894-259">Указывает, следует ли разрешить режим совместного доступа к устройству.</span><span class="sxs-lookup"><span data-stu-id="c0894-259">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="c0894-260">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="c0894-260">storageBlockGoogleBackup</span></span>|<span data-ttu-id="c0894-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-261">Boolean</span></span>|<span data-ttu-id="c0894-262">Указывает, следует ли блокировать резервное копирование Google.</span><span class="sxs-lookup"><span data-stu-id="c0894-262">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="c0894-263">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="c0894-263">storageBlockRemovableStorage</span></span>|<span data-ttu-id="c0894-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-264">Boolean</span></span>|<span data-ttu-id="c0894-265">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="c0894-265">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="c0894-266">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="c0894-266">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="c0894-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-267">Boolean</span></span>|<span data-ttu-id="c0894-268">Указывает, обязательно ли шифрование устройства.</span><span class="sxs-lookup"><span data-stu-id="c0894-268">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="c0894-269">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="c0894-269">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="c0894-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-270">Boolean</span></span>|<span data-ttu-id="c0894-271">Указывает, обязательно ли шифрование съемных носителей.</span><span class="sxs-lookup"><span data-stu-id="c0894-271">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="c0894-272">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="c0894-272">voiceAssistantBlocked</span></span>|<span data-ttu-id="c0894-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-273">Boolean</span></span>|<span data-ttu-id="c0894-274">Указывает, следует ли блокировать использование голосового помощника.</span><span class="sxs-lookup"><span data-stu-id="c0894-274">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="c0894-275">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="c0894-275">voiceDialingBlocked</span></span>|<span data-ttu-id="c0894-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-276">Boolean</span></span>|<span data-ttu-id="c0894-277">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="c0894-277">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="c0894-278">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="c0894-278">webBrowserBlockPopups</span></span>|<span data-ttu-id="c0894-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-279">Boolean</span></span>|<span data-ttu-id="c0894-280">Указывает, следует ли блокировать всплывающие окна в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="c0894-280">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="c0894-281">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="c0894-281">webBrowserBlockAutofill</span></span>|<span data-ttu-id="c0894-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-282">Boolean</span></span>|<span data-ttu-id="c0894-283">Указывает, следует ли заблокировать функцию автозаполнения в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="c0894-283">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="c0894-284">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="c0894-284">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="c0894-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-285">Boolean</span></span>|<span data-ttu-id="c0894-286">Указывает, следует ли заблокировать JavaScript в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="c0894-286">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="c0894-287">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="c0894-287">webBrowserBlocked</span></span>|<span data-ttu-id="c0894-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-288">Boolean</span></span>|<span data-ttu-id="c0894-289">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="c0894-289">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="c0894-290">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="c0894-290">webBrowserCookieSettings</span></span>|[<span data-ttu-id="c0894-291">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="c0894-291">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="c0894-292">Настройки файлов cookie в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="c0894-292">Cookie settings within the web browser.</span></span> <span data-ttu-id="c0894-293">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="c0894-293">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="c0894-294">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="c0894-294">wiFiBlocked</span></span>|<span data-ttu-id="c0894-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-295">Boolean</span></span>|<span data-ttu-id="c0894-296">Указывает, следует ли заблокировать синхронизацию Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="c0894-296">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="c0894-297">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="c0894-297">appsInstallAllowList</span></span>|<span data-ttu-id="c0894-298">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c0894-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c0894-299">Список приложений, которые можно установить на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="c0894-299">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="c0894-300">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c0894-300">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c0894-301">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="c0894-301">appsLaunchBlockList</span></span>|<span data-ttu-id="c0894-302">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c0894-302">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c0894-303">Список приложений, которые запрещено запускать на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="c0894-303">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="c0894-304">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c0894-304">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c0894-305">appsHideList</span><span class="sxs-lookup"><span data-stu-id="c0894-305">appsHideList</span></span>|<span data-ttu-id="c0894-306">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c0894-306">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c0894-307">Список приложений, которые следует скрыть на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="c0894-307">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="c0894-308">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c0894-308">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c0894-309">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="c0894-309">securityRequireVerifyApps</span></span>|<span data-ttu-id="c0894-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0894-310">Boolean</span></span>|<span data-ttu-id="c0894-311">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="c0894-311">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="c0894-312">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0894-312">Response</span></span>
<span data-ttu-id="c0894-313">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c0894-313">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0894-314">Пример</span><span class="sxs-lookup"><span data-stu-id="c0894-314">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0894-315">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0894-315">Request</span></span>
<span data-ttu-id="c0894-316">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0894-316">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3033

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="c0894-317">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0894-317">Response</span></span>
<span data-ttu-id="c0894-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0894-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3205

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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




