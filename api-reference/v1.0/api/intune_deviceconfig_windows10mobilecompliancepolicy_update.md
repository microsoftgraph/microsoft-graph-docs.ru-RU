# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="4f177-101">Обновление windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4f177-101">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="4f177-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4f177-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f177-103">Обновление свойств объекта [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4f177-103">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f177-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4f177-104">Prerequisites</span></span>
<span data-ttu-id="4f177-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4f177-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4f177-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f177-107">Permission type</span></span>|<span data-ttu-id="4f177-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f177-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f177-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f177-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4f177-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f177-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f177-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f177-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f177-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f177-112">Not supported.</span></span>|
|<span data-ttu-id="4f177-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f177-113">Application</span></span>|<span data-ttu-id="4f177-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f177-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f177-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f177-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="4f177-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f177-116">Request headers</span></span>
|<span data-ttu-id="4f177-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f177-117">Header</span></span>|<span data-ttu-id="4f177-118">Значение</span><span class="sxs-lookup"><span data-stu-id="4f177-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f177-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f177-119">Authorization</span></span>|<span data-ttu-id="4f177-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="4f177-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f177-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4f177-121">Accept</span></span>|<span data-ttu-id="4f177-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4f177-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f177-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4f177-123">Request body</span></span>
<span data-ttu-id="4f177-124">В теле запроса добавьте представление объекта [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f177-124">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="4f177-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4f177-125">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="4f177-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f177-126">Property</span></span>|<span data-ttu-id="4f177-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4f177-127">Type</span></span>|<span data-ttu-id="4f177-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4f177-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f177-129">id</span><span class="sxs-lookup"><span data-stu-id="4f177-129">id</span></span>|<span data-ttu-id="4f177-130">Строка</span><span class="sxs-lookup"><span data-stu-id="4f177-130">String</span></span>|<span data-ttu-id="4f177-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4f177-131">Key of the entity.</span></span> <span data-ttu-id="4f177-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4f177-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4f177-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f177-133">createdDateTime</span></span>|<span data-ttu-id="4f177-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f177-134">DateTimeOffset</span></span>|<span data-ttu-id="4f177-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4f177-135">DateTime the object was created.</span></span> <span data-ttu-id="4f177-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4f177-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4f177-137">description</span><span class="sxs-lookup"><span data-stu-id="4f177-137">description</span></span>|<span data-ttu-id="4f177-138">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4f177-138">String</span></span>|<span data-ttu-id="4f177-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4f177-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4f177-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4f177-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4f177-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f177-141">lastModifiedDateTime</span></span>|<span data-ttu-id="4f177-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f177-142">DateTimeOffset</span></span>|<span data-ttu-id="4f177-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4f177-143">DateTime the object was last modified.</span></span> <span data-ttu-id="4f177-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4f177-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4f177-145">displayName</span><span class="sxs-lookup"><span data-stu-id="4f177-145">displayName</span></span>|<span data-ttu-id="4f177-146">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4f177-146">String</span></span>|<span data-ttu-id="4f177-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4f177-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4f177-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4f177-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4f177-149">version</span><span class="sxs-lookup"><span data-stu-id="4f177-149">version</span></span>|<span data-ttu-id="4f177-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4f177-150">Int32</span></span>|<span data-ttu-id="4f177-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4f177-151">Version of the device configuration.</span></span> <span data-ttu-id="4f177-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4f177-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4f177-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4f177-153">passwordRequired</span></span>|<span data-ttu-id="4f177-154">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="4f177-154">Boolean</span></span>|<span data-ttu-id="4f177-155">Указывает, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="4f177-155">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="4f177-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4f177-156">passwordBlockSimple</span></span>|<span data-ttu-id="4f177-157">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="4f177-157">Boolean</span></span>|<span data-ttu-id="4f177-158">Указывает, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="4f177-158">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="4f177-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4f177-159">passwordMinimumLength</span></span>|<span data-ttu-id="4f177-160">Int32</span><span class="sxs-lookup"><span data-stu-id="4f177-160">Int32</span></span>|<span data-ttu-id="4f177-161">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="4f177-161">Minimum password length.</span></span> <span data-ttu-id="4f177-162">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="4f177-162">Valid values 4 to 16</span></span>|
|<span data-ttu-id="4f177-163">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4f177-163">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4f177-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4f177-164">Int32</span></span>|<span data-ttu-id="4f177-165">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="4f177-165">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="4f177-166">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4f177-166">passwordRequiredType</span></span>|[<span data-ttu-id="4f177-167">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4f177-167">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="4f177-168">Тип требуемого пароля.</span><span class="sxs-lookup"><span data-stu-id="4f177-168">The required password type.</span></span> <span data-ttu-id="4f177-169">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="4f177-169">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="4f177-170">счётчик блокировки пароля при вводе предыдущего пароля</span><span class="sxs-lookup"><span data-stu-id="4f177-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4f177-171">Int32</span><span class="sxs-lookup"><span data-stu-id="4f177-171">Int32</span></span>|<span data-ttu-id="4f177-172">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="4f177-172">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="4f177-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4f177-173">passwordExpirationDays</span></span>|<span data-ttu-id="4f177-174">Int32</span><span class="sxs-lookup"><span data-stu-id="4f177-174">Int32</span></span>|<span data-ttu-id="4f177-175">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="4f177-175">Number of days before password expiration.</span></span> <span data-ttu-id="4f177-176">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="4f177-176">Valid values 1 to 255</span></span>|
|<span data-ttu-id="4f177-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4f177-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4f177-178">Int32</span><span class="sxs-lookup"><span data-stu-id="4f177-178">Int32</span></span>|<span data-ttu-id="4f177-179">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="4f177-179">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="4f177-180">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="4f177-180">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="4f177-181">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="4f177-181">Boolean</span></span>|<span data-ttu-id="4f177-182">Указывает, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="4f177-182">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="4f177-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4f177-183">osMinimumVersion</span></span>|<span data-ttu-id="4f177-184">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4f177-184">String</span></span>|<span data-ttu-id="4f177-185">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="4f177-185">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="4f177-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4f177-186">osMaximumVersion</span></span>|<span data-ttu-id="4f177-187">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4f177-187">String</span></span>|<span data-ttu-id="4f177-188">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="4f177-188">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="4f177-189">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="4f177-189">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="4f177-190">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="4f177-190">Boolean</span></span>|<span data-ttu-id="4f177-191">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="4f177-191">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="4f177-192">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="4f177-192">bitLockerEnabled</span></span>|<span data-ttu-id="4f177-193">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="4f177-193">Boolean</span></span>|<span data-ttu-id="4f177-194">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="4f177-194">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="4f177-195">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="4f177-195">secureBootEnabled</span></span>|<span data-ttu-id="4f177-196">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="4f177-196">Boolean</span></span>|<span data-ttu-id="4f177-197">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="4f177-197">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="4f177-198">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="4f177-198">codeIntegrityEnabled</span></span>|<span data-ttu-id="4f177-199">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="4f177-199">Boolean</span></span>|<span data-ttu-id="4f177-200">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="4f177-200">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="4f177-201">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4f177-201">storageRequireEncryption</span></span>|<span data-ttu-id="4f177-202">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="4f177-202">Boolean</span></span>|<span data-ttu-id="4f177-203">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="4f177-203">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="4f177-204">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f177-204">Response</span></span>
<span data-ttu-id="4f177-205">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4f177-205">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f177-206">Пример</span><span class="sxs-lookup"><span data-stu-id="4f177-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f177-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f177-207">Request</span></span>
<span data-ttu-id="4f177-208">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f177-208">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 786

{
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="4f177-209">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f177-209">Response</span></span>
<span data-ttu-id="4f177-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f177-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 964

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "id": "3d4237b0-37b0-3d42-b037-423db037423d",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```



