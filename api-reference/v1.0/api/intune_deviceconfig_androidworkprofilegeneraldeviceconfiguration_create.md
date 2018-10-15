# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="6b0bb-101">Создание androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="6b0bb-101">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="6b0bb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b0bb-103">Создание нового объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b0bb-103">Create a new [deviceConfigurationAssignment](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6b0bb-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6b0bb-104">Prerequisites</span></span>
<span data-ttu-id="6b0bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6b0bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6b0bb-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b0bb-107">Permission type</span></span>|<span data-ttu-id="6b0bb-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b0bb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b0bb-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b0bb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6b0bb-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b0bb-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b0bb-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b0bb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b0bb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-112">Not supported.</span></span>|
|<span data-ttu-id="6b0bb-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b0bb-113">Application</span></span>|<span data-ttu-id="6b0bb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b0bb-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b0bb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6b0bb-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b0bb-116">Request headers</span></span>
|<span data-ttu-id="6b0bb-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b0bb-117">Header</span></span>|<span data-ttu-id="6b0bb-118">Значение</span><span class="sxs-lookup"><span data-stu-id="6b0bb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b0bb-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b0bb-119">Authorization</span></span>|<span data-ttu-id="6b0bb-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="6b0bb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b0bb-121">Принять</span><span class="sxs-lookup"><span data-stu-id="6b0bb-121">Accept</span></span>|<span data-ttu-id="6b0bb-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="6b0bb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b0bb-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b0bb-123">Request body</span></span>
<span data-ttu-id="6b0bb-124">В тексте запроса укажите представление объекта androidWorkProfileGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-124">In the request body, supply a JSON representation for the deviceManagement object.</span></span>

<span data-ttu-id="6b0bb-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта androidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-125">The following table shows the properties that are required when you create the deviceAppManagement.</span></span>

