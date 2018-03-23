# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="69e9d-101">Обновление объекта windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="69e9d-101">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="69e9d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="69e9d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69e9d-103">Обновление свойств объекта [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69e9d-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69e9d-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="69e9d-104">Prerequisites</span></span>
<span data-ttu-id="69e9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="69e9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="69e9d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69e9d-107">Permission type</span></span>|<span data-ttu-id="69e9d-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69e9d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69e9d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69e9d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="69e9d-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69e9d-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69e9d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69e9d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69e9d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69e9d-112">Not supported.</span></span>|
|<span data-ttu-id="69e9d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69e9d-113">Application</span></span>|<span data-ttu-id="69e9d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69e9d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69e9d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69e9d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="69e9d-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69e9d-116">Request headers</span></span>
|<span data-ttu-id="69e9d-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69e9d-117">Header</span></span>|<span data-ttu-id="69e9d-118">Значение</span><span class="sxs-lookup"><span data-stu-id="69e9d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69e9d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="69e9d-119">Authorization</span></span>|<span data-ttu-id="69e9d-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69e9d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="69e9d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="69e9d-121">Accept</span></span>|<span data-ttu-id="69e9d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="69e9d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69e9d-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69e9d-123">Request body</span></span>
<span data-ttu-id="69e9d-124">В теле запроса добавьте представление объекта [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69e9d-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="69e9d-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69e9d-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="69e9d-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="69e9d-126">Property</span></span>|<span data-ttu-id="69e9d-127">Тип</span><span class="sxs-lookup"><span data-stu-id="69e9d-127">Type</span></span>|<span data-ttu-id="69e9d-128">Описание</span><span class="sxs-lookup"><span data-stu-id="69e9d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69e9d-129">id</span><span class="sxs-lookup"><span data-stu-id="69e9d-129">id</span></span>|<span data-ttu-id="69e9d-130">String</span><span class="sxs-lookup"><span data-stu-id="69e9d-130">String</span></span>|<span data-ttu-id="69e9d-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="69e9d-131">Key of the setting.</span></span> <span data-ttu-id="69e9d-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69e9d-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69e9d-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69e9d-133">lastModifiedDateTime</span></span>|<span data-ttu-id="69e9d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69e9d-134">DateTimeOffset</span></span>|<span data-ttu-id="69e9d-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="69e9d-135">DateTime the object was last modified.</span></span> <span data-ttu-id="69e9d-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69e9d-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69e9d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69e9d-137">createdDateTime</span></span>|<span data-ttu-id="69e9d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69e9d-138">DateTimeOffset</span></span>|<span data-ttu-id="69e9d-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="69e9d-139">DateTime the object was created.</span></span> <span data-ttu-id="69e9d-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69e9d-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69e9d-141">description</span><span class="sxs-lookup"><span data-stu-id="69e9d-141">description</span></span>|<span data-ttu-id="69e9d-142">String</span><span class="sxs-lookup"><span data-stu-id="69e9d-142">String</span></span>|<span data-ttu-id="69e9d-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="69e9d-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="69e9d-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69e9d-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69e9d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="69e9d-145">displayName</span></span>|<span data-ttu-id="69e9d-146">String</span><span class="sxs-lookup"><span data-stu-id="69e9d-146">String</span></span>|<span data-ttu-id="69e9d-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="69e9d-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="69e9d-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69e9d-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69e9d-149">version</span><span class="sxs-lookup"><span data-stu-id="69e9d-149">version</span></span>|<span data-ttu-id="69e9d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="69e9d-150">Int32</span></span>|<span data-ttu-id="69e9d-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="69e9d-151">Version of the device configuration.</span></span> <span data-ttu-id="69e9d-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69e9d-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69e9d-153">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="69e9d-153">deliveryOptimizationMode</span></span>|<span data-ttu-id="69e9d-154">String</span><span class="sxs-lookup"><span data-stu-id="69e9d-154">String</span></span>|<span data-ttu-id="69e9d-155">Режим оптимизации доставки. Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="69e9d-155">Delivery Optimization Mode Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="69e9d-156">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="69e9d-156">prereleaseFeatures</span></span>|<span data-ttu-id="69e9d-157">String</span><span class="sxs-lookup"><span data-stu-id="69e9d-157">String</span></span>|<span data-ttu-id="69e9d-158">Функции предварительного выпуска.</span><span class="sxs-lookup"><span data-stu-id="69e9d-158">The pre-release features.</span></span> <span data-ttu-id="69e9d-159">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="69e9d-159">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="69e9d-160">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="69e9d-160">automaticUpdateMode</span></span>|<span data-ttu-id="69e9d-161">String</span><span class="sxs-lookup"><span data-stu-id="69e9d-161">String</span></span>|<span data-ttu-id="69e9d-162">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="69e9d-162">Automatic update mode.</span></span> <span data-ttu-id="69e9d-163">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="69e9d-163">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="69e9d-164">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="69e9d-164">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="69e9d-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="69e9d-165">Boolean</span></span>|<span data-ttu-id="69e9d-166">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="69e9d-166">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="69e9d-167">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="69e9d-167">driversExcluded</span></span>|<span data-ttu-id="69e9d-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="69e9d-168">Boolean</span></span>|<span data-ttu-id="69e9d-169">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="69e9d-169">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="69e9d-170">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="69e9d-170">installationSchedule</span></span>|[<span data-ttu-id="69e9d-171">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="69e9d-171">windowsUpdateInstallScheduleType</span></span>](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)|<span data-ttu-id="69e9d-172">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="69e9d-172">Installation schedule</span></span>|
|<span data-ttu-id="69e9d-173">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="69e9d-173">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="69e9d-174">Int32</span><span class="sxs-lookup"><span data-stu-id="69e9d-174">Int32</span></span>|<span data-ttu-id="69e9d-175">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="69e9d-175">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="69e9d-176">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="69e9d-176">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="69e9d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="69e9d-177">Int32</span></span>|<span data-ttu-id="69e9d-178">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="69e9d-178">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="69e9d-179">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="69e9d-179">qualityUpdatesPaused</span></span>|<span data-ttu-id="69e9d-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="69e9d-180">Boolean</span></span>|<span data-ttu-id="69e9d-181">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="69e9d-181">Pause Quality Updates</span></span>|
|<span data-ttu-id="69e9d-182">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="69e9d-182">featureUpdatesPaused</span></span>|<span data-ttu-id="69e9d-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="69e9d-183">Boolean</span></span>|<span data-ttu-id="69e9d-184">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="69e9d-184">Pause Feature Updates</span></span>|
|<span data-ttu-id="69e9d-185">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="69e9d-185">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="69e9d-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69e9d-186">DateTimeOffset</span></span>|<span data-ttu-id="69e9d-187">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="69e9d-187">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="69e9d-188">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="69e9d-188">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="69e9d-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69e9d-189">DateTimeOffset</span></span>|<span data-ttu-id="69e9d-190">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="69e9d-190">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="69e9d-191">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="69e9d-191">businessReadyUpdatesOnly</span></span>|<span data-ttu-id="69e9d-192">String</span><span class="sxs-lookup"><span data-stu-id="69e9d-192">String</span></span>|<span data-ttu-id="69e9d-193">Определяет ветвь обновления для устройств. Возможные значения: `userDefined`, `all`, `businessReadyOnly`.</span><span class="sxs-lookup"><span data-stu-id="69e9d-193">Determines which branch devices will receive their updates from Possible values are: `userDefined`, `all`, `businessReadyOnly`.</span></span>|



## <a name="response"></a><span data-ttu-id="69e9d-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="69e9d-194">Response</span></span>
<span data-ttu-id="69e9d-195">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="69e9d-195">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69e9d-196">Пример</span><span class="sxs-lookup"><span data-stu-id="69e9d-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="69e9d-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="69e9d-197">Request</span></span>
<span data-ttu-id="69e9d-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69e9d-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 898

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all"
}
```

### <a name="response"></a><span data-ttu-id="69e9d-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="69e9d-199">Response</span></span>
<span data-ttu-id="69e9d-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="69e9d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1082

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all"
}
```



