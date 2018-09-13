# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="f1700-101">Создание windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f1700-101">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="f1700-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f1700-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1700-103">Создает объект [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1700-103">Create a new [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1700-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1700-104">Prerequisites</span></span>
<span data-ttu-id="f1700-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1700-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f1700-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1700-107">Permission type</span></span>|<span data-ttu-id="f1700-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1700-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1700-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1700-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f1700-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1700-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1700-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1700-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1700-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1700-112">Not supported.</span></span>|
|<span data-ttu-id="f1700-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1700-113">Application</span></span>|<span data-ttu-id="f1700-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1700-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1700-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1700-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f1700-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1700-116">Request headers</span></span>
|<span data-ttu-id="f1700-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1700-117">Header</span></span>|<span data-ttu-id="f1700-118">Значение</span><span class="sxs-lookup"><span data-stu-id="f1700-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1700-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1700-119">Authorization</span></span>|<span data-ttu-id="f1700-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="f1700-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1700-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f1700-121">Accept</span></span>|<span data-ttu-id="f1700-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f1700-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1700-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1700-123">Request body</span></span>
<span data-ttu-id="f1700-124">В теле запроса добавьте представление объекта windows10CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1700-124">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="f1700-125">Ниже показаны свойства, которые необходимо указывать при создании объекта windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="f1700-125">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="f1700-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1700-126">Property</span></span>|<span data-ttu-id="f1700-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f1700-127">Type</span></span>|<span data-ttu-id="f1700-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f1700-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1700-129">id</span><span class="sxs-lookup"><span data-stu-id="f1700-129">id</span></span>|<span data-ttu-id="f1700-130">Строка</span><span class="sxs-lookup"><span data-stu-id="f1700-130">String</span></span>|<span data-ttu-id="f1700-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f1700-131">Key of the entity.</span></span> <span data-ttu-id="f1700-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1700-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1700-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1700-133">createdDateTime</span></span>|<span data-ttu-id="f1700-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1700-134">DateTimeOffset</span></span>|<span data-ttu-id="f1700-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f1700-135">DateTime the object was created.</span></span> <span data-ttu-id="f1700-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1700-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1700-137">описание</span><span class="sxs-lookup"><span data-stu-id="f1700-137">description</span></span>|<span data-ttu-id="f1700-138">Строка</span><span class="sxs-lookup"><span data-stu-id="f1700-138">String</span></span>|<span data-ttu-id="f1700-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1700-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f1700-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1700-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1700-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1700-141">lastModifiedDateTime</span></span>|<span data-ttu-id="f1700-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1700-142">DateTimeOffset</span></span>|<span data-ttu-id="f1700-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f1700-143">DateTime the object was last modified.</span></span> <span data-ttu-id="f1700-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1700-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1700-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f1700-145">displayName</span></span>|<span data-ttu-id="f1700-146">Строка</span><span class="sxs-lookup"><span data-stu-id="f1700-146">String</span></span>|<span data-ttu-id="f1700-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1700-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f1700-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1700-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1700-149">version</span><span class="sxs-lookup"><span data-stu-id="f1700-149">version</span></span>|<span data-ttu-id="f1700-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f1700-150">Int32</span></span>|<span data-ttu-id="f1700-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1700-151">Version of the device configuration.</span></span> <span data-ttu-id="f1700-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1700-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1700-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f1700-153">passwordRequired</span></span>|<span data-ttu-id="f1700-154">Логический</span><span class="sxs-lookup"><span data-stu-id="f1700-154">Boolean</span></span>|<span data-ttu-id="f1700-155">Указывает, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="f1700-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="f1700-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f1700-156">passwordBlockSimple</span></span>|<span data-ttu-id="f1700-157">Логический</span><span class="sxs-lookup"><span data-stu-id="f1700-157">Boolean</span></span>|<span data-ttu-id="f1700-158">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="f1700-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="f1700-159">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="f1700-159">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="f1700-160">Логический</span><span class="sxs-lookup"><span data-stu-id="f1700-160">Boolean</span></span>|<span data-ttu-id="f1700-161">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="f1700-161">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="f1700-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f1700-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f1700-163">Int32</span><span class="sxs-lookup"><span data-stu-id="f1700-163">Int32</span></span>|<span data-ttu-id="f1700-164">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="f1700-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f1700-165">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f1700-165">passwordExpirationDays</span></span>|<span data-ttu-id="f1700-166">Int32</span><span class="sxs-lookup"><span data-stu-id="f1700-166">Int32</span></span>|<span data-ttu-id="f1700-167">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="f1700-167">The password expiration in days.</span></span>|
|<span data-ttu-id="f1700-168">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f1700-168">passwordMinimumLength</span></span>|<span data-ttu-id="f1700-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f1700-169">Int32</span></span>|<span data-ttu-id="f1700-170">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="f1700-170">The minimum password length.</span></span>|
|<span data-ttu-id="f1700-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f1700-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f1700-172">Int32</span><span class="sxs-lookup"><span data-stu-id="f1700-172">Int32</span></span>|<span data-ttu-id="f1700-173">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="f1700-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f1700-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f1700-174">passwordRequiredType</span></span>|[<span data-ttu-id="f1700-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f1700-175">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="f1700-p108">Требуемый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f1700-p108">The required password type. The possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f1700-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f1700-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f1700-179">Int32</span><span class="sxs-lookup"><span data-stu-id="f1700-179">Int32</span></span>|<span data-ttu-id="f1700-180">Количество предыдущих паролей, повторное использование которых требуется запретить.</span><span class="sxs-lookup"><span data-stu-id="f1700-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="f1700-181">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="f1700-181">requireHealthyDeviceReport</span></span>|<span data-ttu-id="f1700-182">Логический</span><span class="sxs-lookup"><span data-stu-id="f1700-182">Boolean</span></span>|<span data-ttu-id="f1700-183">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="f1700-183">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="f1700-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f1700-184">osMinimumVersion</span></span>|<span data-ttu-id="f1700-185">Строка</span><span class="sxs-lookup"><span data-stu-id="f1700-185">String</span></span>|<span data-ttu-id="f1700-186">Минимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f1700-186">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="f1700-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f1700-187">osMaximumVersion</span></span>|<span data-ttu-id="f1700-188">Строка</span><span class="sxs-lookup"><span data-stu-id="f1700-188">String</span></span>|<span data-ttu-id="f1700-189">Максимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f1700-189">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="f1700-190">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f1700-190">mobileOsMinimumVersion</span></span>|<span data-ttu-id="f1700-191">Строка</span><span class="sxs-lookup"><span data-stu-id="f1700-191">String</span></span>|<span data-ttu-id="f1700-192">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f1700-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="f1700-193">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f1700-193">mobileOsMaximumVersion</span></span>|<span data-ttu-id="f1700-194">Строка</span><span class="sxs-lookup"><span data-stu-id="f1700-194">String</span></span>|<span data-ttu-id="f1700-195">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f1700-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="f1700-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="f1700-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="f1700-197">Логический</span><span class="sxs-lookup"><span data-stu-id="f1700-197">Boolean</span></span>|<span data-ttu-id="f1700-198">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="f1700-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="f1700-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="f1700-199">bitLockerEnabled</span></span>|<span data-ttu-id="f1700-200">Логический</span><span class="sxs-lookup"><span data-stu-id="f1700-200">Boolean</span></span>|<span data-ttu-id="f1700-201">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="f1700-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="f1700-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="f1700-202">secureBootEnabled</span></span>|<span data-ttu-id="f1700-203">Логический</span><span class="sxs-lookup"><span data-stu-id="f1700-203">Boolean</span></span>|<span data-ttu-id="f1700-204">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="f1700-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="f1700-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="f1700-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="f1700-206">Логический</span><span class="sxs-lookup"><span data-stu-id="f1700-206">Boolean</span></span>|<span data-ttu-id="f1700-207">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="f1700-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="f1700-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f1700-208">storageRequireEncryption</span></span>|<span data-ttu-id="f1700-209">Логический</span><span class="sxs-lookup"><span data-stu-id="f1700-209">Boolean</span></span>|<span data-ttu-id="f1700-210">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="f1700-210">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="f1700-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1700-211">Response</span></span>
<span data-ttu-id="f1700-212">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f1700-212">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1700-213">Пример</span><span class="sxs-lookup"><span data-stu-id="f1700-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1700-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1700-214">Request</span></span>
<span data-ttu-id="f1700-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1700-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1018

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="f1700-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1700-216">Response</span></span>
<span data-ttu-id="f1700-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1700-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```