|<span data-ttu-id="6b0bb-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b0bb-126">Property</span></span>|<span data-ttu-id="6b0bb-127">Тип</span><span class="sxs-lookup"><span data-stu-id="6b0bb-127">Type</span></span>|<span data-ttu-id="6b0bb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6b0bb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b0bb-129">id</span><span class="sxs-lookup"><span data-stu-id="6b0bb-129">id</span></span>|<span data-ttu-id="6b0bb-130">Строка</span><span class="sxs-lookup"><span data-stu-id="6b0bb-130">String</span></span>|<span data-ttu-id="6b0bb-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-131">Key of the entity.</span></span> <span data-ttu-id="6b0bb-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b0bb-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b0bb-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b0bb-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6b0bb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b0bb-134">DateTimeOffset</span></span>|<span data-ttu-id="6b0bb-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-135">DateTime the object was last modified.</span></span> <span data-ttu-id="6b0bb-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b0bb-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b0bb-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b0bb-137">createdDateTime</span></span>|<span data-ttu-id="6b0bb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b0bb-138">DateTimeOffset</span></span>|<span data-ttu-id="6b0bb-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-139">DateTime the object was created.</span></span> <span data-ttu-id="6b0bb-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b0bb-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b0bb-141">описание</span><span class="sxs-lookup"><span data-stu-id="6b0bb-141">description</span></span>|<span data-ttu-id="6b0bb-142">Строка</span><span class="sxs-lookup"><span data-stu-id="6b0bb-142">String</span></span>|<span data-ttu-id="6b0bb-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6b0bb-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b0bb-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b0bb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="6b0bb-145">displayName</span></span>|<span data-ttu-id="6b0bb-146">Строка</span><span class="sxs-lookup"><span data-stu-id="6b0bb-146">String</span></span>|<span data-ttu-id="6b0bb-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6b0bb-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b0bb-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b0bb-149">version</span><span class="sxs-lookup"><span data-stu-id="6b0bb-149">version</span></span>|<span data-ttu-id="6b0bb-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-150">Int32</span></span>|<span data-ttu-id="6b0bb-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-151">Version of the device configuration.</span></span> <span data-ttu-id="6b0bb-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b0bb-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b0bb-153">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6b0bb-153">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="6b0bb-154">Логический</span><span class="sxs-lookup"><span data-stu-id="6b0bb-154">Boolean</span></span>|<span data-ttu-id="6b0bb-155">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-155">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="6b0bb-156">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="6b0bb-156">passwordBlockTrustAgents</span></span>|<span data-ttu-id="6b0bb-157">Логический</span><span class="sxs-lookup"><span data-stu-id="6b0bb-157">Boolean</span></span>|<span data-ttu-id="6b0bb-158">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-158">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="6b0bb-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6b0bb-159">passwordExpirationDays</span></span>|<span data-ttu-id="6b0bb-160">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-160">Int32</span></span>|<span data-ttu-id="6b0bb-161">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-161">Number of days before the password expires.</span></span> <span data-ttu-id="6b0bb-162">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-162">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6b0bb-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6b0bb-163">passwordMinimumLength</span></span>|<span data-ttu-id="6b0bb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-164">Int32</span></span>|<span data-ttu-id="6b0bb-165">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-165">Minimum length of passwords.</span></span> <span data-ttu-id="6b0bb-166">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6b0bb-167">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6b0bb-167">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6b0bb-168">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-168">Int32</span></span>|<span data-ttu-id="6b0bb-169">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="6b0bb-169">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6b0bb-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6b0bb-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6b0bb-171">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-171">Int32</span></span>|<span data-ttu-id="6b0bb-172">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-172">Number of previous passwords to block.</span></span> <span data-ttu-id="6b0bb-173">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="6b0bb-173">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6b0bb-174">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="6b0bb-174">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="6b0bb-175">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-175">Int32</span></span>|<span data-ttu-id="6b0bb-176">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-176">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="6b0bb-177">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="6b0bb-177">Valid values 4 to 11</span></span>|
|<span data-ttu-id="6b0bb-178">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6b0bb-178">passwordRequiredType</span></span>|[<span data-ttu-id="6b0bb-179">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6b0bb-179">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="6b0bb-180">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-180">Type of password that is required.</span></span> <span data-ttu-id="6b0bb-181">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-181">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="6b0bb-182">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="6b0bb-182">workProfileDataSharingType</span></span>|[<span data-ttu-id="6b0bb-183">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="6b0bb-183">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune_deviceconfig_androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="6b0bb-184">Разрешенный тип общего доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-184">Type of data sharing that is allowed.</span></span> <span data-ttu-id="6b0bb-185">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-185">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="6b0bb-186">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="6b0bb-186">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="6b0bb-187">Логическое</span><span class="sxs-lookup"><span data-stu-id="6b0bb-187">Boolean</span></span>|<span data-ttu-id="6b0bb-188">Указывает, следует ли блокировать уведомления, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-188">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="6b0bb-189">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="6b0bb-189">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="6b0bb-190">Логическое</span><span class="sxs-lookup"><span data-stu-id="6b0bb-190">Boolean</span></span>|<span data-ttu-id="6b0bb-191">Установка запрета для пользователей на добавление или удаление учетных записей в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-191">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="6b0bb-192">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="6b0bb-192">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="6b0bb-193">Логическое</span><span class="sxs-lookup"><span data-stu-id="6b0bb-193">Boolean</span></span>|<span data-ttu-id="6b0bb-194">Разрешение устройствам bluetooth получать доступ к контактам предприятия.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-194">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="6b0bb-195">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="6b0bb-195">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="6b0bb-196">Логическое</span><span class="sxs-lookup"><span data-stu-id="6b0bb-196">Boolean</span></span>|<span data-ttu-id="6b0bb-197">Установка запрета на снимок экрана в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-197">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="6b0bb-198">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="6b0bb-198">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="6b0bb-199">Логическое</span><span class="sxs-lookup"><span data-stu-id="6b0bb-199">Boolean</span></span>|<span data-ttu-id="6b0bb-200">Установка запрета на отображение в личном профиле идентификатора вызывающего абонента рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-200">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="6b0bb-201">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="6b0bb-201">workProfileBlockCamera</span></span>|<span data-ttu-id="6b0bb-202">Логическое</span><span class="sxs-lookup"><span data-stu-id="6b0bb-202">Boolean</span></span>|<span data-ttu-id="6b0bb-203">Блокировка камеры рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-203">Block work profile camera.</span></span>|
|<span data-ttu-id="6b0bb-204">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="6b0bb-204">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="6b0bb-205">Логическое</span><span class="sxs-lookup"><span data-stu-id="6b0bb-205">Boolean</span></span>|<span data-ttu-id="6b0bb-206">Блокировка доступности контактов рабочего профиля в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-206">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="6b0bb-207">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="6b0bb-207">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="6b0bb-208">Логическое</span><span class="sxs-lookup"><span data-stu-id="6b0bb-208">Boolean</span></span>|<span data-ttu-id="6b0bb-209">Логическое значение, которое указывает, включена ли настройка запрета копирования или вставки между профилями.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-209">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="6b0bb-210">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="6b0bb-210">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="6b0bb-211">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="6b0bb-211">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune_deviceconfig_androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="6b0bb-212">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-212">Type of password that is required.</span></span> <span data-ttu-id="6b0bb-213">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-213">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="6b0bb-214">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6b0bb-214">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="6b0bb-215">Логическое</span><span class="sxs-lookup"><span data-stu-id="6b0bb-215">Boolean</span></span>|<span data-ttu-id="6b0bb-216">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца для рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-216">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="6b0bb-217">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="6b0bb-217">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="6b0bb-218">Логическое</span><span class="sxs-lookup"><span data-stu-id="6b0bb-218">Boolean</span></span>|<span data-ttu-id="6b0bb-219">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности для рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-219">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="6b0bb-220">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6b0bb-220">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="6b0bb-221">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-221">Int32</span></span>|<span data-ttu-id="6b0bb-222">Количество дней до окончания срока действия пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-222">Number of days before the password expires.</span></span> <span data-ttu-id="6b0bb-223">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-223">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6b0bb-224">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6b0bb-224">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="6b0bb-225">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-225">Int32</span></span>|<span data-ttu-id="6b0bb-226">Минимальная длина пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-226">Minimum length of work profile password.</span></span> <span data-ttu-id="6b0bb-227">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-227">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6b0bb-228">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="6b0bb-228">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="6b0bb-229">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-229">Int32</span></span>|<span data-ttu-id="6b0bb-230">Требуемое минимальное количество цифровых символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-230">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="6b0bb-231">Допустимые значения: от 1 до 10.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-231">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6b0bb-232">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6b0bb-232">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="6b0bb-233">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-233">Int32</span></span>|<span data-ttu-id="6b0bb-234">Требуемое минимальное количество небуквенных символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-234">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="6b0bb-235">Допустимые значения: от 1 до 10.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-235">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6b0bb-236">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6b0bb-236">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="6b0bb-237">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-237">Int32</span></span>|<span data-ttu-id="6b0bb-238">Требуемое минимальное количество буквенных символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-238">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="6b0bb-239">Допустимые значения: от 1 до 10.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-239">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6b0bb-240">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6b0bb-240">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="6b0bb-241">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-241">Int32</span></span>|<span data-ttu-id="6b0bb-242">Требуемое минимальное количество строчных букв в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-242">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="6b0bb-243">Допустимые значения: от 1 до 10.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-243">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6b0bb-244">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6b0bb-244">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="6b0bb-245">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-245">Int32</span></span>|<span data-ttu-id="6b0bb-246">Требуемое минимальное количество прописных букв в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-246">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="6b0bb-247">Допустимые значения: от 1 до 10.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-247">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6b0bb-248">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="6b0bb-248">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="6b0bb-249">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-249">Int32</span></span>|<span data-ttu-id="6b0bb-250">Требуемое минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-250">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="6b0bb-251">Допустимые значения: от 1 до 10.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-251">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6b0bb-252">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6b0bb-252">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6b0bb-253">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-253">Int32</span></span>|<span data-ttu-id="6b0bb-254">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="6b0bb-254">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6b0bb-255">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6b0bb-255">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6b0bb-256">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-256">Int32</span></span>|<span data-ttu-id="6b0bb-257">Количество предыдущих паролей рабочего профиля, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-257">Number of previous passwords to block.</span></span> <span data-ttu-id="6b0bb-258">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-258">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6b0bb-259">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="6b0bb-259">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="6b0bb-260">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0bb-260">Int32</span></span>|<span data-ttu-id="6b0bb-261">Количество неудачных попыток входа до удаления рабочего профиля и всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-261">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="6b0bb-262">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="6b0bb-262">Valid values 4 to 11</span></span>|
|<span data-ttu-id="6b0bb-263">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6b0bb-263">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="6b0bb-264">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6b0bb-264">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="6b0bb-265">Требуемый тип пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-265">Type of password that is required.</span></span> <span data-ttu-id="6b0bb-266">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-266">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="6b0bb-267">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="6b0bb-267">workProfileRequirePassword</span></span>|<span data-ttu-id="6b0bb-268">Логическое</span><span class="sxs-lookup"><span data-stu-id="6b0bb-268">Boolean</span></span>|<span data-ttu-id="6b0bb-269">Требуется ли пароль для рабочего профиля</span><span class="sxs-lookup"><span data-stu-id="6b0bb-269">Password is required or not for work profile</span></span>|
|<span data-ttu-id="6b0bb-270">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="6b0bb-270">securityRequireVerifyApps</span></span>|<span data-ttu-id="6b0bb-271">Логический</span><span class="sxs-lookup"><span data-stu-id="6b0bb-271">Boolean</span></span>|<span data-ttu-id="6b0bb-272">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-272">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="6b0bb-273">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b0bb-273">Response</span></span>
<span data-ttu-id="6b0bb-274">В случае успешного выполнения этот метод возвращает `201 Created` код ответа и объект [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-274">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b0bb-275">Пример</span><span class="sxs-lookup"><span data-stu-id="6b0bb-275">Example</span></span>
### <a name="request"></a><span data-ttu-id="6b0bb-276">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b0bb-276">Request</span></span>
<span data-ttu-id="6b0bb-277">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-277">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1895

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="6b0bb-278">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b0bb-278">Response</span></span>
<span data-ttu-id="6b0bb-p126">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b0bb-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```








