# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="cde48-101">Create macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="cde48-101">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="cde48-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cde48-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cde48-103">Создание объекта [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cde48-103">Create a new [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cde48-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cde48-104">Prerequisites</span></span>
<span data-ttu-id="cde48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cde48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cde48-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cde48-107">Permission type</span></span>|<span data-ttu-id="cde48-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cde48-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cde48-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cde48-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cde48-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cde48-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cde48-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cde48-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cde48-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cde48-112">Not supported.</span></span>|
|<span data-ttu-id="cde48-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cde48-113">Application</span></span>|<span data-ttu-id="cde48-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cde48-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cde48-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cde48-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="cde48-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cde48-116">Request headers</span></span>
|<span data-ttu-id="cde48-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cde48-117">Header</span></span>|<span data-ttu-id="cde48-118">Значение</span><span class="sxs-lookup"><span data-stu-id="cde48-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cde48-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="cde48-119">Authorization</span></span>|<span data-ttu-id="cde48-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cde48-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cde48-121">Accept</span><span class="sxs-lookup"><span data-stu-id="cde48-121">Accept</span></span>|<span data-ttu-id="cde48-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cde48-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cde48-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cde48-123">Request body</span></span>
<span data-ttu-id="cde48-124">В теле запроса добавьте представление объекта macOSCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cde48-124">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="cde48-125">Ниже показаны свойства, которые необходимо указывать при создании объекта macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="cde48-125">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="cde48-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="cde48-126">Property</span></span>|<span data-ttu-id="cde48-127">Тип</span><span class="sxs-lookup"><span data-stu-id="cde48-127">Type</span></span>|<span data-ttu-id="cde48-128">Описание</span><span class="sxs-lookup"><span data-stu-id="cde48-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cde48-129">id</span><span class="sxs-lookup"><span data-stu-id="cde48-129">id</span></span>|<span data-ttu-id="cde48-130">String</span><span class="sxs-lookup"><span data-stu-id="cde48-130">String</span></span>|<span data-ttu-id="cde48-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cde48-131">Key of the entity.</span></span> <span data-ttu-id="cde48-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cde48-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cde48-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cde48-133">createdDateTime</span></span>|<span data-ttu-id="cde48-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cde48-134">DateTimeOffset</span></span>|<span data-ttu-id="cde48-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="cde48-135">DateTime the object was created.</span></span> <span data-ttu-id="cde48-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cde48-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cde48-137">description</span><span class="sxs-lookup"><span data-stu-id="cde48-137">description</span></span>|<span data-ttu-id="cde48-138">String</span><span class="sxs-lookup"><span data-stu-id="cde48-138">String</span></span>|<span data-ttu-id="cde48-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cde48-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cde48-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cde48-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cde48-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cde48-141">lastModifiedDateTime</span></span>|<span data-ttu-id="cde48-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cde48-142">DateTimeOffset</span></span>|<span data-ttu-id="cde48-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cde48-143">DateTime the object was last modified.</span></span> <span data-ttu-id="cde48-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cde48-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cde48-145">displayName</span><span class="sxs-lookup"><span data-stu-id="cde48-145">displayName</span></span>|<span data-ttu-id="cde48-146">String</span><span class="sxs-lookup"><span data-stu-id="cde48-146">String</span></span>|<span data-ttu-id="cde48-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cde48-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cde48-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cde48-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cde48-149">version</span><span class="sxs-lookup"><span data-stu-id="cde48-149">version</span></span>|<span data-ttu-id="cde48-150">Int32</span><span class="sxs-lookup"><span data-stu-id="cde48-150">Int32</span></span>|<span data-ttu-id="cde48-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cde48-151">Version of the device configuration.</span></span> <span data-ttu-id="cde48-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cde48-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cde48-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="cde48-153">passwordRequired</span></span>|<span data-ttu-id="cde48-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="cde48-154">Boolean</span></span>|<span data-ttu-id="cde48-155">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="cde48-155">Whether or not to require a password.</span></span>|
|<span data-ttu-id="cde48-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="cde48-156">passwordBlockSimple</span></span>|<span data-ttu-id="cde48-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="cde48-157">Boolean</span></span>|<span data-ttu-id="cde48-158">Указывает, требуется ли блокировать простые пароли.</span><span class="sxs-lookup"><span data-stu-id="cde48-158">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="cde48-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cde48-159">passwordExpirationDays</span></span>|<span data-ttu-id="cde48-160">Int32</span><span class="sxs-lookup"><span data-stu-id="cde48-160">Int32</span></span>|<span data-ttu-id="cde48-161">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="cde48-161">Number of days before the password expires.</span></span> <span data-ttu-id="cde48-162">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="cde48-162">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="cde48-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cde48-163">passwordMinimumLength</span></span>|<span data-ttu-id="cde48-164">Int32</span><span class="sxs-lookup"><span data-stu-id="cde48-164">Int32</span></span>|<span data-ttu-id="cde48-165">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="cde48-165">Minimum length of password.</span></span> <span data-ttu-id="cde48-166">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="cde48-166">Valid values 4 to 14</span></span>|
|<span data-ttu-id="cde48-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="cde48-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="cde48-168">Int32</span><span class="sxs-lookup"><span data-stu-id="cde48-168">Int32</span></span>|<span data-ttu-id="cde48-169">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="cde48-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="cde48-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="cde48-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="cde48-171">Int32</span><span class="sxs-lookup"><span data-stu-id="cde48-171">Int32</span></span>|<span data-ttu-id="cde48-172">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="cde48-172">Number of previous passwords to block.</span></span> <span data-ttu-id="cde48-173">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="cde48-173">Valid values 1 to 24</span></span>|
|<span data-ttu-id="cde48-174">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="cde48-174">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="cde48-175">Int32</span><span class="sxs-lookup"><span data-stu-id="cde48-175">Int32</span></span>|<span data-ttu-id="cde48-176">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="cde48-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="cde48-177">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="cde48-177">passwordRequiredType</span></span>|[<span data-ttu-id="cde48-178">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="cde48-178">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="cde48-179">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="cde48-179">The required password type.</span></span> <span data-ttu-id="cde48-180">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="cde48-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="cde48-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="cde48-181">osMinimumVersion</span></span>|<span data-ttu-id="cde48-182">String</span><span class="sxs-lookup"><span data-stu-id="cde48-182">String</span></span>|<span data-ttu-id="cde48-183">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="cde48-183">Minimum IOS version.</span></span>|
|<span data-ttu-id="cde48-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="cde48-184">osMaximumVersion</span></span>|<span data-ttu-id="cde48-185">String</span><span class="sxs-lookup"><span data-stu-id="cde48-185">String</span></span>|<span data-ttu-id="cde48-186">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="cde48-186">Maximum IOS version.</span></span>|
|<span data-ttu-id="cde48-187">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="cde48-187">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="cde48-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="cde48-188">Boolean</span></span>|<span data-ttu-id="cde48-189">Указывает на то, что защита целостности системы для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="cde48-189">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="cde48-190">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="cde48-190">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="cde48-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="cde48-191">Boolean</span></span>|<span data-ttu-id="cde48-192">Указывает на то, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="cde48-192">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="cde48-193">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="cde48-193">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="cde48-194">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="cde48-194">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="cde48-195">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="cde48-195">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="cde48-196">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="cde48-196">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="cde48-197">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="cde48-197">storageRequireEncryption</span></span>|<span data-ttu-id="cde48-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="cde48-198">Boolean</span></span>|<span data-ttu-id="cde48-199">Указывает, обязательно ли шифрование данных на устройствах с Mac OS.</span><span class="sxs-lookup"><span data-stu-id="cde48-199">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="cde48-200">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="cde48-200">firewallEnabled</span></span>|<span data-ttu-id="cde48-201">Логический</span><span class="sxs-lookup"><span data-stu-id="cde48-201">Boolean</span></span>|<span data-ttu-id="cde48-202">Является ли брандмауэра должна быть включена или нет.</span><span class="sxs-lookup"><span data-stu-id="cde48-202">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="cde48-203">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="cde48-203">firewallBlockAllIncoming</span></span>|<span data-ttu-id="cde48-204">Логический</span><span class="sxs-lookup"><span data-stu-id="cde48-204">Boolean</span></span>|<span data-ttu-id="cde48-205">Соответствующий параметр «Блокировать все входящие подключения».</span><span class="sxs-lookup"><span data-stu-id="cde48-205">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="cde48-206">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="cde48-206">firewallEnableStealthMode</span></span>|<span data-ttu-id="cde48-207">Логический</span><span class="sxs-lookup"><span data-stu-id="cde48-207">Boolean</span></span>|<span data-ttu-id="cde48-208">Соответствует «Включить режим скрытое».</span><span class="sxs-lookup"><span data-stu-id="cde48-208">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="cde48-209">Ответ</span><span class="sxs-lookup"><span data-stu-id="cde48-209">Response</span></span>
<span data-ttu-id="cde48-210">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cde48-210">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cde48-211">Пример</span><span class="sxs-lookup"><span data-stu-id="cde48-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="cde48-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="cde48-212">Request</span></span>
<span data-ttu-id="cde48-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cde48-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="cde48-214">Ответ</span><span class="sxs-lookup"><span data-stu-id="cde48-214">Response</span></span>
<span data-ttu-id="cde48-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cde48-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



