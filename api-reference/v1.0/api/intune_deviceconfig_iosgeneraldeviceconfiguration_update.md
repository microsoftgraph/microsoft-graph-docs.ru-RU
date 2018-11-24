# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="572d4-101">Обновление объекта iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="572d4-101">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="572d4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="572d4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="572d4-103">Обновление свойств объекта [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="572d4-103">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="572d4-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="572d4-104">Prerequisites</span></span>
<span data-ttu-id="572d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="572d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="572d4-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="572d4-107">Permission type</span></span>|<span data-ttu-id="572d4-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="572d4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="572d4-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="572d4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="572d4-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="572d4-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="572d4-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="572d4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="572d4-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="572d4-112">Not supported.</span></span>|
|<span data-ttu-id="572d4-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="572d4-113">Application</span></span>|<span data-ttu-id="572d4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="572d4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="572d4-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="572d4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="572d4-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="572d4-116">Request headers</span></span>
|<span data-ttu-id="572d4-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="572d4-117">Header</span></span>|<span data-ttu-id="572d4-118">Значение</span><span class="sxs-lookup"><span data-stu-id="572d4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="572d4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="572d4-119">Authorization</span></span>|<span data-ttu-id="572d4-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="572d4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="572d4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="572d4-121">Accept</span></span>|<span data-ttu-id="572d4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="572d4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="572d4-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="572d4-123">Request body</span></span>
<span data-ttu-id="572d4-124">В тексте запроса добавьте представление объекта [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="572d4-124">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="572d4-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="572d4-125">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="572d4-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="572d4-126">Property</span></span>|<span data-ttu-id="572d4-127">Тип</span><span class="sxs-lookup"><span data-stu-id="572d4-127">Type</span></span>|<span data-ttu-id="572d4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="572d4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="572d4-129">id</span><span class="sxs-lookup"><span data-stu-id="572d4-129">id</span></span>|<span data-ttu-id="572d4-130">String</span><span class="sxs-lookup"><span data-stu-id="572d4-130">String</span></span>|<span data-ttu-id="572d4-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="572d4-131">Key of the entity.</span></span> <span data-ttu-id="572d4-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="572d4-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="572d4-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="572d4-133">lastModifiedDateTime</span></span>|<span data-ttu-id="572d4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="572d4-134">DateTimeOffset</span></span>|<span data-ttu-id="572d4-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="572d4-135">DateTime the object was last modified.</span></span> <span data-ttu-id="572d4-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="572d4-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="572d4-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="572d4-137">createdDateTime</span></span>|<span data-ttu-id="572d4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="572d4-138">DateTimeOffset</span></span>|<span data-ttu-id="572d4-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="572d4-139">DateTime the object was created.</span></span> <span data-ttu-id="572d4-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="572d4-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="572d4-141">description</span><span class="sxs-lookup"><span data-stu-id="572d4-141">description</span></span>|<span data-ttu-id="572d4-142">String</span><span class="sxs-lookup"><span data-stu-id="572d4-142">String</span></span>|<span data-ttu-id="572d4-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="572d4-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="572d4-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="572d4-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="572d4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="572d4-145">displayName</span></span>|<span data-ttu-id="572d4-146">String</span><span class="sxs-lookup"><span data-stu-id="572d4-146">String</span></span>|<span data-ttu-id="572d4-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="572d4-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="572d4-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="572d4-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="572d4-149">version</span><span class="sxs-lookup"><span data-stu-id="572d4-149">version</span></span>|<span data-ttu-id="572d4-150">Int32</span><span class="sxs-lookup"><span data-stu-id="572d4-150">Int32</span></span>|<span data-ttu-id="572d4-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="572d4-151">Version of the device configuration.</span></span> <span data-ttu-id="572d4-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="572d4-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="572d4-153">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="572d4-153">accountBlockModification</span></span>|<span data-ttu-id="572d4-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-154">Boolean</span></span>|<span data-ttu-id="572d4-155">Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-155">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="572d4-156">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="572d4-156">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="572d4-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-157">Boolean</span></span>|<span data-ttu-id="572d4-158">Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-158">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="572d4-159">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-159">airDropBlocked</span></span>|<span data-ttu-id="572d4-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-160">Boolean</span></span>|<span data-ttu-id="572d4-161">Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-161">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="572d4-162">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="572d4-162">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="572d4-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-163">Boolean</span></span>|<span data-ttu-id="572d4-164">Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-164">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="572d4-165">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="572d4-165">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="572d4-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-166">Boolean</span></span>|<span data-ttu-id="572d4-167">Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.</span><span class="sxs-lookup"><span data-stu-id="572d4-167">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="572d4-168">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="572d4-168">appleWatchBlockPairing</span></span>|<span data-ttu-id="572d4-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-169">Boolean</span></span>|<span data-ttu-id="572d4-170">Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-170">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="572d4-171">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="572d4-171">appleWatchForceWristDetection</span></span>|<span data-ttu-id="572d4-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-172">Boolean</span></span>|<span data-ttu-id="572d4-173">Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-173">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="572d4-174">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-174">appleNewsBlocked</span></span>|<span data-ttu-id="572d4-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-175">Boolean</span></span>|<span data-ttu-id="572d4-176">Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-176">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="572d4-177">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="572d4-177">appsSingleAppModeList</span></span>|<span data-ttu-id="572d4-178">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="572d4-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="572d4-179">Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы.</span><span class="sxs-lookup"><span data-stu-id="572d4-179">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="572d4-180">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-180">Supervised only.</span></span> <span data-ttu-id="572d4-181">iOS 7.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="572d4-181">iOS 7.0 and later.</span></span> <span data-ttu-id="572d4-182">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="572d4-182">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="572d4-183">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="572d4-183">appsVisibilityList</span></span>|<span data-ttu-id="572d4-184">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="572d4-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="572d4-185">Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-185">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="572d4-186">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="572d4-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="572d4-187">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="572d4-187">appsVisibilityListType</span></span>|[<span data-ttu-id="572d4-188">appListType</span><span class="sxs-lookup"><span data-stu-id="572d4-188">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="572d4-189">Тип списка, определенного свойством AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="572d4-189">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="572d4-190">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="572d4-190">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="572d4-191">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="572d4-191">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="572d4-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-192">Boolean</span></span>|<span data-ttu-id="572d4-193">Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-193">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="572d4-194">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-194">appStoreBlocked</span></span>|<span data-ttu-id="572d4-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-195">Boolean</span></span>|<span data-ttu-id="572d4-196">Указывает, следует ли запретить использовать App Store.</span><span class="sxs-lookup"><span data-stu-id="572d4-196">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="572d4-197">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="572d4-197">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="572d4-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-198">Boolean</span></span>|<span data-ttu-id="572d4-199">Указывает, следует ли запретить пользователю совершать покупки из приложения.</span><span class="sxs-lookup"><span data-stu-id="572d4-199">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="572d4-200">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="572d4-200">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="572d4-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-201">Boolean</span></span>|<span data-ttu-id="572d4-202">Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения.</span><span class="sxs-lookup"><span data-stu-id="572d4-202">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="572d4-203">Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-203">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="572d4-204">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="572d4-204">appStoreRequirePassword</span></span>|<span data-ttu-id="572d4-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-205">Boolean</span></span>|<span data-ttu-id="572d4-206">Указывает, требуется ли пароль, когда вы используете приложение App Store.</span><span class="sxs-lookup"><span data-stu-id="572d4-206">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="572d4-207">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="572d4-207">bluetoothBlockModification</span></span>|<span data-ttu-id="572d4-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-208">Boolean</span></span>|<span data-ttu-id="572d4-209">Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-209">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="572d4-210">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-210">cameraBlocked</span></span>|<span data-ttu-id="572d4-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-211">Boolean</span></span>|<span data-ttu-id="572d4-212">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="572d4-212">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="572d4-213">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="572d4-213">cellularBlockDataRoaming</span></span>|<span data-ttu-id="572d4-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-214">Boolean</span></span>|<span data-ttu-id="572d4-215">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="572d4-215">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="572d4-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="572d4-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="572d4-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-217">Boolean</span></span>|<span data-ttu-id="572d4-218">Указывает, следует ли заблокировать получение фоновых данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="572d4-218">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="572d4-219">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="572d4-219">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="572d4-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-220">Boolean</span></span>|<span data-ttu-id="572d4-221">Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-221">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="572d4-222">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="572d4-222">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="572d4-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-223">Boolean</span></span>|<span data-ttu-id="572d4-224">Указывает, следует ли заблокировать личный хот-спот.</span><span class="sxs-lookup"><span data-stu-id="572d4-224">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="572d4-225">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="572d4-225">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="572d4-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-226">Boolean</span></span>|<span data-ttu-id="572d4-227">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="572d4-227">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="572d4-228">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="572d4-228">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="572d4-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-229">Boolean</span></span>|<span data-ttu-id="572d4-230">Указывает, следует ли заблокировать ненадежные сертификаты TLS.</span><span class="sxs-lookup"><span data-stu-id="572d4-230">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="572d4-231">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="572d4-231">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="572d4-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-232">Boolean</span></span>|<span data-ttu-id="572d4-233">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-233">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="572d4-234">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="572d4-234">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="572d4-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-235">Boolean</span></span>|<span data-ttu-id="572d4-236">Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-236">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="572d4-237">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="572d4-237">compliantAppsList</span></span>|<span data-ttu-id="572d4-238">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="572d4-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="572d4-239">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="572d4-239">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="572d4-240">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="572d4-240">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="572d4-241">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="572d4-241">compliantAppListType</span></span>|[<span data-ttu-id="572d4-242">appListType</span><span class="sxs-lookup"><span data-stu-id="572d4-242">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="572d4-243">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="572d4-243">List that is in the AppComplianceList.</span></span> <span data-ttu-id="572d4-244">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="572d4-244">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="572d4-245">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="572d4-245">configurationProfileBlockChanges</span></span>|<span data-ttu-id="572d4-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-246">Boolean</span></span>|<span data-ttu-id="572d4-247">Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-247">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="572d4-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-248">definitionLookupBlocked</span></span>|<span data-ttu-id="572d4-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-249">Boolean</span></span>|<span data-ttu-id="572d4-250">Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-250">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="572d4-251">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="572d4-251">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="572d4-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-252">Boolean</span></span>|<span data-ttu-id="572d4-253">Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-253">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="572d4-254">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="572d4-254">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="572d4-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-255">Boolean</span></span>|<span data-ttu-id="572d4-256">Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-256">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="572d4-257">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="572d4-257">deviceBlockNameModification</span></span>|<span data-ttu-id="572d4-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-258">Boolean</span></span>|<span data-ttu-id="572d4-259">Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-259">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="572d4-260">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="572d4-260">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="572d4-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-261">Boolean</span></span>|<span data-ttu-id="572d4-262">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="572d4-262">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="572d4-263">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="572d4-263">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="572d4-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-264">Boolean</span></span>|<span data-ttu-id="572d4-265">Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-265">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="572d4-266">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="572d4-266">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="572d4-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-267">Boolean</span></span>|<span data-ttu-id="572d4-268">Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="572d4-268">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="572d4-269">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="572d4-269">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="572d4-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-270">Boolean</span></span>|<span data-ttu-id="572d4-271">Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="572d4-271">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="572d4-272">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="572d4-272">emailInDomainSuffixes</span></span>|<span data-ttu-id="572d4-273">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="572d4-273">String collection</span></span>|<span data-ttu-id="572d4-274">Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.</span><span class="sxs-lookup"><span data-stu-id="572d4-274">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="572d4-275">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="572d4-275">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="572d4-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-276">Boolean</span></span>|<span data-ttu-id="572d4-277">Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="572d4-277">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="572d4-278">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="572d4-278">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="572d4-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-279">Boolean</span></span>|<span data-ttu-id="572d4-280">Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="572d4-280">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="572d4-281">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-281">faceTimeBlocked</span></span>|<span data-ttu-id="572d4-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-282">Boolean</span></span>|<span data-ttu-id="572d4-283">Указывает, следует ли запретить использовать FaceTime.</span><span class="sxs-lookup"><span data-stu-id="572d4-283">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="572d4-284">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-284">findMyFriendsBlocked</span></span>|<span data-ttu-id="572d4-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-285">Boolean</span></span>|<span data-ttu-id="572d4-286">Указывает, следует ли заблокировать функцию "Найти друзей", когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-286">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="572d4-287">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="572d4-287">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="572d4-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-288">Boolean</span></span>|<span data-ttu-id="572d4-289">Указывает, следует ли запретить пользователю добавлять друзей в Game Center.</span><span class="sxs-lookup"><span data-stu-id="572d4-289">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="572d4-290">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="572d4-290">gamingBlockMultiplayer</span></span>|<span data-ttu-id="572d4-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-291">Boolean</span></span>|<span data-ttu-id="572d4-292">Указывает, следует ли запретить пользователю играть с несколькими игроками.</span><span class="sxs-lookup"><span data-stu-id="572d4-292">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="572d4-293">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-293">gameCenterBlocked</span></span>|<span data-ttu-id="572d4-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-294">Boolean</span></span>|<span data-ttu-id="572d4-295">Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-295">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="572d4-296">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-296">hostPairingBlocked</span></span>|<span data-ttu-id="572d4-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-297">Boolean</span></span>|<span data-ttu-id="572d4-298">Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-298">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="572d4-299">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-299">iBooksStoreBlocked</span></span>|<span data-ttu-id="572d4-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-300">Boolean</span></span>|<span data-ttu-id="572d4-301">Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-301">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="572d4-302">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="572d4-302">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="572d4-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-303">Boolean</span></span>|<span data-ttu-id="572d4-304">Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".</span><span class="sxs-lookup"><span data-stu-id="572d4-304">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="572d4-305">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="572d4-305">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="572d4-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-306">Boolean</span></span>|<span data-ttu-id="572d4-307">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве с iOS или macOS.</span><span class="sxs-lookup"><span data-stu-id="572d4-307">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="572d4-308">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="572d4-308">iCloudBlockBackup</span></span>|<span data-ttu-id="572d4-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-309">Boolean</span></span>|<span data-ttu-id="572d4-310">Указывает, следует ли заблокировать резервное копирование iCloud.</span><span class="sxs-lookup"><span data-stu-id="572d4-310">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="572d4-311">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="572d4-311">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="572d4-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-312">Boolean</span></span>|<span data-ttu-id="572d4-313">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="572d4-313">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="572d4-314">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="572d4-314">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="572d4-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-315">Boolean</span></span>|<span data-ttu-id="572d4-316">Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="572d4-316">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="572d4-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="572d4-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="572d4-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-318">Boolean</span></span>|<span data-ttu-id="572d4-319">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="572d4-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="572d4-320">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="572d4-320">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="572d4-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-321">Boolean</span></span>|<span data-ttu-id="572d4-322">Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.</span><span class="sxs-lookup"><span data-stu-id="572d4-322">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="572d4-323">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="572d4-323">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="572d4-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-324">Boolean</span></span>|<span data-ttu-id="572d4-325">Указывает, следует ли заблокировать общий фотопоток.</span><span class="sxs-lookup"><span data-stu-id="572d4-325">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="572d4-326">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="572d4-326">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="572d4-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-327">Boolean</span></span>|<span data-ttu-id="572d4-328">Указывает, обязательно ли шифровать резервные копии iCloud.</span><span class="sxs-lookup"><span data-stu-id="572d4-328">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="572d4-329">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="572d4-329">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="572d4-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-330">Boolean</span></span>|<span data-ttu-id="572d4-331">Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.</span><span class="sxs-lookup"><span data-stu-id="572d4-331">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="572d4-332">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="572d4-332">iTunesBlockMusicService</span></span>|<span data-ttu-id="572d4-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-333">Boolean</span></span>|<span data-ttu-id="572d4-334">Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-334">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="572d4-335">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="572d4-335">iTunesBlockRadio</span></span>|<span data-ttu-id="572d4-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-336">Boolean</span></span>|<span data-ttu-id="572d4-337">Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-337">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="572d4-338">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="572d4-338">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="572d4-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-339">Boolean</span></span>|<span data-ttu-id="572d4-340">Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-340">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="572d4-341">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="572d4-341">keyboardBlockDictation</span></span>|<span data-ttu-id="572d4-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-342">Boolean</span></span>|<span data-ttu-id="572d4-343">Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-343">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="572d4-344">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="572d4-344">keyboardBlockPredictive</span></span>|<span data-ttu-id="572d4-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-345">Boolean</span></span>|<span data-ttu-id="572d4-346">Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-346">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="572d4-347">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="572d4-347">keyboardBlockShortcuts</span></span>|<span data-ttu-id="572d4-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-348">Boolean</span></span>|<span data-ttu-id="572d4-349">Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-349">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="572d4-350">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="572d4-350">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="572d4-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-351">Boolean</span></span>|<span data-ttu-id="572d4-352">Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-352">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="572d4-353">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="572d4-353">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="572d4-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-354">Boolean</span></span>|<span data-ttu-id="572d4-355">Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-355">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-356">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="572d4-356">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="572d4-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-357">Boolean</span></span>|<span data-ttu-id="572d4-358">Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-358">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-359">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="572d4-359">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="572d4-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-360">Boolean</span></span>|<span data-ttu-id="572d4-361">Указывает, следует ли запретить автоблокировку устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-361">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-362">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="572d4-362">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="572d4-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-363">Boolean</span></span>|<span data-ttu-id="572d4-364">Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-364">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-365">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="572d4-365">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="572d4-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-366">Boolean</span></span>|<span data-ttu-id="572d4-367">Указывает, можно ли использовать переключатель звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-367">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-368">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="572d4-368">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="572d4-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-369">Boolean</span></span>|<span data-ttu-id="572d4-370">Указывает, следует ли запретить поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-370">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-371">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="572d4-371">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="572d4-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-372">Boolean</span></span>|<span data-ttu-id="572d4-373">Указывает, можно ли использовать кнопку "Сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-373">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-374">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="572d4-374">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="572d4-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-375">Boolean</span></span>|<span data-ttu-id="572d4-376">Указывает, можно ли использовать сенсорный экран в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-376">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-377">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="572d4-377">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="572d4-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-378">Boolean</span></span>|<span data-ttu-id="572d4-379">Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-379">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-380">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="572d4-380">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="572d4-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-381">Boolean</span></span>|<span data-ttu-id="572d4-382">Указывает, можно ли использовать кнопки громкости в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-382">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-383">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="572d4-383">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="572d4-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="572d4-384">Boolean</span></span>|<span data-ttu-id="572d4-385">Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-385">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-386">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="572d4-386">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="572d4-387">String</span><span class="sxs-lookup"><span data-stu-id="572d4-387">String</span></span>|<span data-ttu-id="572d4-388">URL-адрес приложения в App Store для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-388">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="572d4-389">Используйте, если свойство KioskModeManagedAppId не известно.</span><span class="sxs-lookup"><span data-stu-id="572d4-389">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="572d4-390">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="572d4-390">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="572d4-391">String</span><span class="sxs-lookup"><span data-stu-id="572d4-391">String</span></span>|<span data-ttu-id="572d4-392">КОД для встроенных приложений для использования в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-392">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="572d4-393">Используется при KioskModeManagedAppId и KioskModeAppStoreUrl не установлен.</span><span class="sxs-lookup"><span data-stu-id="572d4-393">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="572d4-394">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="572d4-394">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="572d4-395">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-395">Boolean</span></span>|<span data-ttu-id="572d4-396">Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-396">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-397">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="572d4-397">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="572d4-398">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-398">Boolean</span></span>|<span data-ttu-id="572d4-399">Указывает, обязательно ли использовать инверсию цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-399">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-400">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="572d4-400">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="572d4-401">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-401">Boolean</span></span>|<span data-ttu-id="572d4-402">Указывает, обязательно ли использовать монозвук в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-402">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-403">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="572d4-403">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="572d4-404">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-404">Boolean</span></span>|<span data-ttu-id="572d4-405">Указывает, обязательно ли использовать VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-405">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-406">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="572d4-406">kioskModeRequireZoom</span></span>|<span data-ttu-id="572d4-407">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-407">Boolean</span></span>|<span data-ttu-id="572d4-408">Указывает, обязательно ли использовать масштабирование в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-408">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="572d4-409">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="572d4-409">kioskModeManagedAppId</span></span>|<span data-ttu-id="572d4-410">String</span><span class="sxs-lookup"><span data-stu-id="572d4-410">String</span></span>|<span data-ttu-id="572d4-411">Идентификатор управляемого приложения для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="572d4-411">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="572d4-412">Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.</span><span class="sxs-lookup"><span data-stu-id="572d4-412">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="572d4-413">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="572d4-413">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="572d4-414">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-414">Boolean</span></span>|<span data-ttu-id="572d4-415">Указывает, следует ли запретить использовать центр управления на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="572d4-415">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="572d4-416">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="572d4-416">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="572d4-417">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-417">Boolean</span></span>|<span data-ttu-id="572d4-418">Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="572d4-418">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="572d4-419">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="572d4-419">lockScreenBlockPassbook</span></span>|<span data-ttu-id="572d4-420">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-420">Boolean</span></span>|<span data-ttu-id="572d4-421">Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="572d4-421">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="572d4-422">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="572d4-422">lockScreenBlockTodayView</span></span>|<span data-ttu-id="572d4-423">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-423">Boolean</span></span>|<span data-ttu-id="572d4-424">Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="572d4-424">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="572d4-425">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="572d4-425">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="572d4-426">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="572d4-426">mediaContentRatingAustralia</span></span>](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|<span data-ttu-id="572d4-427">Настройки возрастных ограничений для Австралии</span><span class="sxs-lookup"><span data-stu-id="572d4-427">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="572d4-428">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="572d4-428">mediaContentRatingCanada</span></span>|[<span data-ttu-id="572d4-429">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="572d4-429">mediaContentRatingCanada</span></span>](../resources/intune_deviceconfig_mediacontentratingcanada.md)|<span data-ttu-id="572d4-430">Настройки возрастных ограничений для Канады</span><span class="sxs-lookup"><span data-stu-id="572d4-430">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="572d4-431">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="572d4-431">mediaContentRatingFrance</span></span>|[<span data-ttu-id="572d4-432">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="572d4-432">mediaContentRatingFrance</span></span>](../resources/intune_deviceconfig_mediacontentratingfrance.md)|<span data-ttu-id="572d4-433">Настройки возрастных ограничений для Франции</span><span class="sxs-lookup"><span data-stu-id="572d4-433">Media content rating settings for France</span></span>|
|<span data-ttu-id="572d4-434">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="572d4-434">mediaContentRatingGermany</span></span>|[<span data-ttu-id="572d4-435">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="572d4-435">mediaContentRatingGermany</span></span>](../resources/intune_deviceconfig_mediacontentratinggermany.md)|<span data-ttu-id="572d4-436">Настройки возрастных ограничений для Германии</span><span class="sxs-lookup"><span data-stu-id="572d4-436">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="572d4-437">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="572d4-437">mediaContentRatingIreland</span></span>|[<span data-ttu-id="572d4-438">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="572d4-438">mediaContentRatingIreland</span></span>](../resources/intune_deviceconfig_mediacontentratingireland.md)|<span data-ttu-id="572d4-439">Настройки возрастных ограничений для Ирландии</span><span class="sxs-lookup"><span data-stu-id="572d4-439">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="572d4-440">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="572d4-440">mediaContentRatingJapan</span></span>|[<span data-ttu-id="572d4-441">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="572d4-441">mediaContentRatingJapan</span></span>](../resources/intune_deviceconfig_mediacontentratingjapan.md)|<span data-ttu-id="572d4-442">Настройки возрастных ограничений для Японии</span><span class="sxs-lookup"><span data-stu-id="572d4-442">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="572d4-443">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="572d4-443">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="572d4-444">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="572d4-444">mediaContentRatingNewZealand</span></span>](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|<span data-ttu-id="572d4-445">Настройки возрастных ограничений для Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="572d4-445">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="572d4-446">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="572d4-446">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="572d4-447">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="572d4-447">mediaContentRatingUnitedKingdom</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|<span data-ttu-id="572d4-448">Настройки возрастных ограничений для Соединенного Королевства</span><span class="sxs-lookup"><span data-stu-id="572d4-448">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="572d4-449">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="572d4-449">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="572d4-450">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="572d4-450">mediaContentRatingUnitedStates</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|<span data-ttu-id="572d4-451">Настройки возрастных ограничений для Соединенных Штатов</span><span class="sxs-lookup"><span data-stu-id="572d4-451">Media content rating settings for United States</span></span>|
|<span data-ttu-id="572d4-452">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="572d4-452">networkUsageRules</span></span>|<span data-ttu-id="572d4-453">Коллекция [iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="572d4-453">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="572d4-454">Список управляемых приложений и сетевых правил, которые к ним применяются.</span><span class="sxs-lookup"><span data-stu-id="572d4-454">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="572d4-455">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="572d4-455">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="572d4-456">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="572d4-456">mediaContentRatingApps</span></span>|[<span data-ttu-id="572d4-457">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="572d4-457">ratingAppsType</span></span>](../resources/intune_deviceconfig_ratingappstype.md)|<span data-ttu-id="572d4-458">Оценка параметры для приложений контента мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="572d4-458">Media content rating settings for Apps.</span></span> <span data-ttu-id="572d4-459">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="572d4-459">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="572d4-460">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-460">messagesBlocked</span></span>|<span data-ttu-id="572d4-461">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-461">Boolean</span></span>|<span data-ttu-id="572d4-462">Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="572d4-462">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="572d4-463">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="572d4-463">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="572d4-464">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-464">Boolean</span></span>|<span data-ttu-id="572d4-465">Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-465">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="572d4-466">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="572d4-466">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="572d4-467">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-467">Boolean</span></span>|<span data-ttu-id="572d4-468">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="572d4-468">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="572d4-469">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="572d4-469">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="572d4-470">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-470">Boolean</span></span>|<span data-ttu-id="572d4-471">Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-471">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="572d4-472">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="572d4-472">passcodeBlockModification</span></span>|<span data-ttu-id="572d4-473">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-473">Boolean</span></span>|<span data-ttu-id="572d4-474">Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-474">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="572d4-475">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="572d4-475">passcodeBlockSimple</span></span>|<span data-ttu-id="572d4-476">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-476">Boolean</span></span>|<span data-ttu-id="572d4-477">Указывает, следует ли блокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="572d4-477">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="572d4-478">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="572d4-478">passcodeExpirationDays</span></span>|<span data-ttu-id="572d4-479">Int32</span><span class="sxs-lookup"><span data-stu-id="572d4-479">Int32</span></span>|<span data-ttu-id="572d4-480">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="572d4-480">Number of days before the passcode expires.</span></span> <span data-ttu-id="572d4-481">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="572d4-481">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="572d4-482">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="572d4-482">passcodeMinimumLength</span></span>|<span data-ttu-id="572d4-483">Int32</span><span class="sxs-lookup"><span data-stu-id="572d4-483">Int32</span></span>|<span data-ttu-id="572d4-484">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="572d4-484">Minimum length of passcode.</span></span> <span data-ttu-id="572d4-485">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="572d4-485">Valid values 4 to 14</span></span>|
|<span data-ttu-id="572d4-486">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="572d4-486">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="572d4-487">Int32</span><span class="sxs-lookup"><span data-stu-id="572d4-487">Int32</span></span>|<span data-ttu-id="572d4-488">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="572d4-488">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="572d4-489">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="572d4-489">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="572d4-490">Int32</span><span class="sxs-lookup"><span data-stu-id="572d4-490">Int32</span></span>|<span data-ttu-id="572d4-491">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="572d4-491">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="572d4-492">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="572d4-492">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="572d4-493">Int32</span><span class="sxs-lookup"><span data-stu-id="572d4-493">Int32</span></span>|<span data-ttu-id="572d4-494">Количество наборов символов, которые должен содержать секретный код.</span><span class="sxs-lookup"><span data-stu-id="572d4-494">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="572d4-495">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="572d4-495">Valid values 0 to 4</span></span>|
|<span data-ttu-id="572d4-496">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="572d4-496">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="572d4-497">Int32</span><span class="sxs-lookup"><span data-stu-id="572d4-497">Int32</span></span>|<span data-ttu-id="572d4-498">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="572d4-498">Number of previous passcodes to block.</span></span> <span data-ttu-id="572d4-499">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="572d4-499">Valid values 1 to 24</span></span>|
|<span data-ttu-id="572d4-500">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="572d4-500">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="572d4-501">Int32</span><span class="sxs-lookup"><span data-stu-id="572d4-501">Int32</span></span>|<span data-ttu-id="572d4-502">Количество неудачных попыток входа до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="572d4-502">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="572d4-503">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="572d4-503">Valid values 4 to 11</span></span>|
|<span data-ttu-id="572d4-504">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="572d4-504">passcodeRequiredType</span></span>|[<span data-ttu-id="572d4-505">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="572d4-505">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="572d4-506">Необходимый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="572d4-506">Type of passcode that is required.</span></span> <span data-ttu-id="572d4-507">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="572d4-507">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="572d4-508">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="572d4-508">passcodeRequired</span></span>|<span data-ttu-id="572d4-509">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-509">Boolean</span></span>|<span data-ttu-id="572d4-510">Указывает, обязательно ли использовать секретный код.</span><span class="sxs-lookup"><span data-stu-id="572d4-510">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="572d4-511">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-511">podcastsBlocked</span></span>|<span data-ttu-id="572d4-512">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-512">Boolean</span></span>|<span data-ttu-id="572d4-513">Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-513">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="572d4-514">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="572d4-514">safariBlockAutofill</span></span>|<span data-ttu-id="572d4-515">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-515">Boolean</span></span>|<span data-ttu-id="572d4-516">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="572d4-516">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="572d4-517">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="572d4-517">safariBlockJavaScript</span></span>|<span data-ttu-id="572d4-518">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-518">Boolean</span></span>|<span data-ttu-id="572d4-519">Указывает, следует ли заблокировать JavaScript в Safari.</span><span class="sxs-lookup"><span data-stu-id="572d4-519">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="572d4-520">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="572d4-520">safariBlockPopups</span></span>|<span data-ttu-id="572d4-521">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-521">Boolean</span></span>|<span data-ttu-id="572d4-522">Указывает, следует ли блокировать всплывающие окна в Safari.</span><span class="sxs-lookup"><span data-stu-id="572d4-522">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="572d4-523">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-523">safariBlocked</span></span>|<span data-ttu-id="572d4-524">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-524">Boolean</span></span>|<span data-ttu-id="572d4-525">Указывает, следует ли запретить использовать Safari.</span><span class="sxs-lookup"><span data-stu-id="572d4-525">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="572d4-526">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="572d4-526">safariCookieSettings</span></span>|[<span data-ttu-id="572d4-527">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="572d4-527">webBrowserCookieSettings</span></span>](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|<span data-ttu-id="572d4-528">Настройки файлов cookie для Safari.</span><span class="sxs-lookup"><span data-stu-id="572d4-528">Cookie settings for Safari.</span></span> <span data-ttu-id="572d4-529">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="572d4-529">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="572d4-530">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="572d4-530">safariManagedDomains</span></span>|<span data-ttu-id="572d4-531">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="572d4-531">String collection</span></span>|<span data-ttu-id="572d4-532">URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.</span><span class="sxs-lookup"><span data-stu-id="572d4-532">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="572d4-533">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="572d4-533">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="572d4-534">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="572d4-534">String collection</span></span>|<span data-ttu-id="572d4-535">Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам.</span><span class="sxs-lookup"><span data-stu-id="572d4-535">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="572d4-536">Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-536">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="572d4-537">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="572d4-537">safariRequireFraudWarning</span></span>|<span data-ttu-id="572d4-538">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-538">Boolean</span></span>|<span data-ttu-id="572d4-539">Указывает, обязательно ли предупреждение о мошенничестве в Safari.</span><span class="sxs-lookup"><span data-stu-id="572d4-539">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="572d4-540">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-540">screenCaptureBlocked</span></span>|<span data-ttu-id="572d4-541">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-541">Boolean</span></span>|<span data-ttu-id="572d4-542">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="572d4-542">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="572d4-543">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-543">siriBlocked</span></span>|<span data-ttu-id="572d4-544">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-544">Boolean</span></span>|<span data-ttu-id="572d4-545">Указывает, следует ли запретить использовать Siri.</span><span class="sxs-lookup"><span data-stu-id="572d4-545">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="572d4-546">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="572d4-546">siriBlockedWhenLocked</span></span>|<span data-ttu-id="572d4-547">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-547">Boolean</span></span>|<span data-ttu-id="572d4-548">Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="572d4-548">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="572d4-549">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="572d4-549">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="572d4-550">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-550">Boolean</span></span>|<span data-ttu-id="572d4-551">Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="572d4-551">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="572d4-552">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="572d4-552">siriRequireProfanityFilter</span></span>|<span data-ttu-id="572d4-553">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-553">Boolean</span></span>|<span data-ttu-id="572d4-554">Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="572d4-554">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="572d4-555">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="572d4-555">spotlightBlockInternetResults</span></span>|<span data-ttu-id="572d4-556">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-556">Boolean</span></span>|<span data-ttu-id="572d4-557">Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="572d4-557">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="572d4-558">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="572d4-558">voiceDialingBlocked</span></span>|<span data-ttu-id="572d4-559">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-559">Boolean</span></span>|<span data-ttu-id="572d4-560">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="572d4-560">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="572d4-561">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="572d4-561">wallpaperBlockModification</span></span>|<span data-ttu-id="572d4-562">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-562">Boolean</span></span>|<span data-ttu-id="572d4-563">Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="572d4-563">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="572d4-564">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="572d4-564">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="572d4-565">Логический</span><span class="sxs-lookup"><span data-stu-id="572d4-565">Boolean</span></span>|<span data-ttu-id="572d4-566">Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="572d4-566">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="572d4-567">Отклик</span><span class="sxs-lookup"><span data-stu-id="572d4-567">Response</span></span>
<span data-ttu-id="572d4-568">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="572d4-568">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="572d4-569">Пример</span><span class="sxs-lookup"><span data-stu-id="572d4-569">Example</span></span>
### <a name="request"></a><span data-ttu-id="572d4-570">Запрос</span><span class="sxs-lookup"><span data-stu-id="572d4-570">Request</span></span>
<span data-ttu-id="572d4-571">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="572d4-571">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 7841

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```

### <a name="response"></a><span data-ttu-id="572d4-572">Ответ</span><span class="sxs-lookup"><span data-stu-id="572d4-572">Response</span></span>
<span data-ttu-id="572d4-p127">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="572d4-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8013

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```



