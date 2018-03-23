# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="6f895-101">Обновление объекта iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="6f895-101">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="6f895-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f895-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f895-103">Обновление свойств объекта [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f895-103">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f895-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6f895-104">Prerequisites</span></span>
<span data-ttu-id="6f895-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6f895-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6f895-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f895-107">Permission type</span></span>|<span data-ttu-id="6f895-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f895-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f895-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f895-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6f895-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f895-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f895-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f895-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f895-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f895-112">Not supported.</span></span>|
|<span data-ttu-id="6f895-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f895-113">Application</span></span>|<span data-ttu-id="6f895-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f895-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f895-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f895-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6f895-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f895-116">Request headers</span></span>
|<span data-ttu-id="6f895-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f895-117">Header</span></span>|<span data-ttu-id="6f895-118">Значение</span><span class="sxs-lookup"><span data-stu-id="6f895-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f895-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f895-119">Authorization</span></span>|<span data-ttu-id="6f895-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f895-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f895-121">Accept</span><span class="sxs-lookup"><span data-stu-id="6f895-121">Accept</span></span>|<span data-ttu-id="6f895-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6f895-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f895-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f895-123">Request body</span></span>
<span data-ttu-id="6f895-124">В тексте запроса добавьте представление объекта [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f895-124">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="6f895-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f895-125">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="6f895-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f895-126">Property</span></span>|<span data-ttu-id="6f895-127">Тип</span><span class="sxs-lookup"><span data-stu-id="6f895-127">Type</span></span>|<span data-ttu-id="6f895-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6f895-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f895-129">id</span><span class="sxs-lookup"><span data-stu-id="6f895-129">id</span></span>|<span data-ttu-id="6f895-130">String</span><span class="sxs-lookup"><span data-stu-id="6f895-130">String</span></span>|<span data-ttu-id="6f895-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6f895-131">Key of the entity.</span></span> <span data-ttu-id="6f895-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f895-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f895-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f895-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6f895-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f895-134">DateTimeOffset</span></span>|<span data-ttu-id="6f895-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6f895-135">DateTime the object was last modified.</span></span> <span data-ttu-id="6f895-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f895-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f895-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f895-137">createdDateTime</span></span>|<span data-ttu-id="6f895-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f895-138">DateTimeOffset</span></span>|<span data-ttu-id="6f895-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6f895-139">DateTime the object was created.</span></span> <span data-ttu-id="6f895-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f895-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f895-141">description</span><span class="sxs-lookup"><span data-stu-id="6f895-141">description</span></span>|<span data-ttu-id="6f895-142">String</span><span class="sxs-lookup"><span data-stu-id="6f895-142">String</span></span>|<span data-ttu-id="6f895-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6f895-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6f895-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f895-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f895-145">displayName</span><span class="sxs-lookup"><span data-stu-id="6f895-145">displayName</span></span>|<span data-ttu-id="6f895-146">String</span><span class="sxs-lookup"><span data-stu-id="6f895-146">String</span></span>|<span data-ttu-id="6f895-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6f895-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6f895-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f895-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f895-149">version</span><span class="sxs-lookup"><span data-stu-id="6f895-149">version</span></span>|<span data-ttu-id="6f895-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6f895-150">Int32</span></span>|<span data-ttu-id="6f895-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6f895-151">Version of the device configuration.</span></span> <span data-ttu-id="6f895-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f895-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f895-153">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="6f895-153">accountBlockModification</span></span>|<span data-ttu-id="6f895-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-154">Boolean</span></span>|<span data-ttu-id="6f895-155">Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-155">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f895-156">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="6f895-156">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="6f895-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-157">Boolean</span></span>|<span data-ttu-id="6f895-158">Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-158">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="6f895-159">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-159">airDropBlocked</span></span>|<span data-ttu-id="6f895-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-160">Boolean</span></span>|<span data-ttu-id="6f895-161">Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-161">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f895-162">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="6f895-162">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="6f895-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-163">Boolean</span></span>|<span data-ttu-id="6f895-164">Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-164">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f895-165">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="6f895-165">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="6f895-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-166">Boolean</span></span>|<span data-ttu-id="6f895-167">Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.</span><span class="sxs-lookup"><span data-stu-id="6f895-167">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="6f895-168">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="6f895-168">appleWatchBlockPairing</span></span>|<span data-ttu-id="6f895-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-169">Boolean</span></span>|<span data-ttu-id="6f895-170">Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-170">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f895-171">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="6f895-171">appleWatchForceWristDetection</span></span>|<span data-ttu-id="6f895-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-172">Boolean</span></span>|<span data-ttu-id="6f895-173">Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-173">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="6f895-174">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-174">appleNewsBlocked</span></span>|<span data-ttu-id="6f895-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-175">Boolean</span></span>|<span data-ttu-id="6f895-176">Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-176">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f895-177">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="6f895-177">appsSingleAppModeList</span></span>|<span data-ttu-id="6f895-178">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6f895-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="6f895-179">Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы.</span><span class="sxs-lookup"><span data-stu-id="6f895-179">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="6f895-180">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-180">Supervised only.</span></span> <span data-ttu-id="6f895-181">iOS 7.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="6f895-181">iOS 7.0 and later.</span></span> <span data-ttu-id="6f895-182">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6f895-182">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6f895-183">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="6f895-183">appsVisibilityList</span></span>|<span data-ttu-id="6f895-184">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6f895-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="6f895-185">Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-185">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="6f895-186">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="6f895-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6f895-187">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="6f895-187">appsVisibilityListType</span></span>|<span data-ttu-id="6f895-188">String</span><span class="sxs-lookup"><span data-stu-id="6f895-188">String</span></span>|<span data-ttu-id="6f895-189">Тип списка, определенного свойством AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="6f895-189">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="6f895-190">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="6f895-190">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="6f895-191">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="6f895-191">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="6f895-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-192">Boolean</span></span>|<span data-ttu-id="6f895-193">Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-193">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f895-194">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-194">appStoreBlocked</span></span>|<span data-ttu-id="6f895-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-195">Boolean</span></span>|<span data-ttu-id="6f895-196">Указывает, следует ли запретить использовать App Store.</span><span class="sxs-lookup"><span data-stu-id="6f895-196">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="6f895-197">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="6f895-197">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="6f895-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-198">Boolean</span></span>|<span data-ttu-id="6f895-199">Указывает, следует ли запретить пользователю совершать покупки из приложения.</span><span class="sxs-lookup"><span data-stu-id="6f895-199">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="6f895-200">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="6f895-200">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="6f895-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-201">Boolean</span></span>|<span data-ttu-id="6f895-202">Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения.</span><span class="sxs-lookup"><span data-stu-id="6f895-202">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="6f895-203">Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-203">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f895-204">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="6f895-204">appStoreRequirePassword</span></span>|<span data-ttu-id="6f895-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-205">Boolean</span></span>|<span data-ttu-id="6f895-206">Указывает, требуется ли пароль, когда вы используете приложение App Store.</span><span class="sxs-lookup"><span data-stu-id="6f895-206">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="6f895-207">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="6f895-207">bluetoothBlockModification</span></span>|<span data-ttu-id="6f895-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-208">Boolean</span></span>|<span data-ttu-id="6f895-209">Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-209">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="6f895-210">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-210">cameraBlocked</span></span>|<span data-ttu-id="6f895-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-211">Boolean</span></span>|<span data-ttu-id="6f895-212">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="6f895-212">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="6f895-213">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="6f895-213">cellularBlockDataRoaming</span></span>|<span data-ttu-id="6f895-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-214">Boolean</span></span>|<span data-ttu-id="6f895-215">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="6f895-215">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="6f895-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="6f895-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="6f895-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-217">Boolean</span></span>|<span data-ttu-id="6f895-218">Указывает, следует ли заблокировать получение фоновых данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="6f895-218">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="6f895-219">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="6f895-219">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="6f895-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-220">Boolean</span></span>|<span data-ttu-id="6f895-221">Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-221">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f895-222">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="6f895-222">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="6f895-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-223">Boolean</span></span>|<span data-ttu-id="6f895-224">Указывает, следует ли заблокировать личный хот-спот.</span><span class="sxs-lookup"><span data-stu-id="6f895-224">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="6f895-225">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="6f895-225">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="6f895-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-226">Boolean</span></span>|<span data-ttu-id="6f895-227">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="6f895-227">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="6f895-228">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="6f895-228">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="6f895-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-229">Boolean</span></span>|<span data-ttu-id="6f895-230">Указывает, следует ли заблокировать ненадежные сертификаты TLS.</span><span class="sxs-lookup"><span data-stu-id="6f895-230">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="6f895-231">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="6f895-231">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="6f895-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-232">Boolean</span></span>|<span data-ttu-id="6f895-233">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-233">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6f895-234">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="6f895-234">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="6f895-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-235">Boolean</span></span>|<span data-ttu-id="6f895-236">Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-236">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f895-237">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="6f895-237">compliantAppsList</span></span>|<span data-ttu-id="6f895-238">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6f895-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="6f895-239">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="6f895-239">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="6f895-240">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="6f895-240">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6f895-241">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="6f895-241">compliantAppListType</span></span>|<span data-ttu-id="6f895-242">String</span><span class="sxs-lookup"><span data-stu-id="6f895-242">String</span></span>|<span data-ttu-id="6f895-243">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="6f895-243">List that is in the AppComplianceList.</span></span> <span data-ttu-id="6f895-244">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="6f895-244">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="6f895-245">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="6f895-245">configurationProfileBlockChanges</span></span>|<span data-ttu-id="6f895-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-246">Boolean</span></span>|<span data-ttu-id="6f895-247">Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-247">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f895-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-248">definitionLookupBlocked</span></span>|<span data-ttu-id="6f895-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-249">Boolean</span></span>|<span data-ttu-id="6f895-250">Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-250">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="6f895-251">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="6f895-251">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="6f895-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-252">Boolean</span></span>|<span data-ttu-id="6f895-253">Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-253">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f895-254">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="6f895-254">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="6f895-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-255">Boolean</span></span>|<span data-ttu-id="6f895-256">Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-256">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f895-257">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="6f895-257">deviceBlockNameModification</span></span>|<span data-ttu-id="6f895-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-258">Boolean</span></span>|<span data-ttu-id="6f895-259">Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-259">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f895-260">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="6f895-260">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="6f895-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-261">Boolean</span></span>|<span data-ttu-id="6f895-262">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="6f895-262">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="6f895-263">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="6f895-263">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="6f895-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-264">Boolean</span></span>|<span data-ttu-id="6f895-265">Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-265">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="6f895-266">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="6f895-266">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="6f895-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-267">Boolean</span></span>|<span data-ttu-id="6f895-268">Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="6f895-268">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="6f895-269">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="6f895-269">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="6f895-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-270">Boolean</span></span>|<span data-ttu-id="6f895-271">Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="6f895-271">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="6f895-272">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="6f895-272">emailInDomainSuffixes</span></span>|<span data-ttu-id="6f895-273">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6f895-273">String collection</span></span>|<span data-ttu-id="6f895-274">Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.</span><span class="sxs-lookup"><span data-stu-id="6f895-274">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="6f895-275">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="6f895-275">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="6f895-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-276">Boolean</span></span>|<span data-ttu-id="6f895-277">Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="6f895-277">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="6f895-278">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="6f895-278">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="6f895-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-279">Boolean</span></span>|<span data-ttu-id="6f895-280">Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="6f895-280">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="6f895-281">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-281">faceTimeBlocked</span></span>|<span data-ttu-id="6f895-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-282">Boolean</span></span>|<span data-ttu-id="6f895-283">Указывает, следует ли запретить использовать FaceTime.</span><span class="sxs-lookup"><span data-stu-id="6f895-283">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="6f895-284">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-284">findMyFriendsBlocked</span></span>|<span data-ttu-id="6f895-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-285">Boolean</span></span>|<span data-ttu-id="6f895-286">Указывает, следует ли заблокировать функцию "Найти друзей", когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-286">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f895-287">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="6f895-287">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="6f895-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-288">Boolean</span></span>|<span data-ttu-id="6f895-289">Указывает, следует ли запретить пользователю добавлять друзей в Game Center.</span><span class="sxs-lookup"><span data-stu-id="6f895-289">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="6f895-290">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="6f895-290">gamingBlockMultiplayer</span></span>|<span data-ttu-id="6f895-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-291">Boolean</span></span>|<span data-ttu-id="6f895-292">Указывает, следует ли запретить пользователю играть с несколькими игроками.</span><span class="sxs-lookup"><span data-stu-id="6f895-292">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="6f895-293">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-293">gameCenterBlocked</span></span>|<span data-ttu-id="6f895-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-294">Boolean</span></span>|<span data-ttu-id="6f895-295">Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-295">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f895-296">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-296">hostPairingBlocked</span></span>|<span data-ttu-id="6f895-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-297">Boolean</span></span>|<span data-ttu-id="6f895-298">Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-298">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="6f895-299">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-299">iBooksStoreBlocked</span></span>|<span data-ttu-id="6f895-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-300">Boolean</span></span>|<span data-ttu-id="6f895-301">Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-301">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f895-302">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="6f895-302">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="6f895-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-303">Boolean</span></span>|<span data-ttu-id="6f895-304">Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".</span><span class="sxs-lookup"><span data-stu-id="6f895-304">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="6f895-305">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="6f895-305">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="6f895-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-306">Boolean</span></span>|<span data-ttu-id="6f895-307">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве iOS или macOS.</span><span class="sxs-lookup"><span data-stu-id="6f895-307">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="6f895-308">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="6f895-308">iCloudBlockBackup</span></span>|<span data-ttu-id="6f895-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-309">Boolean</span></span>|<span data-ttu-id="6f895-310">Указывает, следует ли заблокировать резервное копирование iCloud.</span><span class="sxs-lookup"><span data-stu-id="6f895-310">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="6f895-311">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="6f895-311">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="6f895-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-312">Boolean</span></span>|<span data-ttu-id="6f895-313">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="6f895-313">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="6f895-314">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="6f895-314">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="6f895-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-315">Boolean</span></span>|<span data-ttu-id="6f895-316">Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="6f895-316">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="6f895-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="6f895-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="6f895-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-318">Boolean</span></span>|<span data-ttu-id="6f895-319">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="6f895-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="6f895-320">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="6f895-320">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="6f895-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-321">Boolean</span></span>|<span data-ttu-id="6f895-322">Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.</span><span class="sxs-lookup"><span data-stu-id="6f895-322">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="6f895-323">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="6f895-323">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="6f895-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-324">Boolean</span></span>|<span data-ttu-id="6f895-325">Указывает, следует ли заблокировать общий фотопоток.</span><span class="sxs-lookup"><span data-stu-id="6f895-325">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="6f895-326">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="6f895-326">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="6f895-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-327">Boolean</span></span>|<span data-ttu-id="6f895-328">Указывает, обязательно ли шифровать резервные копии iCloud.</span><span class="sxs-lookup"><span data-stu-id="6f895-328">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="6f895-329">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="6f895-329">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="6f895-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-330">Boolean</span></span>|<span data-ttu-id="6f895-331">Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.</span><span class="sxs-lookup"><span data-stu-id="6f895-331">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="6f895-332">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="6f895-332">iTunesBlockMusicService</span></span>|<span data-ttu-id="6f895-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-333">Boolean</span></span>|<span data-ttu-id="6f895-334">Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-334">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="6f895-335">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="6f895-335">iTunesBlockRadio</span></span>|<span data-ttu-id="6f895-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-336">Boolean</span></span>|<span data-ttu-id="6f895-337">Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-337">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6f895-338">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="6f895-338">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="6f895-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-339">Boolean</span></span>|<span data-ttu-id="6f895-340">Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-340">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="6f895-341">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="6f895-341">keyboardBlockDictation</span></span>|<span data-ttu-id="6f895-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-342">Boolean</span></span>|<span data-ttu-id="6f895-343">Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-343">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f895-344">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="6f895-344">keyboardBlockPredictive</span></span>|<span data-ttu-id="6f895-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-345">Boolean</span></span>|<span data-ttu-id="6f895-346">Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-346">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="6f895-347">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="6f895-347">keyboardBlockShortcuts</span></span>|<span data-ttu-id="6f895-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-348">Boolean</span></span>|<span data-ttu-id="6f895-349">Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-349">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f895-350">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="6f895-350">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="6f895-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-351">Boolean</span></span>|<span data-ttu-id="6f895-352">Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-352">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="6f895-353">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="6f895-353">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="6f895-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-354">Boolean</span></span>|<span data-ttu-id="6f895-355">Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-355">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-356">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="6f895-356">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="6f895-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-357">Boolean</span></span>|<span data-ttu-id="6f895-358">Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-358">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-359">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="6f895-359">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="6f895-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-360">Boolean</span></span>|<span data-ttu-id="6f895-361">Указывает, следует ли запретить автоблокировку устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-361">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-362">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="6f895-362">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="6f895-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-363">Boolean</span></span>|<span data-ttu-id="6f895-364">Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-364">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-365">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="6f895-365">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="6f895-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-366">Boolean</span></span>|<span data-ttu-id="6f895-367">Указывает, можно ли использовать переключатель звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-367">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-368">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="6f895-368">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="6f895-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-369">Boolean</span></span>|<span data-ttu-id="6f895-370">Указывает, следует ли запретить поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-370">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-371">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="6f895-371">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="6f895-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-372">Boolean</span></span>|<span data-ttu-id="6f895-373">Указывает, можно ли использовать кнопку "Сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-373">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-374">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="6f895-374">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="6f895-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-375">Boolean</span></span>|<span data-ttu-id="6f895-376">Указывает, можно ли использовать сенсорный экран в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-376">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-377">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="6f895-377">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="6f895-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-378">Boolean</span></span>|<span data-ttu-id="6f895-379">Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-379">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-380">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="6f895-380">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="6f895-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-381">Boolean</span></span>|<span data-ttu-id="6f895-382">Указывает, можно ли использовать кнопки громкости в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-382">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-383">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="6f895-383">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="6f895-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-384">Boolean</span></span>|<span data-ttu-id="6f895-385">Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-385">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-386">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6f895-386">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="6f895-387">String</span><span class="sxs-lookup"><span data-stu-id="6f895-387">String</span></span>|<span data-ttu-id="6f895-388">URL-адрес приложения в App Store для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-388">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="6f895-389">Используйте, если свойство KioskModeManagedAppId не известно.</span><span class="sxs-lookup"><span data-stu-id="6f895-389">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="6f895-390">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="6f895-390">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="6f895-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-391">Boolean</span></span>|<span data-ttu-id="6f895-392">Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-392">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-393">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="6f895-393">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="6f895-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-394">Boolean</span></span>|<span data-ttu-id="6f895-395">Указывает, обязательно ли использовать инверсию цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-395">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-396">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="6f895-396">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="6f895-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-397">Boolean</span></span>|<span data-ttu-id="6f895-398">Указывает, обязательно ли использовать монозвук в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-398">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-399">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="6f895-399">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="6f895-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-400">Boolean</span></span>|<span data-ttu-id="6f895-401">Указывает, обязательно ли использовать VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-401">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-402">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="6f895-402">kioskModeRequireZoom</span></span>|<span data-ttu-id="6f895-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-403">Boolean</span></span>|<span data-ttu-id="6f895-404">Указывает, обязательно ли использовать масштабирование в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-404">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="6f895-405">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="6f895-405">kioskModeManagedAppId</span></span>|<span data-ttu-id="6f895-406">String</span><span class="sxs-lookup"><span data-stu-id="6f895-406">String</span></span>|<span data-ttu-id="6f895-407">Идентификатор управляемого приложения для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6f895-407">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="6f895-408">Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.</span><span class="sxs-lookup"><span data-stu-id="6f895-408">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="6f895-409">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="6f895-409">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="6f895-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-410">Boolean</span></span>|<span data-ttu-id="6f895-411">Указывает, следует ли запретить использовать центр управления на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="6f895-411">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="6f895-412">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="6f895-412">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="6f895-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-413">Boolean</span></span>|<span data-ttu-id="6f895-414">Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="6f895-414">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="6f895-415">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="6f895-415">lockScreenBlockPassbook</span></span>|<span data-ttu-id="6f895-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-416">Boolean</span></span>|<span data-ttu-id="6f895-417">Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="6f895-417">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="6f895-418">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="6f895-418">lockScreenBlockTodayView</span></span>|<span data-ttu-id="6f895-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-419">Boolean</span></span>|<span data-ttu-id="6f895-420">Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="6f895-420">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="6f895-421">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="6f895-421">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="6f895-422">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="6f895-422">mediaContentRatingAustralia</span></span>](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|<span data-ttu-id="6f895-423">Настройки возрастных ограничений для Австралии</span><span class="sxs-lookup"><span data-stu-id="6f895-423">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="6f895-424">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="6f895-424">mediaContentRatingCanada</span></span>|[<span data-ttu-id="6f895-425">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="6f895-425">mediaContentRatingCanada</span></span>](../resources/intune_deviceconfig_mediacontentratingcanada.md)|<span data-ttu-id="6f895-426">Настройки возрастных ограничений для Канады</span><span class="sxs-lookup"><span data-stu-id="6f895-426">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="6f895-427">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="6f895-427">mediaContentRatingFrance</span></span>|[<span data-ttu-id="6f895-428">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="6f895-428">mediaContentRatingFrance</span></span>](../resources/intune_deviceconfig_mediacontentratingfrance.md)|<span data-ttu-id="6f895-429">Настройки возрастных ограничений для Франции</span><span class="sxs-lookup"><span data-stu-id="6f895-429">Media content rating settings for France</span></span>|
|<span data-ttu-id="6f895-430">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="6f895-430">mediaContentRatingGermany</span></span>|[<span data-ttu-id="6f895-431">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="6f895-431">mediaContentRatingGermany</span></span>](../resources/intune_deviceconfig_mediacontentratinggermany.md)|<span data-ttu-id="6f895-432">Настройки возрастных ограничений для Германии</span><span class="sxs-lookup"><span data-stu-id="6f895-432">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="6f895-433">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="6f895-433">mediaContentRatingIreland</span></span>|[<span data-ttu-id="6f895-434">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="6f895-434">mediaContentRatingIreland</span></span>](../resources/intune_deviceconfig_mediacontentratingireland.md)|<span data-ttu-id="6f895-435">Настройки возрастных ограничений для Ирландии</span><span class="sxs-lookup"><span data-stu-id="6f895-435">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="6f895-436">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="6f895-436">mediaContentRatingJapan</span></span>|[<span data-ttu-id="6f895-437">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="6f895-437">mediaContentRatingJapan</span></span>](../resources/intune_deviceconfig_mediacontentratingjapan.md)|<span data-ttu-id="6f895-438">Настройки возрастных ограничений для Японии</span><span class="sxs-lookup"><span data-stu-id="6f895-438">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="6f895-439">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="6f895-439">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="6f895-440">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="6f895-440">mediaContentRatingNewZealand</span></span>](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|<span data-ttu-id="6f895-441">Настройки возрастных ограничений для Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="6f895-441">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="6f895-442">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="6f895-442">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="6f895-443">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="6f895-443">mediaContentRatingUnitedKingdom</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|<span data-ttu-id="6f895-444">Настройки возрастных ограничений для Соединенного Королевства</span><span class="sxs-lookup"><span data-stu-id="6f895-444">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="6f895-445">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="6f895-445">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="6f895-446">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="6f895-446">mediaContentRatingUnitedStates</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|<span data-ttu-id="6f895-447">Настройки возрастных ограничений для Соединенных Штатов</span><span class="sxs-lookup"><span data-stu-id="6f895-447">Media content rating settings for United States</span></span>|
|<span data-ttu-id="6f895-448">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="6f895-448">networkUsageRules</span></span>|<span data-ttu-id="6f895-449">Коллекция [iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="6f895-449">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="6f895-450">Список управляемых приложений и сетевых правил, которые к ним применяются.</span><span class="sxs-lookup"><span data-stu-id="6f895-450">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="6f895-451">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="6f895-451">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="6f895-452">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="6f895-452">mediaContentRatingApps</span></span>|<span data-ttu-id="6f895-453">String</span><span class="sxs-lookup"><span data-stu-id="6f895-453">String</span></span>|<span data-ttu-id="6f895-454">Настройки возрастных ограничений для приложений. Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="6f895-454">Media content rating settings for Apps Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="6f895-455">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-455">messagesBlocked</span></span>|<span data-ttu-id="6f895-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-456">Boolean</span></span>|<span data-ttu-id="6f895-457">Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="6f895-457">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="6f895-458">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="6f895-458">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="6f895-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-459">Boolean</span></span>|<span data-ttu-id="6f895-460">Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-460">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6f895-461">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6f895-461">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="6f895-462">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-462">Boolean</span></span>|<span data-ttu-id="6f895-463">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="6f895-463">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="6f895-464">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="6f895-464">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="6f895-465">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-465">Boolean</span></span>|<span data-ttu-id="6f895-466">Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-466">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="6f895-467">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="6f895-467">passcodeBlockModification</span></span>|<span data-ttu-id="6f895-468">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-468">Boolean</span></span>|<span data-ttu-id="6f895-469">Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-469">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f895-470">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6f895-470">passcodeBlockSimple</span></span>|<span data-ttu-id="6f895-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-471">Boolean</span></span>|<span data-ttu-id="6f895-472">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="6f895-472">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="6f895-473">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6f895-473">passcodeExpirationDays</span></span>|<span data-ttu-id="6f895-474">Int32</span><span class="sxs-lookup"><span data-stu-id="6f895-474">Int32</span></span>|<span data-ttu-id="6f895-475">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="6f895-475">Number of days before the passcode expires.</span></span> <span data-ttu-id="6f895-476">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="6f895-476">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6f895-477">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6f895-477">passcodeMinimumLength</span></span>|<span data-ttu-id="6f895-478">Int32</span><span class="sxs-lookup"><span data-stu-id="6f895-478">Int32</span></span>|<span data-ttu-id="6f895-479">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="6f895-479">Minimum length of passcode.</span></span> <span data-ttu-id="6f895-480">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="6f895-480">Valid values 4 to 14</span></span>|
|<span data-ttu-id="6f895-481">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6f895-481">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6f895-482">Int32</span><span class="sxs-lookup"><span data-stu-id="6f895-482">Int32</span></span>|<span data-ttu-id="6f895-483">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="6f895-483">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="6f895-484">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6f895-484">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6f895-485">Int32</span><span class="sxs-lookup"><span data-stu-id="6f895-485">Int32</span></span>|<span data-ttu-id="6f895-486">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="6f895-486">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6f895-487">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6f895-487">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="6f895-488">Int32</span><span class="sxs-lookup"><span data-stu-id="6f895-488">Int32</span></span>|<span data-ttu-id="6f895-489">Количество наборов символов, которые должен содержать секретный код.</span><span class="sxs-lookup"><span data-stu-id="6f895-489">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="6f895-490">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="6f895-490">Valid values 0 to 4</span></span>|
|<span data-ttu-id="6f895-491">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="6f895-491">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="6f895-492">Int32</span><span class="sxs-lookup"><span data-stu-id="6f895-492">Int32</span></span>|<span data-ttu-id="6f895-493">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="6f895-493">Number of previous passcodes to block.</span></span> <span data-ttu-id="6f895-494">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="6f895-494">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6f895-495">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="6f895-495">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="6f895-496">Int32</span><span class="sxs-lookup"><span data-stu-id="6f895-496">Int32</span></span>|<span data-ttu-id="6f895-497">Количество неудачных попыток входа до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="6f895-497">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="6f895-498">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="6f895-498">Valid values 4 to 11</span></span>|
|<span data-ttu-id="6f895-499">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="6f895-499">passcodeRequiredType</span></span>|<span data-ttu-id="6f895-500">String</span><span class="sxs-lookup"><span data-stu-id="6f895-500">String</span></span>|<span data-ttu-id="6f895-501">Необходимый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="6f895-501">Type of passcode that is required.</span></span> <span data-ttu-id="6f895-502">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6f895-502">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6f895-503">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="6f895-503">passcodeRequired</span></span>|<span data-ttu-id="6f895-504">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-504">Boolean</span></span>|<span data-ttu-id="6f895-505">Указывает, обязательно ли использовать секретный код.</span><span class="sxs-lookup"><span data-stu-id="6f895-505">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="6f895-506">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-506">podcastsBlocked</span></span>|<span data-ttu-id="6f895-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-507">Boolean</span></span>|<span data-ttu-id="6f895-508">Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-508">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="6f895-509">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="6f895-509">safariBlockAutofill</span></span>|<span data-ttu-id="6f895-510">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-510">Boolean</span></span>|<span data-ttu-id="6f895-511">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="6f895-511">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="6f895-512">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="6f895-512">safariBlockJavaScript</span></span>|<span data-ttu-id="6f895-513">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-513">Boolean</span></span>|<span data-ttu-id="6f895-514">Указывает, следует ли заблокировать JavaScript в Safari.</span><span class="sxs-lookup"><span data-stu-id="6f895-514">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="6f895-515">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="6f895-515">safariBlockPopups</span></span>|<span data-ttu-id="6f895-516">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-516">Boolean</span></span>|<span data-ttu-id="6f895-517">Указывает, следует ли блокировать всплывающие окна в Safari.</span><span class="sxs-lookup"><span data-stu-id="6f895-517">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="6f895-518">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-518">safariBlocked</span></span>|<span data-ttu-id="6f895-519">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-519">Boolean</span></span>|<span data-ttu-id="6f895-520">Указывает, следует ли запретить использовать Safari.</span><span class="sxs-lookup"><span data-stu-id="6f895-520">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="6f895-521">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="6f895-521">safariCookieSettings</span></span>|<span data-ttu-id="6f895-522">String</span><span class="sxs-lookup"><span data-stu-id="6f895-522">String</span></span>|<span data-ttu-id="6f895-523">Настройки файлов cookie для Safari.</span><span class="sxs-lookup"><span data-stu-id="6f895-523">Cookie settings for Safari.</span></span> <span data-ttu-id="6f895-524">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="6f895-524">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="6f895-525">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="6f895-525">safariManagedDomains</span></span>|<span data-ttu-id="6f895-526">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6f895-526">String collection</span></span>|<span data-ttu-id="6f895-527">URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.</span><span class="sxs-lookup"><span data-stu-id="6f895-527">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="6f895-528">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="6f895-528">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="6f895-529">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6f895-529">String collection</span></span>|<span data-ttu-id="6f895-530">Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам.</span><span class="sxs-lookup"><span data-stu-id="6f895-530">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="6f895-531">Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-531">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6f895-532">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="6f895-532">safariRequireFraudWarning</span></span>|<span data-ttu-id="6f895-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-533">Boolean</span></span>|<span data-ttu-id="6f895-534">Указывает, обязательно ли предупреждение о мошенничестве в Safari.</span><span class="sxs-lookup"><span data-stu-id="6f895-534">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="6f895-535">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-535">screenCaptureBlocked</span></span>|<span data-ttu-id="6f895-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-536">Boolean</span></span>|<span data-ttu-id="6f895-537">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="6f895-537">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="6f895-538">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-538">siriBlocked</span></span>|<span data-ttu-id="6f895-539">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-539">Boolean</span></span>|<span data-ttu-id="6f895-540">Указывает, следует ли запретить использовать Siri.</span><span class="sxs-lookup"><span data-stu-id="6f895-540">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="6f895-541">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="6f895-541">siriBlockedWhenLocked</span></span>|<span data-ttu-id="6f895-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-542">Boolean</span></span>|<span data-ttu-id="6f895-543">Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="6f895-543">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="6f895-544">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="6f895-544">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="6f895-545">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-545">Boolean</span></span>|<span data-ttu-id="6f895-546">Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="6f895-546">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="6f895-547">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="6f895-547">siriRequireProfanityFilter</span></span>|<span data-ttu-id="6f895-548">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-548">Boolean</span></span>|<span data-ttu-id="6f895-549">Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="6f895-549">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="6f895-550">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="6f895-550">spotlightBlockInternetResults</span></span>|<span data-ttu-id="6f895-551">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-551">Boolean</span></span>|<span data-ttu-id="6f895-552">Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="6f895-552">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="6f895-553">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="6f895-553">voiceDialingBlocked</span></span>|<span data-ttu-id="6f895-554">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-554">Boolean</span></span>|<span data-ttu-id="6f895-555">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="6f895-555">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="6f895-556">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="6f895-556">wallpaperBlockModification</span></span>|<span data-ttu-id="6f895-557">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-557">Boolean</span></span>|<span data-ttu-id="6f895-558">Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6f895-558">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="6f895-559">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="6f895-559">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="6f895-560">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f895-560">Boolean</span></span>|<span data-ttu-id="6f895-561">Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6f895-561">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="6f895-562">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f895-562">Response</span></span>
<span data-ttu-id="6f895-563">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f895-563">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f895-564">Пример</span><span class="sxs-lookup"><span data-stu-id="6f895-564">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f895-565">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f895-565">Request</span></span>
<span data-ttu-id="6f895-566">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f895-566">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 7773

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="6f895-567">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f895-567">Response</span></span>
<span data-ttu-id="6f895-p125">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6f895-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7949

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



