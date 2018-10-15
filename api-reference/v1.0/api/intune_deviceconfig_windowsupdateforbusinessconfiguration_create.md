# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="f0cad-101">Создание объекта windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="f0cad-101">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="f0cad-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f0cad-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0cad-103">Создание объекта [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cad-103">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0cad-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f0cad-104">Prerequisites</span></span>
<span data-ttu-id="f0cad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f0cad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f0cad-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0cad-107">Permission type</span></span>|<span data-ttu-id="f0cad-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0cad-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0cad-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0cad-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f0cad-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0cad-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0cad-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0cad-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0cad-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0cad-112">Not supported.</span></span>|
|<span data-ttu-id="f0cad-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0cad-113">Application</span></span>|<span data-ttu-id="f0cad-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0cad-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0cad-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0cad-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f0cad-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0cad-116">Request headers</span></span>
|<span data-ttu-id="f0cad-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0cad-117">Header</span></span>|<span data-ttu-id="f0cad-118">Значение</span><span class="sxs-lookup"><span data-stu-id="f0cad-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0cad-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0cad-119">Authorization</span></span>|<span data-ttu-id="f0cad-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="f0cad-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0cad-121">Принять</span><span class="sxs-lookup"><span data-stu-id="f0cad-121">Accept</span></span>|<span data-ttu-id="f0cad-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f0cad-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0cad-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0cad-123">Request body</span></span>
<span data-ttu-id="f0cad-124">В тексте запроса добавьте представление объекта windowsUpdateForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0cad-124">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="f0cad-125">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f0cad-125">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="f0cad-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0cad-126">Property</span></span>|<span data-ttu-id="f0cad-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f0cad-127">Type</span></span>|<span data-ttu-id="f0cad-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f0cad-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0cad-129">id</span><span class="sxs-lookup"><span data-stu-id="f0cad-129">id</span></span>|<span data-ttu-id="f0cad-130">Строка</span><span class="sxs-lookup"><span data-stu-id="f0cad-130">String</span></span>|<span data-ttu-id="f0cad-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f0cad-131">Key of the entity.</span></span> <span data-ttu-id="f0cad-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cad-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0cad-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0cad-133">lastModifiedDateTime</span></span>|<span data-ttu-id="f0cad-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0cad-134">DateTimeOffset</span></span>|<span data-ttu-id="f0cad-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f0cad-135">DateTime the object was last modified.</span></span> <span data-ttu-id="f0cad-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cad-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0cad-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0cad-137">createdDateTime</span></span>|<span data-ttu-id="f0cad-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0cad-138">DateTimeOffset</span></span>|<span data-ttu-id="f0cad-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f0cad-139">DateTime the object was created.</span></span> <span data-ttu-id="f0cad-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cad-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0cad-141">description</span><span class="sxs-lookup"><span data-stu-id="f0cad-141">description</span></span>|<span data-ttu-id="f0cad-142">Строка</span><span class="sxs-lookup"><span data-stu-id="f0cad-142">String</span></span>|<span data-ttu-id="f0cad-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f0cad-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f0cad-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cad-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0cad-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f0cad-145">displayName</span></span>|<span data-ttu-id="f0cad-146">Строка</span><span class="sxs-lookup"><span data-stu-id="f0cad-146">String</span></span>|<span data-ttu-id="f0cad-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f0cad-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f0cad-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cad-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0cad-149">version</span><span class="sxs-lookup"><span data-stu-id="f0cad-149">version</span></span>|<span data-ttu-id="f0cad-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f0cad-150">Int32</span></span>|<span data-ttu-id="f0cad-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f0cad-151">Version of the device configuration.</span></span> <span data-ttu-id="f0cad-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cad-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0cad-153">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="f0cad-153">deliveryOptimizationMode</span></span>|[<span data-ttu-id="f0cad-154">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="f0cad-154">windowsDeliveryOptimizationMode</span></span>](../resources/intune_deviceconfig_windowsdeliveryoptimizationmode.md)|<span data-ttu-id="f0cad-155">Оптимизация режима поставки.</span><span class="sxs-lookup"><span data-stu-id="f0cad-155">Delivery Optimization Mode Possible values are: , , , , , , .</span></span> <span data-ttu-id="f0cad-156">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="f0cad-156">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="f0cad-157">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="f0cad-157">prereleaseFeatures</span></span>|[<span data-ttu-id="f0cad-158">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="f0cad-158">prereleaseFeatures</span></span>](../resources/intune_deviceconfig_prereleasefeatures.md)|<span data-ttu-id="f0cad-159">Экспериментальные функции.</span><span class="sxs-lookup"><span data-stu-id="f0cad-159">The pre-release features.</span></span> <span data-ttu-id="f0cad-160">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="f0cad-160">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="f0cad-161">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="f0cad-161">automaticUpdateMode</span></span>|[<span data-ttu-id="f0cad-162">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="f0cad-162">automaticUpdateMode</span></span>](../resources/intune_deviceconfig_automaticupdatemode.md)|<span data-ttu-id="f0cad-163">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="f0cad-163">Automatic update mode.</span></span> <span data-ttu-id="f0cad-164">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="f0cad-164">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="f0cad-165">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="f0cad-165">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="f0cad-166">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cad-166">Boolean</span></span>|<span data-ttu-id="f0cad-167">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="f0cad-167">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="f0cad-168">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="f0cad-168">driversExcluded</span></span>|<span data-ttu-id="f0cad-169">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cad-169">Boolean</span></span>|<span data-ttu-id="f0cad-170">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="f0cad-170">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="f0cad-171">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="f0cad-171">installationSchedule</span></span>|[<span data-ttu-id="f0cad-172">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="f0cad-172">windowsUpdateInstallScheduleType</span></span>](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)|<span data-ttu-id="f0cad-173">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="f0cad-173">Installation schedule</span></span>|
|<span data-ttu-id="f0cad-174">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="f0cad-174">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="f0cad-175">Int32</span><span class="sxs-lookup"><span data-stu-id="f0cad-175">Int32</span></span>|<span data-ttu-id="f0cad-176">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="f0cad-176">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="f0cad-177">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="f0cad-177">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="f0cad-178">Int32</span><span class="sxs-lookup"><span data-stu-id="f0cad-178">Int32</span></span>|<span data-ttu-id="f0cad-179">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="f0cad-179">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="f0cad-180">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="f0cad-180">qualityUpdatesPaused</span></span>|<span data-ttu-id="f0cad-181">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cad-181">Boolean</span></span>|<span data-ttu-id="f0cad-182">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="f0cad-182">Pause Quality Updates</span></span>|
|<span data-ttu-id="f0cad-183">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="f0cad-183">featureUpdatesPaused</span></span>|<span data-ttu-id="f0cad-184">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cad-184">Boolean</span></span>|<span data-ttu-id="f0cad-185">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="f0cad-185">Pause Feature Updates</span></span>|
|<span data-ttu-id="f0cad-186">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="f0cad-186">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="f0cad-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0cad-187">DateTimeOffset</span></span>|<span data-ttu-id="f0cad-188">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="f0cad-188">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="f0cad-189">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="f0cad-189">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="f0cad-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0cad-190">DateTimeOffset</span></span>|<span data-ttu-id="f0cad-191">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="f0cad-191">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="f0cad-192">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="f0cad-192">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="f0cad-193">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="f0cad-193">windowsUpdateType</span></span>](../resources/intune_deviceconfig_windowsupdatetype.md)|<span data-ttu-id="f0cad-194">Определяет, от какой ветви устройства будут получать обновления.</span><span class="sxs-lookup"><span data-stu-id="f0cad-194">Determines which branch devices will receive their updates from Possible values are: , , .</span></span> <span data-ttu-id="f0cad-195">Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="f0cad-195">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="f0cad-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0cad-196">Response</span></span>
<span data-ttu-id="f0cad-197">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f0cad-197">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0cad-198">Пример</span><span class="sxs-lookup"><span data-stu-id="f0cad-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0cad-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0cad-199">Request</span></span>
<span data-ttu-id="f0cad-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0cad-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 974

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
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

### <a name="response"></a><span data-ttu-id="f0cad-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0cad-201">Response</span></span>
<span data-ttu-id="f0cad-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0cad-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








