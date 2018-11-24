# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="462ca-101">Create androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="462ca-101">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="462ca-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="462ca-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="462ca-103">Создание нового объекта [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="462ca-103">Create a new [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="462ca-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="462ca-104">Prerequisites</span></span>
<span data-ttu-id="462ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="462ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="462ca-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="462ca-107">Permission type</span></span>|<span data-ttu-id="462ca-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="462ca-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="462ca-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="462ca-109">Delegated (work or school account)</span></span>|<span data-ttu-id="462ca-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="462ca-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="462ca-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="462ca-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="462ca-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="462ca-112">Not supported.</span></span>|
|<span data-ttu-id="462ca-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="462ca-113">Application</span></span>|<span data-ttu-id="462ca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="462ca-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="462ca-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="462ca-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="462ca-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="462ca-116">Request headers</span></span>
|<span data-ttu-id="462ca-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="462ca-117">Header</span></span>|<span data-ttu-id="462ca-118">Значение</span><span class="sxs-lookup"><span data-stu-id="462ca-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="462ca-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="462ca-119">Authorization</span></span>|<span data-ttu-id="462ca-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="462ca-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="462ca-121">Accept</span><span class="sxs-lookup"><span data-stu-id="462ca-121">Accept</span></span>|<span data-ttu-id="462ca-122">application/json</span><span class="sxs-lookup"><span data-stu-id="462ca-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="462ca-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="462ca-123">Request body</span></span>
<span data-ttu-id="462ca-124">В теле запроса добавьте представление объекта androidCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="462ca-124">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="462ca-125">Ниже показаны свойства, которые необходимо указывать при создании объекта androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="462ca-125">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="462ca-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="462ca-126">Property</span></span>|<span data-ttu-id="462ca-127">Тип</span><span class="sxs-lookup"><span data-stu-id="462ca-127">Type</span></span>|<span data-ttu-id="462ca-128">Описание</span><span class="sxs-lookup"><span data-stu-id="462ca-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="462ca-129">id</span><span class="sxs-lookup"><span data-stu-id="462ca-129">id</span></span>|<span data-ttu-id="462ca-130">String</span><span class="sxs-lookup"><span data-stu-id="462ca-130">String</span></span>|<span data-ttu-id="462ca-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="462ca-131">Key of the entity.</span></span> <span data-ttu-id="462ca-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="462ca-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="462ca-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="462ca-133">createdDateTime</span></span>|<span data-ttu-id="462ca-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="462ca-134">DateTimeOffset</span></span>|<span data-ttu-id="462ca-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="462ca-135">DateTime the object was created.</span></span> <span data-ttu-id="462ca-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="462ca-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="462ca-137">description</span><span class="sxs-lookup"><span data-stu-id="462ca-137">description</span></span>|<span data-ttu-id="462ca-138">String</span><span class="sxs-lookup"><span data-stu-id="462ca-138">String</span></span>|<span data-ttu-id="462ca-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="462ca-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="462ca-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="462ca-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="462ca-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="462ca-141">lastModifiedDateTime</span></span>|<span data-ttu-id="462ca-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="462ca-142">DateTimeOffset</span></span>|<span data-ttu-id="462ca-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="462ca-143">DateTime the object was last modified.</span></span> <span data-ttu-id="462ca-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="462ca-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="462ca-145">displayName</span><span class="sxs-lookup"><span data-stu-id="462ca-145">displayName</span></span>|<span data-ttu-id="462ca-146">String</span><span class="sxs-lookup"><span data-stu-id="462ca-146">String</span></span>|<span data-ttu-id="462ca-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="462ca-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="462ca-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="462ca-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="462ca-149">version</span><span class="sxs-lookup"><span data-stu-id="462ca-149">version</span></span>|<span data-ttu-id="462ca-150">Int32</span><span class="sxs-lookup"><span data-stu-id="462ca-150">Int32</span></span>|<span data-ttu-id="462ca-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="462ca-151">Version of the device configuration.</span></span> <span data-ttu-id="462ca-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="462ca-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="462ca-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="462ca-153">passwordRequired</span></span>|<span data-ttu-id="462ca-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="462ca-154">Boolean</span></span>|<span data-ttu-id="462ca-155">Указывает на то, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="462ca-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="462ca-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="462ca-156">passwordMinimumLength</span></span>|<span data-ttu-id="462ca-157">Int32</span><span class="sxs-lookup"><span data-stu-id="462ca-157">Int32</span></span>|<span data-ttu-id="462ca-158">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="462ca-158">Minimum password length.</span></span> <span data-ttu-id="462ca-159">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="462ca-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="462ca-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="462ca-160">passwordRequiredType</span></span>|[<span data-ttu-id="462ca-161">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="462ca-161">androidRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|<span data-ttu-id="462ca-162">Тип символов в поле пароль.</span><span class="sxs-lookup"><span data-stu-id="462ca-162">Type of characters in password.</span></span> <span data-ttu-id="462ca-163">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="462ca-163">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="462ca-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="462ca-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="462ca-165">Int32</span><span class="sxs-lookup"><span data-stu-id="462ca-165">Int32</span></span>|<span data-ttu-id="462ca-166">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="462ca-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="462ca-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="462ca-167">passwordExpirationDays</span></span>|<span data-ttu-id="462ca-168">Int32</span><span class="sxs-lookup"><span data-stu-id="462ca-168">Int32</span></span>|<span data-ttu-id="462ca-169">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="462ca-169">Number of days before the password expires.</span></span> <span data-ttu-id="462ca-170">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="462ca-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="462ca-171">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="462ca-171">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="462ca-172">Int32</span><span class="sxs-lookup"><span data-stu-id="462ca-172">Int32</span></span>|<span data-ttu-id="462ca-173">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="462ca-173">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="462ca-174">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="462ca-174">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="462ca-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="462ca-175">Boolean</span></span>|<span data-ttu-id="462ca-176">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="462ca-176">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="462ca-177">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="462ca-177">securityDisableUsbDebugging</span></span>|<span data-ttu-id="462ca-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="462ca-178">Boolean</span></span>|<span data-ttu-id="462ca-179">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="462ca-179">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="462ca-180">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="462ca-180">securityRequireVerifyApps</span></span>|<span data-ttu-id="462ca-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="462ca-181">Boolean</span></span>|<span data-ttu-id="462ca-182">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="462ca-182">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="462ca-183">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="462ca-183">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="462ca-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="462ca-184">Boolean</span></span>|<span data-ttu-id="462ca-185">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="462ca-185">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="462ca-186">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="462ca-186">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="462ca-187">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="462ca-187">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="462ca-188">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="462ca-188">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="462ca-189">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="462ca-189">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="462ca-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="462ca-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="462ca-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="462ca-191">Boolean</span></span>|<span data-ttu-id="462ca-192">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="462ca-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="462ca-193">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="462ca-193">osMinimumVersion</span></span>|<span data-ttu-id="462ca-194">String</span><span class="sxs-lookup"><span data-stu-id="462ca-194">String</span></span>|<span data-ttu-id="462ca-195">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="462ca-195">Minimum Android version.</span></span>|
|<span data-ttu-id="462ca-196">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="462ca-196">osMaximumVersion</span></span>|<span data-ttu-id="462ca-197">String</span><span class="sxs-lookup"><span data-stu-id="462ca-197">String</span></span>|<span data-ttu-id="462ca-198">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="462ca-198">Maximum Android version.</span></span>|
|<span data-ttu-id="462ca-199">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="462ca-199">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="462ca-200">String</span><span class="sxs-lookup"><span data-stu-id="462ca-200">String</span></span>|<span data-ttu-id="462ca-201">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="462ca-201">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="462ca-202">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="462ca-202">storageRequireEncryption</span></span>|<span data-ttu-id="462ca-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="462ca-203">Boolean</span></span>|<span data-ttu-id="462ca-204">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="462ca-204">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="462ca-205">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="462ca-205">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="462ca-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="462ca-206">Boolean</span></span>|<span data-ttu-id="462ca-207">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="462ca-207">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="462ca-208">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="462ca-208">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="462ca-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="462ca-209">Boolean</span></span>|<span data-ttu-id="462ca-210">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="462ca-210">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="462ca-211">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="462ca-211">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="462ca-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="462ca-212">Boolean</span></span>|<span data-ttu-id="462ca-213">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="462ca-213">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="462ca-214">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="462ca-214">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="462ca-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="462ca-215">Boolean</span></span>|<span data-ttu-id="462ca-216">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="462ca-216">Require the device to have up to date security providers.</span></span> <span data-ttu-id="462ca-217">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="462ca-217">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="462ca-218">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="462ca-218">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="462ca-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="462ca-219">Boolean</span></span>|<span data-ttu-id="462ca-220">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="462ca-220">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="462ca-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="462ca-221">Response</span></span>
<span data-ttu-id="462ca-222">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="462ca-222">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="462ca-223">Пример</span><span class="sxs-lookup"><span data-stu-id="462ca-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="462ca-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="462ca-224">Request</span></span>
<span data-ttu-id="462ca-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="462ca-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1159

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```

### <a name="response"></a><span data-ttu-id="462ca-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="462ca-226">Response</span></span>
<span data-ttu-id="462ca-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="462ca-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "id": "752c820f-820f-752c-0f82-2c750f822c75",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```



