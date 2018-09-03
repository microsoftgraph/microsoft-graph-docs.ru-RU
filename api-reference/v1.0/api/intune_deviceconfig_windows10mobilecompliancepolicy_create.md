# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="8a21c-101">Создать windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="8a21c-101">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="8a21c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8a21c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a21c-103">Создание объекта [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8a21c-103">Create a new [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8a21c-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8a21c-104">Prerequisites</span></span>
<span data-ttu-id="8a21c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8a21c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8a21c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a21c-107">Permission type</span></span>|<span data-ttu-id="8a21c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a21c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a21c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a21c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8a21c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a21c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8a21c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a21c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a21c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a21c-112">Not supported.</span></span>|
|<span data-ttu-id="8a21c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a21c-113">Application</span></span>|<span data-ttu-id="8a21c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a21c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a21c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a21c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="8a21c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a21c-116">Request headers</span></span>
|<span data-ttu-id="8a21c-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a21c-117">Header</span></span>|<span data-ttu-id="8a21c-118">Значение</span><span class="sxs-lookup"><span data-stu-id="8a21c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a21c-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a21c-119">Authorization</span></span>|<span data-ttu-id="8a21c-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="8a21c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a21c-121">Принять</span><span class="sxs-lookup"><span data-stu-id="8a21c-121">Accept</span></span>|<span data-ttu-id="8a21c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8a21c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a21c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a21c-123">Request body</span></span>
<span data-ttu-id="8a21c-124">В тексте запроса добавьте представление объекта windows10MobileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a21c-124">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="8a21c-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="8a21c-125">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="8a21c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a21c-126">Property</span></span>|<span data-ttu-id="8a21c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="8a21c-127">Type</span></span>|<span data-ttu-id="8a21c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8a21c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a21c-129">id</span><span class="sxs-lookup"><span data-stu-id="8a21c-129">id</span></span>|<span data-ttu-id="8a21c-130">Строка</span><span class="sxs-lookup"><span data-stu-id="8a21c-130">String</span></span>|<span data-ttu-id="8a21c-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8a21c-131">Key of the entity.</span></span> <span data-ttu-id="8a21c-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8a21c-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8a21c-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a21c-133">createdDateTime</span></span>|<span data-ttu-id="8a21c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a21c-134">DateTimeOffset</span></span>|<span data-ttu-id="8a21c-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8a21c-135">DateTime the object was created.</span></span> <span data-ttu-id="8a21c-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8a21c-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8a21c-137">description</span><span class="sxs-lookup"><span data-stu-id="8a21c-137">description</span></span>|<span data-ttu-id="8a21c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="8a21c-138">String</span></span>|<span data-ttu-id="8a21c-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8a21c-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8a21c-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8a21c-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8a21c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a21c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="8a21c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a21c-142">DateTimeOffset</span></span>|<span data-ttu-id="8a21c-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8a21c-143">DateTime the object was last modified.</span></span> <span data-ttu-id="8a21c-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8a21c-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8a21c-145">displayName</span><span class="sxs-lookup"><span data-stu-id="8a21c-145">displayName</span></span>|<span data-ttu-id="8a21c-146">Строка</span><span class="sxs-lookup"><span data-stu-id="8a21c-146">String</span></span>|<span data-ttu-id="8a21c-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8a21c-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8a21c-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8a21c-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8a21c-149">version</span><span class="sxs-lookup"><span data-stu-id="8a21c-149">version</span></span>|<span data-ttu-id="8a21c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8a21c-150">Int32</span></span>|<span data-ttu-id="8a21c-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8a21c-151">Version of the device configuration.</span></span> <span data-ttu-id="8a21c-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8a21c-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8a21c-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="8a21c-153">passwordRequired</span></span>|<span data-ttu-id="8a21c-154">Логический</span><span class="sxs-lookup"><span data-stu-id="8a21c-154">Boolean</span></span>|<span data-ttu-id="8a21c-155">Указывает, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="8a21c-155">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="8a21c-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="8a21c-156">passwordBlockSimple</span></span>|<span data-ttu-id="8a21c-157">Логический</span><span class="sxs-lookup"><span data-stu-id="8a21c-157">Boolean</span></span>|<span data-ttu-id="8a21c-158">Указывает, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="8a21c-158">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="8a21c-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8a21c-159">passwordMinimumLength</span></span>|<span data-ttu-id="8a21c-160">Int32</span><span class="sxs-lookup"><span data-stu-id="8a21c-160">Int32</span></span>|<span data-ttu-id="8a21c-161">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="8a21c-161">Minimum password length.</span></span> <span data-ttu-id="8a21c-162">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="8a21c-162">Valid values 4 to 16</span></span>|
|<span data-ttu-id="8a21c-163">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8a21c-163">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8a21c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8a21c-164">Int32</span></span>|<span data-ttu-id="8a21c-165">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="8a21c-165">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8a21c-166">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8a21c-166">passwordRequiredType</span></span>|[<span data-ttu-id="8a21c-167">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8a21c-167">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="8a21c-168">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="8a21c-168">The required password type.</span></span> <span data-ttu-id="8a21c-169">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="8a21c-169">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="8a21c-170">счётчик блокировки пароля при вводе предыдущего пароля</span><span class="sxs-lookup"><span data-stu-id="8a21c-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8a21c-171">Int32</span><span class="sxs-lookup"><span data-stu-id="8a21c-171">Int32</span></span>|<span data-ttu-id="8a21c-172">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="8a21c-172">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="8a21c-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8a21c-173">passwordExpirationDays</span></span>|<span data-ttu-id="8a21c-174">Int32</span><span class="sxs-lookup"><span data-stu-id="8a21c-174">Int32</span></span>|<span data-ttu-id="8a21c-175">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="8a21c-175">Number of days before password expiration.</span></span> <span data-ttu-id="8a21c-176">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="8a21c-176">Valid values 1 to 255</span></span>|
|<span data-ttu-id="8a21c-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="8a21c-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="8a21c-178">Int32</span><span class="sxs-lookup"><span data-stu-id="8a21c-178">Int32</span></span>|<span data-ttu-id="8a21c-179">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="8a21c-179">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="8a21c-180">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="8a21c-180">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="8a21c-181">Логический</span><span class="sxs-lookup"><span data-stu-id="8a21c-181">Boolean</span></span>|<span data-ttu-id="8a21c-182">Указывает, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="8a21c-182">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="8a21c-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8a21c-183">osMinimumVersion</span></span>|<span data-ttu-id="8a21c-184">Строка</span><span class="sxs-lookup"><span data-stu-id="8a21c-184">String</span></span>|<span data-ttu-id="8a21c-185">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="8a21c-185">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="8a21c-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8a21c-186">osMaximumVersion</span></span>|<span data-ttu-id="8a21c-187">Строка</span><span class="sxs-lookup"><span data-stu-id="8a21c-187">String</span></span>|<span data-ttu-id="8a21c-188">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="8a21c-188">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="8a21c-189">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="8a21c-189">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="8a21c-190">Логический</span><span class="sxs-lookup"><span data-stu-id="8a21c-190">Boolean</span></span>|<span data-ttu-id="8a21c-191">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="8a21c-191">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="8a21c-192">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="8a21c-192">bitLockerEnabled</span></span>|<span data-ttu-id="8a21c-193">Логический</span><span class="sxs-lookup"><span data-stu-id="8a21c-193">Boolean</span></span>|<span data-ttu-id="8a21c-194">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="8a21c-194">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="8a21c-195">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="8a21c-195">secureBootEnabled</span></span>|<span data-ttu-id="8a21c-196">Логический</span><span class="sxs-lookup"><span data-stu-id="8a21c-196">Boolean</span></span>|<span data-ttu-id="8a21c-197">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="8a21c-197">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="8a21c-198">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="8a21c-198">codeIntegrityEnabled</span></span>|<span data-ttu-id="8a21c-199">Логический</span><span class="sxs-lookup"><span data-stu-id="8a21c-199">Boolean</span></span>|<span data-ttu-id="8a21c-200">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="8a21c-200">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="8a21c-201">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="8a21c-201">storageRequireEncryption</span></span>|<span data-ttu-id="8a21c-202">Логический</span><span class="sxs-lookup"><span data-stu-id="8a21c-202">Boolean</span></span>|<span data-ttu-id="8a21c-203">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="8a21c-203">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="8a21c-204">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a21c-204">Response</span></span>
<span data-ttu-id="8a21c-205">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8a21c-205">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a21c-206">Пример</span><span class="sxs-lookup"><span data-stu-id="8a21c-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="8a21c-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a21c-207">Request</span></span>
<span data-ttu-id="8a21c-208">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a21c-208">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 856

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="8a21c-209">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a21c-209">Response</span></span>
<span data-ttu-id="8a21c-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a21c-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



