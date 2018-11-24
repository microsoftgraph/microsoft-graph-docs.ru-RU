# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="2cbeb-101">Create windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="2cbeb-101">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="2cbeb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2cbeb-103">Создание объекта [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cbeb-103">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2cbeb-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2cbeb-104">Prerequisites</span></span>
<span data-ttu-id="2cbeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2cbeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2cbeb-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cbeb-107">Permission type</span></span>|<span data-ttu-id="2cbeb-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cbeb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cbeb-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cbeb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2cbeb-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cbeb-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2cbeb-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cbeb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cbeb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-112">Not supported.</span></span>|
|<span data-ttu-id="2cbeb-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2cbeb-113">Application</span></span>|<span data-ttu-id="2cbeb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cbeb-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cbeb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2cbeb-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2cbeb-116">Request headers</span></span>
|<span data-ttu-id="2cbeb-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2cbeb-117">Header</span></span>|<span data-ttu-id="2cbeb-118">Значение</span><span class="sxs-lookup"><span data-stu-id="2cbeb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cbeb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cbeb-119">Authorization</span></span>|<span data-ttu-id="2cbeb-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cbeb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2cbeb-121">Accept</span></span>|<span data-ttu-id="2cbeb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2cbeb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cbeb-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2cbeb-123">Request body</span></span>
<span data-ttu-id="2cbeb-124">В тексте запроса добавьте представление объекта windowsUpdateForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-124">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="2cbeb-125">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-125">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="2cbeb-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cbeb-126">Property</span></span>|<span data-ttu-id="2cbeb-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2cbeb-127">Type</span></span>|<span data-ttu-id="2cbeb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2cbeb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cbeb-129">id</span><span class="sxs-lookup"><span data-stu-id="2cbeb-129">id</span></span>|<span data-ttu-id="2cbeb-130">String</span><span class="sxs-lookup"><span data-stu-id="2cbeb-130">String</span></span>|<span data-ttu-id="2cbeb-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-131">Key of the entity.</span></span> <span data-ttu-id="2cbeb-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2cbeb-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cbeb-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2cbeb-133">lastModifiedDateTime</span></span>|<span data-ttu-id="2cbeb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cbeb-134">DateTimeOffset</span></span>|<span data-ttu-id="2cbeb-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-135">DateTime the object was last modified.</span></span> <span data-ttu-id="2cbeb-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2cbeb-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cbeb-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2cbeb-137">createdDateTime</span></span>|<span data-ttu-id="2cbeb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cbeb-138">DateTimeOffset</span></span>|<span data-ttu-id="2cbeb-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-139">DateTime the object was created.</span></span> <span data-ttu-id="2cbeb-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2cbeb-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cbeb-141">description</span><span class="sxs-lookup"><span data-stu-id="2cbeb-141">description</span></span>|<span data-ttu-id="2cbeb-142">String</span><span class="sxs-lookup"><span data-stu-id="2cbeb-142">String</span></span>|<span data-ttu-id="2cbeb-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2cbeb-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2cbeb-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cbeb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="2cbeb-145">displayName</span></span>|<span data-ttu-id="2cbeb-146">String</span><span class="sxs-lookup"><span data-stu-id="2cbeb-146">String</span></span>|<span data-ttu-id="2cbeb-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2cbeb-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2cbeb-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cbeb-149">version</span><span class="sxs-lookup"><span data-stu-id="2cbeb-149">version</span></span>|<span data-ttu-id="2cbeb-150">Int32</span><span class="sxs-lookup"><span data-stu-id="2cbeb-150">Int32</span></span>|<span data-ttu-id="2cbeb-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-151">Version of the device configuration.</span></span> <span data-ttu-id="2cbeb-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2cbeb-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cbeb-153">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="2cbeb-153">deliveryOptimizationMode</span></span>|[<span data-ttu-id="2cbeb-154">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="2cbeb-154">windowsDeliveryOptimizationMode</span></span>](../resources/intune_deviceconfig_windowsdeliveryoptimizationmode.md)|<span data-ttu-id="2cbeb-155">Режим оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-155">Delivery Optimization Mode.</span></span> <span data-ttu-id="2cbeb-156">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-156">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="2cbeb-157">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="2cbeb-157">prereleaseFeatures</span></span>|[<span data-ttu-id="2cbeb-158">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="2cbeb-158">prereleaseFeatures</span></span>](../resources/intune_deviceconfig_prereleasefeatures.md)|<span data-ttu-id="2cbeb-159">Экспериментальные функции.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-159">The pre-release features.</span></span> <span data-ttu-id="2cbeb-160">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-160">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="2cbeb-161">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="2cbeb-161">automaticUpdateMode</span></span>|[<span data-ttu-id="2cbeb-162">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="2cbeb-162">automaticUpdateMode</span></span>](../resources/intune_deviceconfig_automaticupdatemode.md)|<span data-ttu-id="2cbeb-163">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-163">Automatic update mode.</span></span> <span data-ttu-id="2cbeb-164">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-164">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="2cbeb-165">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="2cbeb-165">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="2cbeb-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cbeb-166">Boolean</span></span>|<span data-ttu-id="2cbeb-167">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="2cbeb-167">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="2cbeb-168">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="2cbeb-168">driversExcluded</span></span>|<span data-ttu-id="2cbeb-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cbeb-169">Boolean</span></span>|<span data-ttu-id="2cbeb-170">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-170">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="2cbeb-171">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="2cbeb-171">installationSchedule</span></span>|[<span data-ttu-id="2cbeb-172">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="2cbeb-172">windowsUpdateInstallScheduleType</span></span>](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)|<span data-ttu-id="2cbeb-173">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-173">Installation schedule</span></span>|
|<span data-ttu-id="2cbeb-174">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="2cbeb-174">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="2cbeb-175">Int32</span><span class="sxs-lookup"><span data-stu-id="2cbeb-175">Int32</span></span>|<span data-ttu-id="2cbeb-176">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-176">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="2cbeb-177">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="2cbeb-177">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="2cbeb-178">Int32</span><span class="sxs-lookup"><span data-stu-id="2cbeb-178">Int32</span></span>|<span data-ttu-id="2cbeb-179">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-179">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="2cbeb-180">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="2cbeb-180">qualityUpdatesPaused</span></span>|<span data-ttu-id="2cbeb-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cbeb-181">Boolean</span></span>|<span data-ttu-id="2cbeb-182">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-182">Pause Quality Updates</span></span>|
|<span data-ttu-id="2cbeb-183">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="2cbeb-183">featureUpdatesPaused</span></span>|<span data-ttu-id="2cbeb-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cbeb-184">Boolean</span></span>|<span data-ttu-id="2cbeb-185">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-185">Pause Feature Updates</span></span>|
|<span data-ttu-id="2cbeb-186">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="2cbeb-186">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="2cbeb-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cbeb-187">DateTimeOffset</span></span>|<span data-ttu-id="2cbeb-188">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-188">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="2cbeb-189">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="2cbeb-189">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="2cbeb-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cbeb-190">DateTimeOffset</span></span>|<span data-ttu-id="2cbeb-191">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-191">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="2cbeb-192">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="2cbeb-192">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="2cbeb-193">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="2cbeb-193">windowsUpdateType</span></span>](../resources/intune_deviceconfig_windowsupdatetype.md)|<span data-ttu-id="2cbeb-194">Определяет, какие устройства филиала будет получать обновления из.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-194">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="2cbeb-195">Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-195">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="2cbeb-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="2cbeb-196">Response</span></span>
<span data-ttu-id="2cbeb-197">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-197">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cbeb-198">Пример</span><span class="sxs-lookup"><span data-stu-id="2cbeb-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="2cbeb-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cbeb-199">Request</span></span>
<span data-ttu-id="2cbeb-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2cbeb-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 910

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
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

### <a name="response"></a><span data-ttu-id="2cbeb-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="2cbeb-201">Response</span></span>
<span data-ttu-id="2cbeb-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="2cbeb-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



