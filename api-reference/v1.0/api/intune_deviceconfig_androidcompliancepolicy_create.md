# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="5f73d-101">Create androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5f73d-101">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="5f73d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5f73d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f73d-103">Создание нового объекта [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f73d-103">Create a new [plannerBucket](../resources/intune_deviceconfig_androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f73d-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5f73d-104">Prerequisites</span></span>
<span data-ttu-id="5f73d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5f73d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5f73d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f73d-107">Permission type</span></span>|<span data-ttu-id="5f73d-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f73d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f73d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f73d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5f73d-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f73d-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5f73d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f73d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f73d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f73d-112">Not supported.</span></span>|
|<span data-ttu-id="5f73d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f73d-113">Application</span></span>|<span data-ttu-id="5f73d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f73d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f73d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f73d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="5f73d-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5f73d-116">Request headers</span></span>
|<span data-ttu-id="5f73d-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f73d-117">Header</span></span>|<span data-ttu-id="5f73d-118">Значение</span><span class="sxs-lookup"><span data-stu-id="5f73d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f73d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f73d-119">Authorization</span></span>|<span data-ttu-id="5f73d-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f73d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5f73d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5f73d-121">Accept</span></span>|<span data-ttu-id="5f73d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5f73d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f73d-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5f73d-123">Request body</span></span>
<span data-ttu-id="5f73d-124">В теле запроса добавьте представление объекта androidCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f73d-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="5f73d-125">Ниже показаны свойства, которые необходимо указывать при создании объекта androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="5f73d-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5f73d-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f73d-126">Property</span></span>|<span data-ttu-id="5f73d-127">Тип</span><span class="sxs-lookup"><span data-stu-id="5f73d-127">Type</span></span>|<span data-ttu-id="5f73d-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5f73d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f73d-129">id</span><span class="sxs-lookup"><span data-stu-id="5f73d-129">id</span></span>|<span data-ttu-id="5f73d-130">String</span><span class="sxs-lookup"><span data-stu-id="5f73d-130">String</span></span>|<span data-ttu-id="5f73d-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5f73d-131">Key of the setting.</span></span> <span data-ttu-id="5f73d-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f73d-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5f73d-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f73d-133">createdDateTime</span></span>|<span data-ttu-id="5f73d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f73d-134">DateTimeOffset</span></span>|<span data-ttu-id="5f73d-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5f73d-135">DateTime the object was created.</span></span> <span data-ttu-id="5f73d-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f73d-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5f73d-137">description</span><span class="sxs-lookup"><span data-stu-id="5f73d-137">description</span></span>|<span data-ttu-id="5f73d-138">String</span><span class="sxs-lookup"><span data-stu-id="5f73d-138">String</span></span>|<span data-ttu-id="5f73d-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5f73d-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5f73d-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f73d-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5f73d-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f73d-141">lastModifiedDateTime</span></span>|<span data-ttu-id="5f73d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f73d-142">DateTimeOffset</span></span>|<span data-ttu-id="5f73d-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5f73d-143">DateTime the object was last modified.</span></span> <span data-ttu-id="5f73d-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f73d-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5f73d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5f73d-145">displayName</span></span>|<span data-ttu-id="5f73d-146">String</span><span class="sxs-lookup"><span data-stu-id="5f73d-146">String</span></span>|<span data-ttu-id="5f73d-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5f73d-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5f73d-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f73d-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5f73d-149">version</span><span class="sxs-lookup"><span data-stu-id="5f73d-149">version</span></span>|<span data-ttu-id="5f73d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5f73d-150">Int32</span></span>|<span data-ttu-id="5f73d-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5f73d-151">Version of the device configuration.</span></span> <span data-ttu-id="5f73d-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f73d-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5f73d-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5f73d-153">passwordRequired</span></span>|<span data-ttu-id="5f73d-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f73d-154">Boolean</span></span>|<span data-ttu-id="5f73d-155">Указывает на то, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="5f73d-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="5f73d-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5f73d-156">passwordMinimumLength</span></span>|<span data-ttu-id="5f73d-157">Int32</span><span class="sxs-lookup"><span data-stu-id="5f73d-157">Int32</span></span>|<span data-ttu-id="5f73d-158">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="5f73d-158">Minimum password length.</span></span> <span data-ttu-id="5f73d-159">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="5f73d-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="5f73d-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5f73d-160">passwordRequiredType</span></span>|<span data-ttu-id="5f73d-161">String</span><span class="sxs-lookup"><span data-stu-id="5f73d-161">String</span></span>|<span data-ttu-id="5f73d-162">Тип символов в пароле. Допустимые значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="5f73d-162">Type of characters in password Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="5f73d-163">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5f73d-163">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5f73d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5f73d-164">Int32</span></span>|<span data-ttu-id="5f73d-165">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="5f73d-165">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="5f73d-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5f73d-166">passwordExpirationDays</span></span>|<span data-ttu-id="5f73d-167">Int32</span><span class="sxs-lookup"><span data-stu-id="5f73d-167">Int32</span></span>|<span data-ttu-id="5f73d-168">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="5f73d-168">Number of days before the password expires.</span></span> <span data-ttu-id="5f73d-169">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="5f73d-169">Valid values 1 to 365</span></span>|
|<span data-ttu-id="5f73d-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5f73d-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5f73d-171">Int32</span><span class="sxs-lookup"><span data-stu-id="5f73d-171">Int32</span></span>|<span data-ttu-id="5f73d-172">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="5f73d-172">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="5f73d-173">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="5f73d-173">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="5f73d-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f73d-174">Boolean</span></span>|<span data-ttu-id="5f73d-175">Указывает на то, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="5f73d-175">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="5f73d-176">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="5f73d-176">securityDisableUsbDebugging</span></span>|<span data-ttu-id="5f73d-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f73d-177">Boolean</span></span>|<span data-ttu-id="5f73d-178">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="5f73d-178">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="5f73d-179">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="5f73d-179">securityRequireVerifyApps</span></span>|<span data-ttu-id="5f73d-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f73d-180">Boolean</span></span>|<span data-ttu-id="5f73d-181">Указывает на то, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="5f73d-181">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="5f73d-182">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5f73d-182">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="5f73d-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f73d-183">Boolean</span></span>|<span data-ttu-id="5f73d-184">Указывает на то, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="5f73d-184">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="5f73d-185">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="5f73d-185">deviceThreatProtectionRequiredSecurityLevel</span></span>|<span data-ttu-id="5f73d-186">String</span><span class="sxs-lookup"><span data-stu-id="5f73d-186">String</span></span>|<span data-ttu-id="5f73d-187">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="5f73d-187">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="5f73d-188">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="5f73d-188">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="5f73d-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="5f73d-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="5f73d-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f73d-190">Boolean</span></span>|<span data-ttu-id="5f73d-191">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="5f73d-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="5f73d-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5f73d-192">osMinimumVersion</span></span>|<span data-ttu-id="5f73d-193">String</span><span class="sxs-lookup"><span data-stu-id="5f73d-193">String</span></span>|<span data-ttu-id="5f73d-194">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="5f73d-194">Minimum Android version.</span></span>|
|<span data-ttu-id="5f73d-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5f73d-195">osMaximumVersion</span></span>|<span data-ttu-id="5f73d-196">String</span><span class="sxs-lookup"><span data-stu-id="5f73d-196">String</span></span>|<span data-ttu-id="5f73d-197">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="5f73d-197">Maximum Android version.</span></span>|
|<span data-ttu-id="5f73d-198">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="5f73d-198">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="5f73d-199">String</span><span class="sxs-lookup"><span data-stu-id="5f73d-199">String</span></span>|<span data-ttu-id="5f73d-200">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="5f73d-200">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="5f73d-201">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="5f73d-201">storageRequireEncryption</span></span>|<span data-ttu-id="5f73d-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f73d-202">Boolean</span></span>|<span data-ttu-id="5f73d-203">Указывает на то, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="5f73d-203">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="5f73d-204">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="5f73d-204">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="5f73d-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f73d-205">Boolean</span></span>|<span data-ttu-id="5f73d-206">Указывает на то, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="5f73d-206">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="5f73d-207">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="5f73d-207">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="5f73d-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f73d-208">Boolean</span></span>|<span data-ttu-id="5f73d-209">Указывает на то, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="5f73d-209">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="5f73d-210">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="5f73d-210">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="5f73d-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f73d-211">Boolean</span></span>|<span data-ttu-id="5f73d-212">Указывает на то, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="5f73d-212">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="5f73d-213">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="5f73d-213">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="5f73d-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f73d-214">Boolean</span></span>|<span data-ttu-id="5f73d-215">Указывает на то, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="5f73d-215">Require the device to have up to date security providers.</span></span> <span data-ttu-id="5f73d-216">Указывает на то, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="5f73d-216">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="5f73d-217">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="5f73d-217">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="5f73d-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f73d-218">Boolean</span></span>|<span data-ttu-id="5f73d-219">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="5f73d-219">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="5f73d-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="5f73d-220">Response</span></span>
<span data-ttu-id="5f73d-221">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5f73d-221">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_deviceconfig_androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f73d-222">Пример</span><span class="sxs-lookup"><span data-stu-id="5f73d-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f73d-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f73d-223">Request</span></span>
<span data-ttu-id="5f73d-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f73d-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1223

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="5f73d-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="5f73d-225">Response</span></span>
<span data-ttu-id="5f73d-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5f73d-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



