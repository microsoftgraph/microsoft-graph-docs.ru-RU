# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="04e32-101">Обновление windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="04e32-101">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="04e32-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="04e32-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04e32-103">Обновление свойств объекта [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="04e32-103">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04e32-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="04e32-104">Prerequisites</span></span>
<span data-ttu-id="04e32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="04e32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="04e32-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04e32-107">Permission type</span></span>|<span data-ttu-id="04e32-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04e32-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04e32-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04e32-109">Delegated (work or school account)</span></span>|<span data-ttu-id="04e32-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04e32-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="04e32-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04e32-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04e32-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04e32-112">Not supported.</span></span>|
|<span data-ttu-id="04e32-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04e32-113">Application</span></span>|<span data-ttu-id="04e32-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04e32-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04e32-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04e32-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="04e32-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="04e32-116">Request headers</span></span>
|<span data-ttu-id="04e32-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04e32-117">Header</span></span>|<span data-ttu-id="04e32-118">Значение</span><span class="sxs-lookup"><span data-stu-id="04e32-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04e32-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="04e32-119">Authorization</span></span>|<span data-ttu-id="04e32-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04e32-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04e32-121">Accept</span><span class="sxs-lookup"><span data-stu-id="04e32-121">Accept</span></span>|<span data-ttu-id="04e32-122">application/json</span><span class="sxs-lookup"><span data-stu-id="04e32-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04e32-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="04e32-123">Request body</span></span>
<span data-ttu-id="04e32-124">В теле запроса добавьте представление объекта [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04e32-124">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="04e32-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="04e32-125">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="04e32-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="04e32-126">Property</span></span>|<span data-ttu-id="04e32-127">Тип</span><span class="sxs-lookup"><span data-stu-id="04e32-127">Type</span></span>|<span data-ttu-id="04e32-128">Описание</span><span class="sxs-lookup"><span data-stu-id="04e32-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04e32-129">id</span><span class="sxs-lookup"><span data-stu-id="04e32-129">id</span></span>|<span data-ttu-id="04e32-130">String</span><span class="sxs-lookup"><span data-stu-id="04e32-130">String</span></span>|<span data-ttu-id="04e32-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="04e32-131">Key of the entity.</span></span> <span data-ttu-id="04e32-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04e32-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04e32-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04e32-133">lastModifiedDateTime</span></span>|<span data-ttu-id="04e32-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04e32-134">DateTimeOffset</span></span>|<span data-ttu-id="04e32-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="04e32-135">DateTime the object was last modified.</span></span> <span data-ttu-id="04e32-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04e32-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04e32-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04e32-137">createdDateTime</span></span>|<span data-ttu-id="04e32-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04e32-138">DateTimeOffset</span></span>|<span data-ttu-id="04e32-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="04e32-139">DateTime the object was created.</span></span> <span data-ttu-id="04e32-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04e32-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04e32-141">description</span><span class="sxs-lookup"><span data-stu-id="04e32-141">description</span></span>|<span data-ttu-id="04e32-142">String</span><span class="sxs-lookup"><span data-stu-id="04e32-142">String</span></span>|<span data-ttu-id="04e32-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="04e32-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="04e32-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04e32-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04e32-145">displayName</span><span class="sxs-lookup"><span data-stu-id="04e32-145">displayName</span></span>|<span data-ttu-id="04e32-146">String</span><span class="sxs-lookup"><span data-stu-id="04e32-146">String</span></span>|<span data-ttu-id="04e32-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="04e32-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="04e32-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04e32-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04e32-149">version</span><span class="sxs-lookup"><span data-stu-id="04e32-149">version</span></span>|<span data-ttu-id="04e32-150">Int32</span><span class="sxs-lookup"><span data-stu-id="04e32-150">Int32</span></span>|<span data-ttu-id="04e32-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="04e32-151">Version of the device configuration.</span></span> <span data-ttu-id="04e32-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="04e32-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04e32-153">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="04e32-153">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="04e32-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-154">Boolean</span></span>|<span data-ttu-id="04e32-155">Указывает, применяется ли эта политика только к Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="04e32-155">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="04e32-156">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="04e32-156">This property is read-only.</span></span>|
|<span data-ttu-id="04e32-157">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="04e32-157">appsBlockCopyPaste</span></span>|<span data-ttu-id="04e32-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-158">Boolean</span></span>|<span data-ttu-id="04e32-159">Указывает, следует ли заблокировать копирование данных.</span><span class="sxs-lookup"><span data-stu-id="04e32-159">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="04e32-160">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="04e32-160">bluetoothBlocked</span></span>|<span data-ttu-id="04e32-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-161">Boolean</span></span>|<span data-ttu-id="04e32-162">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="04e32-162">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="04e32-163">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="04e32-163">cameraBlocked</span></span>|<span data-ttu-id="04e32-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-164">Boolean</span></span>|<span data-ttu-id="04e32-165">Указывает, следует ли заблокировать камеру.</span><span class="sxs-lookup"><span data-stu-id="04e32-165">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="04e32-166">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="04e32-166">cellularBlockWifiTethering</span></span>|<span data-ttu-id="04e32-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-167">Boolean</span></span>|<span data-ttu-id="04e32-168">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="04e32-168">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="04e32-169">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="04e32-169">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="04e32-170">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="04e32-170">compliantAppsList</span></span>|<span data-ttu-id="04e32-171">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="04e32-171">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="04e32-172">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="04e32-172">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="04e32-173">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="04e32-173">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="04e32-174">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="04e32-174">compliantAppListType</span></span>|[<span data-ttu-id="04e32-175">appListType</span><span class="sxs-lookup"><span data-stu-id="04e32-175">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="04e32-176">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="04e32-176">List that is in the AppComplianceList.</span></span> <span data-ttu-id="04e32-177">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="04e32-177">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="04e32-178">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="04e32-178">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="04e32-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-179">Boolean</span></span>|<span data-ttu-id="04e32-180">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="04e32-180">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="04e32-181">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="04e32-181">emailBlockAddingAccounts</span></span>|<span data-ttu-id="04e32-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-182">Boolean</span></span>|<span data-ttu-id="04e32-183">Указывает, следует ли заблокировать пользовательские учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="04e32-183">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="04e32-184">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="04e32-184">locationServicesBlocked</span></span>|<span data-ttu-id="04e32-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-185">Boolean</span></span>|<span data-ttu-id="04e32-186">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="04e32-186">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="04e32-187">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="04e32-187">microsoftAccountBlocked</span></span>|<span data-ttu-id="04e32-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-188">Boolean</span></span>|<span data-ttu-id="04e32-189">Указывает, следует ли запретить использовать учетную запись Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="04e32-189">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="04e32-190">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="04e32-190">nfcBlocked</span></span>|<span data-ttu-id="04e32-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-191">Boolean</span></span>|<span data-ttu-id="04e32-192">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="04e32-192">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="04e32-193">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="04e32-193">passwordBlockSimple</span></span>|<span data-ttu-id="04e32-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-194">Boolean</span></span>|<span data-ttu-id="04e32-195">Указывает, следует ли заблокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="04e32-195">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="04e32-196">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="04e32-196">passwordExpirationDays</span></span>|<span data-ttu-id="04e32-197">Int32</span><span class="sxs-lookup"><span data-stu-id="04e32-197">Int32</span></span>|<span data-ttu-id="04e32-198">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="04e32-198">Number of days before the password expires.</span></span>|
|<span data-ttu-id="04e32-199">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="04e32-199">passwordMinimumLength</span></span>|<span data-ttu-id="04e32-200">Int32</span><span class="sxs-lookup"><span data-stu-id="04e32-200">Int32</span></span>|<span data-ttu-id="04e32-201">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="04e32-201">Minimum length of passwords.</span></span>|
|<span data-ttu-id="04e32-202">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="04e32-202">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="04e32-203">Int32</span><span class="sxs-lookup"><span data-stu-id="04e32-203">Int32</span></span>|<span data-ttu-id="04e32-204">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="04e32-204">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="04e32-205">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="04e32-205">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="04e32-206">Int32</span><span class="sxs-lookup"><span data-stu-id="04e32-206">Int32</span></span>|<span data-ttu-id="04e32-207">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="04e32-207">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="04e32-208">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="04e32-208">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="04e32-209">Int32</span><span class="sxs-lookup"><span data-stu-id="04e32-209">Int32</span></span>|<span data-ttu-id="04e32-210">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="04e32-210">Number of previous passwords to block.</span></span> <span data-ttu-id="04e32-211">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="04e32-211">Valid values 0 to 24</span></span>|
|<span data-ttu-id="04e32-212">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="04e32-212">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="04e32-213">Int32</span><span class="sxs-lookup"><span data-stu-id="04e32-213">Int32</span></span>|<span data-ttu-id="04e32-214">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="04e32-214">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="04e32-215">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="04e32-215">passwordRequiredType</span></span>|[<span data-ttu-id="04e32-216">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="04e32-216">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="04e32-217">Необходимый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="04e32-217">Password type that is required.</span></span> <span data-ttu-id="04e32-218">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="04e32-218">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="04e32-219">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="04e32-219">passwordRequired</span></span>|<span data-ttu-id="04e32-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-220">Boolean</span></span>|<span data-ttu-id="04e32-221">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="04e32-221">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="04e32-222">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="04e32-222">screenCaptureBlocked</span></span>|<span data-ttu-id="04e32-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-223">Boolean</span></span>|<span data-ttu-id="04e32-224">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="04e32-224">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="04e32-225">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="04e32-225">storageBlockRemovableStorage</span></span>|<span data-ttu-id="04e32-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-226">Boolean</span></span>|<span data-ttu-id="04e32-227">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="04e32-227">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="04e32-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="04e32-228">storageRequireEncryption</span></span>|<span data-ttu-id="04e32-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-229">Boolean</span></span>|<span data-ttu-id="04e32-230">Указывает, обязательно ли шифрование.</span><span class="sxs-lookup"><span data-stu-id="04e32-230">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="04e32-231">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="04e32-231">webBrowserBlocked</span></span>|<span data-ttu-id="04e32-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-232">Boolean</span></span>|<span data-ttu-id="04e32-233">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="04e32-233">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="04e32-234">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="04e32-234">wifiBlocked</span></span>|<span data-ttu-id="04e32-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-235">Boolean</span></span>|<span data-ttu-id="04e32-236">Указывает, следует ли заблокировать Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="04e32-236">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="04e32-237">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="04e32-237">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="04e32-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-238">Boolean</span></span>|<span data-ttu-id="04e32-239">Указывает, следует ли заблокировать автоматическое подключение к хот-спотам Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="04e32-239">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="04e32-240">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="04e32-240">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="04e32-241">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="04e32-241">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="04e32-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-242">Boolean</span></span>|<span data-ttu-id="04e32-243">Указывает, следует ли запретить устройству сообщать об обнаруженных хот-спотах Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="04e32-243">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="04e32-244">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="04e32-244">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="04e32-245">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="04e32-245">windowsStoreBlocked</span></span>|<span data-ttu-id="04e32-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e32-246">Boolean</span></span>|<span data-ttu-id="04e32-247">Указывает, следует ли заблокировать Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="04e32-247">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="04e32-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="04e32-248">Response</span></span>
<span data-ttu-id="04e32-249">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="04e32-249">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04e32-250">Пример</span><span class="sxs-lookup"><span data-stu-id="04e32-250">Example</span></span>
### <a name="request"></a><span data-ttu-id="04e32-251">Запрос</span><span class="sxs-lookup"><span data-stu-id="04e32-251">Request</span></span>
<span data-ttu-id="04e32-252">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04e32-252">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1461

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="04e32-253">Ответ</span><span class="sxs-lookup"><span data-stu-id="04e32-253">Response</span></span>
<span data-ttu-id="04e32-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="04e32-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



