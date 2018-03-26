# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="4c537-101">Создание androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c537-101">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="4c537-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4c537-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c537-103">Создание объекта [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c537-103">Create a new [plannerBucket](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c537-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4c537-104">Prerequisites</span></span>
<span data-ttu-id="4c537-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4c537-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4c537-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c537-107">Permission type</span></span>|<span data-ttu-id="4c537-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c537-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c537-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c537-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4c537-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c537-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c537-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c537-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c537-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c537-112">Not supported.</span></span>|
|<span data-ttu-id="4c537-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c537-113">Application</span></span>|<span data-ttu-id="4c537-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c537-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c537-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c537-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4c537-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4c537-116">Request headers</span></span>
|<span data-ttu-id="4c537-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c537-117">Header</span></span>|<span data-ttu-id="4c537-118">Значение</span><span class="sxs-lookup"><span data-stu-id="4c537-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c537-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c537-119">Authorization</span></span>|<span data-ttu-id="4c537-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c537-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4c537-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4c537-121">Accept</span></span>|<span data-ttu-id="4c537-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4c537-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c537-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c537-123">Request body</span></span>
<span data-ttu-id="4c537-124">В теле запроса добавьте представление объекта androidGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c537-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="4c537-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта androidGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4c537-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="4c537-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c537-126">Property</span></span>|<span data-ttu-id="4c537-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4c537-127">Type</span></span>|<span data-ttu-id="4c537-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4c537-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c537-129">id</span><span class="sxs-lookup"><span data-stu-id="4c537-129">id</span></span>|<span data-ttu-id="4c537-130">String</span><span class="sxs-lookup"><span data-stu-id="4c537-130">String</span></span>|<span data-ttu-id="4c537-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4c537-131">Key of the setting.</span></span> <span data-ttu-id="4c537-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c537-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c537-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c537-133">lastModifiedDateTime</span></span>|<span data-ttu-id="4c537-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c537-134">DateTimeOffset</span></span>|<span data-ttu-id="4c537-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4c537-135">DateTime the object was last modified.</span></span> <span data-ttu-id="4c537-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c537-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c537-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c537-137">createdDateTime</span></span>|<span data-ttu-id="4c537-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c537-138">DateTimeOffset</span></span>|<span data-ttu-id="4c537-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4c537-139">DateTime the object was created.</span></span> <span data-ttu-id="4c537-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c537-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c537-141">description</span><span class="sxs-lookup"><span data-stu-id="4c537-141">description</span></span>|<span data-ttu-id="4c537-142">String</span><span class="sxs-lookup"><span data-stu-id="4c537-142">String</span></span>|<span data-ttu-id="4c537-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4c537-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4c537-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c537-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c537-145">displayName</span><span class="sxs-lookup"><span data-stu-id="4c537-145">displayName</span></span>|<span data-ttu-id="4c537-146">String</span><span class="sxs-lookup"><span data-stu-id="4c537-146">String</span></span>|<span data-ttu-id="4c537-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4c537-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4c537-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c537-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c537-149">version</span><span class="sxs-lookup"><span data-stu-id="4c537-149">version</span></span>|<span data-ttu-id="4c537-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4c537-150">Int32</span></span>|<span data-ttu-id="4c537-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4c537-151">Version of the device configuration.</span></span> <span data-ttu-id="4c537-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c537-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c537-153">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="4c537-153">appsBlockClipboardSharing</span></span>|<span data-ttu-id="4c537-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-154">Boolean</span></span>|<span data-ttu-id="4c537-155">Указывает, следует ли запретить совместное использование буфера обмена для копирования данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="4c537-155">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="4c537-156">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="4c537-156">appsBlockCopyPaste</span></span>|<span data-ttu-id="4c537-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-157">Boolean</span></span>|<span data-ttu-id="4c537-158">Указывает, следует ли запретить копирование данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="4c537-158">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="4c537-159">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="4c537-159">appsBlockYouTube</span></span>|<span data-ttu-id="4c537-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-160">Boolean</span></span>|<span data-ttu-id="4c537-161">Указывает, следует ли заблокировать приложение YouTube.</span><span class="sxs-lookup"><span data-stu-id="4c537-161">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="4c537-162">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="4c537-162">bluetoothBlocked</span></span>|<span data-ttu-id="4c537-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-163">Boolean</span></span>|<span data-ttu-id="4c537-164">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="4c537-164">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="4c537-165">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="4c537-165">cameraBlocked</span></span>|<span data-ttu-id="4c537-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-166">Boolean</span></span>|<span data-ttu-id="4c537-167">Указывает, следует ли запретить использовать камеру.</span><span class="sxs-lookup"><span data-stu-id="4c537-167">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="4c537-168">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="4c537-168">cellularBlockDataRoaming</span></span>|<span data-ttu-id="4c537-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-169">Boolean</span></span>|<span data-ttu-id="4c537-170">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="4c537-170">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="4c537-171">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="4c537-171">cellularBlockMessaging</span></span>|<span data-ttu-id="4c537-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-172">Boolean</span></span>|<span data-ttu-id="4c537-173">Указывает, следует ли запретить обмениваться SMS и MMS.</span><span class="sxs-lookup"><span data-stu-id="4c537-173">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="4c537-174">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="4c537-174">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="4c537-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-175">Boolean</span></span>|<span data-ttu-id="4c537-176">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="4c537-176">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="4c537-177">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="4c537-177">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="4c537-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-178">Boolean</span></span>|<span data-ttu-id="4c537-179">Указывает, следует ли заблокировать синхронизацию модема Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="4c537-179">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="4c537-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="4c537-180">compliantAppsList</span></span>|<span data-ttu-id="4c537-181">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="4c537-181">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="4c537-182">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="4c537-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="4c537-183">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="4c537-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="4c537-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="4c537-184">compliantAppListType</span></span>|<span data-ttu-id="4c537-185">String</span><span class="sxs-lookup"><span data-stu-id="4c537-185">String</span></span>|<span data-ttu-id="4c537-186">Тип списка, определенного свойством CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="4c537-186">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="4c537-187">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="4c537-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="4c537-188">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="4c537-188">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="4c537-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-189">Boolean</span></span>|<span data-ttu-id="4c537-190">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="4c537-190">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="4c537-191">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="4c537-191">locationServicesBlocked</span></span>|<span data-ttu-id="4c537-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-192">Boolean</span></span>|<span data-ttu-id="4c537-193">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="4c537-193">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="4c537-194">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="4c537-194">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="4c537-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-195">Boolean</span></span>|<span data-ttu-id="4c537-196">Указывает, следует ли заблокировать автоматическую синхронизацию учетной записи Google.</span><span class="sxs-lookup"><span data-stu-id="4c537-196">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="4c537-197">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="4c537-197">googlePlayStoreBlocked</span></span>|<span data-ttu-id="4c537-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-198">Boolean</span></span>|<span data-ttu-id="4c537-199">Указывает, следует ли заблокировать Google Play Маркет.</span><span class="sxs-lookup"><span data-stu-id="4c537-199">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="4c537-200">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="4c537-200">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="4c537-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-201">Boolean</span></span>|<span data-ttu-id="4c537-202">Указывает, следует ли заблокировать кнопку спящего режима экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="4c537-202">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="4c537-203">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="4c537-203">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="4c537-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-204">Boolean</span></span>|<span data-ttu-id="4c537-205">Указывает, следует ли заблокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="4c537-205">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="4c537-206">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="4c537-206">kioskModeApps</span></span>|<span data-ttu-id="4c537-207">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="4c537-207">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="4c537-208">Список разрешенных приложений в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="4c537-208">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="4c537-209">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4c537-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4c537-210">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="4c537-210">nfcBlocked</span></span>|<span data-ttu-id="4c537-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-211">Boolean</span></span>|<span data-ttu-id="4c537-212">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="4c537-212">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="4c537-213">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="4c537-213">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="4c537-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-214">Boolean</span></span>|<span data-ttu-id="4c537-215">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="4c537-215">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="4c537-216">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="4c537-216">passwordBlockTrustAgents</span></span>|<span data-ttu-id="4c537-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-217">Boolean</span></span>|<span data-ttu-id="4c537-218">Указывает, следует ли заблокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="4c537-218">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="4c537-219">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4c537-219">passwordExpirationDays</span></span>|<span data-ttu-id="4c537-220">Int32</span><span class="sxs-lookup"><span data-stu-id="4c537-220">Int32</span></span>|<span data-ttu-id="4c537-221">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="4c537-221">Number of days before the password expires.</span></span> <span data-ttu-id="4c537-222">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="4c537-222">Valid values 1 to 365</span></span>|
|<span data-ttu-id="4c537-223">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4c537-223">passwordMinimumLength</span></span>|<span data-ttu-id="4c537-224">Int32</span><span class="sxs-lookup"><span data-stu-id="4c537-224">Int32</span></span>|<span data-ttu-id="4c537-225">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="4c537-225">Minimum length of passwords.</span></span> <span data-ttu-id="4c537-226">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="4c537-226">Valid values 4 to 16</span></span>|
|<span data-ttu-id="4c537-227">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4c537-227">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4c537-228">Int32</span><span class="sxs-lookup"><span data-stu-id="4c537-228">Int32</span></span>|<span data-ttu-id="4c537-229">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="4c537-229">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="4c537-230">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4c537-230">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4c537-231">Int32</span><span class="sxs-lookup"><span data-stu-id="4c537-231">Int32</span></span>|<span data-ttu-id="4c537-232">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="4c537-232">Number of previous passwords to block.</span></span> <span data-ttu-id="4c537-233">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="4c537-233">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4c537-234">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4c537-234">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4c537-235">Int32</span><span class="sxs-lookup"><span data-stu-id="4c537-235">Int32</span></span>|<span data-ttu-id="4c537-236">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="4c537-236">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="4c537-237">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="4c537-237">Valid values 4 to 11</span></span>|
|<span data-ttu-id="4c537-238">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4c537-238">passwordRequiredType</span></span>|<span data-ttu-id="4c537-239">String</span><span class="sxs-lookup"><span data-stu-id="4c537-239">String</span></span>|<span data-ttu-id="4c537-240">Необходимый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="4c537-240">Type of password that is required.</span></span> <span data-ttu-id="4c537-241">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="4c537-241">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`.</span></span>|
|<span data-ttu-id="4c537-242">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4c537-242">passwordRequired</span></span>|<span data-ttu-id="4c537-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-243">Boolean</span></span>|<span data-ttu-id="4c537-244">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="4c537-244">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="4c537-245">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="4c537-245">powerOffBlocked</span></span>|<span data-ttu-id="4c537-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-246">Boolean</span></span>|<span data-ttu-id="4c537-247">Указывает, следует ли заблокировать отключение устройства.</span><span class="sxs-lookup"><span data-stu-id="4c537-247">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="4c537-248">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="4c537-248">factoryResetBlocked</span></span>|<span data-ttu-id="4c537-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-249">Boolean</span></span>|<span data-ttu-id="4c537-250">Указывает, следует ли запретить пользователю восстанавливать заводские настройки.</span><span class="sxs-lookup"><span data-stu-id="4c537-250">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="4c537-251">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="4c537-251">screenCaptureBlocked</span></span>|<span data-ttu-id="4c537-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-252">Boolean</span></span>|<span data-ttu-id="4c537-253">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="4c537-253">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="4c537-254">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="4c537-254">deviceSharingAllowed</span></span>|<span data-ttu-id="4c537-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-255">Boolean</span></span>|<span data-ttu-id="4c537-256">Указывает, следует ли разрешить режим совместного доступа к устройству.</span><span class="sxs-lookup"><span data-stu-id="4c537-256">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="4c537-257">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="4c537-257">storageBlockGoogleBackup</span></span>|<span data-ttu-id="4c537-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-258">Boolean</span></span>|<span data-ttu-id="4c537-259">Указывает, следует ли заблокировать Автозагрузку Google.</span><span class="sxs-lookup"><span data-stu-id="4c537-259">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="4c537-260">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="4c537-260">storageBlockRemovableStorage</span></span>|<span data-ttu-id="4c537-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-261">Boolean</span></span>|<span data-ttu-id="4c537-262">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="4c537-262">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="4c537-263">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="4c537-263">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="4c537-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-264">Boolean</span></span>|<span data-ttu-id="4c537-265">Указывает, обязательно ли шифрование устройства.</span><span class="sxs-lookup"><span data-stu-id="4c537-265">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="4c537-266">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="4c537-266">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="4c537-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-267">Boolean</span></span>|<span data-ttu-id="4c537-268">Указывает, обязательно ли шифрование съемных носителей.</span><span class="sxs-lookup"><span data-stu-id="4c537-268">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="4c537-269">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="4c537-269">voiceAssistantBlocked</span></span>|<span data-ttu-id="4c537-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-270">Boolean</span></span>|<span data-ttu-id="4c537-271">Указывает, следует ли заблокировать голосовой помощник.</span><span class="sxs-lookup"><span data-stu-id="4c537-271">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="4c537-272">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="4c537-272">voiceDialingBlocked</span></span>|<span data-ttu-id="4c537-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-273">Boolean</span></span>|<span data-ttu-id="4c537-274">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="4c537-274">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="4c537-275">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="4c537-275">webBrowserBlockPopups</span></span>|<span data-ttu-id="4c537-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-276">Boolean</span></span>|<span data-ttu-id="4c537-277">Указывает, следует ли блокировать всплывающие окна в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="4c537-277">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="4c537-278">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="4c537-278">webBrowserBlockAutofill</span></span>|<span data-ttu-id="4c537-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-279">Boolean</span></span>|<span data-ttu-id="4c537-280">Указывает, следует ли заблокировать функцию автозаполнения в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="4c537-280">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="4c537-281">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="4c537-281">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="4c537-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-282">Boolean</span></span>|<span data-ttu-id="4c537-283">Указывает, следует ли заблокировать JavaScript в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="4c537-283">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="4c537-284">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="4c537-284">webBrowserBlocked</span></span>|<span data-ttu-id="4c537-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-285">Boolean</span></span>|<span data-ttu-id="4c537-286">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="4c537-286">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="4c537-287">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="4c537-287">webBrowserCookieSettings</span></span>|<span data-ttu-id="4c537-288">String</span><span class="sxs-lookup"><span data-stu-id="4c537-288">String</span></span>|<span data-ttu-id="4c537-289">Настройки файлов cookie в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="4c537-289">Cookie settings within the web browser.</span></span> <span data-ttu-id="4c537-290">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="4c537-290">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="4c537-291">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="4c537-291">wiFiBlocked</span></span>|<span data-ttu-id="4c537-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-292">Boolean</span></span>|<span data-ttu-id="4c537-293">Указывает, следует ли заблокировать синхронизацию Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="4c537-293">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="4c537-294">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="4c537-294">appsInstallAllowList</span></span>|<span data-ttu-id="4c537-295">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="4c537-295">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="4c537-296">Список приложений, которые можно установить на устройства KNOX.</span><span class="sxs-lookup"><span data-stu-id="4c537-296">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="4c537-297">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4c537-297">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4c537-298">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="4c537-298">appsLaunchBlockList</span></span>|<span data-ttu-id="4c537-299">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="4c537-299">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="4c537-300">Список приложений, которые нельзя запускать на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="4c537-300">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="4c537-301">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4c537-301">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4c537-302">appsHideList</span><span class="sxs-lookup"><span data-stu-id="4c537-302">appsHideList</span></span>|<span data-ttu-id="4c537-303">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="4c537-303">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="4c537-304">Список приложений, которые следует скрыть на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="4c537-304">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="4c537-305">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4c537-305">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4c537-306">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="4c537-306">securityRequireVerifyApps</span></span>|<span data-ttu-id="4c537-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c537-307">Boolean</span></span>|<span data-ttu-id="4c537-308">Требует включения функции Android "Проверка приложений".</span><span class="sxs-lookup"><span data-stu-id="4c537-308">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="4c537-309">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c537-309">Response</span></span>
<span data-ttu-id="4c537-310">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4c537-310">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c537-311">Пример</span><span class="sxs-lookup"><span data-stu-id="4c537-311">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c537-312">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c537-312">Request</span></span>
<span data-ttu-id="4c537-313">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c537-313">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3097

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="4c537-314">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c537-314">Response</span></span>
<span data-ttu-id="4c537-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4c537-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



