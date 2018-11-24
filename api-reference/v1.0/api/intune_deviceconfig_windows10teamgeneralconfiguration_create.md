# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="6e1b0-101">Создание объекта windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e1b0-101">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="6e1b0-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e1b0-103">Создает объект [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e1b0-103">Create a new [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6e1b0-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6e1b0-104">Prerequisites</span></span>
<span data-ttu-id="6e1b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6e1b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6e1b0-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e1b0-107">Permission type</span></span>|<span data-ttu-id="6e1b0-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e1b0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e1b0-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e1b0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6e1b0-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e1b0-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e1b0-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e1b0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e1b0-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-112">Not supported.</span></span>|
|<span data-ttu-id="6e1b0-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e1b0-113">Application</span></span>|<span data-ttu-id="6e1b0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e1b0-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e1b0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6e1b0-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6e1b0-116">Request headers</span></span>
|<span data-ttu-id="6e1b0-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e1b0-117">Header</span></span>|<span data-ttu-id="6e1b0-118">Значение</span><span class="sxs-lookup"><span data-stu-id="6e1b0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e1b0-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e1b0-119">Authorization</span></span>|<span data-ttu-id="6e1b0-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e1b0-121">Accept</span><span class="sxs-lookup"><span data-stu-id="6e1b0-121">Accept</span></span>|<span data-ttu-id="6e1b0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6e1b0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e1b0-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e1b0-123">Request body</span></span>
<span data-ttu-id="6e1b0-124">В теле запроса добавьте представление объекта windows10TeamGeneralConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-124">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="6e1b0-125">Ниже показаны свойства, которые необходимо указывать при создании объекта windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-125">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="6e1b0-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e1b0-126">Property</span></span>|<span data-ttu-id="6e1b0-127">Тип</span><span class="sxs-lookup"><span data-stu-id="6e1b0-127">Type</span></span>|<span data-ttu-id="6e1b0-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6e1b0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e1b0-129">id</span><span class="sxs-lookup"><span data-stu-id="6e1b0-129">id</span></span>|<span data-ttu-id="6e1b0-130">String</span><span class="sxs-lookup"><span data-stu-id="6e1b0-130">String</span></span>|<span data-ttu-id="6e1b0-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-131">Key of the entity.</span></span> <span data-ttu-id="6e1b0-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e1b0-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e1b0-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e1b0-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6e1b0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e1b0-134">DateTimeOffset</span></span>|<span data-ttu-id="6e1b0-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-135">DateTime the object was last modified.</span></span> <span data-ttu-id="6e1b0-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e1b0-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e1b0-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e1b0-137">createdDateTime</span></span>|<span data-ttu-id="6e1b0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e1b0-138">DateTimeOffset</span></span>|<span data-ttu-id="6e1b0-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-139">DateTime the object was created.</span></span> <span data-ttu-id="6e1b0-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e1b0-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e1b0-141">description</span><span class="sxs-lookup"><span data-stu-id="6e1b0-141">description</span></span>|<span data-ttu-id="6e1b0-142">String</span><span class="sxs-lookup"><span data-stu-id="6e1b0-142">String</span></span>|<span data-ttu-id="6e1b0-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6e1b0-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e1b0-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e1b0-145">displayName</span><span class="sxs-lookup"><span data-stu-id="6e1b0-145">displayName</span></span>|<span data-ttu-id="6e1b0-146">String</span><span class="sxs-lookup"><span data-stu-id="6e1b0-146">String</span></span>|<span data-ttu-id="6e1b0-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6e1b0-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e1b0-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e1b0-149">version</span><span class="sxs-lookup"><span data-stu-id="6e1b0-149">version</span></span>|<span data-ttu-id="6e1b0-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6e1b0-150">Int32</span></span>|<span data-ttu-id="6e1b0-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-151">Version of the device configuration.</span></span> <span data-ttu-id="6e1b0-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e1b0-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e1b0-153">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="6e1b0-153">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="6e1b0-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e1b0-154">Boolean</span></span>|<span data-ttu-id="6e1b0-155">Указывает, следует ли заблокировать оперативную аналитику Azure.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-155">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="6e1b0-156">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="6e1b0-156">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="6e1b0-157">String</span><span class="sxs-lookup"><span data-stu-id="6e1b0-157">String</span></span>|<span data-ttu-id="6e1b0-158">Идентификатор рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-158">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="6e1b0-159">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="6e1b0-159">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="6e1b0-160">String</span><span class="sxs-lookup"><span data-stu-id="6e1b0-160">String</span></span>|<span data-ttu-id="6e1b0-161">Ключ рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-161">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="6e1b0-162">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="6e1b0-162">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="6e1b0-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e1b0-163">Boolean</span></span>|<span data-ttu-id="6e1b0-164">Указывает, следует ли автоматически запускать приложение Connect, когда начинается проекция.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-164">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="6e1b0-165">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="6e1b0-165">maintenanceWindowBlocked</span></span>|<span data-ttu-id="6e1b0-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e1b0-166">Boolean</span></span>|<span data-ttu-id="6e1b0-167">Указывает, следует ли запретить устанавливать период обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-167">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="6e1b0-168">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="6e1b0-168">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="6e1b0-169">Int32</span><span class="sxs-lookup"><span data-stu-id="6e1b0-169">Int32</span></span>|<span data-ttu-id="6e1b0-170">Длительность периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-170">Maintenance window duration for device updates.</span></span> <span data-ttu-id="6e1b0-171">Допустимые значения: от 0 до 5</span><span class="sxs-lookup"><span data-stu-id="6e1b0-171">Valid values 0 to 5</span></span>|
|<span data-ttu-id="6e1b0-172">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="6e1b0-172">maintenanceWindowStartTime</span></span>|<span data-ttu-id="6e1b0-173">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6e1b0-173">TimeOfDay</span></span>|<span data-ttu-id="6e1b0-174">Начало периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-174">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="6e1b0-175">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="6e1b0-175">miracastChannel</span></span>|[<span data-ttu-id="6e1b0-176">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="6e1b0-176">miracastChannel</span></span>](../resources/intune_deviceconfig_miracastchannel.md)|<span data-ttu-id="6e1b0-177">Канал.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-177">The channel.</span></span> <span data-ttu-id="6e1b0-178">Возможные значения: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-178">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="6e1b0-179">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="6e1b0-179">miracastBlocked</span></span>|<span data-ttu-id="6e1b0-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e1b0-180">Boolean</span></span>|<span data-ttu-id="6e1b0-181">Указывает, следует ли заблокировать беспроводное проецирование.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-181">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="6e1b0-182">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="6e1b0-182">miracastRequirePin</span></span>|<span data-ttu-id="6e1b0-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e1b0-183">Boolean</span></span>|<span data-ttu-id="6e1b0-184">Указывает, обязательно ли использовать ПИН-код для беспроводного проецирования.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-184">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="6e1b0-185">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="6e1b0-185">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="6e1b0-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e1b0-186">Boolean</span></span>|<span data-ttu-id="6e1b0-187">Указывает, следует ли отключить функцию "Мои встречи и файлы" в меню "Пуск", которая показывает собрания и файлы вошедшего пользователя из Office 365.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-187">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="6e1b0-188">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="6e1b0-188">settingsBlockSessionResume</span></span>|<span data-ttu-id="6e1b0-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e1b0-189">Boolean</span></span>|<span data-ttu-id="6e1b0-190">Указывает, следует ли разрешить возобновление сеанса после истечения времени.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-190">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="6e1b0-191">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="6e1b0-191">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="6e1b0-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e1b0-192">Boolean</span></span>|<span data-ttu-id="6e1b0-193">Указывает, следует ли отключить автоматическое добавление в диалоговое окно входа приглашенных из запланированных собраний.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-193">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="6e1b0-194">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="6e1b0-194">settingsDefaultVolume</span></span>|<span data-ttu-id="6e1b0-195">Int32</span><span class="sxs-lookup"><span data-stu-id="6e1b0-195">Int32</span></span>|<span data-ttu-id="6e1b0-196">Задает объем нового сеанса по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-196">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="6e1b0-197">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-197">Permitted values are 0-100.</span></span> <span data-ttu-id="6e1b0-198">Значение по умолчанию — 45.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-198">The default is 45.</span></span> <span data-ttu-id="6e1b0-199">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="6e1b0-199">Valid values 0 to 100</span></span>|
|<span data-ttu-id="6e1b0-200">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="6e1b0-200">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="6e1b0-201">Int32</span><span class="sxs-lookup"><span data-stu-id="6e1b0-201">Int32</span></span>|<span data-ttu-id="6e1b0-202">Определяет время до отключения экрана Центра (в минутах).</span><span class="sxs-lookup"><span data-stu-id="6e1b0-202">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="6e1b0-203">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="6e1b0-203">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="6e1b0-204">Int32</span><span class="sxs-lookup"><span data-stu-id="6e1b0-204">Int32</span></span>|<span data-ttu-id="6e1b0-205">Определяет время до истечения времени сеанса (в минутах).</span><span class="sxs-lookup"><span data-stu-id="6e1b0-205">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="6e1b0-206">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="6e1b0-206">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="6e1b0-207">Int32</span><span class="sxs-lookup"><span data-stu-id="6e1b0-207">Int32</span></span>|<span data-ttu-id="6e1b0-208">Определяет время до перехода Центра в спящий режим (в минутах).</span><span class="sxs-lookup"><span data-stu-id="6e1b0-208">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="6e1b0-209">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="6e1b0-209">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="6e1b0-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e1b0-210">Boolean</span></span>|<span data-ttu-id="6e1b0-211">Указывает, следует ли заблокировать автоматический вывод экрана приветствия из спящего режима, когда кто-то входит в комнату.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-211">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="6e1b0-212">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="6e1b0-212">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="6e1b0-213">String</span><span class="sxs-lookup"><span data-stu-id="6e1b0-213">String</span></span>|<span data-ttu-id="6e1b0-214">URL-адрес фонового изображения экрана приветствия.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-214">The welcome screen background image URL.</span></span> <span data-ttu-id="6e1b0-215">URL-адрес должен начинаться с протокола HTTPS и возвращать PNG-изображение.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-215">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="6e1b0-216">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="6e1b0-216">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="6e1b0-217">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="6e1b0-217">welcomeScreenMeetingInformation</span></span>](../resources/intune_deviceconfig_welcomescreenmeetinginformation.md)|<span data-ttu-id="6e1b0-218">Информация о собраниях, показываемая на экране приветствия.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-218">The welcome screen meeting information shown.</span></span> <span data-ttu-id="6e1b0-219">Возможные значения: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-219">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="6e1b0-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e1b0-220">Response</span></span>
<span data-ttu-id="6e1b0-221">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-221">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e1b0-222">Пример</span><span class="sxs-lookup"><span data-stu-id="6e1b0-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="6e1b0-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e1b0-223">Request</span></span>
<span data-ttu-id="6e1b0-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1150

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```

### <a name="response"></a><span data-ttu-id="6e1b0-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e1b0-225">Response</span></span>
<span data-ttu-id="6e1b0-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6e1b0-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1322

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```



