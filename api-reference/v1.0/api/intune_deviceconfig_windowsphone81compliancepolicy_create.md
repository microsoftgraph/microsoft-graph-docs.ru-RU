# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="e4814-101">Create windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e4814-101">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="e4814-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e4814-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4814-103">Создание объекта [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4814-103">Create a new [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4814-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e4814-104">Prerequisites</span></span>
<span data-ttu-id="e4814-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e4814-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e4814-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4814-107">Permission type</span></span>|<span data-ttu-id="e4814-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4814-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4814-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4814-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e4814-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4814-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4814-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4814-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4814-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4814-112">Not supported.</span></span>|
|<span data-ttu-id="e4814-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4814-113">Application</span></span>|<span data-ttu-id="e4814-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4814-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4814-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4814-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e4814-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4814-116">Request headers</span></span>
|<span data-ttu-id="e4814-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4814-117">Header</span></span>|<span data-ttu-id="e4814-118">Значение</span><span class="sxs-lookup"><span data-stu-id="e4814-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4814-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4814-119">Authorization</span></span>|<span data-ttu-id="e4814-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="e4814-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4814-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e4814-121">Accept</span></span>|<span data-ttu-id="e4814-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e4814-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4814-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4814-123">Request body</span></span>
<span data-ttu-id="e4814-124">В теле запроса добавьте представление объекта windowsPhone81CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4814-124">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="e4814-125">Ниже показаны свойства, которые необходимо указывать при создании объекта windowsPhone81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="e4814-125">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="e4814-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4814-126">Property</span></span>|<span data-ttu-id="e4814-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e4814-127">Type</span></span>|<span data-ttu-id="e4814-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e4814-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4814-129">id</span><span class="sxs-lookup"><span data-stu-id="e4814-129">id</span></span>|<span data-ttu-id="e4814-130">String</span><span class="sxs-lookup"><span data-stu-id="e4814-130">String</span></span>|<span data-ttu-id="e4814-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e4814-131">Key of the entity.</span></span> <span data-ttu-id="e4814-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4814-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4814-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4814-133">createdDateTime</span></span>|<span data-ttu-id="e4814-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4814-134">DateTimeOffset</span></span>|<span data-ttu-id="e4814-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e4814-135">DateTime the object was created.</span></span> <span data-ttu-id="e4814-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4814-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4814-137">description</span><span class="sxs-lookup"><span data-stu-id="e4814-137">description</span></span>|<span data-ttu-id="e4814-138">String</span><span class="sxs-lookup"><span data-stu-id="e4814-138">String</span></span>|<span data-ttu-id="e4814-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e4814-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e4814-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4814-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4814-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4814-141">lastModifiedDateTime</span></span>|<span data-ttu-id="e4814-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4814-142">DateTimeOffset</span></span>|<span data-ttu-id="e4814-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e4814-143">DateTime the object was last modified.</span></span> <span data-ttu-id="e4814-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4814-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4814-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e4814-145">displayName</span></span>|<span data-ttu-id="e4814-146">String</span><span class="sxs-lookup"><span data-stu-id="e4814-146">String</span></span>|<span data-ttu-id="e4814-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e4814-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e4814-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4814-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4814-149">version</span><span class="sxs-lookup"><span data-stu-id="e4814-149">version</span></span>|<span data-ttu-id="e4814-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e4814-150">Int32</span></span>|<span data-ttu-id="e4814-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e4814-151">Version of the device configuration.</span></span> <span data-ttu-id="e4814-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4814-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4814-153">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e4814-153">passwordBlockSimple</span></span>|<span data-ttu-id="e4814-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4814-154">Boolean</span></span>|<span data-ttu-id="e4814-155">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="e4814-155">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="e4814-156">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e4814-156">passwordExpirationDays</span></span>|<span data-ttu-id="e4814-157">Int32</span><span class="sxs-lookup"><span data-stu-id="e4814-157">Int32</span></span>|<span data-ttu-id="e4814-158">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="e4814-158">Number of days before the password expires.</span></span>|
|<span data-ttu-id="e4814-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e4814-159">passwordMinimumLength</span></span>|<span data-ttu-id="e4814-160">Int32</span><span class="sxs-lookup"><span data-stu-id="e4814-160">Int32</span></span>|<span data-ttu-id="e4814-161">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="e4814-161">Minimum length of passwords.</span></span>|
|<span data-ttu-id="e4814-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e4814-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e4814-163">Int32</span><span class="sxs-lookup"><span data-stu-id="e4814-163">Int32</span></span>|<span data-ttu-id="e4814-164">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="e4814-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="e4814-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e4814-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e4814-166">Int32</span><span class="sxs-lookup"><span data-stu-id="e4814-166">Int32</span></span>|<span data-ttu-id="e4814-167">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="e4814-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e4814-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e4814-168">passwordRequiredType</span></span>|[<span data-ttu-id="e4814-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e4814-169">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="e4814-170">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="e4814-170">The required password type.</span></span> <span data-ttu-id="e4814-171">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e4814-171">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="e4814-172">счётчик блокировки пароля при вводе предыдущего пароля</span><span class="sxs-lookup"><span data-stu-id="e4814-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e4814-173">Int32</span><span class="sxs-lookup"><span data-stu-id="e4814-173">Int32</span></span>|<span data-ttu-id="e4814-174">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="e4814-174">Number of previous passwords to block.</span></span> <span data-ttu-id="e4814-175">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="e4814-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e4814-176">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e4814-176">passwordRequired</span></span>|<span data-ttu-id="e4814-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4814-177">Boolean</span></span>|<span data-ttu-id="e4814-178">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="e4814-178">Whether or not to require a password.</span></span>|
|<span data-ttu-id="e4814-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e4814-179">osMinimumVersion</span></span>|<span data-ttu-id="e4814-180">String</span><span class="sxs-lookup"><span data-stu-id="e4814-180">String</span></span>|<span data-ttu-id="e4814-181">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="e4814-181">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="e4814-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e4814-182">osMaximumVersion</span></span>|<span data-ttu-id="e4814-183">String</span><span class="sxs-lookup"><span data-stu-id="e4814-183">String</span></span>|<span data-ttu-id="e4814-184">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="e4814-184">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="e4814-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e4814-185">storageRequireEncryption</span></span>|<span data-ttu-id="e4814-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4814-186">Boolean</span></span>|<span data-ttu-id="e4814-187">Указывает, обязательно ли шифрование данных на устройствах с Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="e4814-187">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="e4814-188">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4814-188">Response</span></span>
<span data-ttu-id="e4814-189">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e4814-189">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4814-190">Пример</span><span class="sxs-lookup"><span data-stu-id="e4814-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4814-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4814-191">Request</span></span>
<span data-ttu-id="e4814-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4814-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 671

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="e4814-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4814-193">Response</span></span>
<span data-ttu-id="e4814-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4814-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



