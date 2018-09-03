# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="748cb-101">Update iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="748cb-101">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="748cb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="748cb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="748cb-103">Обновление свойств объекта [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="748cb-103">Update the properties of a [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="748cb-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="748cb-104">Prerequisites</span></span>
<span data-ttu-id="748cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="748cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="748cb-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="748cb-107">Permission type</span></span>|<span data-ttu-id="748cb-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="748cb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="748cb-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="748cb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="748cb-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="748cb-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="748cb-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="748cb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="748cb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="748cb-112">Not supported.</span></span>|
|<span data-ttu-id="748cb-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="748cb-113">Application</span></span>|<span data-ttu-id="748cb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="748cb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="748cb-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="748cb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="748cb-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="748cb-116">Request headers</span></span>
|<span data-ttu-id="748cb-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="748cb-117">Header</span></span>|<span data-ttu-id="748cb-118">Значение</span><span class="sxs-lookup"><span data-stu-id="748cb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="748cb-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="748cb-119">Authorization</span></span>|<span data-ttu-id="748cb-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="748cb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="748cb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="748cb-121">Accept</span></span>|<span data-ttu-id="748cb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="748cb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="748cb-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="748cb-123">Request body</span></span>
<span data-ttu-id="748cb-124">В теле запроса добавьте представление объекта [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="748cb-124">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="748cb-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="748cb-125">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="748cb-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="748cb-126">Property</span></span>|<span data-ttu-id="748cb-127">Тип</span><span class="sxs-lookup"><span data-stu-id="748cb-127">Type</span></span>|<span data-ttu-id="748cb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="748cb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="748cb-129">id</span><span class="sxs-lookup"><span data-stu-id="748cb-129">id</span></span>|<span data-ttu-id="748cb-130">Строка</span><span class="sxs-lookup"><span data-stu-id="748cb-130">String</span></span>|<span data-ttu-id="748cb-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="748cb-131">Key of the entity.</span></span> <span data-ttu-id="748cb-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="748cb-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="748cb-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="748cb-133">createdDateTime</span></span>|<span data-ttu-id="748cb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="748cb-134">DateTimeOffset</span></span>|<span data-ttu-id="748cb-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="748cb-135">DateTime the object was created.</span></span> <span data-ttu-id="748cb-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="748cb-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="748cb-137">description</span><span class="sxs-lookup"><span data-stu-id="748cb-137">description</span></span>|<span data-ttu-id="748cb-138">Строка</span><span class="sxs-lookup"><span data-stu-id="748cb-138">String</span></span>|<span data-ttu-id="748cb-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="748cb-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="748cb-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="748cb-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="748cb-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="748cb-141">lastModifiedDateTime</span></span>|<span data-ttu-id="748cb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="748cb-142">DateTimeOffset</span></span>|<span data-ttu-id="748cb-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="748cb-143">DateTime the object was last modified.</span></span> <span data-ttu-id="748cb-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="748cb-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="748cb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="748cb-145">displayName</span></span>|<span data-ttu-id="748cb-146">Строка</span><span class="sxs-lookup"><span data-stu-id="748cb-146">String</span></span>|<span data-ttu-id="748cb-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="748cb-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="748cb-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="748cb-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="748cb-149">version</span><span class="sxs-lookup"><span data-stu-id="748cb-149">version</span></span>|<span data-ttu-id="748cb-150">Int32</span><span class="sxs-lookup"><span data-stu-id="748cb-150">Int32</span></span>|<span data-ttu-id="748cb-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="748cb-151">Version of the device configuration.</span></span> <span data-ttu-id="748cb-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="748cb-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="748cb-153">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="748cb-153">passcodeBlockSimple</span></span>|<span data-ttu-id="748cb-154">Логический</span><span class="sxs-lookup"><span data-stu-id="748cb-154">Boolean</span></span>|<span data-ttu-id="748cb-155">Указывает, следует ли блокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="748cb-155">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="748cb-156">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="748cb-156">passcodeExpirationDays</span></span>|<span data-ttu-id="748cb-157">Int32</span><span class="sxs-lookup"><span data-stu-id="748cb-157">Int32</span></span>|<span data-ttu-id="748cb-158">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="748cb-158">Number of days before the passcode expires.</span></span> <span data-ttu-id="748cb-159">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="748cb-159">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="748cb-160">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="748cb-160">passcodeMinimumLength</span></span>|<span data-ttu-id="748cb-161">Int32</span><span class="sxs-lookup"><span data-stu-id="748cb-161">Int32</span></span>|<span data-ttu-id="748cb-162">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="748cb-162">Minimum length of passcode.</span></span> <span data-ttu-id="748cb-163">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="748cb-163">Valid values 4 to 14</span></span>|
|<span data-ttu-id="748cb-164">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="748cb-164">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="748cb-165">Int32</span><span class="sxs-lookup"><span data-stu-id="748cb-165">Int32</span></span>|<span data-ttu-id="748cb-166">Период бездействия (в минутах), по истечении которого будет запрашиваться секретный код.</span><span class="sxs-lookup"><span data-stu-id="748cb-166">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="748cb-167">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="748cb-167">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="748cb-168">Int32</span><span class="sxs-lookup"><span data-stu-id="748cb-168">Int32</span></span>|<span data-ttu-id="748cb-169">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="748cb-169">Number of previous passcodes to block.</span></span> <span data-ttu-id="748cb-170">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="748cb-170">Valid values 1 to 24</span></span>|
|<span data-ttu-id="748cb-171">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="748cb-171">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="748cb-172">Int32</span><span class="sxs-lookup"><span data-stu-id="748cb-172">Int32</span></span>|<span data-ttu-id="748cb-173">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="748cb-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="748cb-174">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="748cb-174">passcodeRequiredType</span></span>|[<span data-ttu-id="748cb-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="748cb-175">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="748cb-176">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="748cb-176">The required passcode type.</span></span> <span data-ttu-id="748cb-177">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="748cb-177">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="748cb-178">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="748cb-178">passcodeRequired</span></span>|<span data-ttu-id="748cb-179">Логический</span><span class="sxs-lookup"><span data-stu-id="748cb-179">Boolean</span></span>|<span data-ttu-id="748cb-180">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="748cb-180">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="748cb-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="748cb-181">osMinimumVersion</span></span>|<span data-ttu-id="748cb-182">Строка</span><span class="sxs-lookup"><span data-stu-id="748cb-182">String</span></span>|<span data-ttu-id="748cb-183">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="748cb-183">Minimum IOS version.</span></span>|
|<span data-ttu-id="748cb-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="748cb-184">osMaximumVersion</span></span>|<span data-ttu-id="748cb-185">Строка</span><span class="sxs-lookup"><span data-stu-id="748cb-185">String</span></span>|<span data-ttu-id="748cb-186">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="748cb-186">Maximum IOS version.</span></span>|
|<span data-ttu-id="748cb-187">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="748cb-187">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="748cb-188">Логический</span><span class="sxs-lookup"><span data-stu-id="748cb-188">Boolean</span></span>|<span data-ttu-id="748cb-189">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="748cb-189">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="748cb-190">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="748cb-190">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="748cb-191">Логический</span><span class="sxs-lookup"><span data-stu-id="748cb-191">Boolean</span></span>|<span data-ttu-id="748cb-192">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="748cb-192">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="748cb-193">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="748cb-193">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="748cb-194">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="748cb-194">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="748cb-195">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="748cb-195">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="748cb-196">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="748cb-196">The possible values are `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`, , , , , , or .</span></span>|
|<span data-ttu-id="748cb-197">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="748cb-197">managedEmailProfileRequired</span></span>|<span data-ttu-id="748cb-198">Логический</span><span class="sxs-lookup"><span data-stu-id="748cb-198">Boolean</span></span>|<span data-ttu-id="748cb-199">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="748cb-199">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="748cb-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="748cb-200">Response</span></span>
<span data-ttu-id="748cb-201">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="748cb-201">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="748cb-202">Пример</span><span class="sxs-lookup"><span data-stu-id="748cb-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="748cb-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="748cb-203">Request</span></span>
<span data-ttu-id="748cb-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="748cb-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 751

{
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```

### <a name="response"></a><span data-ttu-id="748cb-205">Ответ</span><span class="sxs-lookup"><span data-stu-id="748cb-205">Response</span></span>
<span data-ttu-id="748cb-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="748cb-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "id": "4f501351-1351-4f50-5113-504f5113504f",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```



