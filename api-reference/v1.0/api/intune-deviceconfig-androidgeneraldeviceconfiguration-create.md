---
title: Создание androidGeneralDeviceConfiguration
description: Создание объекта androidGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 169e0185d39d4e7a891c6a05472cb09cc9f6b201
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253486"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="39efd-103">Создание androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="39efd-103">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="39efd-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39efd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39efd-105">Создание объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39efd-105">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39efd-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="39efd-106">Prerequisites</span></span>
<span data-ttu-id="39efd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="39efd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="39efd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39efd-109">Permission type</span></span>|<span data-ttu-id="39efd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="39efd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39efd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39efd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="39efd-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39efd-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39efd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39efd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39efd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39efd-114">Not supported.</span></span>|
|<span data-ttu-id="39efd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39efd-115">Application</span></span>|<span data-ttu-id="39efd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39efd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39efd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39efd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="39efd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39efd-118">Request headers</span></span>
|<span data-ttu-id="39efd-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39efd-119">Header</span></span>|<span data-ttu-id="39efd-120">Значение</span><span class="sxs-lookup"><span data-stu-id="39efd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39efd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39efd-121">Authorization</span></span>|<span data-ttu-id="39efd-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="39efd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39efd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="39efd-123">Accept</span></span>|<span data-ttu-id="39efd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="39efd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39efd-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="39efd-125">Request body</span></span>
<span data-ttu-id="39efd-126">В теле запроса добавьте представление объекта androidGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39efd-126">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="39efd-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта androidGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="39efd-127">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="39efd-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="39efd-128">Property</span></span>|<span data-ttu-id="39efd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="39efd-129">Type</span></span>|<span data-ttu-id="39efd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="39efd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39efd-131">id</span><span class="sxs-lookup"><span data-stu-id="39efd-131">id</span></span>|<span data-ttu-id="39efd-132">String</span><span class="sxs-lookup"><span data-stu-id="39efd-132">String</span></span>|<span data-ttu-id="39efd-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="39efd-133">Key of the entity.</span></span> <span data-ttu-id="39efd-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39efd-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39efd-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39efd-135">lastModifiedDateTime</span></span>|<span data-ttu-id="39efd-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39efd-136">DateTimeOffset</span></span>|<span data-ttu-id="39efd-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="39efd-137">DateTime the object was last modified.</span></span> <span data-ttu-id="39efd-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39efd-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39efd-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39efd-139">createdDateTime</span></span>|<span data-ttu-id="39efd-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39efd-140">DateTimeOffset</span></span>|<span data-ttu-id="39efd-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="39efd-141">DateTime the object was created.</span></span> <span data-ttu-id="39efd-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39efd-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39efd-143">description</span><span class="sxs-lookup"><span data-stu-id="39efd-143">description</span></span>|<span data-ttu-id="39efd-144">String</span><span class="sxs-lookup"><span data-stu-id="39efd-144">String</span></span>|<span data-ttu-id="39efd-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="39efd-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="39efd-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39efd-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39efd-147">displayName</span><span class="sxs-lookup"><span data-stu-id="39efd-147">displayName</span></span>|<span data-ttu-id="39efd-148">String</span><span class="sxs-lookup"><span data-stu-id="39efd-148">String</span></span>|<span data-ttu-id="39efd-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="39efd-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="39efd-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39efd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39efd-151">version</span><span class="sxs-lookup"><span data-stu-id="39efd-151">version</span></span>|<span data-ttu-id="39efd-152">Int32</span><span class="sxs-lookup"><span data-stu-id="39efd-152">Int32</span></span>|<span data-ttu-id="39efd-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="39efd-153">Version of the device configuration.</span></span> <span data-ttu-id="39efd-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39efd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39efd-155">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="39efd-155">appsBlockClipboardSharing</span></span>|<span data-ttu-id="39efd-156">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-156">Boolean</span></span>|<span data-ttu-id="39efd-157">Указывает, следует ли запретить совместное использование буфера обмена для копирования данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="39efd-157">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="39efd-158">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="39efd-158">appsBlockCopyPaste</span></span>|<span data-ttu-id="39efd-159">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-159">Boolean</span></span>|<span data-ttu-id="39efd-160">Указывает, следует ли запретить копирование данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="39efd-160">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="39efd-161">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="39efd-161">appsBlockYouTube</span></span>|<span data-ttu-id="39efd-162">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-162">Boolean</span></span>|<span data-ttu-id="39efd-163">Указывает, следует ли заблокировать приложение YouTube.</span><span class="sxs-lookup"><span data-stu-id="39efd-163">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="39efd-164">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="39efd-164">bluetoothBlocked</span></span>|<span data-ttu-id="39efd-165">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-165">Boolean</span></span>|<span data-ttu-id="39efd-166">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="39efd-166">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="39efd-167">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="39efd-167">cameraBlocked</span></span>|<span data-ttu-id="39efd-168">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-168">Boolean</span></span>|<span data-ttu-id="39efd-169">Указывает, следует ли запретить использовать камеру.</span><span class="sxs-lookup"><span data-stu-id="39efd-169">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="39efd-170">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="39efd-170">cellularBlockDataRoaming</span></span>|<span data-ttu-id="39efd-171">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-171">Boolean</span></span>|<span data-ttu-id="39efd-172">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="39efd-172">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="39efd-173">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="39efd-173">cellularBlockMessaging</span></span>|<span data-ttu-id="39efd-174">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-174">Boolean</span></span>|<span data-ttu-id="39efd-175">Указывает, следует ли запретить обмениваться SMS и MMS.</span><span class="sxs-lookup"><span data-stu-id="39efd-175">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="39efd-176">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="39efd-176">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="39efd-177">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-177">Boolean</span></span>|<span data-ttu-id="39efd-178">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="39efd-178">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="39efd-179">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="39efd-179">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="39efd-180">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-180">Boolean</span></span>|<span data-ttu-id="39efd-181">Указывает, следует ли блокировать синхронизацию модема Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="39efd-181">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="39efd-182">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="39efd-182">compliantAppsList</span></span>|<span data-ttu-id="39efd-183">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="39efd-183">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="39efd-184">Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="39efd-184">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="39efd-185">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="39efd-185">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="39efd-186">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="39efd-186">compliantAppListType</span></span>|[<span data-ttu-id="39efd-187">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="39efd-187">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="39efd-188">Тип списка, определенного свойством CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="39efd-188">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="39efd-189">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="39efd-189">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="39efd-190">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="39efd-190">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="39efd-191">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-191">Boolean</span></span>|<span data-ttu-id="39efd-192">Указывает, следует ли блокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="39efd-192">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="39efd-193">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="39efd-193">locationServicesBlocked</span></span>|<span data-ttu-id="39efd-194">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-194">Boolean</span></span>|<span data-ttu-id="39efd-195">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="39efd-195">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="39efd-196">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="39efd-196">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="39efd-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="39efd-197">Boolean</span></span>|<span data-ttu-id="39efd-198">Указывает, следует ли блокировать автоматическую синхронизацию учетной записи Google.</span><span class="sxs-lookup"><span data-stu-id="39efd-198">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="39efd-199">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="39efd-199">googlePlayStoreBlocked</span></span>|<span data-ttu-id="39efd-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="39efd-200">Boolean</span></span>|<span data-ttu-id="39efd-201">Указывает, следует ли блокировать Google Play Маркет.</span><span class="sxs-lookup"><span data-stu-id="39efd-201">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="39efd-202">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="39efd-202">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="39efd-203">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-203">Boolean</span></span>|<span data-ttu-id="39efd-204">Указывает, следует ли блокировать кнопку спящего режима экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="39efd-204">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="39efd-205">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="39efd-205">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="39efd-206">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-206">Boolean</span></span>|<span data-ttu-id="39efd-207">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="39efd-207">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="39efd-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="39efd-208">kioskModeApps</span></span>|<span data-ttu-id="39efd-209">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="39efd-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="39efd-210">Список разрешенных приложений в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="39efd-210">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="39efd-211">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="39efd-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="39efd-212">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="39efd-212">nfcBlocked</span></span>|<span data-ttu-id="39efd-213">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-213">Boolean</span></span>|<span data-ttu-id="39efd-214">Указывает, следует ли блокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="39efd-214">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="39efd-215">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="39efd-215">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="39efd-216">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-216">Boolean</span></span>|<span data-ttu-id="39efd-217">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="39efd-217">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="39efd-218">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="39efd-218">passwordBlockTrustAgents</span></span>|<span data-ttu-id="39efd-219">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-219">Boolean</span></span>|<span data-ttu-id="39efd-220">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="39efd-220">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="39efd-221">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="39efd-221">passwordExpirationDays</span></span>|<span data-ttu-id="39efd-222">Int32</span><span class="sxs-lookup"><span data-stu-id="39efd-222">Int32</span></span>|<span data-ttu-id="39efd-223">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="39efd-223">Number of days before the password expires.</span></span> <span data-ttu-id="39efd-224">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="39efd-224">Valid values 1 to 365</span></span>|
|<span data-ttu-id="39efd-225">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="39efd-225">passwordMinimumLength</span></span>|<span data-ttu-id="39efd-226">Int32</span><span class="sxs-lookup"><span data-stu-id="39efd-226">Int32</span></span>|<span data-ttu-id="39efd-227">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="39efd-227">Minimum length of passwords.</span></span> <span data-ttu-id="39efd-228">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="39efd-228">Valid values 4 to 16</span></span>|
|<span data-ttu-id="39efd-229">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="39efd-229">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="39efd-230">Int32</span><span class="sxs-lookup"><span data-stu-id="39efd-230">Int32</span></span>|<span data-ttu-id="39efd-231">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="39efd-231">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="39efd-232">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="39efd-232">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="39efd-233">Int32</span><span class="sxs-lookup"><span data-stu-id="39efd-233">Int32</span></span>|<span data-ttu-id="39efd-234">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="39efd-234">Number of previous passwords to block.</span></span> <span data-ttu-id="39efd-235">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="39efd-235">Valid values 0 to 24</span></span>|
|<span data-ttu-id="39efd-236">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="39efd-236">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="39efd-237">Int32</span><span class="sxs-lookup"><span data-stu-id="39efd-237">Int32</span></span>|<span data-ttu-id="39efd-238">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="39efd-238">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="39efd-239">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="39efd-239">Valid values 1 to 16</span></span>|
|<span data-ttu-id="39efd-240">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="39efd-240">passwordRequiredType</span></span>|[<span data-ttu-id="39efd-241">Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="39efd-241">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="39efd-242">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="39efd-242">Type of password that is required.</span></span> <span data-ttu-id="39efd-243">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="39efd-243">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="39efd-244">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="39efd-244">passwordRequired</span></span>|<span data-ttu-id="39efd-245">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-245">Boolean</span></span>|<span data-ttu-id="39efd-246">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="39efd-246">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="39efd-247">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="39efd-247">powerOffBlocked</span></span>|<span data-ttu-id="39efd-248">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-248">Boolean</span></span>|<span data-ttu-id="39efd-249">Указывает, следует ли блокировать отключение устройства.</span><span class="sxs-lookup"><span data-stu-id="39efd-249">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="39efd-250">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="39efd-250">factoryResetBlocked</span></span>|<span data-ttu-id="39efd-251">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-251">Boolean</span></span>|<span data-ttu-id="39efd-252">Указывает, следует ли запретить пользователю восстанавливать заводские настройки.</span><span class="sxs-lookup"><span data-stu-id="39efd-252">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="39efd-253">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="39efd-253">screenCaptureBlocked</span></span>|<span data-ttu-id="39efd-254">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-254">Boolean</span></span>|<span data-ttu-id="39efd-255">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="39efd-255">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="39efd-256">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="39efd-256">deviceSharingAllowed</span></span>|<span data-ttu-id="39efd-257">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-257">Boolean</span></span>|<span data-ttu-id="39efd-258">Указывает, следует ли разрешить режим совместного доступа к устройству.</span><span class="sxs-lookup"><span data-stu-id="39efd-258">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="39efd-259">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="39efd-259">storageBlockGoogleBackup</span></span>|<span data-ttu-id="39efd-260">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-260">Boolean</span></span>|<span data-ttu-id="39efd-261">Указывает, следует ли блокировать резервное копирование Google.</span><span class="sxs-lookup"><span data-stu-id="39efd-261">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="39efd-262">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="39efd-262">storageBlockRemovableStorage</span></span>|<span data-ttu-id="39efd-263">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-263">Boolean</span></span>|<span data-ttu-id="39efd-264">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="39efd-264">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="39efd-265">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="39efd-265">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="39efd-266">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-266">Boolean</span></span>|<span data-ttu-id="39efd-267">Указывает, обязательно ли шифрование устройства.</span><span class="sxs-lookup"><span data-stu-id="39efd-267">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="39efd-268">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="39efd-268">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="39efd-269">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-269">Boolean</span></span>|<span data-ttu-id="39efd-270">Указывает, обязательно ли шифрование съемных носителей.</span><span class="sxs-lookup"><span data-stu-id="39efd-270">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="39efd-271">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="39efd-271">voiceAssistantBlocked</span></span>|<span data-ttu-id="39efd-272">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-272">Boolean</span></span>|<span data-ttu-id="39efd-273">Указывает, следует ли блокировать использование голосового помощника.</span><span class="sxs-lookup"><span data-stu-id="39efd-273">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="39efd-274">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="39efd-274">voiceDialingBlocked</span></span>|<span data-ttu-id="39efd-275">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-275">Boolean</span></span>|<span data-ttu-id="39efd-276">Указывает, следует ли блокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="39efd-276">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="39efd-277">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="39efd-277">webBrowserBlockPopups</span></span>|<span data-ttu-id="39efd-278">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-278">Boolean</span></span>|<span data-ttu-id="39efd-279">Указывает, следует ли блокировать всплывающие окна в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="39efd-279">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="39efd-280">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="39efd-280">webBrowserBlockAutofill</span></span>|<span data-ttu-id="39efd-281">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-281">Boolean</span></span>|<span data-ttu-id="39efd-282">Указывает, следует ли заблокировать функцию автозаполнения в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="39efd-282">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="39efd-283">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="39efd-283">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="39efd-284">Логический</span><span class="sxs-lookup"><span data-stu-id="39efd-284">Boolean</span></span>|<span data-ttu-id="39efd-285">Указывает, следует ли заблокировать JavaScript в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="39efd-285">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="39efd-286">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="39efd-286">webBrowserBlocked</span></span>|<span data-ttu-id="39efd-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="39efd-287">Boolean</span></span>|<span data-ttu-id="39efd-288">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="39efd-288">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="39efd-289">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="39efd-289">webBrowserCookieSettings</span></span>|[<span data-ttu-id="39efd-290">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="39efd-290">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="39efd-291">Настройки файлов cookie в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="39efd-291">Cookie settings within the web browser.</span></span> <span data-ttu-id="39efd-292">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="39efd-292">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="39efd-293">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="39efd-293">wiFiBlocked</span></span>|<span data-ttu-id="39efd-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="39efd-294">Boolean</span></span>|<span data-ttu-id="39efd-295">Указывает, следует ли заблокировать синхронизацию Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="39efd-295">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="39efd-296">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="39efd-296">appsInstallAllowList</span></span>|<span data-ttu-id="39efd-297">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="39efd-297">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="39efd-298">Список приложений, которые можно установить на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="39efd-298">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="39efd-299">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="39efd-299">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="39efd-300">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="39efd-300">appsLaunchBlockList</span></span>|<span data-ttu-id="39efd-301">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="39efd-301">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="39efd-302">Список приложений, которые запрещено запускать на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="39efd-302">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="39efd-303">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="39efd-303">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="39efd-304">appsHideList</span><span class="sxs-lookup"><span data-stu-id="39efd-304">appsHideList</span></span>|<span data-ttu-id="39efd-305">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="39efd-305">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="39efd-306">Список приложений, которые следует скрыть на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="39efd-306">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="39efd-307">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="39efd-307">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="39efd-308">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="39efd-308">securityRequireVerifyApps</span></span>|<span data-ttu-id="39efd-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="39efd-309">Boolean</span></span>|<span data-ttu-id="39efd-310">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="39efd-310">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="39efd-311">Отклик</span><span class="sxs-lookup"><span data-stu-id="39efd-311">Response</span></span>
<span data-ttu-id="39efd-312">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="39efd-312">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39efd-313">Пример</span><span class="sxs-lookup"><span data-stu-id="39efd-313">Example</span></span>

### <a name="request"></a><span data-ttu-id="39efd-314">Запрос</span><span class="sxs-lookup"><span data-stu-id="39efd-314">Request</span></span>
<span data-ttu-id="39efd-315">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39efd-315">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="39efd-316">Ответ</span><span class="sxs-lookup"><span data-stu-id="39efd-316">Response</span></span>
<span data-ttu-id="39efd-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39efd-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



