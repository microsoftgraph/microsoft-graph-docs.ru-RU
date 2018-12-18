---
title: Update androidGeneralDeviceConfiguration
description: Обновление свойств объекта androidGeneralDeviceConfiguration.
author: tfitzmac
ms.openlocfilehash: bce3fa318ed7ff0e818c19a6907a34c26b804b35
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302445"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="beeae-103">Update androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="beeae-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="beeae-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="beeae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="beeae-105">Обновление свойств объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="beeae-105">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="beeae-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="beeae-106">Prerequisites</span></span>
<span data-ttu-id="beeae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beeae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beeae-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="beeae-109">Permission type</span></span>|<span data-ttu-id="beeae-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="beeae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="beeae-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="beeae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="beeae-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beeae-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="beeae-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="beeae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="beeae-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beeae-114">Not supported.</span></span>|
|<span data-ttu-id="beeae-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="beeae-115">Application</span></span>|<span data-ttu-id="beeae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beeae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="beeae-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="beeae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="beeae-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="beeae-118">Request headers</span></span>
|<span data-ttu-id="beeae-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="beeae-119">Header</span></span>|<span data-ttu-id="beeae-120">Значение</span><span class="sxs-lookup"><span data-stu-id="beeae-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="beeae-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="beeae-121">Authorization</span></span>|<span data-ttu-id="beeae-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="beeae-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="beeae-123">Accept</span><span class="sxs-lookup"><span data-stu-id="beeae-123">Accept</span></span>|<span data-ttu-id="beeae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="beeae-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="beeae-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="beeae-125">Request body</span></span>
<span data-ttu-id="beeae-126">В тексте запроса добавьте представление объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="beeae-126">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="beeae-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="beeae-127">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="beeae-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="beeae-128">Property</span></span>|<span data-ttu-id="beeae-129">Тип</span><span class="sxs-lookup"><span data-stu-id="beeae-129">Type</span></span>|<span data-ttu-id="beeae-130">Описание</span><span class="sxs-lookup"><span data-stu-id="beeae-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beeae-131">id</span><span class="sxs-lookup"><span data-stu-id="beeae-131">id</span></span>|<span data-ttu-id="beeae-132">Строка</span><span class="sxs-lookup"><span data-stu-id="beeae-132">String</span></span>|<span data-ttu-id="beeae-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="beeae-133">Key of the entity.</span></span> <span data-ttu-id="beeae-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="beeae-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beeae-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="beeae-135">lastModifiedDateTime</span></span>|<span data-ttu-id="beeae-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="beeae-136">DateTimeOffset</span></span>|<span data-ttu-id="beeae-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="beeae-137">DateTime the object was last modified.</span></span> <span data-ttu-id="beeae-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="beeae-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beeae-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="beeae-139">createdDateTime</span></span>|<span data-ttu-id="beeae-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="beeae-140">DateTimeOffset</span></span>|<span data-ttu-id="beeae-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="beeae-141">DateTime the object was created.</span></span> <span data-ttu-id="beeae-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="beeae-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beeae-143">описание</span><span class="sxs-lookup"><span data-stu-id="beeae-143">description</span></span>|<span data-ttu-id="beeae-144">Строка</span><span class="sxs-lookup"><span data-stu-id="beeae-144">String</span></span>|<span data-ttu-id="beeae-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="beeae-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="beeae-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="beeae-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beeae-147">displayName</span><span class="sxs-lookup"><span data-stu-id="beeae-147">displayName</span></span>|<span data-ttu-id="beeae-148">Строка</span><span class="sxs-lookup"><span data-stu-id="beeae-148">String</span></span>|<span data-ttu-id="beeae-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="beeae-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="beeae-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="beeae-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beeae-151">version</span><span class="sxs-lookup"><span data-stu-id="beeae-151">version</span></span>|<span data-ttu-id="beeae-152">Int32</span><span class="sxs-lookup"><span data-stu-id="beeae-152">Int32</span></span>|<span data-ttu-id="beeae-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="beeae-153">Version of the device configuration.</span></span> <span data-ttu-id="beeae-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="beeae-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beeae-155">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="beeae-155">appsBlockClipboardSharing</span></span>|<span data-ttu-id="beeae-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-156">Boolean</span></span>|<span data-ttu-id="beeae-157">Указывает, следует ли запретить совместное использование буфера обмена для копирования данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="beeae-157">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="beeae-158">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="beeae-158">appsBlockCopyPaste</span></span>|<span data-ttu-id="beeae-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-159">Boolean</span></span>|<span data-ttu-id="beeae-160">Указывает, следует ли запретить копирование данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="beeae-160">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="beeae-161">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="beeae-161">appsBlockYouTube</span></span>|<span data-ttu-id="beeae-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-162">Boolean</span></span>|<span data-ttu-id="beeae-163">Указывает, следует ли заблокировать приложение YouTube.</span><span class="sxs-lookup"><span data-stu-id="beeae-163">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="beeae-164">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="beeae-164">bluetoothBlocked</span></span>|<span data-ttu-id="beeae-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-165">Boolean</span></span>|<span data-ttu-id="beeae-166">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="beeae-166">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="beeae-167">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="beeae-167">cameraBlocked</span></span>|<span data-ttu-id="beeae-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-168">Boolean</span></span>|<span data-ttu-id="beeae-169">Указывает, следует ли запретить использовать камеру.</span><span class="sxs-lookup"><span data-stu-id="beeae-169">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="beeae-170">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="beeae-170">cellularBlockDataRoaming</span></span>|<span data-ttu-id="beeae-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-171">Boolean</span></span>|<span data-ttu-id="beeae-172">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="beeae-172">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="beeae-173">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="beeae-173">cellularBlockMessaging</span></span>|<span data-ttu-id="beeae-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-174">Boolean</span></span>|<span data-ttu-id="beeae-175">Указывает, следует ли запретить обмениваться SMS и MMS.</span><span class="sxs-lookup"><span data-stu-id="beeae-175">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="beeae-176">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="beeae-176">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="beeae-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-177">Boolean</span></span>|<span data-ttu-id="beeae-178">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="beeae-178">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="beeae-179">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="beeae-179">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="beeae-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-180">Boolean</span></span>|<span data-ttu-id="beeae-181">Указывает, следует ли блокировать синхронизацию модема Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="beeae-181">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="beeae-182">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="beeae-182">compliantAppsList</span></span>|<span data-ttu-id="beeae-183">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="beeae-183">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="beeae-184">Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="beeae-184">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="beeae-185">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="beeae-185">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="beeae-186">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="beeae-186">compliantAppListType</span></span>|[<span data-ttu-id="beeae-187">appListType</span><span class="sxs-lookup"><span data-stu-id="beeae-187">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="beeae-188">Тип списка, определенного свойством CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="beeae-188">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="beeae-189">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="beeae-189">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="beeae-190">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="beeae-190">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="beeae-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-191">Boolean</span></span>|<span data-ttu-id="beeae-192">Указывает, следует ли блокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="beeae-192">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="beeae-193">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="beeae-193">locationServicesBlocked</span></span>|<span data-ttu-id="beeae-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-194">Boolean</span></span>|<span data-ttu-id="beeae-195">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="beeae-195">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="beeae-196">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="beeae-196">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="beeae-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-197">Boolean</span></span>|<span data-ttu-id="beeae-198">Указывает, следует ли блокировать автоматическую синхронизацию учетной записи Google.</span><span class="sxs-lookup"><span data-stu-id="beeae-198">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="beeae-199">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="beeae-199">googlePlayStoreBlocked</span></span>|<span data-ttu-id="beeae-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-200">Boolean</span></span>|<span data-ttu-id="beeae-201">Указывает, следует ли блокировать Google Play Маркет.</span><span class="sxs-lookup"><span data-stu-id="beeae-201">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="beeae-202">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="beeae-202">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="beeae-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-203">Boolean</span></span>|<span data-ttu-id="beeae-204">Указывает, следует ли блокировать кнопку спящего режима экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="beeae-204">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="beeae-205">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="beeae-205">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="beeae-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-206">Boolean</span></span>|<span data-ttu-id="beeae-207">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="beeae-207">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="beeae-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="beeae-208">kioskModeApps</span></span>|<span data-ttu-id="beeae-209">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="beeae-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="beeae-210">Список разрешенных приложений в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="beeae-210">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="beeae-211">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="beeae-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="beeae-212">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="beeae-212">nfcBlocked</span></span>|<span data-ttu-id="beeae-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-213">Boolean</span></span>|<span data-ttu-id="beeae-214">Указывает, следует ли блокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="beeae-214">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="beeae-215">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="beeae-215">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="beeae-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-216">Boolean</span></span>|<span data-ttu-id="beeae-217">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="beeae-217">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="beeae-218">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="beeae-218">passwordBlockTrustAgents</span></span>|<span data-ttu-id="beeae-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-219">Boolean</span></span>|<span data-ttu-id="beeae-220">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="beeae-220">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="beeae-221">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="beeae-221">passwordExpirationDays</span></span>|<span data-ttu-id="beeae-222">Int32</span><span class="sxs-lookup"><span data-stu-id="beeae-222">Int32</span></span>|<span data-ttu-id="beeae-223">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="beeae-223">Number of days before the password expires.</span></span> <span data-ttu-id="beeae-224">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="beeae-224">Valid values 1 to 365</span></span>|
|<span data-ttu-id="beeae-225">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="beeae-225">passwordMinimumLength</span></span>|<span data-ttu-id="beeae-226">Int32</span><span class="sxs-lookup"><span data-stu-id="beeae-226">Int32</span></span>|<span data-ttu-id="beeae-227">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="beeae-227">Minimum length of passwords.</span></span> <span data-ttu-id="beeae-228">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="beeae-228">Valid values 4 to 16</span></span>|
|<span data-ttu-id="beeae-229">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="beeae-229">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="beeae-230">Int32</span><span class="sxs-lookup"><span data-stu-id="beeae-230">Int32</span></span>|<span data-ttu-id="beeae-231">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="beeae-231">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="beeae-232">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="beeae-232">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="beeae-233">Int32</span><span class="sxs-lookup"><span data-stu-id="beeae-233">Int32</span></span>|<span data-ttu-id="beeae-234">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="beeae-234">Number of previous passwords to block.</span></span> <span data-ttu-id="beeae-235">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="beeae-235">Valid values 0 to 24</span></span>|
|<span data-ttu-id="beeae-236">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="beeae-236">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="beeae-237">Int32</span><span class="sxs-lookup"><span data-stu-id="beeae-237">Int32</span></span>|<span data-ttu-id="beeae-238">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="beeae-238">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="beeae-239">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="beeae-239">Valid values 4 to 11</span></span>|
|<span data-ttu-id="beeae-240">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="beeae-240">passwordRequiredType</span></span>|[<span data-ttu-id="beeae-241">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="beeae-241">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="beeae-242">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="beeae-242">Type of password that is required.</span></span> <span data-ttu-id="beeae-243">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="beeae-243">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="beeae-244">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="beeae-244">passwordRequired</span></span>|<span data-ttu-id="beeae-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-245">Boolean</span></span>|<span data-ttu-id="beeae-246">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="beeae-246">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="beeae-247">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="beeae-247">powerOffBlocked</span></span>|<span data-ttu-id="beeae-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-248">Boolean</span></span>|<span data-ttu-id="beeae-249">Указывает, следует ли блокировать отключение устройства.</span><span class="sxs-lookup"><span data-stu-id="beeae-249">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="beeae-250">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="beeae-250">factoryResetBlocked</span></span>|<span data-ttu-id="beeae-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-251">Boolean</span></span>|<span data-ttu-id="beeae-252">Указывает, следует ли запретить пользователю восстанавливать заводские настройки.</span><span class="sxs-lookup"><span data-stu-id="beeae-252">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="beeae-253">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="beeae-253">screenCaptureBlocked</span></span>|<span data-ttu-id="beeae-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-254">Boolean</span></span>|<span data-ttu-id="beeae-255">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="beeae-255">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="beeae-256">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="beeae-256">deviceSharingAllowed</span></span>|<span data-ttu-id="beeae-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-257">Boolean</span></span>|<span data-ttu-id="beeae-258">Указывает, следует ли разрешить режим совместного доступа к устройству.</span><span class="sxs-lookup"><span data-stu-id="beeae-258">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="beeae-259">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="beeae-259">storageBlockGoogleBackup</span></span>|<span data-ttu-id="beeae-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-260">Boolean</span></span>|<span data-ttu-id="beeae-261">Указывает, следует ли блокировать резервное копирование Google.</span><span class="sxs-lookup"><span data-stu-id="beeae-261">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="beeae-262">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="beeae-262">storageBlockRemovableStorage</span></span>|<span data-ttu-id="beeae-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-263">Boolean</span></span>|<span data-ttu-id="beeae-264">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="beeae-264">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="beeae-265">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="beeae-265">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="beeae-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-266">Boolean</span></span>|<span data-ttu-id="beeae-267">Указывает, обязательно ли шифрование устройства.</span><span class="sxs-lookup"><span data-stu-id="beeae-267">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="beeae-268">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="beeae-268">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="beeae-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-269">Boolean</span></span>|<span data-ttu-id="beeae-270">Указывает, обязательно ли шифрование съемных носителей.</span><span class="sxs-lookup"><span data-stu-id="beeae-270">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="beeae-271">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="beeae-271">voiceAssistantBlocked</span></span>|<span data-ttu-id="beeae-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-272">Boolean</span></span>|<span data-ttu-id="beeae-273">Указывает, следует ли блокировать использование голосового помощника.</span><span class="sxs-lookup"><span data-stu-id="beeae-273">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="beeae-274">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="beeae-274">voiceDialingBlocked</span></span>|<span data-ttu-id="beeae-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-275">Boolean</span></span>|<span data-ttu-id="beeae-276">Указывает, следует ли блокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="beeae-276">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="beeae-277">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="beeae-277">webBrowserBlockPopups</span></span>|<span data-ttu-id="beeae-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-278">Boolean</span></span>|<span data-ttu-id="beeae-279">Указывает, следует ли блокировать всплывающие окна в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="beeae-279">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="beeae-280">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="beeae-280">webBrowserBlockAutofill</span></span>|<span data-ttu-id="beeae-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-281">Boolean</span></span>|<span data-ttu-id="beeae-282">Указывает, следует ли заблокировать функцию автозаполнения в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="beeae-282">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="beeae-283">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="beeae-283">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="beeae-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-284">Boolean</span></span>|<span data-ttu-id="beeae-285">Указывает, следует ли заблокировать JavaScript в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="beeae-285">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="beeae-286">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="beeae-286">webBrowserBlocked</span></span>|<span data-ttu-id="beeae-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-287">Boolean</span></span>|<span data-ttu-id="beeae-288">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="beeae-288">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="beeae-289">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="beeae-289">webBrowserCookieSettings</span></span>|[<span data-ttu-id="beeae-290">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="beeae-290">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="beeae-291">Настройки файлов cookie в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="beeae-291">Cookie settings within the web browser.</span></span> <span data-ttu-id="beeae-292">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="beeae-292">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="beeae-293">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="beeae-293">wiFiBlocked</span></span>|<span data-ttu-id="beeae-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-294">Boolean</span></span>|<span data-ttu-id="beeae-295">Указывает, следует ли заблокировать синхронизацию Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="beeae-295">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="beeae-296">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="beeae-296">appsInstallAllowList</span></span>|<span data-ttu-id="beeae-297">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="beeae-297">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="beeae-298">Список приложений, которые можно установить на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="beeae-298">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="beeae-299">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="beeae-299">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="beeae-300">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="beeae-300">appsLaunchBlockList</span></span>|<span data-ttu-id="beeae-301">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="beeae-301">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="beeae-302">Список приложений, которые запрещено запускать на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="beeae-302">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="beeae-303">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="beeae-303">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="beeae-304">appsHideList</span><span class="sxs-lookup"><span data-stu-id="beeae-304">appsHideList</span></span>|<span data-ttu-id="beeae-305">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="beeae-305">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="beeae-306">Список приложений, которые следует скрыть на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="beeae-306">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="beeae-307">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="beeae-307">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="beeae-308">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="beeae-308">securityRequireVerifyApps</span></span>|<span data-ttu-id="beeae-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="beeae-309">Boolean</span></span>|<span data-ttu-id="beeae-310">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="beeae-310">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="beeae-311">Ответ</span><span class="sxs-lookup"><span data-stu-id="beeae-311">Response</span></span>
<span data-ttu-id="beeae-312">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="beeae-312">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beeae-313">Пример</span><span class="sxs-lookup"><span data-stu-id="beeae-313">Example</span></span>
### <a name="request"></a><span data-ttu-id="beeae-314">Запрос</span><span class="sxs-lookup"><span data-stu-id="beeae-314">Request</span></span>
<span data-ttu-id="beeae-315">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="beeae-315">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="beeae-316">Ответ</span><span class="sxs-lookup"><span data-stu-id="beeae-316">Response</span></span>
<span data-ttu-id="beeae-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="beeae-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



