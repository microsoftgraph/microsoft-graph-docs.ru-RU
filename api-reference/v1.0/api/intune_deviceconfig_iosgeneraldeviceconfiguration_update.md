# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="e8938-101">Обновление объекта iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e8938-101">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="e8938-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e8938-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8938-103">Обновление свойств объекта [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8938-103">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8938-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e8938-104">Prerequisites</span></span>
<span data-ttu-id="e8938-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e8938-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e8938-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8938-107">Permission type</span></span>|<span data-ttu-id="e8938-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8938-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8938-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8938-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e8938-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8938-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8938-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8938-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8938-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8938-112">Not supported.</span></span>|
|<span data-ttu-id="e8938-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8938-113">Application</span></span>|<span data-ttu-id="e8938-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8938-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8938-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8938-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e8938-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8938-116">Request headers</span></span>
|<span data-ttu-id="e8938-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8938-117">Header</span></span>|<span data-ttu-id="e8938-118">Значение</span><span class="sxs-lookup"><span data-stu-id="e8938-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8938-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8938-119">Authorization</span></span>|<span data-ttu-id="e8938-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="e8938-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8938-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e8938-121">Accept</span></span>|<span data-ttu-id="e8938-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e8938-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8938-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8938-123">Request body</span></span>
<span data-ttu-id="e8938-124">В тексте запроса добавьте представление объекта [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8938-124">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="e8938-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8938-125">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="e8938-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8938-126">Property</span></span>|<span data-ttu-id="e8938-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e8938-127">Type</span></span>|<span data-ttu-id="e8938-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e8938-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8938-129">id</span><span class="sxs-lookup"><span data-stu-id="e8938-129">id</span></span>|<span data-ttu-id="e8938-130">Строка</span><span class="sxs-lookup"><span data-stu-id="e8938-130">String</span></span>|<span data-ttu-id="e8938-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e8938-131">Key of the entity.</span></span> <span data-ttu-id="e8938-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8938-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8938-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8938-133">lastModifiedDateTime</span></span>|<span data-ttu-id="e8938-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8938-134">DateTimeOffset</span></span>|<span data-ttu-id="e8938-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e8938-135">DateTime the object was last modified.</span></span> <span data-ttu-id="e8938-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8938-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8938-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8938-137">createdDateTime</span></span>|<span data-ttu-id="e8938-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8938-138">DateTimeOffset</span></span>|<span data-ttu-id="e8938-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e8938-139">DateTime the object was created.</span></span> <span data-ttu-id="e8938-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8938-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8938-141">description</span><span class="sxs-lookup"><span data-stu-id="e8938-141">description</span></span>|<span data-ttu-id="e8938-142">String</span><span class="sxs-lookup"><span data-stu-id="e8938-142">String</span></span>|<span data-ttu-id="e8938-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e8938-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e8938-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8938-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8938-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e8938-145">displayName</span></span>|<span data-ttu-id="e8938-146">String</span><span class="sxs-lookup"><span data-stu-id="e8938-146">String</span></span>|<span data-ttu-id="e8938-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e8938-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e8938-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8938-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8938-149">version</span><span class="sxs-lookup"><span data-stu-id="e8938-149">version</span></span>|<span data-ttu-id="e8938-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e8938-150">Int32</span></span>|<span data-ttu-id="e8938-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e8938-151">Version of the device configuration.</span></span> <span data-ttu-id="e8938-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8938-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8938-153">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="e8938-153">accountBlockModification</span></span>|<span data-ttu-id="e8938-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-154">Boolean</span></span>|<span data-ttu-id="e8938-155">Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-155">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e8938-156">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="e8938-156">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="e8938-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-157">Boolean</span></span>|<span data-ttu-id="e8938-158">Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-158">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="e8938-159">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-159">airDropBlocked</span></span>|<span data-ttu-id="e8938-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-160">Boolean</span></span>|<span data-ttu-id="e8938-161">Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-161">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e8938-162">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="e8938-162">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="e8938-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-163">Boolean</span></span>|<span data-ttu-id="e8938-164">Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-164">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e8938-165">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="e8938-165">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="e8938-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-166">Boolean</span></span>|<span data-ttu-id="e8938-167">Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.</span><span class="sxs-lookup"><span data-stu-id="e8938-167">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="e8938-168">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="e8938-168">appleWatchBlockPairing</span></span>|<span data-ttu-id="e8938-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-169">Boolean</span></span>|<span data-ttu-id="e8938-170">Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-170">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e8938-171">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="e8938-171">appleWatchForceWristDetection</span></span>|<span data-ttu-id="e8938-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-172">Boolean</span></span>|<span data-ttu-id="e8938-173">Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-173">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="e8938-174">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-174">appleNewsBlocked</span></span>|<span data-ttu-id="e8938-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-175">Boolean</span></span>|<span data-ttu-id="e8938-176">Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-176">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e8938-177">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="e8938-177">appsSingleAppModeList</span></span>|<span data-ttu-id="e8938-178">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="e8938-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="e8938-179">Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы.</span><span class="sxs-lookup"><span data-stu-id="e8938-179">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="e8938-180">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-180">Supervised only.</span></span> <span data-ttu-id="e8938-181">iOS 7.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="e8938-181">iOS 7.0 and later.</span></span> <span data-ttu-id="e8938-182">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e8938-182">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e8938-183">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="e8938-183">appsVisibilityList</span></span>|<span data-ttu-id="e8938-184">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="e8938-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="e8938-185">Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-185">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="e8938-186">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="e8938-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="e8938-187">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="e8938-187">appsVisibilityListType</span></span>|[<span data-ttu-id="e8938-188">appListType</span><span class="sxs-lookup"><span data-stu-id="e8938-188">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="e8938-189">Тип списка, определенного свойством AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="e8938-189">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="e8938-190">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="e8938-190">The possible values are `none`, `appsInListCompliant`, `appsNotInListCompliant`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="e8938-191">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="e8938-191">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="e8938-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-192">Boolean</span></span>|<span data-ttu-id="e8938-193">Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-193">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e8938-194">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-194">appStoreBlocked</span></span>|<span data-ttu-id="e8938-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-195">Boolean</span></span>|<span data-ttu-id="e8938-196">Указывает, следует ли запретить использовать App Store.</span><span class="sxs-lookup"><span data-stu-id="e8938-196">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="e8938-197">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="e8938-197">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="e8938-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-198">Boolean</span></span>|<span data-ttu-id="e8938-199">Указывает, следует ли запретить пользователю совершать покупки из приложения.</span><span class="sxs-lookup"><span data-stu-id="e8938-199">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="e8938-200">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="e8938-200">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="e8938-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-201">Boolean</span></span>|<span data-ttu-id="e8938-202">Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения.</span><span class="sxs-lookup"><span data-stu-id="e8938-202">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="e8938-203">Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-203">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e8938-204">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="e8938-204">appStoreRequirePassword</span></span>|<span data-ttu-id="e8938-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-205">Boolean</span></span>|<span data-ttu-id="e8938-206">Указывает, требуется ли пароль, когда вы используете приложение App Store.</span><span class="sxs-lookup"><span data-stu-id="e8938-206">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="e8938-207">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="e8938-207">bluetoothBlockModification</span></span>|<span data-ttu-id="e8938-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-208">Boolean</span></span>|<span data-ttu-id="e8938-209">Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-209">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="e8938-210">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-210">cameraBlocked</span></span>|<span data-ttu-id="e8938-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-211">Boolean</span></span>|<span data-ttu-id="e8938-212">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="e8938-212">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="e8938-213">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="e8938-213">cellularBlockDataRoaming</span></span>|<span data-ttu-id="e8938-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-214">Boolean</span></span>|<span data-ttu-id="e8938-215">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="e8938-215">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="e8938-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="e8938-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="e8938-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-217">Boolean</span></span>|<span data-ttu-id="e8938-218">Указывает, следует ли заблокировать получение фоновых данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="e8938-218">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="e8938-219">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="e8938-219">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="e8938-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-220">Boolean</span></span>|<span data-ttu-id="e8938-221">Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-221">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e8938-222">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="e8938-222">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="e8938-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-223">Boolean</span></span>|<span data-ttu-id="e8938-224">Указывает, следует ли заблокировать личный хот-спот.</span><span class="sxs-lookup"><span data-stu-id="e8938-224">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="e8938-225">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="e8938-225">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="e8938-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-226">Boolean</span></span>|<span data-ttu-id="e8938-227">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="e8938-227">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="e8938-228">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="e8938-228">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="e8938-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-229">Boolean</span></span>|<span data-ttu-id="e8938-230">Указывает, следует ли заблокировать ненадежные сертификаты TLS.</span><span class="sxs-lookup"><span data-stu-id="e8938-230">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="e8938-231">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="e8938-231">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="e8938-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-232">Boolean</span></span>|<span data-ttu-id="e8938-233">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-233">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="e8938-234">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="e8938-234">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="e8938-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-235">Boolean</span></span>|<span data-ttu-id="e8938-236">Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-236">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e8938-237">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="e8938-237">compliantAppsList</span></span>|<span data-ttu-id="e8938-238">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="e8938-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="e8938-239">Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="e8938-239">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="e8938-240">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="e8938-240">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="e8938-241">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="e8938-241">compliantAppListType</span></span>|[<span data-ttu-id="e8938-242">appListType</span><span class="sxs-lookup"><span data-stu-id="e8938-242">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="e8938-243">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="e8938-243">List that is in the AppComplianceList.</span></span> <span data-ttu-id="e8938-244">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="e8938-244">The possible values are `none`, `appsInListCompliant`, `appsNotInListCompliant`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="e8938-245">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="e8938-245">configurationProfileBlockChanges</span></span>|<span data-ttu-id="e8938-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-246">Boolean</span></span>|<span data-ttu-id="e8938-247">Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-247">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e8938-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-248">definitionLookupBlocked</span></span>|<span data-ttu-id="e8938-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-249">Boolean</span></span>|<span data-ttu-id="e8938-250">Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-250">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="e8938-251">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="e8938-251">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="e8938-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-252">Boolean</span></span>|<span data-ttu-id="e8938-253">Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-253">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e8938-254">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="e8938-254">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="e8938-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-255">Boolean</span></span>|<span data-ttu-id="e8938-256">Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-256">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e8938-257">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="e8938-257">deviceBlockNameModification</span></span>|<span data-ttu-id="e8938-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-258">Boolean</span></span>|<span data-ttu-id="e8938-259">Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-259">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e8938-260">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="e8938-260">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="e8938-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-261">Boolean</span></span>|<span data-ttu-id="e8938-262">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="e8938-262">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="e8938-263">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="e8938-263">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="e8938-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-264">Boolean</span></span>|<span data-ttu-id="e8938-265">Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-265">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="e8938-266">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="e8938-266">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="e8938-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-267">Boolean</span></span>|<span data-ttu-id="e8938-268">Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="e8938-268">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="e8938-269">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="e8938-269">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="e8938-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-270">Boolean</span></span>|<span data-ttu-id="e8938-271">Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="e8938-271">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="e8938-272">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="e8938-272">emailInDomainSuffixes</span></span>|<span data-ttu-id="e8938-273">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e8938-273">String collection</span></span>|<span data-ttu-id="e8938-274">Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.</span><span class="sxs-lookup"><span data-stu-id="e8938-274">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="e8938-275">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="e8938-275">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="e8938-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-276">Boolean</span></span>|<span data-ttu-id="e8938-277">Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="e8938-277">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="e8938-278">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="e8938-278">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="e8938-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-279">Boolean</span></span>|<span data-ttu-id="e8938-280">Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="e8938-280">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="e8938-281">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-281">faceTimeBlocked</span></span>|<span data-ttu-id="e8938-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-282">Boolean</span></span>|<span data-ttu-id="e8938-283">Указывает, следует ли запретить использовать FaceTime.</span><span class="sxs-lookup"><span data-stu-id="e8938-283">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="e8938-284">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-284">findMyFriendsBlocked</span></span>|<span data-ttu-id="e8938-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-285">Boolean</span></span>|<span data-ttu-id="e8938-286">Указывает, следует ли заблокировать функцию "Найти друзей", когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-286">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e8938-287">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="e8938-287">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="e8938-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-288">Boolean</span></span>|<span data-ttu-id="e8938-289">Указывает, следует ли запретить пользователю добавлять друзей в Game Center.</span><span class="sxs-lookup"><span data-stu-id="e8938-289">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="e8938-290">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="e8938-290">gamingBlockMultiplayer</span></span>|<span data-ttu-id="e8938-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-291">Boolean</span></span>|<span data-ttu-id="e8938-292">Указывает, следует ли запретить пользователю играть с несколькими игроками.</span><span class="sxs-lookup"><span data-stu-id="e8938-292">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="e8938-293">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-293">gameCenterBlocked</span></span>|<span data-ttu-id="e8938-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-294">Boolean</span></span>|<span data-ttu-id="e8938-295">Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-295">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e8938-296">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-296">hostPairingBlocked</span></span>|<span data-ttu-id="e8938-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-297">Boolean</span></span>|<span data-ttu-id="e8938-298">Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-298">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="e8938-299">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-299">iBooksStoreBlocked</span></span>|<span data-ttu-id="e8938-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-300">Boolean</span></span>|<span data-ttu-id="e8938-301">Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-301">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e8938-302">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="e8938-302">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="e8938-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-303">Boolean</span></span>|<span data-ttu-id="e8938-304">Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".</span><span class="sxs-lookup"><span data-stu-id="e8938-304">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="e8938-305">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="e8938-305">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="e8938-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-306">Boolean</span></span>|<span data-ttu-id="e8938-307">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве с iOS или macOS.</span><span class="sxs-lookup"><span data-stu-id="e8938-307">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="e8938-308">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="e8938-308">iCloudBlockBackup</span></span>|<span data-ttu-id="e8938-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-309">Boolean</span></span>|<span data-ttu-id="e8938-310">Указывает, следует ли заблокировать резервное копирование iCloud.</span><span class="sxs-lookup"><span data-stu-id="e8938-310">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="e8938-311">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="e8938-311">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="e8938-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-312">Boolean</span></span>|<span data-ttu-id="e8938-313">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="e8938-313">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="e8938-314">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="e8938-314">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="e8938-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-315">Boolean</span></span>|<span data-ttu-id="e8938-316">Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="e8938-316">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="e8938-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="e8938-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="e8938-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-318">Boolean</span></span>|<span data-ttu-id="e8938-319">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="e8938-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="e8938-320">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="e8938-320">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="e8938-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-321">Boolean</span></span>|<span data-ttu-id="e8938-322">Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.</span><span class="sxs-lookup"><span data-stu-id="e8938-322">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="e8938-323">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="e8938-323">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="e8938-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-324">Boolean</span></span>|<span data-ttu-id="e8938-325">Указывает, следует ли заблокировать общий фотопоток.</span><span class="sxs-lookup"><span data-stu-id="e8938-325">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="e8938-326">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="e8938-326">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="e8938-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-327">Boolean</span></span>|<span data-ttu-id="e8938-328">Указывает, обязательно ли шифровать резервные копии iCloud.</span><span class="sxs-lookup"><span data-stu-id="e8938-328">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="e8938-329">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="e8938-329">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="e8938-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-330">Boolean</span></span>|<span data-ttu-id="e8938-331">Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.</span><span class="sxs-lookup"><span data-stu-id="e8938-331">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="e8938-332">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="e8938-332">iTunesBlockMusicService</span></span>|<span data-ttu-id="e8938-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-333">Boolean</span></span>|<span data-ttu-id="e8938-334">Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-334">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="e8938-335">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="e8938-335">iTunesBlockRadio</span></span>|<span data-ttu-id="e8938-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-336">Boolean</span></span>|<span data-ttu-id="e8938-337">Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-337">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="e8938-338">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="e8938-338">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="e8938-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-339">Boolean</span></span>|<span data-ttu-id="e8938-340">Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-340">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="e8938-341">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="e8938-341">keyboardBlockDictation</span></span>|<span data-ttu-id="e8938-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-342">Boolean</span></span>|<span data-ttu-id="e8938-343">Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-343">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e8938-344">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="e8938-344">keyboardBlockPredictive</span></span>|<span data-ttu-id="e8938-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-345">Boolean</span></span>|<span data-ttu-id="e8938-346">Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-346">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="e8938-347">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="e8938-347">keyboardBlockShortcuts</span></span>|<span data-ttu-id="e8938-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-348">Boolean</span></span>|<span data-ttu-id="e8938-349">Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-349">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e8938-350">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="e8938-350">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="e8938-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-351">Boolean</span></span>|<span data-ttu-id="e8938-352">Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-352">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="e8938-353">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="e8938-353">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="e8938-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-354">Boolean</span></span>|<span data-ttu-id="e8938-355">Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-355">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-356">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="e8938-356">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="e8938-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-357">Boolean</span></span>|<span data-ttu-id="e8938-358">Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-358">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-359">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="e8938-359">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="e8938-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-360">Boolean</span></span>|<span data-ttu-id="e8938-361">Указывает, следует ли запретить автоблокировку устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-361">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-362">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="e8938-362">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="e8938-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-363">Boolean</span></span>|<span data-ttu-id="e8938-364">Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-364">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-365">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="e8938-365">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="e8938-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-366">Boolean</span></span>|<span data-ttu-id="e8938-367">Указывает, можно ли использовать переключатель звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-367">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-368">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="e8938-368">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="e8938-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-369">Boolean</span></span>|<span data-ttu-id="e8938-370">Указывает, следует ли запретить поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-370">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-371">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="e8938-371">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="e8938-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-372">Boolean</span></span>|<span data-ttu-id="e8938-373">Указывает, можно ли использовать кнопку "Сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-373">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-374">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="e8938-374">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="e8938-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-375">Boolean</span></span>|<span data-ttu-id="e8938-376">Указывает, можно ли использовать сенсорный экран в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-376">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-377">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="e8938-377">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="e8938-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-378">Boolean</span></span>|<span data-ttu-id="e8938-379">Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-379">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-380">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="e8938-380">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="e8938-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-381">Boolean</span></span>|<span data-ttu-id="e8938-382">Указывает, можно ли использовать кнопки громкости в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-382">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-383">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="e8938-383">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="e8938-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-384">Boolean</span></span>|<span data-ttu-id="e8938-385">Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-385">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-386">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e8938-386">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="e8938-387">String</span><span class="sxs-lookup"><span data-stu-id="e8938-387">String</span></span>|<span data-ttu-id="e8938-388">URL-адрес приложения в App Store для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-388">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="e8938-389">Используйте, если свойство KioskModeManagedAppId не известно.</span><span class="sxs-lookup"><span data-stu-id="e8938-389">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="e8938-390">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="e8938-390">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="e8938-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-391">Boolean</span></span>|<span data-ttu-id="e8938-392">Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-392">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-393">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="e8938-393">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="e8938-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-394">Boolean</span></span>|<span data-ttu-id="e8938-395">Указывает, обязательно ли использовать инверсию цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-395">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-396">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="e8938-396">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="e8938-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-397">Boolean</span></span>|<span data-ttu-id="e8938-398">Указывает, обязательно ли использовать монозвук в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-398">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-399">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="e8938-399">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="e8938-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-400">Boolean</span></span>|<span data-ttu-id="e8938-401">Указывает, обязательно ли использовать VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-401">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-402">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="e8938-402">kioskModeRequireZoom</span></span>|<span data-ttu-id="e8938-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-403">Boolean</span></span>|<span data-ttu-id="e8938-404">Указывает, обязательно ли использовать масштабирование в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-404">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="e8938-405">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="e8938-405">kioskModeManagedAppId</span></span>|<span data-ttu-id="e8938-406">String</span><span class="sxs-lookup"><span data-stu-id="e8938-406">String</span></span>|<span data-ttu-id="e8938-407">Идентификатор управляемого приложения для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e8938-407">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="e8938-408">Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.</span><span class="sxs-lookup"><span data-stu-id="e8938-408">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="e8938-409">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="e8938-409">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="e8938-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-410">Boolean</span></span>|<span data-ttu-id="e8938-411">Указывает, следует ли запретить использовать центр управления на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="e8938-411">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="e8938-412">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="e8938-412">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="e8938-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-413">Boolean</span></span>|<span data-ttu-id="e8938-414">Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="e8938-414">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="e8938-415">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="e8938-415">lockScreenBlockPassbook</span></span>|<span data-ttu-id="e8938-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-416">Boolean</span></span>|<span data-ttu-id="e8938-417">Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="e8938-417">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="e8938-418">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="e8938-418">lockScreenBlockTodayView</span></span>|<span data-ttu-id="e8938-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-419">Boolean</span></span>|<span data-ttu-id="e8938-420">Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="e8938-420">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="e8938-421">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="e8938-421">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="e8938-422">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="e8938-422">mediaContentRatingAustralia</span></span>](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|<span data-ttu-id="e8938-423">Настройки возрастных ограничений для Австралии</span><span class="sxs-lookup"><span data-stu-id="e8938-423">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="e8938-424">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="e8938-424">mediaContentRatingCanada</span></span>|[<span data-ttu-id="e8938-425">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="e8938-425">mediaContentRatingCanada</span></span>](../resources/intune_deviceconfig_mediacontentratingcanada.md)|<span data-ttu-id="e8938-426">Настройки возрастных ограничений для Канады</span><span class="sxs-lookup"><span data-stu-id="e8938-426">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="e8938-427">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="e8938-427">mediaContentRatingFrance</span></span>|[<span data-ttu-id="e8938-428">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="e8938-428">mediaContentRatingFrance</span></span>](../resources/intune_deviceconfig_mediacontentratingfrance.md)|<span data-ttu-id="e8938-429">Настройки возрастных ограничений для Франции</span><span class="sxs-lookup"><span data-stu-id="e8938-429">Media content rating settings for France</span></span>|
|<span data-ttu-id="e8938-430">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="e8938-430">mediaContentRatingGermany</span></span>|[<span data-ttu-id="e8938-431">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="e8938-431">mediaContentRatingGermany</span></span>](../resources/intune_deviceconfig_mediacontentratinggermany.md)|<span data-ttu-id="e8938-432">Настройки возрастных ограничений для Германии</span><span class="sxs-lookup"><span data-stu-id="e8938-432">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="e8938-433">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="e8938-433">mediaContentRatingIreland</span></span>|[<span data-ttu-id="e8938-434">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="e8938-434">mediaContentRatingIreland</span></span>](../resources/intune_deviceconfig_mediacontentratingireland.md)|<span data-ttu-id="e8938-435">Настройки возрастных ограничений для Ирландии</span><span class="sxs-lookup"><span data-stu-id="e8938-435">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="e8938-436">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="e8938-436">mediaContentRatingJapan</span></span>|[<span data-ttu-id="e8938-437">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="e8938-437">mediaContentRatingJapan</span></span>](../resources/intune_deviceconfig_mediacontentratingjapan.md)|<span data-ttu-id="e8938-438">Настройки возрастных ограничений для Японии</span><span class="sxs-lookup"><span data-stu-id="e8938-438">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="e8938-439">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="e8938-439">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="e8938-440">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="e8938-440">mediaContentRatingNewZealand</span></span>](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|<span data-ttu-id="e8938-441">Настройки возрастных ограничений для Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="e8938-441">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="e8938-442">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="e8938-442">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="e8938-443">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="e8938-443">mediaContentRatingUnitedKingdom</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|<span data-ttu-id="e8938-444">Настройки возрастных ограничений для Соединенного Королевства</span><span class="sxs-lookup"><span data-stu-id="e8938-444">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="e8938-445">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="e8938-445">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="e8938-446">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="e8938-446">mediaContentRatingUnitedStates</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|<span data-ttu-id="e8938-447">Настройки возрастных ограничений для Соединенных Штатов</span><span class="sxs-lookup"><span data-stu-id="e8938-447">Media content rating settings for United States</span></span>|
|<span data-ttu-id="e8938-448">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="e8938-448">networkUsageRules</span></span>|<span data-ttu-id="e8938-449">Коллекция [iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="e8938-449">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="e8938-450">Список управляемых приложений и сетевых правил, которые к ним применяются.</span><span class="sxs-lookup"><span data-stu-id="e8938-450">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="e8938-451">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="e8938-451">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="e8938-452">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="e8938-452">mediaContentRatingApps</span></span>|[<span data-ttu-id="e8938-453">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="e8938-453">ratingAppsType</span></span>](../resources/intune_deviceconfig_ratingappstype.md)|<span data-ttu-id="e8938-454">Параметры оценки содержимого мультимедиа для приложений.</span><span class="sxs-lookup"><span data-stu-id="e8938-454">Media content rating settings for Germany</span></span> <span data-ttu-id="e8938-455">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="e8938-455">The possible values are `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`, , , , , , or .</span></span>|
|<span data-ttu-id="e8938-456">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-456">messagesBlocked</span></span>|<span data-ttu-id="e8938-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-457">Boolean</span></span>|<span data-ttu-id="e8938-458">Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="e8938-458">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="e8938-459">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="e8938-459">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="e8938-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-460">Boolean</span></span>|<span data-ttu-id="e8938-461">Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-461">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="e8938-462">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e8938-462">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="e8938-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-463">Boolean</span></span>|<span data-ttu-id="e8938-464">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="e8938-464">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="e8938-465">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="e8938-465">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="e8938-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-466">Boolean</span></span>|<span data-ttu-id="e8938-467">Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-467">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="e8938-468">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="e8938-468">passcodeBlockModification</span></span>|<span data-ttu-id="e8938-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-469">Boolean</span></span>|<span data-ttu-id="e8938-470">Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-470">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e8938-471">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e8938-471">passcodeBlockSimple</span></span>|<span data-ttu-id="e8938-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-472">Boolean</span></span>|<span data-ttu-id="e8938-473">Указывает, следует ли блокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="e8938-473">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="e8938-474">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e8938-474">passcodeExpirationDays</span></span>|<span data-ttu-id="e8938-475">Int32</span><span class="sxs-lookup"><span data-stu-id="e8938-475">Int32</span></span>|<span data-ttu-id="e8938-476">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="e8938-476">Number of days before the passcode expires.</span></span> <span data-ttu-id="e8938-477">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="e8938-477">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="e8938-478">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e8938-478">passcodeMinimumLength</span></span>|<span data-ttu-id="e8938-479">Int32</span><span class="sxs-lookup"><span data-stu-id="e8938-479">Int32</span></span>|<span data-ttu-id="e8938-480">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="e8938-480">Minimum length of passcode.</span></span> <span data-ttu-id="e8938-481">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="e8938-481">Valid values 4 to 14</span></span>|
|<span data-ttu-id="e8938-482">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e8938-482">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e8938-483">Int32</span><span class="sxs-lookup"><span data-stu-id="e8938-483">Int32</span></span>|<span data-ttu-id="e8938-484">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="e8938-484">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="e8938-485">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e8938-485">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e8938-486">Int32</span><span class="sxs-lookup"><span data-stu-id="e8938-486">Int32</span></span>|<span data-ttu-id="e8938-487">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="e8938-487">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e8938-488">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e8938-488">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="e8938-489">Int32</span><span class="sxs-lookup"><span data-stu-id="e8938-489">Int32</span></span>|<span data-ttu-id="e8938-490">Количество наборов символов, которые должен содержать секретный код.</span><span class="sxs-lookup"><span data-stu-id="e8938-490">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="e8938-491">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="e8938-491">Valid values 0 to 4</span></span>|
|<span data-ttu-id="e8938-492">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="e8938-492">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="e8938-493">Int32</span><span class="sxs-lookup"><span data-stu-id="e8938-493">Int32</span></span>|<span data-ttu-id="e8938-494">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="e8938-494">Number of previous passcodes to block.</span></span> <span data-ttu-id="e8938-495">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="e8938-495">Valid values 1 to 24</span></span>|
|<span data-ttu-id="e8938-496">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="e8938-496">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="e8938-497">Int32</span><span class="sxs-lookup"><span data-stu-id="e8938-497">Int32</span></span>|<span data-ttu-id="e8938-498">Количество неудачных попыток входа до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="e8938-498">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="e8938-499">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="e8938-499">Valid values 4 to 11</span></span>|
|<span data-ttu-id="e8938-500">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="e8938-500">passcodeRequiredType</span></span>|[<span data-ttu-id="e8938-501">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e8938-501">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="e8938-502">Необходимый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="e8938-502">Type of passcode that is required.</span></span> <span data-ttu-id="e8938-503">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e8938-503">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="e8938-504">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="e8938-504">passcodeRequired</span></span>|<span data-ttu-id="e8938-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-505">Boolean</span></span>|<span data-ttu-id="e8938-506">Указывает, обязательно ли использовать секретный код.</span><span class="sxs-lookup"><span data-stu-id="e8938-506">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="e8938-507">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-507">podcastsBlocked</span></span>|<span data-ttu-id="e8938-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-508">Boolean</span></span>|<span data-ttu-id="e8938-509">Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-509">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="e8938-510">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="e8938-510">safariBlockAutofill</span></span>|<span data-ttu-id="e8938-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-511">Boolean</span></span>|<span data-ttu-id="e8938-512">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="e8938-512">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="e8938-513">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="e8938-513">safariBlockJavaScript</span></span>|<span data-ttu-id="e8938-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-514">Boolean</span></span>|<span data-ttu-id="e8938-515">Указывает, следует ли заблокировать JavaScript в Safari.</span><span class="sxs-lookup"><span data-stu-id="e8938-515">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="e8938-516">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="e8938-516">safariBlockPopups</span></span>|<span data-ttu-id="e8938-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-517">Boolean</span></span>|<span data-ttu-id="e8938-518">Указывает, следует ли блокировать всплывающие окна в Safari.</span><span class="sxs-lookup"><span data-stu-id="e8938-518">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="e8938-519">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-519">safariBlocked</span></span>|<span data-ttu-id="e8938-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-520">Boolean</span></span>|<span data-ttu-id="e8938-521">Указывает, следует ли запретить использовать Safari.</span><span class="sxs-lookup"><span data-stu-id="e8938-521">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="e8938-522">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="e8938-522">safariCookieSettings</span></span>|[<span data-ttu-id="e8938-523">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="e8938-523">webBrowserCookieSettings</span></span>](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|<span data-ttu-id="e8938-524">Настройки файлов cookie для Safari.</span><span class="sxs-lookup"><span data-stu-id="e8938-524">Cookie settings for Safari.</span></span> <span data-ttu-id="e8938-525">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="e8938-525">The possible values are `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`, , , , , , , or .</span></span>|
|<span data-ttu-id="e8938-526">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="e8938-526">safariManagedDomains</span></span>|<span data-ttu-id="e8938-527">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e8938-527">String collection</span></span>|<span data-ttu-id="e8938-528">URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.</span><span class="sxs-lookup"><span data-stu-id="e8938-528">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="e8938-529">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="e8938-529">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="e8938-530">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e8938-530">String collection</span></span>|<span data-ttu-id="e8938-531">Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам.</span><span class="sxs-lookup"><span data-stu-id="e8938-531">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="e8938-532">Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-532">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="e8938-533">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="e8938-533">safariRequireFraudWarning</span></span>|<span data-ttu-id="e8938-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-534">Boolean</span></span>|<span data-ttu-id="e8938-535">Указывает, обязательно ли предупреждение о мошенничестве в Safari.</span><span class="sxs-lookup"><span data-stu-id="e8938-535">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="e8938-536">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-536">screenCaptureBlocked</span></span>|<span data-ttu-id="e8938-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-537">Boolean</span></span>|<span data-ttu-id="e8938-538">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="e8938-538">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="e8938-539">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-539">siriBlocked</span></span>|<span data-ttu-id="e8938-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-540">Boolean</span></span>|<span data-ttu-id="e8938-541">Указывает, следует ли запретить использовать Siri.</span><span class="sxs-lookup"><span data-stu-id="e8938-541">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="e8938-542">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="e8938-542">siriBlockedWhenLocked</span></span>|<span data-ttu-id="e8938-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-543">Boolean</span></span>|<span data-ttu-id="e8938-544">Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="e8938-544">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="e8938-545">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="e8938-545">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="e8938-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-546">Boolean</span></span>|<span data-ttu-id="e8938-547">Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="e8938-547">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="e8938-548">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="e8938-548">siriRequireProfanityFilter</span></span>|<span data-ttu-id="e8938-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-549">Boolean</span></span>|<span data-ttu-id="e8938-550">Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="e8938-550">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="e8938-551">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="e8938-551">spotlightBlockInternetResults</span></span>|<span data-ttu-id="e8938-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-552">Boolean</span></span>|<span data-ttu-id="e8938-553">Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="e8938-553">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="e8938-554">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="e8938-554">voiceDialingBlocked</span></span>|<span data-ttu-id="e8938-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-555">Boolean</span></span>|<span data-ttu-id="e8938-556">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="e8938-556">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="e8938-557">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="e8938-557">wallpaperBlockModification</span></span>|<span data-ttu-id="e8938-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-558">Boolean</span></span>|<span data-ttu-id="e8938-559">Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e8938-559">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="e8938-560">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="e8938-560">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="e8938-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8938-561">Boolean</span></span>|<span data-ttu-id="e8938-562">Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8938-562">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="e8938-563">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8938-563">Response</span></span>
<span data-ttu-id="e8938-564">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8938-564">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8938-565">Пример</span><span class="sxs-lookup"><span data-stu-id="e8938-565">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8938-566">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8938-566">Request</span></span>
<span data-ttu-id="e8938-567">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8938-567">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e8938-568">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8938-568">Response</span></span>
<span data-ttu-id="e8938-p126">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8938-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



