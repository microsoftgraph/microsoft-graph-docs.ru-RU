# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="c8cb1-101">Обновление объекта windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c8cb1-101">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="c8cb1-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8cb1-103">Обновление свойств объекта [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c8cb1-103">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8cb1-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c8cb1-104">Prerequisites</span></span>
<span data-ttu-id="c8cb1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c8cb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c8cb1-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8cb1-107">Permission type</span></span>|<span data-ttu-id="c8cb1-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8cb1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8cb1-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8cb1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c8cb1-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8cb1-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8cb1-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8cb1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8cb1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-112">Not supported.</span></span>|
|<span data-ttu-id="c8cb1-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8cb1-113">Application</span></span>|<span data-ttu-id="c8cb1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8cb1-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8cb1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="c8cb1-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8cb1-116">Request headers</span></span>
|<span data-ttu-id="c8cb1-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8cb1-117">Header</span></span>|<span data-ttu-id="c8cb1-118">Значение</span><span class="sxs-lookup"><span data-stu-id="c8cb1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8cb1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8cb1-119">Authorization</span></span>|<span data-ttu-id="c8cb1-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8cb1-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c8cb1-121">Accept</span></span>|<span data-ttu-id="c8cb1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c8cb1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8cb1-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c8cb1-123">Request body</span></span>
<span data-ttu-id="c8cb1-124">В теле запроса добавьте представление объекта [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-124">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="c8cb1-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c8cb1-125">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="c8cb1-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8cb1-126">Property</span></span>|<span data-ttu-id="c8cb1-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c8cb1-127">Type</span></span>|<span data-ttu-id="c8cb1-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c8cb1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8cb1-129">id</span><span class="sxs-lookup"><span data-stu-id="c8cb1-129">id</span></span>|<span data-ttu-id="c8cb1-130">String</span><span class="sxs-lookup"><span data-stu-id="c8cb1-130">String</span></span>|<span data-ttu-id="c8cb1-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-131">Key of the entity.</span></span> <span data-ttu-id="c8cb1-132">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c8cb1-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c8cb1-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8cb1-133">createdDateTime</span></span>|<span data-ttu-id="c8cb1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8cb1-134">DateTimeOffset</span></span>|<span data-ttu-id="c8cb1-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-135">DateTime the object was created.</span></span> <span data-ttu-id="c8cb1-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c8cb1-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c8cb1-137">description</span><span class="sxs-lookup"><span data-stu-id="c8cb1-137">description</span></span>|<span data-ttu-id="c8cb1-138">String</span><span class="sxs-lookup"><span data-stu-id="c8cb1-138">String</span></span>|<span data-ttu-id="c8cb1-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c8cb1-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c8cb1-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c8cb1-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8cb1-141">lastModifiedDateTime</span></span>|<span data-ttu-id="c8cb1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8cb1-142">DateTimeOffset</span></span>|<span data-ttu-id="c8cb1-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-143">DateTime the object was last modified.</span></span> <span data-ttu-id="c8cb1-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c8cb1-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c8cb1-145">displayName</span><span class="sxs-lookup"><span data-stu-id="c8cb1-145">displayName</span></span>|<span data-ttu-id="c8cb1-146">String</span><span class="sxs-lookup"><span data-stu-id="c8cb1-146">String</span></span>|<span data-ttu-id="c8cb1-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c8cb1-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c8cb1-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c8cb1-149">version</span><span class="sxs-lookup"><span data-stu-id="c8cb1-149">version</span></span>|<span data-ttu-id="c8cb1-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c8cb1-150">Int32</span></span>|<span data-ttu-id="c8cb1-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-151">Version of the device configuration.</span></span> <span data-ttu-id="c8cb1-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c8cb1-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c8cb1-153">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c8cb1-153">passwordBlockSimple</span></span>|<span data-ttu-id="c8cb1-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8cb1-154">Boolean</span></span>|<span data-ttu-id="c8cb1-155">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-155">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="c8cb1-156">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c8cb1-156">passwordExpirationDays</span></span>|<span data-ttu-id="c8cb1-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c8cb1-157">Int32</span></span>|<span data-ttu-id="c8cb1-158">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-158">Number of days before the password expires.</span></span>|
|<span data-ttu-id="c8cb1-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c8cb1-159">passwordMinimumLength</span></span>|<span data-ttu-id="c8cb1-160">Int32</span><span class="sxs-lookup"><span data-stu-id="c8cb1-160">Int32</span></span>|<span data-ttu-id="c8cb1-161">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-161">Minimum length of passwords.</span></span>|
|<span data-ttu-id="c8cb1-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c8cb1-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c8cb1-163">Int32</span><span class="sxs-lookup"><span data-stu-id="c8cb1-163">Int32</span></span>|<span data-ttu-id="c8cb1-164">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c8cb1-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c8cb1-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c8cb1-166">Int32</span><span class="sxs-lookup"><span data-stu-id="c8cb1-166">Int32</span></span>|<span data-ttu-id="c8cb1-167">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c8cb1-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c8cb1-168">passwordRequiredType</span></span>|[<span data-ttu-id="c8cb1-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c8cb1-169">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="c8cb1-170">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-170">The required password type.</span></span> <span data-ttu-id="c8cb1-171">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c8cb1-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c8cb1-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c8cb1-173">Int32</span><span class="sxs-lookup"><span data-stu-id="c8cb1-173">Int32</span></span>|<span data-ttu-id="c8cb1-174">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-174">Number of previous passwords to block.</span></span> <span data-ttu-id="c8cb1-175">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c8cb1-176">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c8cb1-176">passwordRequired</span></span>|<span data-ttu-id="c8cb1-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8cb1-177">Boolean</span></span>|<span data-ttu-id="c8cb1-178">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-178">Whether or not to require a password.</span></span>|
|<span data-ttu-id="c8cb1-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c8cb1-179">osMinimumVersion</span></span>|<span data-ttu-id="c8cb1-180">String</span><span class="sxs-lookup"><span data-stu-id="c8cb1-180">String</span></span>|<span data-ttu-id="c8cb1-181">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-181">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="c8cb1-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c8cb1-182">osMaximumVersion</span></span>|<span data-ttu-id="c8cb1-183">String</span><span class="sxs-lookup"><span data-stu-id="c8cb1-183">String</span></span>|<span data-ttu-id="c8cb1-184">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-184">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="c8cb1-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c8cb1-185">storageRequireEncryption</span></span>|<span data-ttu-id="c8cb1-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8cb1-186">Boolean</span></span>|<span data-ttu-id="c8cb1-187">Указывает, обязательно ли шифрование данных на устройствах с Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-187">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="c8cb1-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8cb1-188">Response</span></span>
<span data-ttu-id="c8cb1-189">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-189">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8cb1-190">Пример</span><span class="sxs-lookup"><span data-stu-id="c8cb1-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8cb1-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8cb1-191">Request</span></span>
<span data-ttu-id="c8cb1-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 607

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="c8cb1-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8cb1-193">Response</span></span>
<span data-ttu-id="c8cb1-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c8cb1-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



