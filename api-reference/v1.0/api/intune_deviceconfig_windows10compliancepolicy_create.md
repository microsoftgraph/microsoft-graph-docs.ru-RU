# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="d4e22-101">Создание windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d4e22-101">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="d4e22-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d4e22-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4e22-103">Создает объект [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d4e22-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4e22-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d4e22-104">Prerequisites</span></span>
<span data-ttu-id="d4e22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d4e22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d4e22-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4e22-107">Permission type</span></span>|<span data-ttu-id="d4e22-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4e22-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4e22-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4e22-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d4e22-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e22-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4e22-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4e22-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4e22-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4e22-112">Not supported.</span></span>|
|<span data-ttu-id="d4e22-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4e22-113">Application</span></span>|<span data-ttu-id="d4e22-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4e22-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4e22-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4e22-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="d4e22-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4e22-116">Request headers</span></span>
|<span data-ttu-id="d4e22-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4e22-117">Header</span></span>|<span data-ttu-id="d4e22-118">Значение</span><span class="sxs-lookup"><span data-stu-id="d4e22-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4e22-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4e22-119">Authorization</span></span>|<span data-ttu-id="d4e22-120">&lt;Токен&gt; носителя. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4e22-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d4e22-121">Принять</span><span class="sxs-lookup"><span data-stu-id="d4e22-121">Accept</span></span>|<span data-ttu-id="d4e22-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d4e22-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4e22-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4e22-123">Request body</span></span>
<span data-ttu-id="d4e22-124">В теле запроса добавьте представление объекта windows10CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4e22-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="d4e22-125">Ниже показаны свойства, которые необходимо указывать при создании объекта windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d4e22-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="d4e22-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4e22-126">Property</span></span>|<span data-ttu-id="d4e22-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d4e22-127">Type</span></span>|<span data-ttu-id="d4e22-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d4e22-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4e22-129">id</span><span class="sxs-lookup"><span data-stu-id="d4e22-129">id</span></span>|<span data-ttu-id="d4e22-130">String</span><span class="sxs-lookup"><span data-stu-id="d4e22-130">String</span></span>|<span data-ttu-id="d4e22-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d4e22-131">Key of the setting.</span></span> <span data-ttu-id="d4e22-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d4e22-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d4e22-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4e22-133">createdDateTime</span></span>|<span data-ttu-id="d4e22-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4e22-134">DateTimeOffset</span></span>|<span data-ttu-id="d4e22-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d4e22-135">DateTime the object was created.</span></span> <span data-ttu-id="d4e22-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d4e22-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d4e22-137">description</span><span class="sxs-lookup"><span data-stu-id="d4e22-137">description</span></span>|<span data-ttu-id="d4e22-138">String</span><span class="sxs-lookup"><span data-stu-id="d4e22-138">String</span></span>|<span data-ttu-id="d4e22-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d4e22-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d4e22-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d4e22-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d4e22-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4e22-141">lastModifiedDateTime</span></span>|<span data-ttu-id="d4e22-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4e22-142">DateTimeOffset</span></span>|<span data-ttu-id="d4e22-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d4e22-143">DateTime the object was last modified.</span></span> <span data-ttu-id="d4e22-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d4e22-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d4e22-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d4e22-145">displayName</span></span>|<span data-ttu-id="d4e22-146">String</span><span class="sxs-lookup"><span data-stu-id="d4e22-146">String</span></span>|<span data-ttu-id="d4e22-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d4e22-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d4e22-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d4e22-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d4e22-149">version</span><span class="sxs-lookup"><span data-stu-id="d4e22-149">version</span></span>|<span data-ttu-id="d4e22-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e22-150">Int32</span></span>|<span data-ttu-id="d4e22-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d4e22-151">Version of the device configuration.</span></span> <span data-ttu-id="d4e22-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d4e22-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d4e22-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="d4e22-153">passwordRequired</span></span>|<span data-ttu-id="d4e22-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4e22-154">Boolean</span></span>|<span data-ttu-id="d4e22-155">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="d4e22-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="d4e22-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d4e22-156">passwordBlockSimple</span></span>|<span data-ttu-id="d4e22-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4e22-157">Boolean</span></span>|<span data-ttu-id="d4e22-158">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="d4e22-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="d4e22-159">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="d4e22-159">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="d4e22-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4e22-160">Boolean</span></span>|<span data-ttu-id="d4e22-161">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="d4e22-161">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="d4e22-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d4e22-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d4e22-163">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e22-163">Int32</span></span>|<span data-ttu-id="d4e22-164">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="d4e22-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="d4e22-165">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d4e22-165">passwordExpirationDays</span></span>|<span data-ttu-id="d4e22-166">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e22-166">Int32</span></span>|<span data-ttu-id="d4e22-167">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="d4e22-167">The password expiration in days.</span></span>|
|<span data-ttu-id="d4e22-168">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d4e22-168">passwordMinimumLength</span></span>|<span data-ttu-id="d4e22-169">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e22-169">Int32</span></span>|<span data-ttu-id="d4e22-170">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="d4e22-170">The minimum password length.</span></span>|
|<span data-ttu-id="d4e22-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d4e22-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="d4e22-172">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e22-172">Int32</span></span>|<span data-ttu-id="d4e22-173">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="d4e22-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="d4e22-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d4e22-174">passwordRequiredType</span></span>|<span data-ttu-id="d4e22-175">String</span><span class="sxs-lookup"><span data-stu-id="d4e22-175">String</span></span>|<span data-ttu-id="d4e22-176">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="d4e22-176">The required password type.</span></span> <span data-ttu-id="d4e22-177">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="d4e22-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d4e22-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d4e22-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d4e22-179">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e22-179">Int32</span></span>|<span data-ttu-id="d4e22-180">Количество предыдущих паролей, повторное использование которых требуется запретить.</span><span class="sxs-lookup"><span data-stu-id="d4e22-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="d4e22-181">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="d4e22-181">requireHealthyDeviceReport</span></span>|<span data-ttu-id="d4e22-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4e22-182">Boolean</span></span>|<span data-ttu-id="d4e22-183">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="d4e22-183">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="d4e22-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="d4e22-184">osMinimumVersion</span></span>|<span data-ttu-id="d4e22-185">String</span><span class="sxs-lookup"><span data-stu-id="d4e22-185">String</span></span>|<span data-ttu-id="d4e22-186">Минимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="d4e22-186">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="d4e22-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="d4e22-187">osMaximumVersion</span></span>|<span data-ttu-id="d4e22-188">String</span><span class="sxs-lookup"><span data-stu-id="d4e22-188">String</span></span>|<span data-ttu-id="d4e22-189">Максимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="d4e22-189">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="d4e22-190">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="d4e22-190">mobileOsMinimumVersion</span></span>|<span data-ttu-id="d4e22-191">String</span><span class="sxs-lookup"><span data-stu-id="d4e22-191">String</span></span>|<span data-ttu-id="d4e22-192">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="d4e22-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="d4e22-193">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="d4e22-193">mobileOsMaximumVersion</span></span>|<span data-ttu-id="d4e22-194">String</span><span class="sxs-lookup"><span data-stu-id="d4e22-194">String</span></span>|<span data-ttu-id="d4e22-195">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="d4e22-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="d4e22-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="d4e22-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="d4e22-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4e22-197">Boolean</span></span>|<span data-ttu-id="d4e22-198">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="d4e22-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="d4e22-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="d4e22-199">bitLockerEnabled</span></span>|<span data-ttu-id="d4e22-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4e22-200">Boolean</span></span>|<span data-ttu-id="d4e22-201">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="d4e22-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="d4e22-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="d4e22-202">secureBootEnabled</span></span>|<span data-ttu-id="d4e22-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4e22-203">Boolean</span></span>|<span data-ttu-id="d4e22-204">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="d4e22-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="d4e22-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="d4e22-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="d4e22-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4e22-206">Boolean</span></span>|<span data-ttu-id="d4e22-207">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="d4e22-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="d4e22-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="d4e22-208">storageRequireEncryption</span></span>|<span data-ttu-id="d4e22-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4e22-209">Boolean</span></span>|<span data-ttu-id="d4e22-210">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="d4e22-210">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="d4e22-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4e22-211">Response</span></span>
<span data-ttu-id="d4e22-212">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d4e22-212">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4e22-213">Пример</span><span class="sxs-lookup"><span data-stu-id="d4e22-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4e22-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4e22-214">Request</span></span>
<span data-ttu-id="d4e22-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4e22-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4e22-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4e22-216">Response</span></span>
<span data-ttu-id="d4e22-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d4e22-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



