# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="866f1-101">Обновление windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="866f1-101">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="866f1-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="866f1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="866f1-103">Обновление свойств объекта [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="866f1-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="866f1-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="866f1-104">Prerequisites</span></span>
<span data-ttu-id="866f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="866f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="866f1-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="866f1-107">Permission type</span></span>|<span data-ttu-id="866f1-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="866f1-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="866f1-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="866f1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="866f1-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="866f1-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="866f1-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="866f1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="866f1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="866f1-112">Not supported.</span></span>|
|<span data-ttu-id="866f1-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="866f1-113">Application</span></span>|<span data-ttu-id="866f1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="866f1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="866f1-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="866f1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="866f1-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="866f1-116">Request headers</span></span>
|<span data-ttu-id="866f1-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="866f1-117">Header</span></span>|<span data-ttu-id="866f1-118">Значение</span><span class="sxs-lookup"><span data-stu-id="866f1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="866f1-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="866f1-119">Authorization</span></span>|<span data-ttu-id="866f1-120">&lt;Токен&gt; носителя. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="866f1-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="866f1-121">Принять</span><span class="sxs-lookup"><span data-stu-id="866f1-121">Accept</span></span>|<span data-ttu-id="866f1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="866f1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="866f1-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="866f1-123">Request body</span></span>
<span data-ttu-id="866f1-124">В теле запроса добавьте представление объекта [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="866f1-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="866f1-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="866f1-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="866f1-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="866f1-126">Property</span></span>|<span data-ttu-id="866f1-127">Тип</span><span class="sxs-lookup"><span data-stu-id="866f1-127">Type</span></span>|<span data-ttu-id="866f1-128">Описание</span><span class="sxs-lookup"><span data-stu-id="866f1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="866f1-129">id</span><span class="sxs-lookup"><span data-stu-id="866f1-129">id</span></span>|<span data-ttu-id="866f1-130">String</span><span class="sxs-lookup"><span data-stu-id="866f1-130">String</span></span>|<span data-ttu-id="866f1-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="866f1-131">Key of the setting.</span></span> <span data-ttu-id="866f1-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="866f1-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="866f1-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="866f1-133">createdDateTime</span></span>|<span data-ttu-id="866f1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="866f1-134">DateTimeOffset</span></span>|<span data-ttu-id="866f1-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="866f1-135">DateTime the object was created.</span></span> <span data-ttu-id="866f1-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="866f1-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="866f1-137">description</span><span class="sxs-lookup"><span data-stu-id="866f1-137">description</span></span>|<span data-ttu-id="866f1-138">String</span><span class="sxs-lookup"><span data-stu-id="866f1-138">String</span></span>|<span data-ttu-id="866f1-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="866f1-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="866f1-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="866f1-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="866f1-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="866f1-141">lastModifiedDateTime</span></span>|<span data-ttu-id="866f1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="866f1-142">DateTimeOffset</span></span>|<span data-ttu-id="866f1-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="866f1-143">DateTime the object was last modified.</span></span> <span data-ttu-id="866f1-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="866f1-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="866f1-145">displayName</span><span class="sxs-lookup"><span data-stu-id="866f1-145">displayName</span></span>|<span data-ttu-id="866f1-146">String</span><span class="sxs-lookup"><span data-stu-id="866f1-146">String</span></span>|<span data-ttu-id="866f1-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="866f1-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="866f1-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="866f1-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="866f1-149">version</span><span class="sxs-lookup"><span data-stu-id="866f1-149">version</span></span>|<span data-ttu-id="866f1-150">Int32</span><span class="sxs-lookup"><span data-stu-id="866f1-150">Int32</span></span>|<span data-ttu-id="866f1-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="866f1-151">Version of the device configuration.</span></span> <span data-ttu-id="866f1-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="866f1-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="866f1-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="866f1-153">passwordRequired</span></span>|<span data-ttu-id="866f1-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="866f1-154">Boolean</span></span>|<span data-ttu-id="866f1-155">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="866f1-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="866f1-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="866f1-156">passwordBlockSimple</span></span>|<span data-ttu-id="866f1-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="866f1-157">Boolean</span></span>|<span data-ttu-id="866f1-158">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="866f1-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="866f1-159">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="866f1-159">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="866f1-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="866f1-160">Boolean</span></span>|<span data-ttu-id="866f1-161">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="866f1-161">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="866f1-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="866f1-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="866f1-163">Int32</span><span class="sxs-lookup"><span data-stu-id="866f1-163">Int32</span></span>|<span data-ttu-id="866f1-164">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="866f1-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="866f1-165">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="866f1-165">passwordExpirationDays</span></span>|<span data-ttu-id="866f1-166">Int32</span><span class="sxs-lookup"><span data-stu-id="866f1-166">Int32</span></span>|<span data-ttu-id="866f1-167">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="866f1-167">The password expiration in days.</span></span>|
|<span data-ttu-id="866f1-168">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="866f1-168">passwordMinimumLength</span></span>|<span data-ttu-id="866f1-169">Int32</span><span class="sxs-lookup"><span data-stu-id="866f1-169">Int32</span></span>|<span data-ttu-id="866f1-170">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="866f1-170">The minimum password length.</span></span>|
|<span data-ttu-id="866f1-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="866f1-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="866f1-172">Int32</span><span class="sxs-lookup"><span data-stu-id="866f1-172">Int32</span></span>|<span data-ttu-id="866f1-173">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="866f1-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="866f1-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="866f1-174">passwordRequiredType</span></span>|<span data-ttu-id="866f1-175">String</span><span class="sxs-lookup"><span data-stu-id="866f1-175">String</span></span>|<span data-ttu-id="866f1-176">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="866f1-176">The required password type.</span></span> <span data-ttu-id="866f1-177">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="866f1-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="866f1-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="866f1-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="866f1-179">Int32</span><span class="sxs-lookup"><span data-stu-id="866f1-179">Int32</span></span>|<span data-ttu-id="866f1-180">Количество предыдущих паролей, повторное использование которых требуется запретить.</span><span class="sxs-lookup"><span data-stu-id="866f1-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="866f1-181">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="866f1-181">requireHealthyDeviceReport</span></span>|<span data-ttu-id="866f1-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="866f1-182">Boolean</span></span>|<span data-ttu-id="866f1-183">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="866f1-183">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="866f1-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="866f1-184">osMinimumVersion</span></span>|<span data-ttu-id="866f1-185">String</span><span class="sxs-lookup"><span data-stu-id="866f1-185">String</span></span>|<span data-ttu-id="866f1-186">Минимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="866f1-186">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="866f1-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="866f1-187">osMaximumVersion</span></span>|<span data-ttu-id="866f1-188">String</span><span class="sxs-lookup"><span data-stu-id="866f1-188">String</span></span>|<span data-ttu-id="866f1-189">Максимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="866f1-189">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="866f1-190">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="866f1-190">mobileOsMinimumVersion</span></span>|<span data-ttu-id="866f1-191">String</span><span class="sxs-lookup"><span data-stu-id="866f1-191">String</span></span>|<span data-ttu-id="866f1-192">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="866f1-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="866f1-193">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="866f1-193">mobileOsMaximumVersion</span></span>|<span data-ttu-id="866f1-194">String</span><span class="sxs-lookup"><span data-stu-id="866f1-194">String</span></span>|<span data-ttu-id="866f1-195">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="866f1-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="866f1-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="866f1-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="866f1-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="866f1-197">Boolean</span></span>|<span data-ttu-id="866f1-198">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="866f1-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="866f1-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="866f1-199">bitLockerEnabled</span></span>|<span data-ttu-id="866f1-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="866f1-200">Boolean</span></span>|<span data-ttu-id="866f1-201">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="866f1-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="866f1-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="866f1-202">secureBootEnabled</span></span>|<span data-ttu-id="866f1-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="866f1-203">Boolean</span></span>|<span data-ttu-id="866f1-204">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="866f1-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="866f1-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="866f1-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="866f1-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="866f1-206">Boolean</span></span>|<span data-ttu-id="866f1-207">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="866f1-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="866f1-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="866f1-208">storageRequireEncryption</span></span>|<span data-ttu-id="866f1-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="866f1-209">Boolean</span></span>|<span data-ttu-id="866f1-210">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="866f1-210">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="866f1-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="866f1-211">Response</span></span>
<span data-ttu-id="866f1-212">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="866f1-212">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="866f1-213">Пример</span><span class="sxs-lookup"><span data-stu-id="866f1-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="866f1-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="866f1-214">Request</span></span>
<span data-ttu-id="866f1-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="866f1-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 954

{
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

### <a name="response"></a><span data-ttu-id="866f1-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="866f1-216">Response</span></span>
<span data-ttu-id="866f1-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="866f1-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



