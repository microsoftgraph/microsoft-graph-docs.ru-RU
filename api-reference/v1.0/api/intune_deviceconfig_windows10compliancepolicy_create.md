# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="504eb-101">Создание windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="504eb-101">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="504eb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="504eb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="504eb-103">Создает объект [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="504eb-103">Create a new [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="504eb-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="504eb-104">Prerequisites</span></span>
<span data-ttu-id="504eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="504eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="504eb-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="504eb-107">Permission type</span></span>|<span data-ttu-id="504eb-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="504eb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="504eb-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="504eb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="504eb-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="504eb-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="504eb-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="504eb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="504eb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="504eb-112">Not supported.</span></span>|
|<span data-ttu-id="504eb-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="504eb-113">Application</span></span>|<span data-ttu-id="504eb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="504eb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="504eb-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="504eb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="504eb-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="504eb-116">Request headers</span></span>
|<span data-ttu-id="504eb-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="504eb-117">Header</span></span>|<span data-ttu-id="504eb-118">Значение</span><span class="sxs-lookup"><span data-stu-id="504eb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="504eb-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="504eb-119">Authorization</span></span>|<span data-ttu-id="504eb-120">&lt;Токен&gt; носителя. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="504eb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="504eb-121">Принять</span><span class="sxs-lookup"><span data-stu-id="504eb-121">Accept</span></span>|<span data-ttu-id="504eb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="504eb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="504eb-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="504eb-123">Request body</span></span>
<span data-ttu-id="504eb-124">В теле запроса добавьте представление объекта windows10CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="504eb-124">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="504eb-125">Ниже показаны свойства, которые необходимо указывать при создании объекта windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="504eb-125">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="504eb-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="504eb-126">Property</span></span>|<span data-ttu-id="504eb-127">Тип</span><span class="sxs-lookup"><span data-stu-id="504eb-127">Type</span></span>|<span data-ttu-id="504eb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="504eb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="504eb-129">id</span><span class="sxs-lookup"><span data-stu-id="504eb-129">id</span></span>|<span data-ttu-id="504eb-130">String</span><span class="sxs-lookup"><span data-stu-id="504eb-130">String</span></span>|<span data-ttu-id="504eb-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="504eb-131">Key of the entity.</span></span> <span data-ttu-id="504eb-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="504eb-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="504eb-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="504eb-133">createdDateTime</span></span>|<span data-ttu-id="504eb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="504eb-134">DateTimeOffset</span></span>|<span data-ttu-id="504eb-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="504eb-135">DateTime the object was created.</span></span> <span data-ttu-id="504eb-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="504eb-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="504eb-137">description</span><span class="sxs-lookup"><span data-stu-id="504eb-137">description</span></span>|<span data-ttu-id="504eb-138">String</span><span class="sxs-lookup"><span data-stu-id="504eb-138">String</span></span>|<span data-ttu-id="504eb-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="504eb-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="504eb-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="504eb-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="504eb-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="504eb-141">lastModifiedDateTime</span></span>|<span data-ttu-id="504eb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="504eb-142">DateTimeOffset</span></span>|<span data-ttu-id="504eb-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="504eb-143">DateTime the object was last modified.</span></span> <span data-ttu-id="504eb-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="504eb-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="504eb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="504eb-145">displayName</span></span>|<span data-ttu-id="504eb-146">String</span><span class="sxs-lookup"><span data-stu-id="504eb-146">String</span></span>|<span data-ttu-id="504eb-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="504eb-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="504eb-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="504eb-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="504eb-149">version</span><span class="sxs-lookup"><span data-stu-id="504eb-149">version</span></span>|<span data-ttu-id="504eb-150">Int32</span><span class="sxs-lookup"><span data-stu-id="504eb-150">Int32</span></span>|<span data-ttu-id="504eb-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="504eb-151">Version of the device configuration.</span></span> <span data-ttu-id="504eb-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="504eb-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="504eb-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="504eb-153">passwordRequired</span></span>|<span data-ttu-id="504eb-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="504eb-154">Boolean</span></span>|<span data-ttu-id="504eb-155">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="504eb-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="504eb-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="504eb-156">passwordBlockSimple</span></span>|<span data-ttu-id="504eb-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="504eb-157">Boolean</span></span>|<span data-ttu-id="504eb-158">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="504eb-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="504eb-159">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="504eb-159">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="504eb-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="504eb-160">Boolean</span></span>|<span data-ttu-id="504eb-161">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="504eb-161">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="504eb-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="504eb-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="504eb-163">Int32</span><span class="sxs-lookup"><span data-stu-id="504eb-163">Int32</span></span>|<span data-ttu-id="504eb-164">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="504eb-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="504eb-165">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="504eb-165">passwordExpirationDays</span></span>|<span data-ttu-id="504eb-166">Int32</span><span class="sxs-lookup"><span data-stu-id="504eb-166">Int32</span></span>|<span data-ttu-id="504eb-167">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="504eb-167">The password expiration in days.</span></span>|
|<span data-ttu-id="504eb-168">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="504eb-168">passwordMinimumLength</span></span>|<span data-ttu-id="504eb-169">Int32</span><span class="sxs-lookup"><span data-stu-id="504eb-169">Int32</span></span>|<span data-ttu-id="504eb-170">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="504eb-170">The minimum password length.</span></span>|
|<span data-ttu-id="504eb-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="504eb-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="504eb-172">Int32</span><span class="sxs-lookup"><span data-stu-id="504eb-172">Int32</span></span>|<span data-ttu-id="504eb-173">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="504eb-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="504eb-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="504eb-174">passwordRequiredType</span></span>|[<span data-ttu-id="504eb-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="504eb-175">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="504eb-176">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="504eb-176">The required password type.</span></span> <span data-ttu-id="504eb-177">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="504eb-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="504eb-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="504eb-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="504eb-179">Int32</span><span class="sxs-lookup"><span data-stu-id="504eb-179">Int32</span></span>|<span data-ttu-id="504eb-180">Количество предыдущих паролей, повторное использование которых требуется запретить.</span><span class="sxs-lookup"><span data-stu-id="504eb-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="504eb-181">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="504eb-181">requireHealthyDeviceReport</span></span>|<span data-ttu-id="504eb-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="504eb-182">Boolean</span></span>|<span data-ttu-id="504eb-183">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="504eb-183">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="504eb-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="504eb-184">osMinimumVersion</span></span>|<span data-ttu-id="504eb-185">String</span><span class="sxs-lookup"><span data-stu-id="504eb-185">String</span></span>|<span data-ttu-id="504eb-186">Минимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="504eb-186">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="504eb-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="504eb-187">osMaximumVersion</span></span>|<span data-ttu-id="504eb-188">String</span><span class="sxs-lookup"><span data-stu-id="504eb-188">String</span></span>|<span data-ttu-id="504eb-189">Максимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="504eb-189">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="504eb-190">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="504eb-190">mobileOsMinimumVersion</span></span>|<span data-ttu-id="504eb-191">String</span><span class="sxs-lookup"><span data-stu-id="504eb-191">String</span></span>|<span data-ttu-id="504eb-192">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="504eb-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="504eb-193">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="504eb-193">mobileOsMaximumVersion</span></span>|<span data-ttu-id="504eb-194">String</span><span class="sxs-lookup"><span data-stu-id="504eb-194">String</span></span>|<span data-ttu-id="504eb-195">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="504eb-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="504eb-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="504eb-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="504eb-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="504eb-197">Boolean</span></span>|<span data-ttu-id="504eb-198">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="504eb-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="504eb-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="504eb-199">bitLockerEnabled</span></span>|<span data-ttu-id="504eb-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="504eb-200">Boolean</span></span>|<span data-ttu-id="504eb-201">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="504eb-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="504eb-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="504eb-202">secureBootEnabled</span></span>|<span data-ttu-id="504eb-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="504eb-203">Boolean</span></span>|<span data-ttu-id="504eb-204">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="504eb-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="504eb-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="504eb-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="504eb-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="504eb-206">Boolean</span></span>|<span data-ttu-id="504eb-207">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="504eb-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="504eb-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="504eb-208">storageRequireEncryption</span></span>|<span data-ttu-id="504eb-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="504eb-209">Boolean</span></span>|<span data-ttu-id="504eb-210">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="504eb-210">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="504eb-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="504eb-211">Response</span></span>
<span data-ttu-id="504eb-212">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="504eb-212">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="504eb-213">Пример</span><span class="sxs-lookup"><span data-stu-id="504eb-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="504eb-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="504eb-214">Request</span></span>
<span data-ttu-id="504eb-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="504eb-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 954

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="504eb-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="504eb-216">Response</span></span>
<span data-ttu-id="504eb-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="504eb-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



