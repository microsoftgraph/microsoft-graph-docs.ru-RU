# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="dd0a9-101">Обновление объекта windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="dd0a9-101">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="dd0a9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd0a9-103">Обновление свойств объекта [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd0a9-103">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd0a9-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dd0a9-104">Prerequisites</span></span>
<span data-ttu-id="dd0a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dd0a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dd0a9-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd0a9-107">Permission type</span></span>|<span data-ttu-id="dd0a9-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd0a9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd0a9-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd0a9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="dd0a9-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd0a9-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd0a9-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd0a9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd0a9-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-112">Not supported.</span></span>|
|<span data-ttu-id="dd0a9-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd0a9-113">Application</span></span>|<span data-ttu-id="dd0a9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd0a9-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd0a9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="dd0a9-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd0a9-116">Request headers</span></span>
|<span data-ttu-id="dd0a9-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd0a9-117">Header</span></span>|<span data-ttu-id="dd0a9-118">Значение</span><span class="sxs-lookup"><span data-stu-id="dd0a9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd0a9-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd0a9-119">Authorization</span></span>|<span data-ttu-id="dd0a9-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="dd0a9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd0a9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="dd0a9-121">Accept</span></span>|<span data-ttu-id="dd0a9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="dd0a9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd0a9-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd0a9-123">Request body</span></span>
<span data-ttu-id="dd0a9-124">В теле запроса добавьте представление объекта [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-124">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="dd0a9-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd0a9-125">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="dd0a9-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd0a9-126">Property</span></span>|<span data-ttu-id="dd0a9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="dd0a9-127">Type</span></span>|<span data-ttu-id="dd0a9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="dd0a9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd0a9-129">id</span><span class="sxs-lookup"><span data-stu-id="dd0a9-129">id</span></span>|<span data-ttu-id="dd0a9-130">Строка</span><span class="sxs-lookup"><span data-stu-id="dd0a9-130">String</span></span>|<span data-ttu-id="dd0a9-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-131">Key of the entity.</span></span> <span data-ttu-id="dd0a9-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd0a9-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd0a9-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd0a9-133">createdDateTime</span></span>|<span data-ttu-id="dd0a9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd0a9-134">DateTimeOffset</span></span>|<span data-ttu-id="dd0a9-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-135">DateTime the object was created.</span></span> <span data-ttu-id="dd0a9-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd0a9-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd0a9-137">description</span><span class="sxs-lookup"><span data-stu-id="dd0a9-137">description</span></span>|<span data-ttu-id="dd0a9-138">String (строка)</span><span class="sxs-lookup"><span data-stu-id="dd0a9-138">String</span></span>|<span data-ttu-id="dd0a9-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dd0a9-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd0a9-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd0a9-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd0a9-141">lastModifiedDateTime</span></span>|<span data-ttu-id="dd0a9-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd0a9-142">DateTimeOffset</span></span>|<span data-ttu-id="dd0a9-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-143">DateTime the object was last modified.</span></span> <span data-ttu-id="dd0a9-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd0a9-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd0a9-145">displayName</span><span class="sxs-lookup"><span data-stu-id="dd0a9-145">displayName</span></span>|<span data-ttu-id="dd0a9-146">String (строка)</span><span class="sxs-lookup"><span data-stu-id="dd0a9-146">String</span></span>|<span data-ttu-id="dd0a9-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dd0a9-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd0a9-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd0a9-149">version</span><span class="sxs-lookup"><span data-stu-id="dd0a9-149">version</span></span>|<span data-ttu-id="dd0a9-150">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0a9-150">Int32</span></span>|<span data-ttu-id="dd0a9-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-151">Version of the device configuration.</span></span> <span data-ttu-id="dd0a9-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd0a9-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd0a9-153">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="dd0a9-153">passwordBlockSimple</span></span>|<span data-ttu-id="dd0a9-154">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="dd0a9-154">Boolean</span></span>|<span data-ttu-id="dd0a9-155">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-155">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="dd0a9-156">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="dd0a9-156">passwordExpirationDays</span></span>|<span data-ttu-id="dd0a9-157">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0a9-157">Int32</span></span>|<span data-ttu-id="dd0a9-158">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-158">Number of days before the password expires.</span></span>|
|<span data-ttu-id="dd0a9-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="dd0a9-159">passwordMinimumLength</span></span>|<span data-ttu-id="dd0a9-160">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0a9-160">Int32</span></span>|<span data-ttu-id="dd0a9-161">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-161">Minimum length of passwords.</span></span>|
|<span data-ttu-id="dd0a9-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="dd0a9-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="dd0a9-163">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0a9-163">Int32</span></span>|<span data-ttu-id="dd0a9-164">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="dd0a9-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="dd0a9-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="dd0a9-166">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0a9-166">Int32</span></span>|<span data-ttu-id="dd0a9-167">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="dd0a9-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="dd0a9-168">passwordRequiredType</span></span>|[<span data-ttu-id="dd0a9-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="dd0a9-169">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="dd0a9-170">Тип требуемого пароля.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-170">The required password type.</span></span> <span data-ttu-id="dd0a9-171">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-171">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="dd0a9-172">счётчик блокировки пароля при вводе предыдущего пароля</span><span class="sxs-lookup"><span data-stu-id="dd0a9-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="dd0a9-173">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0a9-173">Int32</span></span>|<span data-ttu-id="dd0a9-174">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-174">Number of previous passwords to block.</span></span> <span data-ttu-id="dd0a9-175">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="dd0a9-176">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="dd0a9-176">passwordRequired</span></span>|<span data-ttu-id="dd0a9-177">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="dd0a9-177">Boolean</span></span>|<span data-ttu-id="dd0a9-178">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-178">Whether or not to require a password.</span></span>|
|<span data-ttu-id="dd0a9-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="dd0a9-179">osMinimumVersion</span></span>|<span data-ttu-id="dd0a9-180">String (строка)</span><span class="sxs-lookup"><span data-stu-id="dd0a9-180">String</span></span>|<span data-ttu-id="dd0a9-181">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-181">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="dd0a9-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="dd0a9-182">osMaximumVersion</span></span>|<span data-ttu-id="dd0a9-183">String (строка)</span><span class="sxs-lookup"><span data-stu-id="dd0a9-183">String</span></span>|<span data-ttu-id="dd0a9-184">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-184">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="dd0a9-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="dd0a9-185">storageRequireEncryption</span></span>|<span data-ttu-id="dd0a9-186">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="dd0a9-186">Boolean</span></span>|<span data-ttu-id="dd0a9-187">Указывает, обязательно ли шифрование данных на устройствах с Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-187">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="dd0a9-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd0a9-188">Response</span></span>
<span data-ttu-id="dd0a9-189">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-189">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd0a9-190">Пример</span><span class="sxs-lookup"><span data-stu-id="dd0a9-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd0a9-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd0a9-191">Request</span></span>
<span data-ttu-id="dd0a9-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 602

{
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="dd0a9-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd0a9-193">Response</span></span>
<span data-ttu-id="dd0a9-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd0a9-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 779

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```



