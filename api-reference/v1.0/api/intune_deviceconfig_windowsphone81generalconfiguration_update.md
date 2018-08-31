# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="fe4ec-101">Обновление windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="fe4ec-101">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="fe4ec-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe4ec-103">Обновление свойств объекта [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe4ec-103">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe4ec-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fe4ec-104">Prerequisites</span></span>
<span data-ttu-id="fe4ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe4ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fe4ec-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe4ec-107">Permission type</span></span>|<span data-ttu-id="fe4ec-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe4ec-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe4ec-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe4ec-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fe4ec-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe4ec-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe4ec-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe4ec-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe4ec-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-112">Not supported.</span></span>|
|<span data-ttu-id="fe4ec-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe4ec-113">Application</span></span>|<span data-ttu-id="fe4ec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe4ec-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe4ec-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fe4ec-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe4ec-116">Request headers</span></span>
|<span data-ttu-id="fe4ec-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe4ec-117">Header</span></span>|<span data-ttu-id="fe4ec-118">Значение</span><span class="sxs-lookup"><span data-stu-id="fe4ec-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe4ec-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe4ec-119">Authorization</span></span>|<span data-ttu-id="fe4ec-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="fe4ec-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe4ec-121">Accept</span><span class="sxs-lookup"><span data-stu-id="fe4ec-121">Accept</span></span>|<span data-ttu-id="fe4ec-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fe4ec-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe4ec-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe4ec-123">Request body</span></span>
<span data-ttu-id="fe4ec-124">В теле запроса добавьте представление объекта [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-124">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="fe4ec-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe4ec-125">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="fe4ec-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe4ec-126">Property</span></span>|<span data-ttu-id="fe4ec-127">Тип</span><span class="sxs-lookup"><span data-stu-id="fe4ec-127">Type</span></span>|<span data-ttu-id="fe4ec-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fe4ec-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe4ec-129">ИД</span><span class="sxs-lookup"><span data-stu-id="fe4ec-129">id</span></span>|<span data-ttu-id="fe4ec-130">Строка</span><span class="sxs-lookup"><span data-stu-id="fe4ec-130">String</span></span>|<span data-ttu-id="fe4ec-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-131">Key of the entity.</span></span> <span data-ttu-id="fe4ec-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe4ec-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe4ec-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe4ec-133">lastModifiedDateTime</span></span>|<span data-ttu-id="fe4ec-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe4ec-134">DateTimeOffset</span></span>|<span data-ttu-id="fe4ec-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-135">DateTime the object was last modified.</span></span> <span data-ttu-id="fe4ec-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe4ec-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe4ec-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe4ec-137">createdDateTime</span></span>|<span data-ttu-id="fe4ec-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe4ec-138">DateTimeOffset</span></span>|<span data-ttu-id="fe4ec-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-139">DateTime the object was created.</span></span> <span data-ttu-id="fe4ec-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe4ec-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe4ec-141">описание</span><span class="sxs-lookup"><span data-stu-id="fe4ec-141">description</span></span>|<span data-ttu-id="fe4ec-142">Строковый</span><span class="sxs-lookup"><span data-stu-id="fe4ec-142">String</span></span>|<span data-ttu-id="fe4ec-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fe4ec-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe4ec-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe4ec-145">displayName</span><span class="sxs-lookup"><span data-stu-id="fe4ec-145">displayName</span></span>|<span data-ttu-id="fe4ec-146">Строковый</span><span class="sxs-lookup"><span data-stu-id="fe4ec-146">String</span></span>|<span data-ttu-id="fe4ec-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fe4ec-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe4ec-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe4ec-149">версия</span><span class="sxs-lookup"><span data-stu-id="fe4ec-149">version</span></span>|<span data-ttu-id="fe4ec-150">Int32</span><span class="sxs-lookup"><span data-stu-id="fe4ec-150">Int32</span></span>|<span data-ttu-id="fe4ec-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-151">Version of the device configuration.</span></span> <span data-ttu-id="fe4ec-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe4ec-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe4ec-153">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="fe4ec-153">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="fe4ec-154">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-154">Boolean</span></span>|<span data-ttu-id="fe4ec-155">Указывает, применяется ли эта политика только к Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-155">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="fe4ec-156">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-156">This property is read-only.</span></span>|
|<span data-ttu-id="fe4ec-157">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="fe4ec-157">appsBlockCopyPaste</span></span>|<span data-ttu-id="fe4ec-158">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-158">Boolean</span></span>|<span data-ttu-id="fe4ec-159">Указывает, следует ли заблокировать копирование данных.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-159">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="fe4ec-160">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="fe4ec-160">bluetoothBlocked</span></span>|<span data-ttu-id="fe4ec-161">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-161">Boolean</span></span>|<span data-ttu-id="fe4ec-162">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-162">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="fe4ec-163">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="fe4ec-163">cameraBlocked</span></span>|<span data-ttu-id="fe4ec-164">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-164">Boolean</span></span>|<span data-ttu-id="fe4ec-165">Указывает, следует ли заблокировать камеру.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-165">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="fe4ec-166">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="fe4ec-166">cellularBlockWifiTethering</span></span>|<span data-ttu-id="fe4ec-167">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-167">Boolean</span></span>|<span data-ttu-id="fe4ec-168">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-168">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="fe4ec-169">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-169">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="fe4ec-170">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="fe4ec-170">compliantAppsList</span></span>|<span data-ttu-id="fe4ec-171">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="fe4ec-171">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="fe4ec-172">Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="fe4ec-172">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="fe4ec-173">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-173">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="fe4ec-174">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="fe4ec-174">compliantAppListType</span></span>|[<span data-ttu-id="fe4ec-175">appListType</span><span class="sxs-lookup"><span data-stu-id="fe4ec-175">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="fe4ec-176">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-176">List that is in the AppComplianceList.</span></span> <span data-ttu-id="fe4ec-177">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-177">The possible values are `none`, `appsInListCompliant`, `appsNotInListCompliant`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="fe4ec-178">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="fe4ec-178">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="fe4ec-179">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-179">Boolean</span></span>|<span data-ttu-id="fe4ec-180">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-180">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="fe4ec-181">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="fe4ec-181">emailBlockAddingAccounts</span></span>|<span data-ttu-id="fe4ec-182">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-182">Boolean</span></span>|<span data-ttu-id="fe4ec-183">Указывает, следует ли заблокировать пользовательские учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-183">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="fe4ec-184">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="fe4ec-184">locationServicesBlocked</span></span>|<span data-ttu-id="fe4ec-185">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-185">Boolean</span></span>|<span data-ttu-id="fe4ec-186">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-186">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="fe4ec-187">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="fe4ec-187">microsoftAccountBlocked</span></span>|<span data-ttu-id="fe4ec-188">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-188">Boolean</span></span>|<span data-ttu-id="fe4ec-189">Указывает, следует ли запретить использовать учетную запись Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-189">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="fe4ec-190">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="fe4ec-190">nfcBlocked</span></span>|<span data-ttu-id="fe4ec-191">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-191">Boolean</span></span>|<span data-ttu-id="fe4ec-192">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-192">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="fe4ec-193">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="fe4ec-193">passwordBlockSimple</span></span>|<span data-ttu-id="fe4ec-194">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-194">Boolean</span></span>|<span data-ttu-id="fe4ec-195">Указывает, следует ли заблокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-195">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="fe4ec-196">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="fe4ec-196">passwordExpirationDays</span></span>|<span data-ttu-id="fe4ec-197">Int32</span><span class="sxs-lookup"><span data-stu-id="fe4ec-197">Int32</span></span>|<span data-ttu-id="fe4ec-198">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-198">Number of days before the password expires.</span></span>|
|<span data-ttu-id="fe4ec-199">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fe4ec-199">passwordMinimumLength</span></span>|<span data-ttu-id="fe4ec-200">Int32</span><span class="sxs-lookup"><span data-stu-id="fe4ec-200">Int32</span></span>|<span data-ttu-id="fe4ec-201">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-201">Minimum length of passwords.</span></span>|
|<span data-ttu-id="fe4ec-202">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="fe4ec-202">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="fe4ec-203">Int32</span><span class="sxs-lookup"><span data-stu-id="fe4ec-203">Int32</span></span>|<span data-ttu-id="fe4ec-204">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="fe4ec-204">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="fe4ec-205">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="fe4ec-205">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="fe4ec-206">Int32</span><span class="sxs-lookup"><span data-stu-id="fe4ec-206">Int32</span></span>|<span data-ttu-id="fe4ec-207">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-207">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="fe4ec-208">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="fe4ec-208">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="fe4ec-209">Int32</span><span class="sxs-lookup"><span data-stu-id="fe4ec-209">Int32</span></span>|<span data-ttu-id="fe4ec-210">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-210">Number of previous passwords to block.</span></span> <span data-ttu-id="fe4ec-211">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="fe4ec-211">Valid values 0 to 24</span></span>|
|<span data-ttu-id="fe4ec-212">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="fe4ec-212">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="fe4ec-213">Int32</span><span class="sxs-lookup"><span data-stu-id="fe4ec-213">Int32</span></span>|<span data-ttu-id="fe4ec-214">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-214">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="fe4ec-215">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="fe4ec-215">passwordRequiredType</span></span>|[<span data-ttu-id="fe4ec-216">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="fe4ec-216">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="fe4ec-217">Необходимый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-217">Password type that is required.</span></span> <span data-ttu-id="fe4ec-218">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-218">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="fe4ec-219">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="fe4ec-219">passwordRequired</span></span>|<span data-ttu-id="fe4ec-220">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-220">Boolean</span></span>|<span data-ttu-id="fe4ec-221">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-221">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="fe4ec-222">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="fe4ec-222">screenCaptureBlocked</span></span>|<span data-ttu-id="fe4ec-223">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-223">Boolean</span></span>|<span data-ttu-id="fe4ec-224">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-224">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="fe4ec-225">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="fe4ec-225">storageBlockRemovableStorage</span></span>|<span data-ttu-id="fe4ec-226">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-226">Boolean</span></span>|<span data-ttu-id="fe4ec-227">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-227">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="fe4ec-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="fe4ec-228">storageRequireEncryption</span></span>|<span data-ttu-id="fe4ec-229">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-229">Boolean</span></span>|<span data-ttu-id="fe4ec-230">Указывает, обязательно ли шифрование.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-230">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="fe4ec-231">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="fe4ec-231">webBrowserBlocked</span></span>|<span data-ttu-id="fe4ec-232">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-232">Boolean</span></span>|<span data-ttu-id="fe4ec-233">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-233">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="fe4ec-234">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="fe4ec-234">wifiBlocked</span></span>|<span data-ttu-id="fe4ec-235">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-235">Boolean</span></span>|<span data-ttu-id="fe4ec-236">Указывает, следует ли заблокировать Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-236">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="fe4ec-237">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="fe4ec-237">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="fe4ec-238">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-238">Boolean</span></span>|<span data-ttu-id="fe4ec-239">Указывает, следует ли заблокировать автоматическое подключение к хот-спотам Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-239">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="fe4ec-240">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-240">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="fe4ec-241">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="fe4ec-241">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="fe4ec-242">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-242">Boolean</span></span>|<span data-ttu-id="fe4ec-243">Указывает, следует ли запретить устройству сообщать об обнаруженных хот-спотах Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-243">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="fe4ec-244">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-244">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="fe4ec-245">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="fe4ec-245">windowsStoreBlocked</span></span>|<span data-ttu-id="fe4ec-246">Логический</span><span class="sxs-lookup"><span data-stu-id="fe4ec-246">Boolean</span></span>|<span data-ttu-id="fe4ec-247">Указывает, следует ли заблокировать Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-247">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="fe4ec-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe4ec-248">Response</span></span>
<span data-ttu-id="fe4ec-249">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-249">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe4ec-250">Пример</span><span class="sxs-lookup"><span data-stu-id="fe4ec-250">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe4ec-251">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe4ec-251">Request</span></span>
<span data-ttu-id="fe4ec-252">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-252">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1452

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
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
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="fe4ec-253">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe4ec-253">Response</span></span>
<span data-ttu-id="fe4ec-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe4ec-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
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
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```



