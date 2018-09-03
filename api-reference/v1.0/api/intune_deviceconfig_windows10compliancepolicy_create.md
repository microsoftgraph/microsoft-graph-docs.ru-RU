# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="96e62-101">Создание windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="96e62-101">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="96e62-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="96e62-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96e62-103">Создает объект [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="96e62-103">Create a new [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96e62-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="96e62-104">Prerequisites</span></span>
<span data-ttu-id="96e62-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="96e62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="96e62-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96e62-107">Permission type</span></span>|<span data-ttu-id="96e62-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96e62-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96e62-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96e62-109">Delegated (work or school account)</span></span>|<span data-ttu-id="96e62-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e62-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96e62-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96e62-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96e62-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96e62-112">Not supported.</span></span>|
|<span data-ttu-id="96e62-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96e62-113">Application</span></span>|<span data-ttu-id="96e62-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96e62-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96e62-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96e62-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="96e62-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96e62-116">Request headers</span></span>
|<span data-ttu-id="96e62-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96e62-117">Header</span></span>|<span data-ttu-id="96e62-118">Значение</span><span class="sxs-lookup"><span data-stu-id="96e62-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96e62-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96e62-119">Authorization</span></span>|<span data-ttu-id="96e62-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="96e62-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96e62-121">Accept</span><span class="sxs-lookup"><span data-stu-id="96e62-121">Accept</span></span>|<span data-ttu-id="96e62-122">application/json</span><span class="sxs-lookup"><span data-stu-id="96e62-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96e62-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96e62-123">Request body</span></span>
<span data-ttu-id="96e62-124">В теле запроса добавьте представление объекта windows10CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96e62-124">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="96e62-125">Ниже показаны свойства, которые необходимо указывать при создании объекта windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="96e62-125">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="96e62-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="96e62-126">Property</span></span>|<span data-ttu-id="96e62-127">Тип</span><span class="sxs-lookup"><span data-stu-id="96e62-127">Type</span></span>|<span data-ttu-id="96e62-128">Описание</span><span class="sxs-lookup"><span data-stu-id="96e62-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96e62-129">id</span><span class="sxs-lookup"><span data-stu-id="96e62-129">id</span></span>|<span data-ttu-id="96e62-130">Строка</span><span class="sxs-lookup"><span data-stu-id="96e62-130">String</span></span>|<span data-ttu-id="96e62-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="96e62-131">Key of the entity.</span></span> <span data-ttu-id="96e62-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="96e62-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96e62-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96e62-133">createdDateTime</span></span>|<span data-ttu-id="96e62-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96e62-134">DateTimeOffset</span></span>|<span data-ttu-id="96e62-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="96e62-135">DateTime the object was created.</span></span> <span data-ttu-id="96e62-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="96e62-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96e62-137">description</span><span class="sxs-lookup"><span data-stu-id="96e62-137">description</span></span>|<span data-ttu-id="96e62-138">Строка</span><span class="sxs-lookup"><span data-stu-id="96e62-138">String</span></span>|<span data-ttu-id="96e62-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="96e62-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="96e62-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="96e62-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96e62-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96e62-141">lastModifiedDateTime</span></span>|<span data-ttu-id="96e62-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96e62-142">DateTimeOffset</span></span>|<span data-ttu-id="96e62-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="96e62-143">DateTime the object was last modified.</span></span> <span data-ttu-id="96e62-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="96e62-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96e62-145">displayName</span><span class="sxs-lookup"><span data-stu-id="96e62-145">displayName</span></span>|<span data-ttu-id="96e62-146">Строка</span><span class="sxs-lookup"><span data-stu-id="96e62-146">String</span></span>|<span data-ttu-id="96e62-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="96e62-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="96e62-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="96e62-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96e62-149">version</span><span class="sxs-lookup"><span data-stu-id="96e62-149">version</span></span>|<span data-ttu-id="96e62-150">Int32</span><span class="sxs-lookup"><span data-stu-id="96e62-150">Int32</span></span>|<span data-ttu-id="96e62-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="96e62-151">Version of the device configuration.</span></span> <span data-ttu-id="96e62-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="96e62-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96e62-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="96e62-153">passwordRequired</span></span>|<span data-ttu-id="96e62-154">Логический</span><span class="sxs-lookup"><span data-stu-id="96e62-154">Boolean</span></span>|<span data-ttu-id="96e62-155">Указывает, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="96e62-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="96e62-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="96e62-156">passwordBlockSimple</span></span>|<span data-ttu-id="96e62-157">Логический</span><span class="sxs-lookup"><span data-stu-id="96e62-157">Boolean</span></span>|<span data-ttu-id="96e62-158">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="96e62-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="96e62-159">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="96e62-159">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="96e62-160">Логический</span><span class="sxs-lookup"><span data-stu-id="96e62-160">Boolean</span></span>|<span data-ttu-id="96e62-161">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="96e62-161">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="96e62-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="96e62-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="96e62-163">Int32</span><span class="sxs-lookup"><span data-stu-id="96e62-163">Int32</span></span>|<span data-ttu-id="96e62-164">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="96e62-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="96e62-165">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="96e62-165">passwordExpirationDays</span></span>|<span data-ttu-id="96e62-166">Int32</span><span class="sxs-lookup"><span data-stu-id="96e62-166">Int32</span></span>|<span data-ttu-id="96e62-167">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="96e62-167">The password expiration in days.</span></span>|
|<span data-ttu-id="96e62-168">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="96e62-168">passwordMinimumLength</span></span>|<span data-ttu-id="96e62-169">Int32</span><span class="sxs-lookup"><span data-stu-id="96e62-169">Int32</span></span>|<span data-ttu-id="96e62-170">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="96e62-170">The minimum password length.</span></span>|
|<span data-ttu-id="96e62-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="96e62-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="96e62-172">Int32</span><span class="sxs-lookup"><span data-stu-id="96e62-172">Int32</span></span>|<span data-ttu-id="96e62-173">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="96e62-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="96e62-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="96e62-174">passwordRequiredType</span></span>|[<span data-ttu-id="96e62-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="96e62-175">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="96e62-176">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="96e62-176">The required password type.</span></span> <span data-ttu-id="96e62-177">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="96e62-177">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="96e62-178">счётчик блокировки пароля при вводе предыдущего пароля</span><span class="sxs-lookup"><span data-stu-id="96e62-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="96e62-179">Int32</span><span class="sxs-lookup"><span data-stu-id="96e62-179">Int32</span></span>|<span data-ttu-id="96e62-180">Количество предыдущих паролей, повторное использование которых требуется запретить.</span><span class="sxs-lookup"><span data-stu-id="96e62-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="96e62-181">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="96e62-181">requireHealthyDeviceReport</span></span>|<span data-ttu-id="96e62-182">Логический</span><span class="sxs-lookup"><span data-stu-id="96e62-182">Boolean</span></span>|<span data-ttu-id="96e62-183">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="96e62-183">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="96e62-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="96e62-184">osMinimumVersion</span></span>|<span data-ttu-id="96e62-185">Строка</span><span class="sxs-lookup"><span data-stu-id="96e62-185">String</span></span>|<span data-ttu-id="96e62-186">Минимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="96e62-186">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="96e62-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="96e62-187">osMaximumVersion</span></span>|<span data-ttu-id="96e62-188">Строка</span><span class="sxs-lookup"><span data-stu-id="96e62-188">String</span></span>|<span data-ttu-id="96e62-189">Максимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="96e62-189">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="96e62-190">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="96e62-190">mobileOsMinimumVersion</span></span>|<span data-ttu-id="96e62-191">Строка</span><span class="sxs-lookup"><span data-stu-id="96e62-191">String</span></span>|<span data-ttu-id="96e62-192">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="96e62-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="96e62-193">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="96e62-193">mobileOsMaximumVersion</span></span>|<span data-ttu-id="96e62-194">Строка</span><span class="sxs-lookup"><span data-stu-id="96e62-194">String</span></span>|<span data-ttu-id="96e62-195">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="96e62-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="96e62-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="96e62-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="96e62-197">Логический</span><span class="sxs-lookup"><span data-stu-id="96e62-197">Boolean</span></span>|<span data-ttu-id="96e62-198">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="96e62-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="96e62-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="96e62-199">bitLockerEnabled</span></span>|<span data-ttu-id="96e62-200">Логический</span><span class="sxs-lookup"><span data-stu-id="96e62-200">Boolean</span></span>|<span data-ttu-id="96e62-201">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="96e62-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="96e62-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="96e62-202">secureBootEnabled</span></span>|<span data-ttu-id="96e62-203">Логический</span><span class="sxs-lookup"><span data-stu-id="96e62-203">Boolean</span></span>|<span data-ttu-id="96e62-204">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="96e62-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="96e62-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="96e62-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="96e62-206">Логический</span><span class="sxs-lookup"><span data-stu-id="96e62-206">Boolean</span></span>|<span data-ttu-id="96e62-207">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="96e62-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="96e62-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="96e62-208">storageRequireEncryption</span></span>|<span data-ttu-id="96e62-209">Логический</span><span class="sxs-lookup"><span data-stu-id="96e62-209">Boolean</span></span>|<span data-ttu-id="96e62-210">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="96e62-210">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="96e62-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="96e62-211">Response</span></span>
<span data-ttu-id="96e62-212">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="96e62-212">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96e62-213">Пример</span><span class="sxs-lookup"><span data-stu-id="96e62-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="96e62-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="96e62-214">Request</span></span>
<span data-ttu-id="96e62-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96e62-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96e62-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="96e62-216">Response</span></span>
<span data-ttu-id="96e62-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96e62-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



