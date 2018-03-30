# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="a9f9b-101">Create windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9f9b-101">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="a9f9b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9f9b-103">Создание объекта [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9f9b-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9f9b-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a9f9b-104">Prerequisites</span></span>
<span data-ttu-id="a9f9b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a9f9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a9f9b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9f9b-107">Permission type</span></span>|<span data-ttu-id="a9f9b-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9f9b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9f9b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9f9b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a9f9b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9f9b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9f9b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9f9b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9f9b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-112">Not supported.</span></span>|
|<span data-ttu-id="a9f9b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9f9b-113">Application</span></span>|<span data-ttu-id="a9f9b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9f9b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9f9b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a9f9b-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a9f9b-116">Request headers</span></span>
|<span data-ttu-id="a9f9b-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9f9b-117">Header</span></span>|<span data-ttu-id="a9f9b-118">Значение</span><span class="sxs-lookup"><span data-stu-id="a9f9b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9f9b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9f9b-119">Authorization</span></span>|<span data-ttu-id="a9f9b-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a9f9b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a9f9b-121">Accept</span></span>|<span data-ttu-id="a9f9b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a9f9b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9f9b-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9f9b-123">Request body</span></span>
<span data-ttu-id="a9f9b-124">В тексте запроса добавьте представление объекта windowsUpdateForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="a9f9b-125">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="a9f9b-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9f9b-126">Property</span></span>|<span data-ttu-id="a9f9b-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a9f9b-127">Type</span></span>|<span data-ttu-id="a9f9b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a9f9b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9f9b-129">id</span><span class="sxs-lookup"><span data-stu-id="a9f9b-129">id</span></span>|<span data-ttu-id="a9f9b-130">String</span><span class="sxs-lookup"><span data-stu-id="a9f9b-130">String</span></span>|<span data-ttu-id="a9f9b-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-131">Key of the setting.</span></span> <span data-ttu-id="a9f9b-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9f9b-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9f9b-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9f9b-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a9f9b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f9b-134">DateTimeOffset</span></span>|<span data-ttu-id="a9f9b-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-135">DateTime the object was last modified.</span></span> <span data-ttu-id="a9f9b-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9f9b-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9f9b-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9f9b-137">createdDateTime</span></span>|<span data-ttu-id="a9f9b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f9b-138">DateTimeOffset</span></span>|<span data-ttu-id="a9f9b-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-139">DateTime the object was created.</span></span> <span data-ttu-id="a9f9b-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9f9b-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9f9b-141">description</span><span class="sxs-lookup"><span data-stu-id="a9f9b-141">description</span></span>|<span data-ttu-id="a9f9b-142">String</span><span class="sxs-lookup"><span data-stu-id="a9f9b-142">String</span></span>|<span data-ttu-id="a9f9b-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a9f9b-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9f9b-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9f9b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a9f9b-145">displayName</span></span>|<span data-ttu-id="a9f9b-146">String</span><span class="sxs-lookup"><span data-stu-id="a9f9b-146">String</span></span>|<span data-ttu-id="a9f9b-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a9f9b-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9f9b-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9f9b-149">version</span><span class="sxs-lookup"><span data-stu-id="a9f9b-149">version</span></span>|<span data-ttu-id="a9f9b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f9b-150">Int32</span></span>|<span data-ttu-id="a9f9b-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-151">Version of the device configuration.</span></span> <span data-ttu-id="a9f9b-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9f9b-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9f9b-153">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="a9f9b-153">deliveryOptimizationMode</span></span>|<span data-ttu-id="a9f9b-154">String</span><span class="sxs-lookup"><span data-stu-id="a9f9b-154">String</span></span>|<span data-ttu-id="a9f9b-155">Режим оптимизации доставки. Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-155">Delivery Optimization Mode Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="a9f9b-156">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="a9f9b-156">prereleaseFeatures</span></span>|<span data-ttu-id="a9f9b-157">String</span><span class="sxs-lookup"><span data-stu-id="a9f9b-157">String</span></span>|<span data-ttu-id="a9f9b-158">Экспериментальные функции.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-158">The pre-release features.</span></span> <span data-ttu-id="a9f9b-159">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-159">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="a9f9b-160">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="a9f9b-160">automaticUpdateMode</span></span>|<span data-ttu-id="a9f9b-161">String</span><span class="sxs-lookup"><span data-stu-id="a9f9b-161">String</span></span>|<span data-ttu-id="a9f9b-162">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-162">Automatic update mode.</span></span> <span data-ttu-id="a9f9b-163">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-163">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="a9f9b-164">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="a9f9b-164">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="a9f9b-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9f9b-165">Boolean</span></span>|<span data-ttu-id="a9f9b-166">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="a9f9b-166">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="a9f9b-167">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="a9f9b-167">driversExcluded</span></span>|<span data-ttu-id="a9f9b-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9f9b-168">Boolean</span></span>|<span data-ttu-id="a9f9b-169">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-169">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="a9f9b-170">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="a9f9b-170">installationSchedule</span></span>|[<span data-ttu-id="a9f9b-171">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="a9f9b-171">windowsUpdateInstallScheduleType</span></span>](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)|<span data-ttu-id="a9f9b-172">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-172">Installation schedule</span></span>|
|<span data-ttu-id="a9f9b-173">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="a9f9b-173">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="a9f9b-174">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f9b-174">Int32</span></span>|<span data-ttu-id="a9f9b-175">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-175">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="a9f9b-176">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="a9f9b-176">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="a9f9b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f9b-177">Int32</span></span>|<span data-ttu-id="a9f9b-178">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-178">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="a9f9b-179">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="a9f9b-179">qualityUpdatesPaused</span></span>|<span data-ttu-id="a9f9b-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9f9b-180">Boolean</span></span>|<span data-ttu-id="a9f9b-181">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-181">Pause Quality Updates</span></span>|
|<span data-ttu-id="a9f9b-182">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="a9f9b-182">featureUpdatesPaused</span></span>|<span data-ttu-id="a9f9b-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9f9b-183">Boolean</span></span>|<span data-ttu-id="a9f9b-184">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-184">Pause Feature Updates</span></span>|
|<span data-ttu-id="a9f9b-185">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="a9f9b-185">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="a9f9b-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f9b-186">DateTimeOffset</span></span>|<span data-ttu-id="a9f9b-187">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-187">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="a9f9b-188">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="a9f9b-188">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="a9f9b-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f9b-189">DateTimeOffset</span></span>|<span data-ttu-id="a9f9b-190">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-190">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="a9f9b-191">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="a9f9b-191">businessReadyUpdatesOnly</span></span>|<span data-ttu-id="a9f9b-192">String</span><span class="sxs-lookup"><span data-stu-id="a9f9b-192">String</span></span>|<span data-ttu-id="a9f9b-193">Определяет ветвь обновления для устройств. Возможные значения: `userDefined`, `all`, `businessReadyOnly`.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-193">Determines which branch devices will receive their updates from Possible values are: `userDefined`, `all`, `businessReadyOnly`.</span></span>|



## <a name="response"></a><span data-ttu-id="a9f9b-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9f9b-194">Response</span></span>
<span data-ttu-id="a9f9b-195">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-195">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9f9b-196">Пример</span><span class="sxs-lookup"><span data-stu-id="a9f9b-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9f9b-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9f9b-197">Request</span></span>
<span data-ttu-id="a9f9b-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a9f9b-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9f9b-199">Response</span></span>
<span data-ttu-id="a9f9b-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a9f9b-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



