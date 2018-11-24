# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="7120c-101">Update windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="7120c-101">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="7120c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7120c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7120c-103">Обновление свойств объекта [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7120c-103">Update the properties of a [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7120c-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7120c-104">Prerequisites</span></span>
<span data-ttu-id="7120c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7120c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7120c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7120c-107">Permission type</span></span>|<span data-ttu-id="7120c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7120c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7120c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7120c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7120c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7120c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7120c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7120c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7120c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7120c-112">Not supported.</span></span>|
|<span data-ttu-id="7120c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7120c-113">Application</span></span>|<span data-ttu-id="7120c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7120c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7120c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7120c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7120c-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7120c-116">Request headers</span></span>
|<span data-ttu-id="7120c-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7120c-117">Header</span></span>|<span data-ttu-id="7120c-118">Значение</span><span class="sxs-lookup"><span data-stu-id="7120c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7120c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7120c-119">Authorization</span></span>|<span data-ttu-id="7120c-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7120c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7120c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7120c-121">Accept</span></span>|<span data-ttu-id="7120c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7120c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7120c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7120c-123">Request body</span></span>
<span data-ttu-id="7120c-124">В тексте запроса добавьте представление объекта [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7120c-124">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="7120c-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7120c-125">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="7120c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="7120c-126">Property</span></span>|<span data-ttu-id="7120c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="7120c-127">Type</span></span>|<span data-ttu-id="7120c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7120c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7120c-129">id</span><span class="sxs-lookup"><span data-stu-id="7120c-129">id</span></span>|<span data-ttu-id="7120c-130">String</span><span class="sxs-lookup"><span data-stu-id="7120c-130">String</span></span>|<span data-ttu-id="7120c-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7120c-131">Key of the entity.</span></span> <span data-ttu-id="7120c-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7120c-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7120c-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7120c-133">lastModifiedDateTime</span></span>|<span data-ttu-id="7120c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7120c-134">DateTimeOffset</span></span>|<span data-ttu-id="7120c-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7120c-135">DateTime the object was last modified.</span></span> <span data-ttu-id="7120c-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7120c-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7120c-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7120c-137">createdDateTime</span></span>|<span data-ttu-id="7120c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7120c-138">DateTimeOffset</span></span>|<span data-ttu-id="7120c-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7120c-139">DateTime the object was created.</span></span> <span data-ttu-id="7120c-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7120c-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7120c-141">description</span><span class="sxs-lookup"><span data-stu-id="7120c-141">description</span></span>|<span data-ttu-id="7120c-142">String</span><span class="sxs-lookup"><span data-stu-id="7120c-142">String</span></span>|<span data-ttu-id="7120c-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7120c-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7120c-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7120c-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7120c-145">displayName</span><span class="sxs-lookup"><span data-stu-id="7120c-145">displayName</span></span>|<span data-ttu-id="7120c-146">String</span><span class="sxs-lookup"><span data-stu-id="7120c-146">String</span></span>|<span data-ttu-id="7120c-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7120c-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7120c-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7120c-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7120c-149">version</span><span class="sxs-lookup"><span data-stu-id="7120c-149">version</span></span>|<span data-ttu-id="7120c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7120c-150">Int32</span></span>|<span data-ttu-id="7120c-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7120c-151">Version of the device configuration.</span></span> <span data-ttu-id="7120c-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7120c-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7120c-153">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="7120c-153">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="7120c-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-154">Boolean</span></span>|<span data-ttu-id="7120c-155">Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="7120c-155">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="7120c-156">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="7120c-156">applyOnlyToWindows81</span></span>|<span data-ttu-id="7120c-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-157">Boolean</span></span>|<span data-ttu-id="7120c-158">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="7120c-158">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="7120c-159">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7120c-159">This property is read-only.</span></span>|
|<span data-ttu-id="7120c-160">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="7120c-160">browserBlockAutofill</span></span>|<span data-ttu-id="7120c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-161">Boolean</span></span>|<span data-ttu-id="7120c-162">Указывает, следует ли заблокировать автозаполнение.</span><span class="sxs-lookup"><span data-stu-id="7120c-162">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="7120c-163">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="7120c-163">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="7120c-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-164">Boolean</span></span>|<span data-ttu-id="7120c-165">Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.</span><span class="sxs-lookup"><span data-stu-id="7120c-165">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="7120c-166">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="7120c-166">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="7120c-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-167">Boolean</span></span>|<span data-ttu-id="7120c-168">Указывает, следует ли заблокировать доступ к корпоративному режиму.</span><span class="sxs-lookup"><span data-stu-id="7120c-168">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="7120c-169">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="7120c-169">browserBlockJavaScript</span></span>|<span data-ttu-id="7120c-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-170">Boolean</span></span>|<span data-ttu-id="7120c-171">Указывает, следует ли запретить использование JavaScript.</span><span class="sxs-lookup"><span data-stu-id="7120c-171">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="7120c-172">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="7120c-172">browserBlockPlugins</span></span>|<span data-ttu-id="7120c-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-173">Boolean</span></span>|<span data-ttu-id="7120c-174">Указывает, следует ли заблокировать подключаемые модули.</span><span class="sxs-lookup"><span data-stu-id="7120c-174">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="7120c-175">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="7120c-175">browserBlockPopups</span></span>|<span data-ttu-id="7120c-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-176">Boolean</span></span>|<span data-ttu-id="7120c-177">Указывает, следует ли блокировать всплывающие окна.</span><span class="sxs-lookup"><span data-stu-id="7120c-177">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="7120c-178">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="7120c-178">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="7120c-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-179">Boolean</span></span>|<span data-ttu-id="7120c-180">Указывает, следует ли запретить пользователю отправлять заголовок DNT.</span><span class="sxs-lookup"><span data-stu-id="7120c-180">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="7120c-181">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="7120c-181">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="7120c-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-182">Boolean</span></span>|<span data-ttu-id="7120c-183">Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.</span><span class="sxs-lookup"><span data-stu-id="7120c-183">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="7120c-184">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="7120c-184">browserRequireSmartScreen</span></span>|<span data-ttu-id="7120c-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-185">Boolean</span></span>|<span data-ttu-id="7120c-186">Указывает, обязательно ли использовать фильтр Smart Screen.</span><span class="sxs-lookup"><span data-stu-id="7120c-186">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="7120c-187">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="7120c-187">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="7120c-188">String</span><span class="sxs-lookup"><span data-stu-id="7120c-188">String</span></span>|<span data-ttu-id="7120c-189">Расположение списка сайтов, запускаемых в корпоративном режиме.</span><span class="sxs-lookup"><span data-stu-id="7120c-189">The enterprise mode site list location.</span></span> <span data-ttu-id="7120c-190">Это может быть локальный файл, локальная сеть или HTTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="7120c-190">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="7120c-191">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="7120c-191">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="7120c-192">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="7120c-192">internetSiteSecurityLevel</span></span>](../resources/intune_deviceconfig_internetsitesecuritylevel.md)|<span data-ttu-id="7120c-193">Уровень интернет-безопасности.</span><span class="sxs-lookup"><span data-stu-id="7120c-193">The internet security level.</span></span> <span data-ttu-id="7120c-194">Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="7120c-194">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="7120c-195">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="7120c-195">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="7120c-196">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="7120c-196">siteSecurityLevel</span></span>](../resources/intune_deviceconfig_sitesecuritylevel.md)|<span data-ttu-id="7120c-197">Уровень безопасности интрасети.</span><span class="sxs-lookup"><span data-stu-id="7120c-197">The Intranet security level.</span></span> <span data-ttu-id="7120c-198">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="7120c-198">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="7120c-199">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="7120c-199">browserLoggingReportLocation</span></span>|<span data-ttu-id="7120c-200">String</span><span class="sxs-lookup"><span data-stu-id="7120c-200">String</span></span>|<span data-ttu-id="7120c-201">Расположение хранения отчетов.</span><span class="sxs-lookup"><span data-stu-id="7120c-201">The logging report location.</span></span>|
|<span data-ttu-id="7120c-202">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="7120c-202">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="7120c-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-203">Boolean</span></span>|<span data-ttu-id="7120c-204">Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.</span><span class="sxs-lookup"><span data-stu-id="7120c-204">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="7120c-205">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="7120c-205">browserRequireFirewall</span></span>|<span data-ttu-id="7120c-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-206">Boolean</span></span>|<span data-ttu-id="7120c-207">Указывает, обязательно ли использовать брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="7120c-207">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="7120c-208">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="7120c-208">browserRequireFraudWarning</span></span>|<span data-ttu-id="7120c-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-209">Boolean</span></span>|<span data-ttu-id="7120c-210">Указывает, обязательно ли предупреждение о мошенничестве.</span><span class="sxs-lookup"><span data-stu-id="7120c-210">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="7120c-211">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="7120c-211">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="7120c-212">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="7120c-212">siteSecurityLevel</span></span>](../resources/intune_deviceconfig_sitesecuritylevel.md)|<span data-ttu-id="7120c-213">Уровень безопасности надежных сайтов.</span><span class="sxs-lookup"><span data-stu-id="7120c-213">The trusted sites security level.</span></span> <span data-ttu-id="7120c-214">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="7120c-214">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="7120c-215">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="7120c-215">cellularBlockDataRoaming</span></span>|<span data-ttu-id="7120c-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-216">Boolean</span></span>|<span data-ttu-id="7120c-217">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="7120c-217">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="7120c-218">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="7120c-218">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="7120c-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-219">Boolean</span></span>|<span data-ttu-id="7120c-220">Указывает, следует ли блокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="7120c-220">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="7120c-221">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="7120c-221">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="7120c-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-222">Boolean</span></span>|<span data-ttu-id="7120c-223">Указывает, следует ли запретить использование графического пароля и ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="7120c-223">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="7120c-224">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7120c-224">passwordExpirationDays</span></span>|<span data-ttu-id="7120c-225">Int32</span><span class="sxs-lookup"><span data-stu-id="7120c-225">Int32</span></span>|<span data-ttu-id="7120c-226">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="7120c-226">Password expiration in days.</span></span>|
|<span data-ttu-id="7120c-227">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7120c-227">passwordMinimumLength</span></span>|<span data-ttu-id="7120c-228">Int32</span><span class="sxs-lookup"><span data-stu-id="7120c-228">Int32</span></span>|<span data-ttu-id="7120c-229">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="7120c-229">The minimum password length.</span></span>|
|<span data-ttu-id="7120c-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="7120c-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="7120c-231">Int32</span><span class="sxs-lookup"><span data-stu-id="7120c-231">Int32</span></span>|<span data-ttu-id="7120c-232">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="7120c-232">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="7120c-233">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7120c-233">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="7120c-234">Int32</span><span class="sxs-lookup"><span data-stu-id="7120c-234">Int32</span></span>|<span data-ttu-id="7120c-235">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="7120c-235">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="7120c-236">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7120c-236">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7120c-237">Int32</span><span class="sxs-lookup"><span data-stu-id="7120c-237">Int32</span></span>|<span data-ttu-id="7120c-238">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="7120c-238">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="7120c-239">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="7120c-239">Valid values 0 to 24</span></span>|
|<span data-ttu-id="7120c-240">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7120c-240">passwordRequiredType</span></span>|[<span data-ttu-id="7120c-241">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7120c-241">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="7120c-242">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="7120c-242">The required password type.</span></span> <span data-ttu-id="7120c-243">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="7120c-243">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7120c-244">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="7120c-244">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="7120c-245">Int32</span><span class="sxs-lookup"><span data-stu-id="7120c-245">Int32</span></span>|<span data-ttu-id="7120c-246">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="7120c-246">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="7120c-247">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="7120c-247">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="7120c-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-248">Boolean</span></span>|<span data-ttu-id="7120c-249">Указывает, обязательно ли шифрование данных на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="7120c-249">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="7120c-250">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="7120c-250">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="7120c-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="7120c-251">Boolean</span></span>|<span data-ttu-id="7120c-252">Указывает, обязательно ли автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="7120c-252">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="7120c-253">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="7120c-253">userAccountControlSettings</span></span>|[<span data-ttu-id="7120c-254">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="7120c-254">windowsUserAccountControlSettings</span></span>](../resources/intune_deviceconfig_windowsuseraccountcontrolsettings.md)|<span data-ttu-id="7120c-255">Настройки контроля учетных записей.</span><span class="sxs-lookup"><span data-stu-id="7120c-255">The user account control settings.</span></span> <span data-ttu-id="7120c-256">Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="7120c-256">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="7120c-257">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="7120c-257">workFoldersUrl</span></span>|<span data-ttu-id="7120c-258">String</span><span class="sxs-lookup"><span data-stu-id="7120c-258">String</span></span>|<span data-ttu-id="7120c-259">URL-адрес рабочей папки.</span><span class="sxs-lookup"><span data-stu-id="7120c-259">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="7120c-260">Ответ</span><span class="sxs-lookup"><span data-stu-id="7120c-260">Response</span></span>
<span data-ttu-id="7120c-261">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7120c-261">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7120c-262">Пример</span><span class="sxs-lookup"><span data-stu-id="7120c-262">Example</span></span>
### <a name="request"></a><span data-ttu-id="7120c-263">Запрос</span><span class="sxs-lookup"><span data-stu-id="7120c-263">Request</span></span>
<span data-ttu-id="7120c-264">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7120c-264">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1693

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="7120c-265">Ответ</span><span class="sxs-lookup"><span data-stu-id="7120c-265">Response</span></span>
<span data-ttu-id="7120c-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7120c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1865

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```



