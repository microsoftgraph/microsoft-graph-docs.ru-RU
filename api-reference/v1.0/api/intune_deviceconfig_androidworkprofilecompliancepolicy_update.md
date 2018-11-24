# <a name="update-androidworkprofilecompliancepolicy"></a><span data-ttu-id="c00ec-101">Обновление androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c00ec-101">Update androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="c00ec-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c00ec-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c00ec-103">Обновление свойства объекта [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="c00ec-103">Update the properties of a [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c00ec-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c00ec-104">Prerequisites</span></span>
<span data-ttu-id="c00ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c00ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c00ec-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c00ec-107">Permission type</span></span>|<span data-ttu-id="c00ec-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c00ec-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c00ec-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c00ec-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c00ec-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c00ec-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c00ec-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c00ec-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c00ec-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c00ec-112">Not supported.</span></span>|
|<span data-ttu-id="c00ec-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c00ec-113">Application</span></span>|<span data-ttu-id="c00ec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c00ec-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c00ec-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c00ec-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="c00ec-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c00ec-116">Request headers</span></span>
|<span data-ttu-id="c00ec-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c00ec-117">Header</span></span>|<span data-ttu-id="c00ec-118">Значение</span><span class="sxs-lookup"><span data-stu-id="c00ec-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c00ec-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c00ec-119">Authorization</span></span>|<span data-ttu-id="c00ec-120">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c00ec-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c00ec-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c00ec-121">Accept</span></span>|<span data-ttu-id="c00ec-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c00ec-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c00ec-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c00ec-123">Request body</span></span>
<span data-ttu-id="c00ec-124">В тексте запроса укажите представление JSON для объекта [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="c00ec-124">In the request body, supply a JSON representation for the [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="c00ec-125">В следующей таблице показаны свойства, которые необходимы для создания [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c00ec-125">The following table shows the properties that are required when you create the [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md).</span></span>

|<span data-ttu-id="c00ec-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c00ec-126">Property</span></span>|<span data-ttu-id="c00ec-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c00ec-127">Type</span></span>|<span data-ttu-id="c00ec-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c00ec-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c00ec-129">id</span><span class="sxs-lookup"><span data-stu-id="c00ec-129">id</span></span>|<span data-ttu-id="c00ec-130">String</span><span class="sxs-lookup"><span data-stu-id="c00ec-130">String</span></span>|<span data-ttu-id="c00ec-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c00ec-131">Key of the entity.</span></span> <span data-ttu-id="c00ec-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c00ec-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c00ec-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c00ec-133">createdDateTime</span></span>|<span data-ttu-id="c00ec-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c00ec-134">DateTimeOffset</span></span>|<span data-ttu-id="c00ec-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c00ec-135">DateTime the object was created.</span></span> <span data-ttu-id="c00ec-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c00ec-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c00ec-137">описание</span><span class="sxs-lookup"><span data-stu-id="c00ec-137">description</span></span>|<span data-ttu-id="c00ec-138">String</span><span class="sxs-lookup"><span data-stu-id="c00ec-138">String</span></span>|<span data-ttu-id="c00ec-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c00ec-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c00ec-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c00ec-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c00ec-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c00ec-141">lastModifiedDateTime</span></span>|<span data-ttu-id="c00ec-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c00ec-142">DateTimeOffset</span></span>|<span data-ttu-id="c00ec-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c00ec-143">DateTime the object was last modified.</span></span> <span data-ttu-id="c00ec-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c00ec-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c00ec-145">displayName</span><span class="sxs-lookup"><span data-stu-id="c00ec-145">displayName</span></span>|<span data-ttu-id="c00ec-146">String</span><span class="sxs-lookup"><span data-stu-id="c00ec-146">String</span></span>|<span data-ttu-id="c00ec-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c00ec-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c00ec-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c00ec-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c00ec-149">version</span><span class="sxs-lookup"><span data-stu-id="c00ec-149">version</span></span>|<span data-ttu-id="c00ec-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c00ec-150">Int32</span></span>|<span data-ttu-id="c00ec-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c00ec-151">Version of the device configuration.</span></span> <span data-ttu-id="c00ec-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c00ec-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c00ec-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c00ec-153">passwordRequired</span></span>|<span data-ttu-id="c00ec-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="c00ec-154">Boolean</span></span>|<span data-ttu-id="c00ec-155">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="c00ec-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="c00ec-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c00ec-156">passwordMinimumLength</span></span>|<span data-ttu-id="c00ec-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c00ec-157">Int32</span></span>|<span data-ttu-id="c00ec-158">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="c00ec-158">Minimum password length.</span></span> <span data-ttu-id="c00ec-159">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="c00ec-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c00ec-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c00ec-160">passwordRequiredType</span></span>|[<span data-ttu-id="c00ec-161">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c00ec-161">androidRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|<span data-ttu-id="c00ec-162">Тип символов в поле пароль.</span><span class="sxs-lookup"><span data-stu-id="c00ec-162">Type of characters in password.</span></span> <span data-ttu-id="c00ec-163">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="c00ec-163">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="c00ec-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c00ec-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c00ec-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c00ec-165">Int32</span></span>|<span data-ttu-id="c00ec-166">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="c00ec-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c00ec-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c00ec-167">passwordExpirationDays</span></span>|<span data-ttu-id="c00ec-168">Int32</span><span class="sxs-lookup"><span data-stu-id="c00ec-168">Int32</span></span>|<span data-ttu-id="c00ec-169">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="c00ec-169">Number of days before the password expires.</span></span> <span data-ttu-id="c00ec-170">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="c00ec-170">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c00ec-171">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c00ec-171">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c00ec-172">Int32</span><span class="sxs-lookup"><span data-stu-id="c00ec-172">Int32</span></span>|<span data-ttu-id="c00ec-173">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="c00ec-173">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="c00ec-174">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="c00ec-174">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="c00ec-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="c00ec-175">Boolean</span></span>|<span data-ttu-id="c00ec-176">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="c00ec-176">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="c00ec-177">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="c00ec-177">securityDisableUsbDebugging</span></span>|<span data-ttu-id="c00ec-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="c00ec-178">Boolean</span></span>|<span data-ttu-id="c00ec-179">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="c00ec-179">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="c00ec-180">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="c00ec-180">securityRequireVerifyApps</span></span>|<span data-ttu-id="c00ec-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="c00ec-181">Boolean</span></span>|<span data-ttu-id="c00ec-182">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="c00ec-182">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="c00ec-183">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c00ec-183">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="c00ec-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="c00ec-184">Boolean</span></span>|<span data-ttu-id="c00ec-185">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="c00ec-185">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="c00ec-186">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c00ec-186">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c00ec-187">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="c00ec-187">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="c00ec-188">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="c00ec-188">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c00ec-189">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="c00ec-189">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c00ec-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="c00ec-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="c00ec-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="c00ec-191">Boolean</span></span>|<span data-ttu-id="c00ec-192">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="c00ec-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="c00ec-193">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c00ec-193">osMinimumVersion</span></span>|<span data-ttu-id="c00ec-194">String</span><span class="sxs-lookup"><span data-stu-id="c00ec-194">String</span></span>|<span data-ttu-id="c00ec-195">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="c00ec-195">Minimum Android version.</span></span>|
|<span data-ttu-id="c00ec-196">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c00ec-196">osMaximumVersion</span></span>|<span data-ttu-id="c00ec-197">String</span><span class="sxs-lookup"><span data-stu-id="c00ec-197">String</span></span>|<span data-ttu-id="c00ec-198">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="c00ec-198">Maximum Android version.</span></span>|
|<span data-ttu-id="c00ec-199">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="c00ec-199">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="c00ec-200">String</span><span class="sxs-lookup"><span data-stu-id="c00ec-200">String</span></span>|<span data-ttu-id="c00ec-201">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="c00ec-201">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="c00ec-202">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c00ec-202">storageRequireEncryption</span></span>|<span data-ttu-id="c00ec-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="c00ec-203">Boolean</span></span>|<span data-ttu-id="c00ec-204">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="c00ec-204">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="c00ec-205">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="c00ec-205">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="c00ec-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="c00ec-206">Boolean</span></span>|<span data-ttu-id="c00ec-207">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="c00ec-207">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="c00ec-208">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="c00ec-208">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="c00ec-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="c00ec-209">Boolean</span></span>|<span data-ttu-id="c00ec-210">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="c00ec-210">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="c00ec-211">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="c00ec-211">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="c00ec-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="c00ec-212">Boolean</span></span>|<span data-ttu-id="c00ec-213">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="c00ec-213">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="c00ec-214">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="c00ec-214">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="c00ec-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="c00ec-215">Boolean</span></span>|<span data-ttu-id="c00ec-216">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="c00ec-216">Require the device to have up to date security providers.</span></span> <span data-ttu-id="c00ec-217">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="c00ec-217">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="c00ec-218">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="c00ec-218">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="c00ec-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="c00ec-219">Boolean</span></span>|<span data-ttu-id="c00ec-220">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="c00ec-220">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="c00ec-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="c00ec-221">Response</span></span>
<span data-ttu-id="c00ec-222">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c00ec-222">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c00ec-223">Пример</span><span class="sxs-lookup"><span data-stu-id="c00ec-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="c00ec-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="c00ec-224">Request</span></span>
<span data-ttu-id="c00ec-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c00ec-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1170

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="c00ec-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="c00ec-226">Response</span></span>
<span data-ttu-id="c00ec-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c00ec-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1342

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "id": "4e385271-5271-4e38-7152-384e7152384e",
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



