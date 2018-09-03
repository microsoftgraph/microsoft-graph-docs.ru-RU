# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="f8634-101">Создание объекта windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f8634-101">Create windows81CompliancePolicy</span></span>

> <span data-ttu-id="f8634-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f8634-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8634-103">Создание объекта [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f8634-103">Create a new [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8634-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f8634-104">Prerequisites</span></span>
<span data-ttu-id="f8634-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f8634-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f8634-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8634-107">Permission type</span></span>|<span data-ttu-id="f8634-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8634-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8634-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8634-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f8634-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8634-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8634-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8634-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8634-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8634-112">Not supported.</span></span>|
|<span data-ttu-id="f8634-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8634-113">Application</span></span>|<span data-ttu-id="f8634-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8634-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8634-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8634-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f8634-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8634-116">Request headers</span></span>
|<span data-ttu-id="f8634-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8634-117">Header</span></span>|<span data-ttu-id="f8634-118">Значение</span><span class="sxs-lookup"><span data-stu-id="f8634-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8634-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8634-119">Authorization</span></span>|<span data-ttu-id="f8634-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="f8634-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8634-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f8634-121">Accept</span></span>|<span data-ttu-id="f8634-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f8634-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8634-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f8634-123">Request body</span></span>
<span data-ttu-id="f8634-124">В теле запроса добавьте представление объекта windows81CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8634-124">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="f8634-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windows81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="f8634-125">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="f8634-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8634-126">Property</span></span>|<span data-ttu-id="f8634-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f8634-127">Type</span></span>|<span data-ttu-id="f8634-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f8634-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8634-129">id</span><span class="sxs-lookup"><span data-stu-id="f8634-129">id</span></span>|<span data-ttu-id="f8634-130">Строка</span><span class="sxs-lookup"><span data-stu-id="f8634-130">String</span></span>|<span data-ttu-id="f8634-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f8634-131">Key of the entity.</span></span> <span data-ttu-id="f8634-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f8634-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f8634-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8634-133">createdDateTime</span></span>|<span data-ttu-id="f8634-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8634-134">DateTimeOffset</span></span>|<span data-ttu-id="f8634-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f8634-135">DateTime the object was created.</span></span> <span data-ttu-id="f8634-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f8634-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f8634-137">description</span><span class="sxs-lookup"><span data-stu-id="f8634-137">description</span></span>|<span data-ttu-id="f8634-138">Строка</span><span class="sxs-lookup"><span data-stu-id="f8634-138">String</span></span>|<span data-ttu-id="f8634-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f8634-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f8634-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f8634-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f8634-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8634-141">lastModifiedDateTime</span></span>|<span data-ttu-id="f8634-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8634-142">DateTimeOffset</span></span>|<span data-ttu-id="f8634-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f8634-143">DateTime the object was last modified.</span></span> <span data-ttu-id="f8634-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f8634-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f8634-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f8634-145">displayName</span></span>|<span data-ttu-id="f8634-146">Строка</span><span class="sxs-lookup"><span data-stu-id="f8634-146">String</span></span>|<span data-ttu-id="f8634-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f8634-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f8634-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f8634-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f8634-149">version</span><span class="sxs-lookup"><span data-stu-id="f8634-149">version</span></span>|<span data-ttu-id="f8634-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f8634-150">Int32</span></span>|<span data-ttu-id="f8634-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f8634-151">Version of the device configuration.</span></span> <span data-ttu-id="f8634-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f8634-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f8634-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f8634-153">passwordRequired</span></span>|<span data-ttu-id="f8634-154">Логический</span><span class="sxs-lookup"><span data-stu-id="f8634-154">Boolean</span></span>|<span data-ttu-id="f8634-155">Указывает, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="f8634-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="f8634-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f8634-156">passwordBlockSimple</span></span>|<span data-ttu-id="f8634-157">Логический</span><span class="sxs-lookup"><span data-stu-id="f8634-157">Boolean</span></span>|<span data-ttu-id="f8634-158">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="f8634-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="f8634-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f8634-159">passwordExpirationDays</span></span>|<span data-ttu-id="f8634-160">Int32</span><span class="sxs-lookup"><span data-stu-id="f8634-160">Int32</span></span>|<span data-ttu-id="f8634-161">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="f8634-161">Password expiration in days.</span></span>|
|<span data-ttu-id="f8634-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f8634-162">passwordMinimumLength</span></span>|<span data-ttu-id="f8634-163">Int32</span><span class="sxs-lookup"><span data-stu-id="f8634-163">Int32</span></span>|<span data-ttu-id="f8634-164">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="f8634-164">The minimum password length.</span></span>|
|<span data-ttu-id="f8634-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f8634-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f8634-166">Int32</span><span class="sxs-lookup"><span data-stu-id="f8634-166">Int32</span></span>|<span data-ttu-id="f8634-167">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="f8634-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f8634-168">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f8634-168">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f8634-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f8634-169">Int32</span></span>|<span data-ttu-id="f8634-170">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="f8634-170">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f8634-171">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f8634-171">passwordRequiredType</span></span>|[<span data-ttu-id="f8634-172">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f8634-172">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="f8634-173">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="f8634-173">The required password type.</span></span> <span data-ttu-id="f8634-174">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f8634-174">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="f8634-175">счётчик блокировки пароля при вводе предыдущего пароля</span><span class="sxs-lookup"><span data-stu-id="f8634-175">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f8634-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f8634-176">Int32</span></span>|<span data-ttu-id="f8634-177">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="f8634-177">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="f8634-178">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="f8634-178">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f8634-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f8634-179">osMinimumVersion</span></span>|<span data-ttu-id="f8634-180">Строка</span><span class="sxs-lookup"><span data-stu-id="f8634-180">String</span></span>|<span data-ttu-id="f8634-181">Минимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="f8634-181">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="f8634-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f8634-182">osMaximumVersion</span></span>|<span data-ttu-id="f8634-183">Строка</span><span class="sxs-lookup"><span data-stu-id="f8634-183">String</span></span>|<span data-ttu-id="f8634-184">Максимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="f8634-184">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="f8634-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f8634-185">storageRequireEncryption</span></span>|<span data-ttu-id="f8634-186">Логический</span><span class="sxs-lookup"><span data-stu-id="f8634-186">Boolean</span></span>|<span data-ttu-id="f8634-187">Указывает, обязательно ли шифрование данных на устройстве с Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="f8634-187">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="f8634-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8634-188">Response</span></span>
<span data-ttu-id="f8634-189">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f8634-189">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8634-190">Пример</span><span class="sxs-lookup"><span data-stu-id="f8634-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8634-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8634-191">Request</span></span>
<span data-ttu-id="f8634-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8634-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 666

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="f8634-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8634-193">Response</span></span>
<span data-ttu-id="f8634-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8634-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 774

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
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
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```



