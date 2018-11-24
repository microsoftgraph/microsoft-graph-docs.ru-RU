# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="612db-101">Update macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="612db-101">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="612db-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="612db-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="612db-103">Обновление свойств объекта [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="612db-103">Update the properties of a [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="612db-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="612db-104">Prerequisites</span></span>
<span data-ttu-id="612db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="612db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="612db-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="612db-107">Permission type</span></span>|<span data-ttu-id="612db-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="612db-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="612db-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="612db-109">Delegated (work or school account)</span></span>|<span data-ttu-id="612db-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="612db-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="612db-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="612db-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="612db-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="612db-112">Not supported.</span></span>|
|<span data-ttu-id="612db-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="612db-113">Application</span></span>|<span data-ttu-id="612db-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="612db-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="612db-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="612db-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="612db-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="612db-116">Request headers</span></span>
|<span data-ttu-id="612db-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="612db-117">Header</span></span>|<span data-ttu-id="612db-118">Значение</span><span class="sxs-lookup"><span data-stu-id="612db-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="612db-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="612db-119">Authorization</span></span>|<span data-ttu-id="612db-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="612db-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="612db-121">Accept</span><span class="sxs-lookup"><span data-stu-id="612db-121">Accept</span></span>|<span data-ttu-id="612db-122">application/json</span><span class="sxs-lookup"><span data-stu-id="612db-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="612db-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="612db-123">Request body</span></span>
<span data-ttu-id="612db-124">В теле запроса добавьте представление объекта [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="612db-124">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="612db-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="612db-125">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="612db-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="612db-126">Property</span></span>|<span data-ttu-id="612db-127">Тип</span><span class="sxs-lookup"><span data-stu-id="612db-127">Type</span></span>|<span data-ttu-id="612db-128">Описание</span><span class="sxs-lookup"><span data-stu-id="612db-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="612db-129">id</span><span class="sxs-lookup"><span data-stu-id="612db-129">id</span></span>|<span data-ttu-id="612db-130">String</span><span class="sxs-lookup"><span data-stu-id="612db-130">String</span></span>|<span data-ttu-id="612db-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="612db-131">Key of the entity.</span></span> <span data-ttu-id="612db-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="612db-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="612db-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="612db-133">createdDateTime</span></span>|<span data-ttu-id="612db-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="612db-134">DateTimeOffset</span></span>|<span data-ttu-id="612db-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="612db-135">DateTime the object was created.</span></span> <span data-ttu-id="612db-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="612db-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="612db-137">description</span><span class="sxs-lookup"><span data-stu-id="612db-137">description</span></span>|<span data-ttu-id="612db-138">String</span><span class="sxs-lookup"><span data-stu-id="612db-138">String</span></span>|<span data-ttu-id="612db-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="612db-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="612db-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="612db-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="612db-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="612db-141">lastModifiedDateTime</span></span>|<span data-ttu-id="612db-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="612db-142">DateTimeOffset</span></span>|<span data-ttu-id="612db-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="612db-143">DateTime the object was last modified.</span></span> <span data-ttu-id="612db-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="612db-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="612db-145">displayName</span><span class="sxs-lookup"><span data-stu-id="612db-145">displayName</span></span>|<span data-ttu-id="612db-146">String</span><span class="sxs-lookup"><span data-stu-id="612db-146">String</span></span>|<span data-ttu-id="612db-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="612db-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="612db-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="612db-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="612db-149">version</span><span class="sxs-lookup"><span data-stu-id="612db-149">version</span></span>|<span data-ttu-id="612db-150">Int32</span><span class="sxs-lookup"><span data-stu-id="612db-150">Int32</span></span>|<span data-ttu-id="612db-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="612db-151">Version of the device configuration.</span></span> <span data-ttu-id="612db-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="612db-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="612db-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="612db-153">passwordRequired</span></span>|<span data-ttu-id="612db-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="612db-154">Boolean</span></span>|<span data-ttu-id="612db-155">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="612db-155">Whether or not to require a password.</span></span>|
|<span data-ttu-id="612db-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="612db-156">passwordBlockSimple</span></span>|<span data-ttu-id="612db-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="612db-157">Boolean</span></span>|<span data-ttu-id="612db-158">Указывает, требуется ли блокировать простые пароли.</span><span class="sxs-lookup"><span data-stu-id="612db-158">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="612db-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="612db-159">passwordExpirationDays</span></span>|<span data-ttu-id="612db-160">Int32</span><span class="sxs-lookup"><span data-stu-id="612db-160">Int32</span></span>|<span data-ttu-id="612db-161">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="612db-161">Number of days before the password expires.</span></span> <span data-ttu-id="612db-162">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="612db-162">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="612db-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="612db-163">passwordMinimumLength</span></span>|<span data-ttu-id="612db-164">Int32</span><span class="sxs-lookup"><span data-stu-id="612db-164">Int32</span></span>|<span data-ttu-id="612db-165">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="612db-165">Minimum length of password.</span></span> <span data-ttu-id="612db-166">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="612db-166">Valid values 4 to 14</span></span>|
|<span data-ttu-id="612db-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="612db-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="612db-168">Int32</span><span class="sxs-lookup"><span data-stu-id="612db-168">Int32</span></span>|<span data-ttu-id="612db-169">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="612db-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="612db-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="612db-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="612db-171">Int32</span><span class="sxs-lookup"><span data-stu-id="612db-171">Int32</span></span>|<span data-ttu-id="612db-172">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="612db-172">Number of previous passwords to block.</span></span> <span data-ttu-id="612db-173">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="612db-173">Valid values 1 to 24</span></span>|
|<span data-ttu-id="612db-174">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="612db-174">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="612db-175">Int32</span><span class="sxs-lookup"><span data-stu-id="612db-175">Int32</span></span>|<span data-ttu-id="612db-176">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="612db-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="612db-177">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="612db-177">passwordRequiredType</span></span>|[<span data-ttu-id="612db-178">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="612db-178">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="612db-179">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="612db-179">The required password type.</span></span> <span data-ttu-id="612db-180">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="612db-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="612db-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="612db-181">osMinimumVersion</span></span>|<span data-ttu-id="612db-182">String</span><span class="sxs-lookup"><span data-stu-id="612db-182">String</span></span>|<span data-ttu-id="612db-183">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="612db-183">Minimum IOS version.</span></span>|
|<span data-ttu-id="612db-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="612db-184">osMaximumVersion</span></span>|<span data-ttu-id="612db-185">String</span><span class="sxs-lookup"><span data-stu-id="612db-185">String</span></span>|<span data-ttu-id="612db-186">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="612db-186">Maximum IOS version.</span></span>|
|<span data-ttu-id="612db-187">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="612db-187">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="612db-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="612db-188">Boolean</span></span>|<span data-ttu-id="612db-189">Указывает на то, что защита целостности системы для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="612db-189">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="612db-190">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="612db-190">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="612db-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="612db-191">Boolean</span></span>|<span data-ttu-id="612db-192">Указывает на то, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="612db-192">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="612db-193">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="612db-193">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="612db-194">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="612db-194">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="612db-195">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="612db-195">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="612db-196">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="612db-196">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="612db-197">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="612db-197">storageRequireEncryption</span></span>|<span data-ttu-id="612db-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="612db-198">Boolean</span></span>|<span data-ttu-id="612db-199">Указывает, обязательно ли шифрование данных на устройствах с Mac OS.</span><span class="sxs-lookup"><span data-stu-id="612db-199">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="612db-200">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="612db-200">firewallEnabled</span></span>|<span data-ttu-id="612db-201">Логический</span><span class="sxs-lookup"><span data-stu-id="612db-201">Boolean</span></span>|<span data-ttu-id="612db-202">Является ли брандмауэра должна быть включена или нет.</span><span class="sxs-lookup"><span data-stu-id="612db-202">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="612db-203">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="612db-203">firewallBlockAllIncoming</span></span>|<span data-ttu-id="612db-204">Логический</span><span class="sxs-lookup"><span data-stu-id="612db-204">Boolean</span></span>|<span data-ttu-id="612db-205">Соответствующий параметр «Блокировать все входящие подключения».</span><span class="sxs-lookup"><span data-stu-id="612db-205">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="612db-206">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="612db-206">firewallEnableStealthMode</span></span>|<span data-ttu-id="612db-207">Логический</span><span class="sxs-lookup"><span data-stu-id="612db-207">Boolean</span></span>|<span data-ttu-id="612db-208">Соответствует «Включить режим скрытое».</span><span class="sxs-lookup"><span data-stu-id="612db-208">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="612db-209">Ответ</span><span class="sxs-lookup"><span data-stu-id="612db-209">Response</span></span>
<span data-ttu-id="612db-210">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="612db-210">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="612db-211">Пример</span><span class="sxs-lookup"><span data-stu-id="612db-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="612db-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="612db-212">Request</span></span>
<span data-ttu-id="612db-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="612db-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 849

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="612db-214">Ответ</span><span class="sxs-lookup"><span data-stu-id="612db-214">Response</span></span>
<span data-ttu-id="612db-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="612db-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1021

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```



