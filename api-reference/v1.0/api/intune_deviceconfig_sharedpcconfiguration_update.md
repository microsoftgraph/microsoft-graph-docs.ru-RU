# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="a493d-101">Обновление объекта sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="a493d-101">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="a493d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a493d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a493d-103">Обновляет свойства объекта [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a493d-103">Update the properties of a [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a493d-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a493d-104">Prerequisites</span></span>
<span data-ttu-id="a493d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a493d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a493d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a493d-107">Permission type</span></span>|<span data-ttu-id="a493d-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a493d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a493d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a493d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a493d-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a493d-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a493d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a493d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a493d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a493d-112">Not supported.</span></span>|
|<span data-ttu-id="a493d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a493d-113">Application</span></span>|<span data-ttu-id="a493d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a493d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a493d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a493d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a493d-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a493d-116">Request headers</span></span>
|<span data-ttu-id="a493d-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a493d-117">Header</span></span>|<span data-ttu-id="a493d-118">Значение</span><span class="sxs-lookup"><span data-stu-id="a493d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a493d-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a493d-119">Authorization</span></span>|<span data-ttu-id="a493d-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="a493d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a493d-121">Принять</span><span class="sxs-lookup"><span data-stu-id="a493d-121">Accept</span></span>|<span data-ttu-id="a493d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a493d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a493d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a493d-123">Request body</span></span>
<span data-ttu-id="a493d-124">В теле запроса добавьте представление объекта [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a493d-124">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="a493d-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a493d-125">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="a493d-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a493d-126">Property</span></span>|<span data-ttu-id="a493d-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a493d-127">Type</span></span>|<span data-ttu-id="a493d-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a493d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a493d-129">id</span><span class="sxs-lookup"><span data-stu-id="a493d-129">id</span></span>|<span data-ttu-id="a493d-130">Строка</span><span class="sxs-lookup"><span data-stu-id="a493d-130">String</span></span>|<span data-ttu-id="a493d-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a493d-131">Key of the entity.</span></span> <span data-ttu-id="a493d-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a493d-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a493d-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a493d-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a493d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a493d-134">DateTimeOffset</span></span>|<span data-ttu-id="a493d-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a493d-135">DateTime the object was last modified.</span></span> <span data-ttu-id="a493d-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a493d-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a493d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a493d-137">createdDateTime</span></span>|<span data-ttu-id="a493d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a493d-138">DateTimeOffset</span></span>|<span data-ttu-id="a493d-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a493d-139">DateTime the object was created.</span></span> <span data-ttu-id="a493d-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a493d-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a493d-141">description</span><span class="sxs-lookup"><span data-stu-id="a493d-141">description</span></span>|<span data-ttu-id="a493d-142">Строка</span><span class="sxs-lookup"><span data-stu-id="a493d-142">String</span></span>|<span data-ttu-id="a493d-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a493d-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a493d-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a493d-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a493d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a493d-145">displayName</span></span>|<span data-ttu-id="a493d-146">Строка</span><span class="sxs-lookup"><span data-stu-id="a493d-146">String</span></span>|<span data-ttu-id="a493d-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a493d-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a493d-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a493d-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a493d-149">version</span><span class="sxs-lookup"><span data-stu-id="a493d-149">version</span></span>|<span data-ttu-id="a493d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a493d-150">Int32</span></span>|<span data-ttu-id="a493d-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a493d-151">Version of the device configuration.</span></span> <span data-ttu-id="a493d-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a493d-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a493d-153">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="a493d-153">accountManagerPolicy</span></span>|[<span data-ttu-id="a493d-154">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="a493d-154">sharedPCAccountManagerPolicy</span></span>](../resources/intune_deviceconfig_sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="a493d-155">Задает способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="a493d-155">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="a493d-156">Применяется, только если для параметра disableAccountManager задано значение false.</span><span class="sxs-lookup"><span data-stu-id="a493d-156">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="a493d-157">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="a493d-157">allowedAccounts</span></span>|[<span data-ttu-id="a493d-158">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="a493d-158">sharedPCAllowedAccountType flags</span></span>](../resources/intune_deviceconfig_sharedpcallowedaccounttype.md)|<span data-ttu-id="a493d-159">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="a493d-159">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="a493d-160">Возможные значения: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="a493d-160">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="a493d-161">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="a493d-161">allowLocalStorage</span></span>|<span data-ttu-id="a493d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a493d-162">Boolean</span></span>|<span data-ttu-id="a493d-163">Указывает, можно ли разместить локальное хранилище на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="a493d-163">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="a493d-164">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="a493d-164">disableAccountManager</span></span>|<span data-ttu-id="a493d-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="a493d-165">Boolean</span></span>|<span data-ttu-id="a493d-166">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="a493d-166">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="a493d-167">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="a493d-167">disableEduPolicies</span></span>|<span data-ttu-id="a493d-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="a493d-168">Boolean</span></span>|<span data-ttu-id="a493d-169">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="a493d-169">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="a493d-170">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="a493d-170">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="a493d-171">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="a493d-171">disablePowerPolicies</span></span>|<span data-ttu-id="a493d-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="a493d-172">Boolean</span></span>|<span data-ttu-id="a493d-173">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="a493d-173">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="a493d-174">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="a493d-174">disableSignInOnResume</span></span>|<span data-ttu-id="a493d-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="a493d-175">Boolean</span></span>|<span data-ttu-id="a493d-176">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="a493d-176">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="a493d-177">enabled</span><span class="sxs-lookup"><span data-stu-id="a493d-177">enabled</span></span>|<span data-ttu-id="a493d-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="a493d-178">Boolean</span></span>|<span data-ttu-id="a493d-179">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="a493d-179">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="a493d-180">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="a493d-180">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="a493d-181">Int32</span><span class="sxs-lookup"><span data-stu-id="a493d-181">Int32</span></span>|<span data-ttu-id="a493d-182">Определяет длительность (в секундах) простоя устройства перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="a493d-182">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="a493d-183">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="a493d-183">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="a493d-184">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="a493d-184">kioskAppDisplayName</span></span>|<span data-ttu-id="a493d-185">String</span><span class="sxs-lookup"><span data-stu-id="a493d-185">String</span></span>|<span data-ttu-id="a493d-186">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, указанного в свойстве SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="a493d-186">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="a493d-187">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="a493d-187">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="a493d-188">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="a493d-188">kioskAppUserModelId</span></span>|<span data-ttu-id="a493d-189">String</span><span class="sxs-lookup"><span data-stu-id="a493d-189">String</span></span>|<span data-ttu-id="a493d-190">Задает ИД пользовательской модели для приложения, используемый с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="a493d-190">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="a493d-191">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="a493d-191">maintenanceStartTime</span></span>|<span data-ttu-id="a493d-192">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a493d-192">TimeOfDay</span></span>|<span data-ttu-id="a493d-193">Задает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="a493d-193">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="a493d-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="a493d-194">Response</span></span>
<span data-ttu-id="a493d-195">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a493d-195">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a493d-196">Пример</span><span class="sxs-lookup"><span data-stu-id="a493d-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="a493d-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="a493d-197">Request</span></span>
<span data-ttu-id="a493d-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a493d-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 864

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="a493d-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="a493d-199">Response</span></span>
<span data-ttu-id="a493d-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a493d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1032

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```








