# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="e2a66-101">Create sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2a66-101">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="e2a66-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e2a66-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2a66-103">Создание объекта [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2a66-103">Create a new [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e2a66-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e2a66-104">Prerequisites</span></span>
<span data-ttu-id="e2a66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e2a66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e2a66-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2a66-107">Permission type</span></span>|<span data-ttu-id="e2a66-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2a66-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2a66-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2a66-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e2a66-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2a66-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2a66-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2a66-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2a66-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2a66-112">Not supported.</span></span>|
|<span data-ttu-id="e2a66-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2a66-113">Application</span></span>|<span data-ttu-id="e2a66-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2a66-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2a66-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2a66-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e2a66-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e2a66-116">Request headers</span></span>
|<span data-ttu-id="e2a66-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2a66-117">Header</span></span>|<span data-ttu-id="e2a66-118">Значение</span><span class="sxs-lookup"><span data-stu-id="e2a66-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2a66-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2a66-119">Authorization</span></span>|<span data-ttu-id="e2a66-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2a66-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2a66-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e2a66-121">Accept</span></span>|<span data-ttu-id="e2a66-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e2a66-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2a66-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2a66-123">Request body</span></span>
<span data-ttu-id="e2a66-124">В тексте запроса добавьте представление объекта sharedPCConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2a66-124">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="e2a66-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e2a66-125">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="e2a66-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2a66-126">Property</span></span>|<span data-ttu-id="e2a66-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e2a66-127">Type</span></span>|<span data-ttu-id="e2a66-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e2a66-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2a66-129">id</span><span class="sxs-lookup"><span data-stu-id="e2a66-129">id</span></span>|<span data-ttu-id="e2a66-130">String</span><span class="sxs-lookup"><span data-stu-id="e2a66-130">String</span></span>|<span data-ttu-id="e2a66-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e2a66-131">Key of the entity.</span></span> <span data-ttu-id="e2a66-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2a66-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2a66-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2a66-133">lastModifiedDateTime</span></span>|<span data-ttu-id="e2a66-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2a66-134">DateTimeOffset</span></span>|<span data-ttu-id="e2a66-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e2a66-135">DateTime the object was last modified.</span></span> <span data-ttu-id="e2a66-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2a66-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2a66-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2a66-137">createdDateTime</span></span>|<span data-ttu-id="e2a66-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2a66-138">DateTimeOffset</span></span>|<span data-ttu-id="e2a66-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e2a66-139">DateTime the object was created.</span></span> <span data-ttu-id="e2a66-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2a66-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2a66-141">description</span><span class="sxs-lookup"><span data-stu-id="e2a66-141">description</span></span>|<span data-ttu-id="e2a66-142">String</span><span class="sxs-lookup"><span data-stu-id="e2a66-142">String</span></span>|<span data-ttu-id="e2a66-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2a66-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e2a66-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2a66-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2a66-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e2a66-145">displayName</span></span>|<span data-ttu-id="e2a66-146">String</span><span class="sxs-lookup"><span data-stu-id="e2a66-146">String</span></span>|<span data-ttu-id="e2a66-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2a66-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e2a66-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2a66-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2a66-149">version</span><span class="sxs-lookup"><span data-stu-id="e2a66-149">version</span></span>|<span data-ttu-id="e2a66-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e2a66-150">Int32</span></span>|<span data-ttu-id="e2a66-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2a66-151">Version of the device configuration.</span></span> <span data-ttu-id="e2a66-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2a66-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2a66-153">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="e2a66-153">accountManagerPolicy</span></span>|[<span data-ttu-id="e2a66-154">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="e2a66-154">sharedPCAccountManagerPolicy</span></span>](../resources/intune_deviceconfig_sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="e2a66-155">Задает способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="e2a66-155">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="e2a66-156">Применяется, только если для параметра disableAccountManager задано значение false.</span><span class="sxs-lookup"><span data-stu-id="e2a66-156">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="e2a66-157">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="e2a66-157">allowedAccounts</span></span>|[<span data-ttu-id="e2a66-158">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="e2a66-158">sharedPCAllowedAccountType</span></span>](../resources/intune_deviceconfig_sharedpcallowedaccounttype.md)|<span data-ttu-id="e2a66-159">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="e2a66-159">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="e2a66-160">Возможные значения: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="e2a66-160">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="e2a66-161">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="e2a66-161">allowLocalStorage</span></span>|<span data-ttu-id="e2a66-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a66-162">Boolean</span></span>|<span data-ttu-id="e2a66-163">Указывает, можно ли разместить локальное хранилище на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="e2a66-163">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="e2a66-164">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="e2a66-164">disableAccountManager</span></span>|<span data-ttu-id="e2a66-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a66-165">Boolean</span></span>|<span data-ttu-id="e2a66-166">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="e2a66-166">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="e2a66-167">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="e2a66-167">disableEduPolicies</span></span>|<span data-ttu-id="e2a66-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a66-168">Boolean</span></span>|<span data-ttu-id="e2a66-169">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="e2a66-169">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="e2a66-170">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="e2a66-170">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="e2a66-171">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="e2a66-171">disablePowerPolicies</span></span>|<span data-ttu-id="e2a66-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a66-172">Boolean</span></span>|<span data-ttu-id="e2a66-173">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="e2a66-173">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="e2a66-174">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="e2a66-174">disableSignInOnResume</span></span>|<span data-ttu-id="e2a66-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a66-175">Boolean</span></span>|<span data-ttu-id="e2a66-176">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="e2a66-176">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="e2a66-177">enabled</span><span class="sxs-lookup"><span data-stu-id="e2a66-177">enabled</span></span>|<span data-ttu-id="e2a66-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a66-178">Boolean</span></span>|<span data-ttu-id="e2a66-179">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="e2a66-179">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="e2a66-180">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="e2a66-180">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="e2a66-181">Int32</span><span class="sxs-lookup"><span data-stu-id="e2a66-181">Int32</span></span>|<span data-ttu-id="e2a66-182">Определяет длительность (в секундах) простоя устройства перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="e2a66-182">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="e2a66-183">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="e2a66-183">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="e2a66-184">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="e2a66-184">kioskAppDisplayName</span></span>|<span data-ttu-id="e2a66-185">String</span><span class="sxs-lookup"><span data-stu-id="e2a66-185">String</span></span>|<span data-ttu-id="e2a66-186">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, указанного в свойстве SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="e2a66-186">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="e2a66-187">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="e2a66-187">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="e2a66-188">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="e2a66-188">kioskAppUserModelId</span></span>|<span data-ttu-id="e2a66-189">String</span><span class="sxs-lookup"><span data-stu-id="e2a66-189">String</span></span>|<span data-ttu-id="e2a66-190">Задает ИД пользовательской модели для приложения, используемый с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="e2a66-190">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="e2a66-191">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="e2a66-191">maintenanceStartTime</span></span>|<span data-ttu-id="e2a66-192">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e2a66-192">TimeOfDay</span></span>|<span data-ttu-id="e2a66-193">Задает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="e2a66-193">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="e2a66-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2a66-194">Response</span></span>
<span data-ttu-id="e2a66-195">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e2a66-195">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2a66-196">Пример</span><span class="sxs-lookup"><span data-stu-id="e2a66-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="e2a66-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2a66-197">Request</span></span>
<span data-ttu-id="e2a66-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2a66-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 860

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
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

### <a name="response"></a><span data-ttu-id="e2a66-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2a66-199">Response</span></span>
<span data-ttu-id="e2a66-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e2a66-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



