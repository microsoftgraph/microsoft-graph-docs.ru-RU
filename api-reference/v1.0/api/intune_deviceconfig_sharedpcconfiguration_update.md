# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="0ceb5-101">Обновление объекта sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ceb5-101">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="0ceb5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ceb5-103">Обновляет свойства объекта [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ceb5-103">Update the properties of a [calendar](../resources/intune_deviceconfig_sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ceb5-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0ceb5-104">Prerequisites</span></span>
<span data-ttu-id="0ceb5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0ceb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0ceb5-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ceb5-107">Permission type</span></span>|<span data-ttu-id="0ceb5-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ceb5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ceb5-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ceb5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0ceb5-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ceb5-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ceb5-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ceb5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ceb5-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-112">Not supported.</span></span>|
|<span data-ttu-id="0ceb5-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ceb5-113">Application</span></span>|<span data-ttu-id="0ceb5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ceb5-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ceb5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0ceb5-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ceb5-116">Request headers</span></span>
|<span data-ttu-id="0ceb5-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ceb5-117">Header</span></span>|<span data-ttu-id="0ceb5-118">Значение</span><span class="sxs-lookup"><span data-stu-id="0ceb5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ceb5-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ceb5-119">Authorization</span></span>|<span data-ttu-id="0ceb5-120">&lt;Токен&gt; носителя. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0ceb5-121">Принять</span><span class="sxs-lookup"><span data-stu-id="0ceb5-121">Accept</span></span>|<span data-ttu-id="0ceb5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0ceb5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ceb5-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ceb5-123">Request body</span></span>
<span data-ttu-id="0ceb5-124">В теле запроса добавьте представление объекта [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="0ceb5-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ceb5-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="0ceb5-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ceb5-126">Property</span></span>|<span data-ttu-id="0ceb5-127">Тип</span><span class="sxs-lookup"><span data-stu-id="0ceb5-127">Type</span></span>|<span data-ttu-id="0ceb5-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0ceb5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ceb5-129">id</span><span class="sxs-lookup"><span data-stu-id="0ceb5-129">id</span></span>|<span data-ttu-id="0ceb5-130">String</span><span class="sxs-lookup"><span data-stu-id="0ceb5-130">String</span></span>|<span data-ttu-id="0ceb5-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-131">Key of the setting.</span></span> <span data-ttu-id="0ceb5-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ceb5-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ceb5-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ceb5-133">lastModifiedDateTime</span></span>|<span data-ttu-id="0ceb5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ceb5-134">DateTimeOffset</span></span>|<span data-ttu-id="0ceb5-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-135">DateTime the object was last modified.</span></span> <span data-ttu-id="0ceb5-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ceb5-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ceb5-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ceb5-137">createdDateTime</span></span>|<span data-ttu-id="0ceb5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ceb5-138">DateTimeOffset</span></span>|<span data-ttu-id="0ceb5-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-139">DateTime the object was created.</span></span> <span data-ttu-id="0ceb5-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ceb5-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ceb5-141">description</span><span class="sxs-lookup"><span data-stu-id="0ceb5-141">description</span></span>|<span data-ttu-id="0ceb5-142">String</span><span class="sxs-lookup"><span data-stu-id="0ceb5-142">String</span></span>|<span data-ttu-id="0ceb5-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0ceb5-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ceb5-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ceb5-145">displayName</span><span class="sxs-lookup"><span data-stu-id="0ceb5-145">displayName</span></span>|<span data-ttu-id="0ceb5-146">String</span><span class="sxs-lookup"><span data-stu-id="0ceb5-146">String</span></span>|<span data-ttu-id="0ceb5-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0ceb5-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ceb5-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ceb5-149">version</span><span class="sxs-lookup"><span data-stu-id="0ceb5-149">version</span></span>|<span data-ttu-id="0ceb5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0ceb5-150">Int32</span></span>|<span data-ttu-id="0ceb5-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-151">Version of the device configuration.</span></span> <span data-ttu-id="0ceb5-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ceb5-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ceb5-153">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="0ceb5-153">accountManagerPolicy</span></span>|[<span data-ttu-id="0ceb5-154">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="0ceb5-154">sharedPCAccountManagerPolicy</span></span>](../resources/intune_deviceconfig_sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="0ceb5-155">Определяет способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-155">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="0ceb5-156">Применяется, только если для параметра disableAccountManager установлено значение false.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-156">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="0ceb5-157">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="0ceb5-157">allowedAccounts</span></span>|<span data-ttu-id="0ceb5-158">String</span><span class="sxs-lookup"><span data-stu-id="0ceb5-158">String</span></span>|<span data-ttu-id="0ceb5-159">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-159">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="0ceb5-160">Возможные значения: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-160">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="0ceb5-161">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="0ceb5-161">allowLocalStorage</span></span>|<span data-ttu-id="0ceb5-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ceb5-162">Boolean</span></span>|<span data-ttu-id="0ceb5-163">Определяет, разрешено ли на общем компьютере локальное хранилище.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-163">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="0ceb5-164">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="0ceb5-164">disableAccountManager</span></span>|<span data-ttu-id="0ceb5-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ceb5-165">Boolean</span></span>|<span data-ttu-id="0ceb5-166">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-166">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="0ceb5-167">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="0ceb5-167">disableEduPolicies</span></span>|<span data-ttu-id="0ceb5-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ceb5-168">Boolean</span></span>|<span data-ttu-id="0ceb5-169">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-169">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="0ceb5-170">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-170">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="0ceb5-171">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="0ceb5-171">disablePowerPolicies</span></span>|<span data-ttu-id="0ceb5-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ceb5-172">Boolean</span></span>|<span data-ttu-id="0ceb5-173">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-173">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="0ceb5-174">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="0ceb5-174">disableSignInOnResume</span></span>|<span data-ttu-id="0ceb5-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ceb5-175">Boolean</span></span>|<span data-ttu-id="0ceb5-176">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-176">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="0ceb5-177">enabled</span><span class="sxs-lookup"><span data-stu-id="0ceb5-177">enabled</span></span>|<span data-ttu-id="0ceb5-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ceb5-178">Boolean</span></span>|<span data-ttu-id="0ceb5-179">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-179">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="0ceb5-180">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="0ceb5-180">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="0ceb5-181">Int32</span><span class="sxs-lookup"><span data-stu-id="0ceb5-181">Int32</span></span>|<span data-ttu-id="0ceb5-182">Определяет длительность (в секундах) пребывания устройства в режиме бездействия перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-182">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="0ceb5-183">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-183">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="0ceb5-184">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="0ceb5-184">kioskAppDisplayName</span></span>|<span data-ttu-id="0ceb5-185">String</span><span class="sxs-lookup"><span data-stu-id="0ceb5-185">String</span></span>|<span data-ttu-id="0ceb5-186">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, определяемого с помощью свойства SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-186">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="0ceb5-187">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-187">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="0ceb5-188">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="0ceb5-188">kioskAppUserModelId</span></span>|<span data-ttu-id="0ceb5-189">String</span><span class="sxs-lookup"><span data-stu-id="0ceb5-189">String</span></span>|<span data-ttu-id="0ceb5-190">Определяет идентификатор пользовательской модели для приложения, используемого с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-190">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="0ceb5-191">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="0ceb5-191">maintenanceStartTime</span></span>|<span data-ttu-id="0ceb5-192">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0ceb5-192">TimeOfDay</span></span>|<span data-ttu-id="0ceb5-193">Указывает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-193">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="0ceb5-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ceb5-194">Response</span></span>
<span data-ttu-id="0ceb5-195">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-195">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ceb5-196">Пример</span><span class="sxs-lookup"><span data-stu-id="0ceb5-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ceb5-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ceb5-197">Request</span></span>
<span data-ttu-id="0ceb5-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ceb5-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ceb5-199">Response</span></span>
<span data-ttu-id="0ceb5-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0ceb5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



