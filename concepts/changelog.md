# <a name="changelog-for-microsoft-graph"></a>Журнал изменений Microsoft Graph

Этот журнал содержит сведения об изменениях Microsoft Graph, в том числе API Microsoft Graph для конечных точек версии 1.0 и бета-версии.  

Дополнительные сведения об известных проблемах с API Microsoft Graph см. в статье [Известные проблемы](known_issues.md).

## <a name="june-2017"></a>Июнь 2017 г.

### <a name="outlook-calendar"></a>Календарь Outlook

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|1.0|Повышен уровень для следующих 4 свойств [calendar](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/calendar) до версии 1.0: **canEdit**, **canShare**, **canViewPrivateItems** и **owner**.|


### <a name="intune-apis"></a>Интерфейсы API Intune

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[defaultDeviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_defaultdevicecompliancepolicy)<br/>[deviceConfigurationUserStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuserstatesummary)<br/>[deviceManagementScriptDeviceState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptdevicestate)<br/>[deviceManagementScriptRunSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptrunsummary)<br/>[deviceManagementScriptUserState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptuserstate)<br/>[iosUpdateDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdatedevicestatus)<br/>[windowsManagedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanageddevice)<br/>[windowsManagementAppHealthState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapphealthstate)<br/>[windowsManagementAppHealthSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapphealthsummary)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[bitLockerFixedDrivePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerfixeddrivepolicy)<br/>[bitLockerRecoveryOptions](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerrecoveryoptions)<br/>[bitLockerRemovableDrivePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerremovabledrivepolicy)<br/>[deleteUserFromSharedAppleDeviceActionResult](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_deleteuserfromsharedappledeviceactionresult)<br/>[iosNetworkUsageRule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnetworkusagerule)<br/>|
|Удаление|Бета-версия|Удалены следующие объекты:<br/>**deviceManagementScriptState**<br/>|
|Удаление|Бета-версия|Удалено действие wipeByDeviceTag для [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_user) |
|Изменение|Бета-версия|Добавлены свойства **innerAuthenticationProtocolForEapTtls**, **innerAuthenticationProtocolForPeap** и **outerIdentityPrivacyTemporaryValue** в объект [androidEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidenterprisewificonfiguration)|
|Изменение|Бета-версия|Удалены свойства **nonEapAuthenticationMethodForEapTtls**, **nonEapAuthenticationMethodForPeap** и **enableOuterIdentityPrivacy** из объекта [androidEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidenterprisewificonfiguration)|
|Изменение|Бета-версия|Добавлено свойство **deployedAppCount** в объект [androidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection)|
|Изменение|Бета-версия|Удалены свойства **instanceDisplayName** и **settingPlatform** из объекта [complianceSettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/complianceSettingStateSummary)|
|Изменение|Бета-версия|Добавлено свойство **deployedAppCount** в объект [defaultManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection)|
|Изменение|Бета-версия|Удалены свойства **instanceDisplayName** и **settingPlatform** из объекта [deviceCompliancePolicySettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary)|
|Изменение|Бета-версия|Удалено свойство **devicePlatform** из объекта [deviceComplianceSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate)|
|Изменение|Бета-версия|Добавлены свойства **assignmentStatus**, **assignmentProgress** и **assignmentErrorMessage** в объект [deviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration)|
|Изменение|Бета-версия|Добавлено свойство **intuneBrand** в объект [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement)|
|Изменение|Бета-версия|Добавлены свойства **enforceSignatureCheck** и **fileName** в объект [deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript)|
|Изменение|Бета-версия|Добавлены свойства **innerAuthenticationProtocolForEapTtls** и **outerIdentityPrivacyTemporaryValue** в объект [iosEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosenterprisewificonfiguration)|
|Изменение|Бета-версия|Удалены свойства **nonEapAuthenticationMethodForEapTtls** и **enableOuterIdentityPrivacy** из объекта [iosEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosenterprisewificonfiguration)|
|Изменение|Бета-версия|Добавлены свойства **classroomAppForceUnpromptedScreenObservation**, **keyboardBlockDictation**, **networkUsageRules** и **wiFiConnectOnlyToConfiguredNetworks** в объект [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration)|
|Изменение|Бета-версия|Добавлено свойство **deployedAppCount** в объект [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection)|
|Изменение|Бета-версия|Добавлено свойство **preSharedKey** в объект [iosWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswificonfiguration)|
|Изменение|Бета-версия|Добавлены свойства **innerAuthenticationProtocolForEapTtls** и **outerIdentityPrivacyTemporaryValue** в объект [macOSEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosenterprisewificonfiguration)|
|Изменение|Бета-версия|Удалены свойства **nonEapAuthenticationMethodForEapTtls** и **enableOuterIdentityPrivacy** из объекта [macOSEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosenterprisewificonfiguration)|
|Изменение|Бета-версия|Удалены свойства **lastModifiedTime** и **deployedAppCount** из объекта [managedAppPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy)|
|Изменение|Бета-версия|Добавлено свойство **serialNumber** в объект [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice)|
|Изменение|Бета-версия|Удалено свойство **managementAgents** из объекта [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice)|
|Изменение|Бета-версия|Добавлено свойство **deployedAppCount** в объект [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration)|
|Изменение|Бета-версия|Добавлены свойства **bitLockerFixedDrivePolicy** и **bitLockerRemovableDrivePolicy** в объект [windows10EndpointProtectionConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration)|
|Изменение|Бета-версия|Добавлены свойства **enterpriseCloudPrintDiscoveryEndPoint**, **enterpriseCloudPrintOAuthAuthority**, **enterpriseCloudPrintOAuthClientIdentifier**, **enterpriseCloudPrintResourceIdentifier**, **enterpriseCloudPrintDiscoveryMaxLimit**, **enterpriseCloudPrintMopriaDiscoveryResourceIdentifier**, **edgeBlockAddressBarDropdown**, **edgeBlockCompatibilityList**, **edgeClearBrowsingDataOnExit**, **edgeAllowStartPagesModification**, **edgeDisableFirstRunPage**, **edgeBlockLiveTileDataCollection** и **edgeSyncFavoritesWithInternetExplorer** в объект [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration)|
|Изменение|Бета-версия|Добавлено свойство **availableVersion** в объект [windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp)|
|Изменение|Бета-версия|Удалены свойства **onboardingStatus**, **deployedVersion** и **lastModifiedTime** из объекта [windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp)|
|Изменение|Бета-версия|Добавлено свойство **packageIdentityName** в объект [windowsStoreForBusinessApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessapp)|
|Изменение|Бета-версия|Добавлены свойства навигации **mobileAppIdentifierDeployments** и **deploymentSummary** в объект [androidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection)|
|Изменение|Бета-версия|Добавлено свойство навигации **mobileAppIdentifierDeployments** в объект [defaultManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection)|
|Изменение|Бета-версия|Добавлены свойства навигации **deviceConfigurationUserStateSummaries** и **iosUpdateStatuses** в объект [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement)|
|Изменение|Бета-версия|Удалено свойство навигации **complianceSettingStateSummaries** из объекта [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement)|
|Изменение|Бета-версия|Добавлены свойства навигации **runSummary**, **deviceRunStates** и **userRunStates** в объект [deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript)|
|Изменение|Бета-версия|Удалено свойство навигации **runStates** из объекта [deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript)|
|Изменение|Бета-версия|Добавлены свойства навигации **mobileAppIdentifierDeployments** и **deploymentSummary** в объект [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection)|
|Изменение|Бета-версия|Удалены свойства навигации **mobileAppIdentifierDeployments** и **deploymentSummary** из объекта [managedAppPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy)|
|Изменение|Бета-версия|Добавлены свойства навигации **mobileAppIdentifierDeployments** и **deploymentSummary** в объект [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration)|
|Изменение|Бета-версия|Добавлены свойства навигации **healthSummary** и **healthStates** в объект [windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp)|
|Изменение|Бета-версия|Добавлены свойства **applicationId**, **appName**, **platformId**, **userFailures** и **deviceFailures** в сложный тип [appInstallationFailure](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure)|
|Изменение|Бета-версия|Добавлены свойства **encryptionMethod**, **startupAuthenticationRequired**, **startupAuthenticationBlockWithoutTpmChip**, **startupAuthenticationTpmUsage**, **startupAuthenticationTpmPinUsage**, **startupAuthenticationTpmKeyUsage**, **startupAuthenticationTpmPinAndKeyUsage**, **recoveryOptions** и **prebootRecoveryEnableMessageAndUrl** в сложный тип [bitLockerSystemDrivePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockersystemdrivepolicy)|
|Изменение|Бета-версия|Удалены свойства **settingName**, **userId**, **userName**, **userEmail** и **currentValue** из сложного типа [deviceCompliancePolicySettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate)|
|Изменение|Бета-версия|Удалены свойства **settingName**, **userId**, **userName**, **userEmail** и **currentValue** из сложного типа [deviceConfigurationSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate)|
|Изменение|Бета-версия|Добавлены свойства **windowsCommercialId** и **windowsCommercialIdLastModifiedTime** в сложный тип [deviceManagementSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings)|
|Изменение|Бета-версия|Добавлено свойство **address** в сложный тип [vpnServer](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_vpnserver)|


## <a name="may-2017"></a>Май 2017 г.

### <a name="application-api-changes"></a>Изменения в API приложений

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Изменение|Бета-версии| Обновление API приложений. Это первый набор изменений, включающий изменение структуры и переименование свойств объекта [application](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/application).<br/>**Новые объекты:** [api](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/api]), [informationalUrl](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/informationalUrl), [installedClient](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/installedclient), [permissionScope](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/permissionscope), [preauthorizedApplication](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/preauthorizedapplication), [web](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/web).<br/>**Удаленные свойства:** addIns, appRoles, availableToOtherOrganizations, knownClientApplications, oauth2AllowUrlPathMatching, recordConsentConditions.<br/>**Переименованные свойства:** с appId на id, с identifierUris на applicationAliases, с availableToOtherTenants на orgRestrictions, с mainLogo на logo, с oauth2Permissions на publishedPermissionsScopes, с publicClient на allowPublicClient, с replyUrls на redirectUrls.<br/>**Новые свойства:** tags. |

### <a name="remove-deprecated-planner-api"></a>Удаление устаревшего API Планировщика
|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:-------------|
|Удаление|Бета-версия|Удалены следующие объекты:<br/>**task**<br/>**plan**<br/>**bucket**<br/>**taskDetails**<br/>**planDetails**<br/>**taskBoardTaskFormat**<br/>**planTaskBoard**|

### <a name="project-rome"></a>Project Rome

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:-------------|
|Дополнение|Бета|Добавлена поддержка Project Rome, в том числе [получения списка устройств](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_list_devices), [отправки команды устройству](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/send_device_command) и [проверки состояния команды](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/get_device_command_status).|

### <a name="administrative-units-property-changes"></a>Изменения свойств административных единиц

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
| Изменение        | Бета       | Тип свойства roleMemberInfo объекта [scopedRoleMembership](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/scopedrolemembership) изменен на [identity](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/identity). |
| Изменение        | Бета       | Свойство навигации scopedAdministratorOf объекта [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/user) заменено на scopedRoleMemberOf. |
| Изменение        | Бета       | Свойство навигации scopedAdministrators объекта [administrativeUnit](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/administrativeunit) заменено на scopedRoleMembers. |
| Изменение        | Бета       | Свойство навигации scopedAdministrators объекта [directoryRole](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/directoryrole) заменено на scopedMembers. |

### <a name="add-users-and-groups-webhook-support-in-preview"></a>Добавлена поддержка пользователей и групп в веб-перехватчиках в бета-версии

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
| Изменение        | Бета       | Добавлена поддержка пользователей и групп в [веб-перехватчиках](https://developer.microsoft.com/graph/docs/api-reference/beta/resources/webhooks).

### <a name="add-delta-query-to-v10"></a>Добавлена поддержка запросов изменений в версии 1.0

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
| Дополнение      | 1.0       | Добавлена поддержка функции delta в версии 1.0. Она позволяет выполнять [запрос изменений](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_overview) для следующих объектов:<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Примеры см. в следующих статьях:<br/>[Получение добавочных изменений для групп](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_groups)<br/>[Получение добавочных изменений для сообщений в папке](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_messages)<br/>[Получение добавочных изменений для пользователей](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_users)|
| Изменение        | Бета       | Добавлена возможность дополнительной фильтрации запросов (по идентификатору) для [пользователей](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_delta) и [групп](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/group_delta). |

### <a name="added-user-resource-support-for-deleted-items"></a>Добавлена поддержка работы с удаленными элементами для ресурса user

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
| Дополнение      | Бета       | Добавлена поддержка [восстановления и окончательного удаления пользователей](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/directory). |

### <a name="added-onpremisesprovisioningerror"></a>Добавлен объект OnPremisesProvisioningError

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
| Дополнение      | Бета       | Новый объект: [OnPremisesProvisioningError](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/onpremisesprovisioningerror) |
| Изменение        | Бета       | В объекты [user](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/user), [group](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/group) и [orgcontact](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/orgcontact) добавлено свойство OnPremisesProvisioningError. |

### <a name="added-deleteddatetime-property"></a>Добавлено свойство deletedDateTime

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Изменение|Бета|В объект [user](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/user) добавлено свойство deletedDateTime.
|Изменение|Бета|В объект [group](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/group) добавлено свойство deletedDateTime.
|Изменение|Бета|В объект [application](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/application) добавлено свойство deletedDateTime.

### <a name="added-domain-operations-to-v10"></a>Добавлены операции с доменами в версии 1.0

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|1.0|Добавлены операции с [доменами](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domain).<br/>Новые объекты:</br>[domain](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domain);<br/>[domainDnsRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domaindnsrecord);<br/>[domainDnsCnameRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domainDnsCnameRecord);<br/>[domainDnsMxRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domainDnsMxRecord);<br/>[domainDnsSrvRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domainDnsSrvRecord);<br/>[domainDnsTxtRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domainDnsTxtRecord);<br/>[domainDnsUnavailableRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domainDnsUnavailableRecord).<br/>Новые действия:</br>[verify](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/api/domain_verify) |

### <a name="added-contracts-to-v10"></a>Добавлены контракты в версии 1.0

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|1.0|Новый объект:</br>[contract](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/contract) |

### <a name="added-licensedetails-to-v10"></a>Добавлен объект licenseDetails в версии 1.0

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|1.0|Новый объект:</br>[licenseDetails](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/licensedetails) |
|Изменение  |1.0|Добавлено свойство навигации [licensedetails](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/api/user_list_licensedetails) для объекта [user](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/user). |


### <a name="drive-api"></a>API Диска

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:----------|:--------------|
| Дополнение | 1.0 | Добавлен тип ресурса **baseItem**, состоящий из базовых свойств объекта **driveItem**.
| Дополнение | 1.0 и бета | В объект **thumbnail** добавлено свойство **sourceItemId**. <br/> В объект **sharepointIds** добавлено свойство **siteUrl**. <br/> В объект **shared** добавлены свойства **sharedBy** и **sharedDateTime**. <br/> В объект **remoteItem** добавлено свойство **shared**. <br/> В объекты**drive** и **itemReference** добавлено свойство **sharepointIds**. <br/> В объект **fileSystemInfo** добавлено свойство **lastAccessedDateTime**. <br/> В объект **sharedDriveItem** добавлены свойства навигации **driveItem** и **site**. <br/> В объект **baseItem** добавлено свойство **parentReference**.
| Изменение | 1.0 и бета | Объекты **driveItem** и **sharedDriveItem** теперь наследуются от объекта **baseItem**. <br/> Тип **identity** отмечен как открытый.
| Изменение | Бета | В объект **sharingLink** добавлены свойства **configuratorUrl** и **webHtml**. <br/> Добавлены тип ресурса **folderView** и свойство **view** для типа ресурса **folder**. <br/> В объект **driveItem** добавлено свойство навигации **listItem**. <br/> В объект **drive** добавлено свойство навигации **list**.


### <a name="extensions-open-extensions"></a>Расширения (открытые расширения)

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|1.0| Поддержка [openTypeExtension](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/opentypeextension) в ресурсах [device](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/device), [group](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/group), [organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/organization) и [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user). |
|Дополнение|1.0 и бета-версия|Если пользователь вошел с помощью личной учетной записи Майкрософт, открытые расширения поддерживаются в ресурсах event, post, group, message, contact и user. (При использовании рабочей или учебной учетной записи открытые расширения также поддерживаются в ресурсах device, group, organization и user.)|
|Дополнение|1.0 и бета|Поддержка параметра `$expand` для [получения открытых расширений](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/opentypeextension_get) в ресурсах [device](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/device), [group](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/group), [organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/organization), [post](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/post) и [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user).|
|Дополнение|Бета|Поддержка параметра `$expand` для [получения открытых расширений](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/opentypeextension_get) в объекте [administrativeUnit](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/administrativeunit).|


### <a name="extensions-schema-extensions"></a>Расширения (расширения схемы) 

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|1.0|Новый ресурс [schemaExtension](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/schemaextension) и методы CRUD для управления определениями расширений для следующих ресурсов: [contact](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/contact), [device](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/device), [event](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/event), [group](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/group), [message](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/message), [organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/organization), [post](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/post) и [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user). Обратите внимание, что объект [administrativeUnit](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/administrativeunit) по-прежнему поддерживается только в бета-версии.|
|Дополнение|1.0|Существующие методы POST, GET и PATCH ресурсов [contact](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/contact), [device](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/device), [event](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/event), [group](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/group), [message](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/message), [organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/organization), [post](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/post) и [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) теперь поддерживают добавление, получение, обновление и удаление пользовательских данных, хранящихся в виде расширений схемы в соответствующих экземплярах ресурсов.|
|Дополнение|1.0 и бета-версия| Теперь вы можете использовать параметр `$filter` для поиска экземпляров ресурсов, свойства которых совпадают с определенным значениями свойств расширений, например имени. Эта возможность рассматривается подробнее в этом [примере](https://devx.microsoft-tst.com/en-us/graph/docs/concepts/extensibility_schema_groups#5-get-a-group-and-its-extension-data). |
|Изменение|1.0 и бета| [Удаление определения расширения схемы](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/schemaextension_delete) больше не влияет на доступ к пользовательским данным, добавленным на основе этого определения. |
|Изменение|1.0 и бета| Теперь вы можете задать для сложного типа расширения схемы значение null, чтобы удалить расширение схемы из экземпляра ресурса. |


### <a name="group"></a>Группа

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:----------|:--------------|
| Дополнение | 1.0 и бета | Добавлены свойства навигации **drives** и **sites** для объекта **group**.

### <a name="insights-apis"></a>API Insights

|**Тип изменения**|**Версия**|**Описание**| 
|:-------------|:-----------|:--------------|
|Дополнение|Бета|Добавлен [API Shared](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_shared).<br />Новые ресурсы:<br />[sharingDetail](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_sharingdetail) <br />[insightIdentity](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_insightidentity) <br />
|Дополнение|Бета|Добавлен [API Used](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_used).<br />Новые ресурсы:<br />[usageDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_usagedetails) <br />
|Изменение|Бета|Новое свойство **Type** в<br />ресурсе [resourceVisualization](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_resourcevisualization). <br />
|Удаление|Бета-версия|Удалены следующие объекты:<br/>**workingWith**<br/>**trendingAround**<br/>|

### <a name="intune-apis"></a>API Intune

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidForWorkMobileAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidforworkmobileappconfiguration)<br/>[cartToClassAssociation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_carttoclassassociation)<br/>[deviceCompliancePolicySettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary)<br/>[eBookInstallSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_ebookinstallsummary)<br/>[eBookVppGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_ebookvppgroupassignment)<br/>[iosUpdateConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdateconfiguration)<br/>[remoteAssistancePartner](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner)<br/>[windows10EndpointProtectionConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration)<br/>[windowsDeviceMalwareState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsdevicemalwarestate)<br/>[windowsInformationProtectionAppLearningSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_wip_windowsinformationprotectionapplearningsummary)<br/>[windowsMalwareInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsmalwareinformation)<br/>[windowsProtectionState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsprotectionstate)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[androidPermissionAction](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidpermissionaction)<br/>[bitLockerSystemDrivePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockersystemdrivepolicy)<br/>[defenderDetectedMalwareActions](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_defenderdetectedmalwareactions)<br/>[settingSource](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_settingsource)<br/>|
|Дополнение|Бета|Добавлено действие [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_books_managedebook_assign) для объекта [managedEBook](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_managedebook). |
|Дополнение|Бета|Добавлено действие [beginOnboarding](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_remoteassistance_remoteassistancepartner_beginonboarding) для объекта [remoteAssistancePartner](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner). |
|Дополнение|Бета|Добавлено действие [disconnect](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_remoteassistance_remoteassistancepartner_disconnect) для объекта [remoteAssistancePartner](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner). |
|Удаление|Бета-версия|Удалены следующие объекты:<br/>**outlookTask**<br/>**outlookTaskFolder**<br/>**outlookTaskGroup**<br/>**outlookUser**<br/>**windowsManagementAppHealthState**<br/>|
|Удаление|Бета-версия|Удалены следующие сложные типы:<br/>**applePushNotificationCertificateSetting**<br/>**eventCreationOptions**<br/>|
|Изменение|Бета|Добавлены свойства **workProfilePasswordBlockFingerprintUnlock**, **workProfilePasswordBlockTrustAgents**, **workProfilePasswordExpirationDays**, **workProfilePasswordMinimumLength**, **workProfilePasswordMinutesOfInactivityBeforeScreenTimeout**, **workProfilePasswordPreviousPasswordBlockCount**, **workProfilePasswordSignInFailureCountBeforeFactoryReset**, **workProfilePasswordRequiredType** и **workProfileRequirePassword** для объекта [androidForWorkGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkgeneraldeviceconfiguration).|
|Изменение|Бета|Добавлено свойство **subjectAlternativeNameFormatString** для объекта [androidForWorkPkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkpkcscertificateprofile).|
|Изменение|Бета|Добавлены свойства **subjectNameFormatString** и **subjectAlternativeNameFormatString** для объекта [androidForWorkScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile).|
|Изменение|Бета|Добавлено свойство **kioskModeManagedApps** для объекта [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration).|
|Изменение|Бета|Удалено свойство **kioskModeManagedAppId** для объекта [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration).|
|Изменение|Бета|Добавлено свойство **subjectAlternativeNameFormatString** для объекта [androidPkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidpkcscertificateprofile).|
|Изменение|Бета|Добавлены свойства **subjectNameFormatString** и **subjectAlternativeNameFormatString** для объекта [androidScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidscepcertificateprofile).|
|Изменение|Бета|Удалено свойство **hexColor** для объекта [calendar](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/calendar).|
|Изменение|Бета|Для объекта [complianceSettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_compliancesettingstatesummary) добавлены свойства **setting** и **platformType**|
|Изменение|Бета|Удалено свойство **windowsManagementAppEnabled** для объекта [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement).|
|Изменение|Бета|Добавлены свойства **userName**, **deviceModel** и **platform** для объекта [deviceComplianceDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus).|
|Изменение|Бета|Добавлены свойства **userPrincipalName** и **deviceModel** для объекта [deviceComplianceSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate).|
|Изменение|Бета|Для объекта [deviceComplianceSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) добавлены свойства **platformType**, **setting**, **userId** и **userEmail**|
|Изменение|Бета|Для объекта [deviceCompliancePolicyDeviceStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary) добавлено свойство **inGracePeriodCount**|
|Изменение|Бета|Добавлены свойства **userName**, **deviceModel** и **platform** для объекта [deviceConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus).|
|Изменение|Бета|Удалено свойство **creationOptions** для объекта [event](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/event).|
|Изменение|Бета|Удалено свойство **isDelegated** для объекта [eventMessage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/eventMessage).|
|Изменение|Бета|Удалены свойства **unseenConversationsCount** и **unseenMessagesCount** для объекта [group](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/group).|
|Изменение|Бета|Добавлены свойства **settingXml** и **settings** для объекта [iosMobileAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_iosmobileappconfiguration).|
|Изменение|Бета|Добавлено свойство **subjectAlternativeNameFormatString** для объекта [iosPkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iospkcscertificateprofile).|
|Изменение|Бета|Добавлено свойство **subjectAlternativeNameFormatString** для объекта [iosScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosscepcertificateprofile).|
|Изменение|Бета|Добавлено свойство **systemIntegrityProtectionEnabled** для объекта [macOSCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscompliancepolicy).|
|Изменение|Бета|Добавлено свойство **subjectAlternativeNameFormatString** для объекта [macOSScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosscepcertificateprofile).|
|Изменение|Бета|Для объекта [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) добавлены свойства **complianceGracePeriodExpirationDateTime**, **userPrincipalName** и **imei**|
|Изменение|Бета|Удалены свойства **settingXml** и **settings** для объекта [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration).|
|Изменение|Бета|Добавлены свойства **useSharedComputerActivation**, **updateChannel**, **officePlatformArchitecture** и **localesToInstall** для объекта [officeSuiteApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp).|
|Изменение|Бета|Удалено свойство **applePushNotificationCertificateSetting** для объекта [organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_organization).|
|Изменение|Бета|Изменены следующие свойства объекта [post](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/post):<br/>свойство **sender** сделано обязательным.<br/>|
|Изменение|Бета|Добавлены свойства **compliantUserCount**, **nonCompliantUserCount**, **remediatedUserCount**, **errorUserCount**, **unknownUserCount**, **conflictUserCount** и **notApplicableUserCount** для объекта [softwareUpdateStatusSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_softwareupdatestatussummary).|
|Изменение|Бета|Добавлены свойства **bluetoothAllowedServices**, **bluetoothBlockPrePairing**, **cellularData**, **defenderDetectedMalwareActions**, **defenderPotentiallyUnwantedAppAction**, **lockScreenAllowTimeoutConfiguration**, **lockScreenBlockCortana**, **lockScreenBlockToastNotifications**, **lockScreenTimeoutInSeconds**, **passwordBlockSimple**, **privacyAutoAcceptPairingAndConsentPrompts**, **privacyBlockInputPersonalization**, **startMenuHideChangeAccountSettings**, **startMenuHideHibernate**, **startMenuHideLock**, **startMenuHideShutDown**, **startMenuHideSignOut**, **startMenuHideSleep**, **startMenuHideSwitchAccount**, **settingsBlockAppsPage**, **settingsBlockGamingPage**, **windowsSpotlightBlockConsumerSpecificFeatures**, **windowsSpotlightBlocked**, **windowsSpotlightBlockOnActionCenter**, **windowsSpotlightBlockTailoredExperiences**, **windowsSpotlightBlockThirdPartyNotifications**, **windowsSpotlightBlockWelcomeExperience**, **windowsSpotlightBlockWindowsTips**, **windowsSpotlightConfigureOnLockScreen** и **connectedDevicesServiceBlocked** для объекта [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration).|
|Изменение|Бета|Удалены свойства **automaticUpdateMode**, **automaticUpdateSchedule**, **automaticUpdateTime**, **prereleaseFeatures**, **experienceBlockWindowsSpotlight**, **experienceBlockWindowsTips** и **experienceBlockConsumerSpecificFeatures** для объекта [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration).|
|Изменение|Бета|Добавлено свойство **subjectAlternativeNameFormatString** для объекта [windows10PkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10pkcscertificateprofile).|
|Изменение|Бета|Добавлены свойства **subjectNameFormatString** и **subjectAlternativeNameFormatString** для объекта [windows81SCEPCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81scepcertificateprofile).|
|Изменение|Бета|Добавлены свойства **indexingEncryptedStoresOrItemsBlocked** и **smbAutoEncryptedFileExtensions** для объекта [windowsInformationProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection).|
|Изменение|Бета|Изменены следующие свойства объекта [windowsInformationProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection):<br/>свойство **rightsManagementServicesTemplateId** сделано необязательным.<br/>|
|Изменение|Бета|Изменены следующие свойства объекта [windowsMobileMSI](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi):<br/>свойство **productCode** сделано необязательным.<br/>|
|Изменение|Бета|Добавлены свойства **subjectNameFormatString** и **subjectAlternativeNameFormatString** для объекта [windowsPhone81SCEPCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81scepcertificateprofile).|
|Изменение|Бета|Добавлено свойство навигации **mobileAppConfigurations** для объекта [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement).|
|Изменение|Бета|Для объекта [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) добавлены свойства **cartToClassAssociations**, **deviceCompliancePolicySettingStateSummaries**, **remoteAssistancePartners**, **windowsInformationProtectionAppLearningSummaries** и **windowsMalwareInformation**|
|Изменение|Бета|Добавлены свойство навигации **eBook** для объекта [eBookGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_ebookgroupassignment).|
|Изменение|Бета|Добавлено свойство навигации **windowsProtectionState** для объекта [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice).|
|Изменение|Бета|Добавлено свойство навигации **installSummary** для объекта [managedEBook](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_managedebook).|
|Изменение|Бета|Удалено свойство навигации **outlook** для объекта [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_user).|
|Изменение|Бета|Удалено свойство навигации **healthStates** для объекта [windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapp).|
|Изменение|Бета|Добавлено свойство **androidForWorkRestrictions** для сложного типа [defaultDeviceEnrollmentRestrictions](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_defaultdeviceenrollmentrestrictions).|
|Изменение|Бета|Добавлены свойства **userPrincipalName** и **sources** для сложного типа [deviceCompliancePolicySettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate).|
|Изменение|Бета|Добавлены свойства **userPrincipalName** и **sources** для сложного типа [deviceConfigurationSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate).|
|Изменение|Бета|Для сложного типа [deviceConfigurationSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) добавлены свойства **settingName**, **userId**, **userName**, **userEmail** и **currentValue**|
|Изменение|Бета|Удалено свойство **archiveFolder** для сложного типа [mailboxSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/mailboxSettings).|


### <a name="outlook-calendar"></a>Календарь Outlook

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|1.0 и бета-версия|Для метода **findMeetingTimes** добавлено значение перечисления **unrestricted**, указываемое в качестве свойства **activityDomain** в составе параметра **timeConstraint**. Это позволяет методу **findMeetingTimes** искать интервалы времени, соответствующие типу планируемого мероприятия. Дополнительные сведения см. в разделе [request body](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_findmeetingtimes#request-body).|
|Дополнение|Бета-версия|Содержание объекта **event** теперь можно получать в виде обычного текста, а не только в формате HTML. Дополнительные сведения см. в описаниях событий [get](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/event_get) и [list](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_list_events).|

### <a name="outlook-mail"></a>Почта Outlook

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Изменение|Бета-версия|Содержание объекта **message** теперь можно получать в виде обычного текста, а не только в формате HTML. Дополнительные сведения см. в описаниях событий [get](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/message_get) и [list](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_list_messages).|


### <a name="outlook-tasks"></a>Задачи Outlook

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|Бета|В объект [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/user) добавлено новое свойство навигации **outlook** для доступа к задачам Outlook.|
|Дополнение|Бета|Новые объекты [outlookuser](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/outlookuser), [outlookTaskGroup](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/outlooktaskgroup), [outlookTaskFolder](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/outlooktaskfolder) и [outlookTask](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/outlooktask), а также их методы поддерживают доступ к задачам Outlook. | 
|Дополнение|Бета|Задачи Outlook поддерживают вложения (ресурсы [attachment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/attachment), [fileAttachment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/fileattachment), [itemAttachment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/itemattachment) и [referenceAttachment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/referenceattachment)). |
|Дополнение|Бета|Задачи Outlook поддерживают [расширенные свойства](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/extended-properties-overview) (ресурсы [singleValueLegacyExtendedProperty](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/singlevaluelegacyextendedproperty) и [multiValueLegacyExtendedProperty](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/multivaluelegacyextendedproperty)). |

### <a name="planner-apis"></a>API Планировщика

|**Тип изменения**|**Версия**|**Описание**| 
|:-------------|:-----------|:--------------|
|Дополнение|1.0|Добавлен [API Планировщика](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/planner_overview).<br />Новые ресурсы:<br />[plannerPlan](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerPlan); <br />[plannerTask](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerTask); <br />[plannerPlanDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerPlanDetails); <br />[plannerTaskDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerTaskDetails); <br />[plannerBucket](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerBucket); <br />[plannerAssignedToTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerassignedtotaskboardtaskformat); <br />[plannerBucketTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerbuckettaskboardtaskformat); <br />[plannerProgressTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerprogresstaskboardtaskformat) | 

### <a name="sharepoint-sites"></a>Сайты SharePoint

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:----------|:--------------|
| Дополнение      | 1.0      | Теперь в конечной точке версии 1.0 доступен ресурс сайтов.<br/> Добавлены типы ресурсов **site** и **siteCollection**.
| Изменение        | Бета      | Изменился формат идентификатора ресурса **site**. Это критическое изменение в бета-версии API.
| Удаленные элементы       | Бета      | Объект **sharePoint** удален из бета-версии API. Эта функциональность теперь доступна из коллекции **sites**.

### <a name="sharepoint-lists"></a>Списки SharePoint

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:----------|:--------------|
| Изменение | Бета | Удалены свойства навигации **sharepoint**. Теперь для доступа к сайтам используется свойство навигации **sites**. <br/> Удален ресурс **fieldDefinition**. Он заменен ресурсом **columnDefinition**. <br/> Удалены свойства **siteCollectionId** и **siteId** объекта **site**. Используйте вместо них свойство **sharepointIds**. <br/> Удалено свойство **listItemId** объекта **listItem**. Используйте вместо него свойство **sharepointIds**. <br/> Свойство **columnSet** объекта **listItem** переименовано на **fields**. <br/> Идентификаторы ресурсов **site** теперь включают имя узла SharePoint.
| Дополнение | Бета | Добавлены типы ресурсов **booleanColumn**, **calculatedColumn**, **choiceColumn**, **dateTimeColumn**, **lookupColumn**, **numberColumn**, **personOrGroupColumn** и **textColumn**. <br/> В объект **site** добавлено свойство **displayName**. <br/> В объект **site** добавлено свойство навигации **columns**. <br/> В объект **sharedDriveItem** добавлены свойства навигации **list** и **listItem**. <br/> В объекты **list**, **listItem** и **site** добавлено свойство **sharepointIds**. <br/> Добавлен тип ресурса **columnDefinition**.




## <a name="april-2017"></a>Апрель 2017 г.

### <a name="administrative-units-property-changes"></a>Изменения свойств административных единиц

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Изменение|Бета-версия| Обновления API административных единиц будут предоставлены в бета-версиях. Первый набор изменений будет применен 3 мая 2017 г. Изменения включают в себя следующие переименования:<br />сложный тип - **roleMemberInfo** для объекта scopedRoleMembership теперь зовется **identity**;<br />свойство навигации - **scopedAdministratorOf** для объекта user теперь зовется **scopedRoleMemberOf**;<br />свойство навигации - **scopedAdministrators** для объекта administrativeUnit теперь зовется **scopedRoleMembers**;<br />свойство навигации - **scopedAdministrators** для объекта directoryRole теперь зовется **scopedMembers**. |

### <a name="application-and-serviceprincipal-api-changes"></a>Изменения в API application и servicePrincipal

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Изменение|Бета-версия| API [application](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/application) и [servicePrincipal](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/serviceprincipal) будут обновлены в бета-версии. Первый набор изменений будет применен 15 мая 2017 г. Изменения включают переименование и реструктуризацию свойств. Некоторые свойства (например, appRoles и addIns) будут доступны только после применения изменений. Прежде чем выйдет версия 1.0 с изменениями, будут выпущены бета-версии. |

### <a name="added-preview-support-for-cloud-solution-provider-developers"></a>Добавлена поддержка бета-версий для разработчиков, присоединившихся к программе Cloud Solution Provider

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|Бета-версия|Приложения, разрешение на использование которых было заранее предоставлено согласно программе Cloud Solution Provider, теперь могут вызывать Microsoft Graph. Описание см. в новой [статье об авторизации](https://graph.microsoft.io/en-us/docs/concepts/auth_cloudsolutionprovider). |

### <a name="added-onpremises-properties-to-user-entity"></a>Добавлены свойства onPremises к объекту user

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|Бета-версия|К объекту [user](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/user) добавлены новые свойства для onPremises: onPremisesDomainName, OnPremisesSamAccountName и onPremisesUserPrincipalName. |

### <a name="new-planner-apis-and-an-update-to-the-group-visibility-property"></a>Новые API Планировщика и обновление свойства видимости группы

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Изменение|Бета-версия|Добавлено значение **HiddenMembership** для свойства видимости объекта [Group](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/group). |
|Дополнение|Бета-версия|Добавлен новый [API Планировщика](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/planner_overview).<br />Новые ресурсы:<br />[plannerPlan](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerPlan); <br />[plannerTask](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerTask); <br />[plannerPlanDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerPlanDetails); <br />[plannerTaskDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerTaskDetails); <br />[plannerBucket](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerBucket); <br />[plannerAssignedToTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerassignedtotaskboardtaskformat); <br />[plannerBucketTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerbuckettaskboardtaskformat); <br />[plannerProgressTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerprogresstaskboardtaskformat). | 

### <a name="intune-apis"></a>API Intune
|**Тип изменения**|**Версия**|**Описание**|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidForWorkCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkcompliancepolicy);<br/>[deviceComplianceSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate);<br/>[deviceInstallState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_deviceinstallstate);<br/>[deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscript)<br/>[deviceManagementScriptGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscriptgroupassignment)<br/>[deviceManagementScriptState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscriptstate)<br/>[eBookGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_ebookgroupassignment);<br/>[iosVppEBook](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_iosvppebook);<br/>[managedEBook](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_managedebook);<br/>[userInstallStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_userinstallstatesummary);<br/>[windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapp)<br/>[windowsManagementAppHealthState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapphealthstate)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[dailySchedule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_dailyschedule)<br/>[hourlySchedule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_hourlyschedule)<br/>[iosBookmark](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosbookmark);<br/>[iosWebContentFilterAutoFilter](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterautofilter);<br/>[iosWebContentFilterBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterbase);<br/>[iosWebContentFilterSpecificWebsitesAccess](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterspecificwebsitesaccess);<br/>[runSchedule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_runschedule)<br/>[sharedAppleDeviceUser](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedappledeviceuser)<br/>[windows10NetworkProxyServer](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10networkproxyserver).<br/>|
|Дополнение|Бета-версия|Добавлено действие [requestRemoteAssistance](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_requestremoteassistance) к объекту [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
|Дополнение|Бета-версия|Добавлено действие [cleanWindowsDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_cleanwindowsdevice) к объекту [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
|Дополнение|Бета-версия|Добавлено действие [logoutSharedAppleDeviceActiveUser](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_logoutsharedappledeviceactiveuser) к объекту [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
|Дополнение|Бета-версия|Добавлено действие [deleteUserFromSharedAppleDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_deleteuserfromsharedappledevice) к объекту [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
|Дополнение|Бета-версия|Добавлено действие [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_devicemanagementscript_assign) к объекту [deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscript). |
|Дополнение|Бета-версия|Добавлено действие [syncLicenses](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_onboarding_applevolumepurchaseprogramtoken_synclicenses) к объекту [appleVolumePurchaseProgramToken](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_applevolumepurchaseprogramtoken). |
|Дополнение|Бета-версия|Добавлена функция **getTopMobileApps** для коллекции [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp). |
|Дополнение|Бета-версия|Добавлена функция [downloadApplePushNotificationCertificateSigningRequest](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest) к объекту [applePushNotificationCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_applepushnotificationcertificate). |
|Дополнение|Бета-версия|Добавлена функция [getDeviceComplianceSettingStates](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_devicemanagement_getdevicecompliancesettingstates) к объекту [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement). |
|Дополнение|Бета-версия|Добавлена функция [deviceConfigurationUserActivity](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity) к объекту [reportRoot](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_reportroot). |
|Дополнение|Бета-версия|Добавлена функция [deviceConfigurationDeviceActivity](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity) к объекту [reportRoot](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_reportroot). |
|Удаление|Бета-версия|Удалены следующие сложные типы:<br/>**enterpriseCloudResource**;<br/>**windowsInformationProtectionAppRule**;<br/>**windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate**;<br/>**windowsInformationProtectionAppRuleDesktopTemplate**;<br/>**windowsInformationProtectionAppRuleStoreAppTemplate**;<br/>**windowsInformationProtectionAppRuleTemplate**;<br/>**windowsInformationProtectionCorporateNetworkLocation**;<br/>**windowsInformationProtectionProtectedLocation**;<br/>**windowsInformationProtectionProtectedLocationEnterpriseCloudResources**;<br/>**windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers**;<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges**;<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges**;<br/>**windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames**;<br/>**windowsInformationProtectionProtectedLocationEnterpriseProxyServers**;<br/>**windowsInformationProtectionProtectedLocationNeutralResources**.<br/>|
|Изменение|Бета-версия|Добавлено свойство **deviceSharingAllowed** к объекту [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration).|
|Изменение|Бета-версия|Удалено **deviceSharingBlocked** свойство из объекта [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration).|
|Изменение|Бета-версия|Добавлено свойство **minimumRequiredSdkVersion** к объекту [defaultManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection).|
|Изменение|Бета-версия|Добавлено свойство **windowsManagementAppEnabled** к объекту [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement).|
|Изменение|Бета-версия|Добавлено свойство **notificationTemplateId** к объекту [deviceComplianceActionItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceactionitem).|
|Изменение|Бета-версия|Добавлено свойство **excludeGroup** к объекту [deviceConfigurationGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationgroupassignment)|
|Изменение|Бета-версия|Изменены следующие свойства объекта [iosCustomConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscustomconfiguration):<br/>**payloadFileName** теперь можно не указывать.<br/>|
|Изменение|Бета-версия|Добавлено свойство **contentFilterSettings** к объекту [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration).|
|Изменение|Бета-версия|Добавлены свойства **cellularBlockPersonalHotspot** и **passcodeBlockFingerprintModification** к объекту [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration).|
|Изменение|Бета-версия|Добавлено свойство **minimumRequiredSdkVersion** к объекту [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection).|
|Изменение|Бета-версия|Изменены следующие свойства объекта [macOSCustomConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscustomconfiguration):<br/>**payloadFileName** теперь можно не указывать.<br/>|
|Изменение|Бета-версия|Добавлены свойства **disableAppPinIfDevicePinIsSet**, **minimumRequiredOsVersion**, **minimumWarningOsVersion**, **minimumRequiredAppVersion** и **minimumWarningAppVersion** к объекту [managedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedappprotection).|
|Изменение|Бета-версия|Добавлены свойства **remoteAssistanceSessionUrl**, **isEncrypted**, **model** и **manufacturer** к объекту [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice).|
|Изменение|Бета-версия|Изменены следующие свойства объекта [getMobileAppCount](https://developer.microsoft.com/en-us/graph/docs/docs/api-reference/beta/api/intune_apps_mobileapp_getmobileappcount):<br/>для **bindingParameter** вместо **mobileApp** теперь используется **коллекция** *mobileApp*;<br/>для свойства **status** вместо типа GUID теперь используется String.<br/>|
|Изменение|Бета-версия|Добавлено свойство **vpnConfigurationId** к объекту [mobileAppGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappgroupassignment).|
|Изменение|Бета-версия|Удалено свойство **fromEmailAddress** из объекта [notificationMessageTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_notificationmessagetemplate).|
|Изменение|Бета-версия|Добавлено свойство **excludedApps** к объекту [officeSuiteApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp).|
|Изменение|Бета-версия|Удалено свойство **excludedOfficeApps** из объекта [officeSuiteApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp).|
|Изменение|Бета-версия|Добавлено свойство **enabled** к объекту [sharedPCConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcconfiguration).|
|Изменение|Бета-версия|Добавлены свойства **networkProxyApplySettingsDeviceWide**, **networkProxyDisableAutoDetect**, **networkProxyAutomaticConfigurationUrl**, **networkProxyServer**, **bluetoothDeviceName**, **wiFiScanInterval**, **wirelessDisplayBlockProjectionToThisDevice**, **wirelessDisplayBlockUserInputFromReceiver**, **wirelessDisplayRequirePinForPairing**, **experienceBlockDeviceDiscovery**, **experienceBlockErrorDialogWhenNoSIM**, **experienceBlockTaskSwitcher**, **startMenuPinnedFolderDocuments**, **startMenuPinnedFolderDownloads**, **startMenuPinnedFolderFileExplorer**, **startMenuPinnedFolderHomeGroup**, **startMenuPinnedFolderMusic**, **startMenuPinnedFolderNetwork**, **startMenuPinnedFolderPersonalFolder**, **startMenuPinnedFolderPictures**, **startMenuPinnedFolderSettings**, **startMenuPinnedFolderVideos**, **startMenuAppListVisibility**, **startMenuHideFrequentlyUsedApps**, **startMenuHideRecentJumpLists**, **startMenuHideRecentlyAddedApps**, **startMenuHideRestartOptions**, **startMenuHideUserTile**, **startMenuHidePowerButton**, **startMenuLayoutEdgeAssetsXml**, **personalizationDesktopImageUrl** и **personalizationLockScreenImageUrl** к объекту [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration).|
|Изменение|Бета-версия|Изменен тип следующих свойств объекта [windowsMobileMSI](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi):<br/>**productCode** теперь относится не к Guid, а к String.<br/>|
|Изменение|Бета-версия|Изменены следующие свойства объекта [windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx):<br/>**phoneProductIdentifier** больше не обязательно указывать;<br/>**phonePublisherId** больше не обязательно указывать.<br/>|
|Изменение|Бета-версия|Изменены следующие свойства объекта [windowsPhone81AppXBundle](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appxbundle):<br/>**appXPackageInformationList** больше не обязательно указывать.<br/>|
|Изменение|Бета-версия|Добавлены свойства **productKey** и **licenseType** к объекту [windowsStoreForBusinessApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessapp).|
|Изменение|Бета-версия|Добавлено свойство **previewBuildSetting** к объекту [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration).|
|Изменение|Бета-версия|Добавлены свойства навигации **windowsManagementApp** и **managedEBooks** к объекту [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement).|
|Изменение|Бета-версия|Добавлены свойства навигации **deviceManagementScripts**, **managedDeviceOverview** и **cloudPkiSubscriptions** к объекту [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement).|
|Изменение|Бета-версия|Добавлены свойства **osMinimumVersion** и **osMaximumVersion** к сложному типу [deviceEnrollmentPlatformRestrictions](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_deviceenrollmentplatformrestrictions).|
|Изменение|Бета-версия|Добавлены свойства **isSharedDevice** и **sharedDeviceCachedUsers** к сложному типу [hardwareInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_hardwareinformation).|
|Изменение|Бета-версия|Изменены следующие свойства сложного типа [omaSettingBase64](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_omasettingbase64):<br/>**fileName** больше не обязательно указывать.<br/>|
|Изменение|Бета-версия|Изменены следующие свойства сложного типа [omaSettingStringXml](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_omasettingstringxml):<br/>**fileName** больше не обязательно указывать.<br/>|

## <a name="march-2017"></a>Март 2017 г.

### <a name="intune-apis"></a>API Intune

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidForWorkApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidforworkapp);<br/>[androidForWorkAppConfigurationSchema](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationschema);<br/>[androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings);<br/>[androidForWorkVpnConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkvpnconfiguration);<br/>[applePushNotificationCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_applepushnotificationcertificate)<br/>[complianceSettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_compliancesettingstatesummary);<br/>[deviceCompliancePolicyDeviceStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary);<br/>[deviceCompliancePolicyState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicystate);<br/>[deviceConfigurationDeviceStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatesummary);<br/>[deviceConfigurationState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationstate);<br/>[enterpriseCodeSigningCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_enterprisecodesigningcertificate);<br/>[iosEduDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosedudeviceconfiguration);<br/>[managedDeviceCertificateState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevicecertificatestate)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicesummary);<br/>[managedDeviceMobileAppConfigurationUserSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationusersummary);<br/>[mdmWindowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_mdmwindowsinformationprotectionpolicy);<br/>[mobileAppInstallSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallsummary);<br/>[mobileAppProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappprovisioningconfiggroupassignment);<br/>[mobileThreatDefenseConnector](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_mobilethreatdefenseconnector);<br/>[officeSuiteApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp);<br/>[settingStateDeviceSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_settingstatedevicesummary);<br/>[softwareUpdateStatusSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_softwareupdatestatussummary);<br/>[symantecCodeSigningCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_symanteccodesigningcertificate);<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration);<br/>[windowsInformationProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection);<br/>[windowsInformationProtectionAppLockerFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionapplockerfile);<br/>[windowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionpolicy);<br/>[windowsMobileMSI](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi).<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[androidForWorkAppConfigurationExample](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationexample);<br/>[androidForWorkAppConfigurationExampleJson](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationexamplejson);<br/>[androidForWorkAppConfigurationSchemaItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationschemaitem);<br/>[deviceCompliancePolicySettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate);<br/>[deviceConfigurationSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate);<br/>[deviceExchangeAccessStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceexchangeaccessstatesummary)<br/>[edgeSearchEngine](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchengine);<br/>[edgeSearchEngineBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchenginebase);<br/>[edgeSearchEngineCustom](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchenginecustom);<br/>[excludedApps](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_excludedapps);<br/>[iosEduCertificateSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducertificatesettings);<br/>[ipRange](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iprange);<br/>[windowsInformationProtectionApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionapp);<br/>[windowsInformationProtectionCloudResource](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioncloudresource);<br/>[windowsInformationProtectionCloudResourceCollection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioncloudresourcecollection);<br/>[windowsInformationProtectionDesktopApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondesktopapp);<br/>[windowsInformationProtectionIPRangeCollection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioniprangecollection);<br/>[windowsInformationProtectionResourceCollection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionresourcecollection);<br/>[windowsInformationProtectionStoreApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionstoreapp).<br/>|
|Дополнение|Бета-версия|Добавлено действие [requestSignupUrl](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_requestsignupurl) к объекту [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings). |
|Дополнение|Бета-версия|Добавлено действие [completeSignup](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_completesignup) к объекту [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings). |
|Дополнение|Бета-версия|Добавлено действие [syncApps](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_syncapps) к объекту [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings). |
|Дополнение|Бета-версия|Добавлено действие [unbind](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_unbind) к объекту [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings). |
|Дополнение|Бета-версия|Добавлено действие [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign) к объекту [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration). |
|Дополнение|Бета-версия|Добавлено действие [recoverPasscode](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_recoverpasscode) к объекту [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
|Дополнение|Бета-версия|Добавлено действие [removeApplePushNotificationCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_onboarding_organization_removeapplepushnotificationcertificate) к объекту [organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_organization). |
|Дополнение|Бета-версия|Добавлено действие [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_iosmanagedappprotection_updatemobileappidentifierdeployments) к объекту [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection). |
|Дополнение|Бета-версия|Добавлено действие [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_androidmanagedappprotection_updatemobileappidentifierdeployments) к объекту [androidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection). |
|Дополнение|Бета-версия|Добавлено действие [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_updatemobileappidentifierdeployments) к объекту [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration). |
|Дополнение|Бета-версия|Добавлено действие [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_iosmanagedappprotection_updatetargetedsecuritygroups) к объекту [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection). |
|Дополнение|Бета-версия|Добавлено действие [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_androidmanagedappprotection_updatetargetedsecuritygroups) к объекту [androidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection). |
|Дополнение|Бета-версия|Добавлено действие [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_windowsinformationprotection_updatetargetedsecuritygroups) к объекту [windowsInformationProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection). |
|Дополнение|Бета-версия|Добавлено действие [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_windowsinformationprotection_updatetargetedsecuritygroups) к объекту [windowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionpolicy). |
|Дополнение|Бета-версия|Добавлено действие [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_mdmwindowsinformationprotectionpolicy_updatetargetedsecuritygroups) к объекту [mdmWindowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_mdmwindowsinformationprotectionpolicy). |
|Дополнение|Бета-версия|Добавлено действие [wipeManagedAppRegistrationByDeviceTag](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_user_wipemanagedappregistrationbydevicetag) к объекту [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_user). |
|Дополнение|Бета-версия|Добавлена функция [getTopMobileApps](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_apps_mobileapp_gettopmobileapps) к объекту [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp). |
|Дополнение|Бета-версия|Добавлена функция [verifyWindowsEnrollmentAutoDiscovery](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_corpenrollment_devicemanagement_verifywindowsenrollmentautodiscovery) к объекту [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement). |
|Удаление|Бета-версия|Удалены следующие объекты:<br/>**appProvisioningConfigGroupAssignment**;<br/>**defaultManagedAppConfiguration**;<br/>**enterpriseCertificate**;<br/>**managedDeviceMobileAppProvisioningConfigurationDeviceStatus**;<br/>**symantecCertificate**;<br/>**windows10WindowsInformationProtectionConfiguration**.<br/>|
|Удаление|Бета-версия|Удалены следующие сложные типы:<br/>**mobileAppInstallSummary**;<br/>**windowsArchitecture**;<br/>**windowsDeviceType**.<br/>|
|Изменение|Бета-версия|Добавлено свойство **webBrowserBlockPopups** к объекту [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration).|
|Изменение|Бета-версия|Удалено свойство **webBrowserAllowPopups** из объекта [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration).|
|Изменение|Бета-версия|Добавлено свойство **appIdentifier** к объекту [androidStoreApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidstoreapp).|
|Изменение|Бета-версия|Удалены свойства **applicationCount**, **failedApplicationCount** и **appInstallFailures** из объекта [appReportingOverviewStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/appReportingOverviewStatus).|
|Изменение|Бета-версия|Добавлены свойства **sharedIPadMaximumUserCount** и **enableSharedIPad** к объекту [depEnrollmentProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_corpenrollment_depenrollmentprofile).|
|Изменение|Бета-версия|Добавлены свойства **shareTokenWithSchoolDataSyncService** и **lastSyncErrorCode** к объекту [depOnboardingSetting](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_deponboardingsetting).|
|Изменение|Бета-версия|Добавлены свойства **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** и **configurationVersion** к объекту [deviceComplianceDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview).|
|Изменение|Бета-версия|Удалены свойства **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** и **policyRevision** из объекта [deviceComplianceDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview).|
|Изменение|Бета-версия|Добавлены свойства **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** и **configurationVersion** к объекту [deviceComplianceUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview).|
|Изменение|Бета-версия|Удалены свойства **numberOfPendingUsers**, **numberOfSucceededUsers**, **numberOfErrorUsers**, **numberOfFailedUsers**, **lastUpdateTime** и **policyRevision** из объекта [deviceComplianceUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview).|
|Изменение|Бета-версия|Добавлены свойства **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** и **configurationVersion** к объекту [deviceConfigurationDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview).|
|Изменение|Бета-версия|Удалены свойства **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** и **policyRevision** из объекта [deviceConfigurationDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview).|
|Изменение|Бета-версия|Добавлены свойства **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** и **configurationVersion** к объекту [deviceConfigurationUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview).|
|Изменение|Бета-версия|Удалены свойства **numberOfPendingUsers**, **numberOfSucceededUsers**, **numberOfErrorUsers**, **numberOfFailedUsers**, **lastUpdateTime** и **policyRevision** из объекта [deviceConfigurationUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview).|
|Изменение|Бета-версия|Добавлено свойство **subscriptionState** к объекту [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement).|
|Изменение|Бета-версия|Добавлено свойство **managedEmailProfileRequired** к объекту [iosCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscompliancepolicy).|
|Изменение|Бета-версия|Добавлено свойство **appsSingleAppModeList** к объекту [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration).|
|Изменение|Бета-версия|Удалено свойство **appsSingleAppModeBundleIds** из объекта [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration).|
|Изменение|Бета-версия|Добавлено свойство **expirationDateTime** к объекту [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration).|
|Изменение|Бета-версия|Удалено свойство **expiration** из объекта [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration).|
|Изменение|Бета-версия|Добавлены свойства **passwordMinimumCharacterSetCount**, **osMinimumVersion**, **osMaximumVersion**, **deviceThreatProtectionEnabled**, **deviceThreatProtectionRequiredSecurityLevel** и **storageRequireEncryption** к объекту [macOSCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscompliancepolicy).|
|Изменение|Бета-версия|Удалено свойство **manifest** из объекта [managedAndroidLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp).|
|Изменение|Бета-версия|Добавлены свойства **isSupervised**, **exchangeLastSuccessfulSyncDateTime**, **exchangeAccessState** и **exchangeAccessStateReason** к объекту [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice).|
|Изменение|Бета-версия|Добавлено свойство **deviceExchangeAccessStateSummary** к объекту [managedDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddeviceoverview).|
|Изменение|Бета-версия|Удалено свойство **manifest** из объекта [managedIOSLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp).|
|Изменение|Бета-версия|Удалено свойство **installSummary** из объекта [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp).|
|Изменение|Бета-версия|Добавлено свойство **uploadState** к объекту [mobileAppContentFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile).|
|Изменение|Бета-версия|Изменены следующие свойства объекта [mobileAppContentFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile):<br/>**azureStorageUriExpirationDateTime** больше не обязательно указывать.<br/>|
|Изменение|Бета-версия|Добавлены свойства **initiatedByUserPrincipalName**, **deviceOwnerUserPrincipalName**, **deviceIMEI** и **actionState** к объекту [remoteActionAudit](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_remoteactionaudit).|
|Изменение|Бета-версия|Добавлены свойства **oneDriveDisableFileSync**, **safeSearchFilter**, **edgeSearchEngine**, **settingsBlockSettingsApp**, **settingsBlockSystemPage**, **settingsBlockDevicesPage**, **settingsBlockNetworkInternetPage**, **settingsBlockPersonalizationPage**, **settingsBlockAccountsPage**, **settingsBlockTimeLanguagePage**, **settingsBlockEaseOfAccessPage**, **settingsBlockPrivacyPage**, **settingsBlockUpdateSecurityPage**, **experienceBlockWindowsSpotlight**, **experienceBlockWindowsTips**, **experienceBlockConsumerSpecificFeatures**, **startMenuLayoutXml**, **startMenuMode**, **logonBlockFastUserSwitching** и **startBlockUnpinningAppsFromTaskbar** к объекту [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration).|
|Изменение|Бета-версия|Добавлены свойства **allowPrinting**, **allowScreenCapture** и **allowTextSuggestion** к объекту [windows10SecureAssessmentConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration).|
|Изменение|Бета-версия|Удалены свойства **blockPrinting**, **blockScreenCapture** и **blockTextSuggestion** из объекта [windows10SecureAssessmentConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration).|
|Изменение|Бета-версия|Добавлено свойство **identityName** к объекту [windowsAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsappx).|
|Изменение|Бета-версия|Изменен тип следующих свойств объекта [windowsAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsappx):<br/>**applicableArchitectures** теперь относится не к [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture), а к String.<br/>|
|Изменение|Бета-версия|Добавлено свойство **identityName** к объекту [windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx).|
|Изменение|Бета-версия|Изменен тип следующих свойств объекта [windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx):<br/>**applicableArchitectures** теперь относится не к [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture), а к String.<br/>|
|Изменение|Бета-версия|Добавлены свойства **identityName**, **identityPublisherHash** и **identityResourceIdentifier** к объекту [windowsUniversalAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx).|
|Изменение|Бета-версия|Изменен тип следующих свойств объекта [windowsUniversalAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx):<br/>**applicableArchitectures** теперь относится не к [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture), а к String;<br/>**applicableDeviceTypes** теперь относится не к [windowsDeviceType](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsDeviceType), а к String.<br/>|
|Изменение|Бета-версия|Добавлено свойство **restartMode** к объекту [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration).|
|Изменение|Бета-версия|Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [androidForWorkScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile).|
|Изменение|Бета-версия|Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [androidScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidscepcertificateprofile).|
|Изменение|Бета-версия|Добавлены свойства навигации **enterpriseCodeSigningCertificates**, **symantecCodeSigningCertificate**, **sideLoadingKeys**, **managedAppPolicies**, **iosManagedAppProtections**, **androidManagedAppProtections**, **defaultManagedAppProtections**, **targetedManagedAppConfigurations**, **mdmWindowsInformationProtectionPolicies**, **windowsInformationProtectionPolicies**, **managedAppRegistrations** и **managedAppStatuses** к объекту [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement).|
|Изменение|Бета-версия|Удалены свойства навигации **appReportingOverview**, **enterpriseCerts** и **symantecCert** из объекта [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement).|
|Изменение|Бета-версия|Добавлено свойство навигации **deviceSettingStateSummaries** к объекту [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy).|
|Изменение|Бета-версия|Добавлено свойство навигации **deviceSettingStateSummaries** к объекту [deviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration).|
|Изменение|Бета-версия|Добавлены свойства навигации **termsAndConditions**, **androidForWorkSettings**, **androidForWorkAppConfigurationSchemas**, **applePushNotificationCertificate**, **softwareUpdateStatusSummary**, **deviceCompliancePolicyDeviceStateSummary**, **complianceSettingStateSummaries**, **deviceConfigurationDeviceStateSummaries** и **mobileThreatDefenseConnectors** к объекту [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement).|
|Изменение|Бета-версия|Удалены свойства навигации **teacherRootCertificates**, **teacherIdentityCertificate**, **studentRootCertificates** и **studentIdentityCertificate** из объекта [iosEducationDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration).|
|Изменение|Бета-версия|Изменен тип следующих свойств объекта [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration):<br/>**deviceStatuses** теперь относится не к коллекции [managedDeviceMobileAppProvisioningConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/managedDeviceMobileAppProvisioningConfigurationDeviceStatus), а к коллекции [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus).<br/>**groupAssignments** теперь относится не к коллекции [appProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/appProvisioningConfigGroupAssignment), а к коллекции [mobileAppProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappprovisioningconfiggroupassignment).<br/>|
|Изменение|Бета-версия|Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [iosScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosscepcertificateprofile).|
|Изменение|Бета-версия|Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [macOSScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosscepcertificateprofile).|
|Изменение|Бета-версия|Добавлены свойства навигации **deviceConfigurationStates** и **deviceCompliancePolicyStates** к объекту [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice).|
|Изменение|Бета-версия|Добавлены свойства навигации **deviceStatusSummary** и **userStatusSummary** к объекту [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration).|
|Изменение|Бета-версия|Добавлено свойство навигации **installSummary** к объекту [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp).|
|Изменение|Бета-версия|Удалено свойство навигации **sideLoadingKeys** из объекта [organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_organization).|
|Изменение|Бета-версия|Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [windows81SCEPCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81scepcertificateprofile).|
|Изменение|Бета-версия|Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [windowsPhone81SCEPCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81scepcertificateprofile).|
|Изменение|Бета-версия|Удалены свойства **applicationId**, **appName**, **platformId**, **userFailures** и **deviceFailures** из сложного типа [appInstallationFailure](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure).|
|Изменение|Бета-версия|Добавлено свойство **displayName** к сложному типу [iosHomeScreenFolderPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolderpage).|
|Изменение|Бета-версия|Добавлено свойство **displayName** к сложному типу [iosHomeScreenPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenpage).|
|Изменение|Бета-версия|Добавлены свойства **subjectName**, **description**, **expirationDateTime** и **certificate** к сложному типу [windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondatarecoverycertificate).|
|Изменение|Бета-версия|Удалены свойства **dataRecoveryCertificate** и **certificateFileName** из сложного типа [windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondatarecoverycertificate).|
|Изменение|Бета-версия|Добавлено свойство **displayName** к сложному типу [windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation).|
|Изменение|Бета-версия|Изменен тип следующих свойств сложного типа [windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation):<br/>**applicableArchitecture** теперь относится не к [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture), а к String.<br/>|
|Изменение|Бета-версия|Изменены следующие свойства сложного типа [windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation):<br/>свойство **applicableArchitecture** сделано обязательным.<br/>|

### <a name="add-contracts-to-microsoft-graph"></a>Добавление контрактов в Microsoft Graph

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|Бета-версия|Новый ресурс:</br>[contract](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/contract). |

### <a name="add-domain-operations-to-microsoft-graph"></a>Добавление операций с доменами в Microsoft Graph

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|Бета-версия|Добавлены функции к объектам [domain](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domain).<br/>Новые объекты:</br>[domain](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domain);<br/>[domainDnsRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domaindnsrecord);<br/>[domainDnsCnameRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsCnameRecord);<br/>[domainDnsMxRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsMxRecord);<br/>[domainDnsSrvRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsSrvRecord);<br/>[domainDnsTxtRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsTxtRecord);<br/>[domainDnsUnavailableRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsUnavailableRecord).<br/>Новые действия:</br>[forceDelete](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/domain_forcedelete);</br>[verify](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/domain_verify). |

### <a name="add-custom-data-to-microsoft-graph-using-schema-extensions"></a>Добавление пользовательских данных в Microsoft Graph с помощью расширений схемы

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|Бета|Добавление данных приложения в Microsoft Graph с помощью [расширений схемы](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_overview#schema-extensions-preview)  поддерживается для следующих ресурсов:<br/>administrative unit;<br/>calendar event;<br/>device;<br/>group;<br/>message;<br/>organization;<br/>personal contact;<br/>post;<br/>user.<br/>Пример приведен в следующей статье:<br/>[Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_schema_groups).|
|Дополнение|Бета|Предоставлен альтернативный способ создания определения расширения схемы без подтвержденного личного домена .com. Подробности см. в разделе [Расширения схемы](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_overview#schema-extensions-preview).|

### <a name="add-custom-data-to-microsoft-graph-using-open-extensions"></a>Добавление пользовательских данных в Microsoft Graph с помощью открытых расширений

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Изменение| 1.0 и бета-версия | Вместо термина "расширения данных Office 365" теперь используется "открытые расширения". |
|Дополнение|Бета-версия|Добавлены ресурсы, которые поддерживают [открытые расширения](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_overview#open-extensions): <br/>administrative unit;<br/>device;<br/>group;<br/>organization;<br/>user.<br/>Пример приведен в следующей статье:<br/>[Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_open_users).|

### <a name="directory-apis"></a>API каталогов

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|Бета-версия|Добавлена поддержка [восстановления и окончательного удаления групп](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/directory).<br/>Новый объект: каталог со свойством навигации deleteditems. |
|Дополнение|Бета|Новый объект:</br>[Конечная точка](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/endpoint) |
|Изменение  |Бета|Новое свойство навигации [endpoints](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/group_list_endpoints) для ресурса [group](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/group) |
|Дополнение|Бета|Новый объект:</br>[licenseDetails](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/licensedetails) |
|Изменение  |Бета|Добавлено свойство навигации [licensedetails](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/user_list_licensedetails) для объекта [user](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/user). |

### <a name="reports-apis"></a>API отчетов

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|Бета|Представлена предварительная версия нового API для функций создания отчетов в Office 365. С его помощью можно получать отчеты об использовании служб Office 365 сотрудниками компании. Например, вы можете определить, кто использует службу по максимуму, а кому вообще не нужна лицензия Office 365. Дополнительные сведения см. в статье о ресурсе [report](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/report).|

### <a name="directory-apis"></a>API каталогов

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|Бета|Новый объект:</br>[contract](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/contract). |

## <a name="february-2017"></a>Февраль 2017 г.

### <a name="intune-apis"></a>API Intune

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidForWorkCertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkcertificateprofilebase)<br/>[androidForWorkEasEmailProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkeasemailprofilebase)<br/>[androidForWorkEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkenterprisewificonfiguration)<br/>[androidForWorkGmailEasConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkgmaileasconfiguration)<br/>[androidForWorkNineWorkEasConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworknineworkeasconfiguration)<br/>[androidForWorkPkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkpkcscertificateprofile)<br/>[androidForWorkScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile)<br/>[androidForWorkTrustedRootCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworktrustedrootcertificate)<br/>[androidForWorkWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkwificonfiguration)<br/>[appleDeviceFeaturesConfigurationBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_appledevicefeaturesconfigurationbase)<br/>[appProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appprovisioningconfiggroupassignment)<br/>[deviceComplianceUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview)<br/>[deviceConfigurationUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview)<br/>[enterpriseCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_enterprisecertificate)<br/>[iosEducationDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)<br/>[macOSDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosdevicefeaturesconfiguration)<br/>[managedAndroidLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp)<br/>[managedDeviceMobileAppProvisioningConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappprovisioningconfigurationdevicestatus)<br/>[managedIOSLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp)<br/>[managedMobileLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedmobilelobapp)<br/>[symantecCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_symanteccertificate)<br/>[windowsAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsappx)<br/>[windowsCertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowscertificateprofilebase)<br/>[windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx)<br/>[windowsPhone81AppXBundle](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appxbundle)<br/>[windowsPhoneXAP](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphonexap)<br/>[windowsUniversalAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[airPrintDestination](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_airprintdestination)<br/>[windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsarchitecture)<br/>[windowsDeviceType](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsdevicetype)<br/>[windowsMinimumOperatingSystem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsminimumoperatingsystem)<br/>[windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation)<br/>|
|Дополнение|Бета|Добавлено действие [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign) к объекту [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration).|
|Дополнение|Бета|Добавлено действие [scheduleActionsForRules](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_devicecompliancepolicy_scheduleactionsforrules) к объекту [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy).|
|Дополнение|Бета|Добавлено действие [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_updatetargetedsecuritygroups) к объекту [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration).|
|Дополнение|Бета|Добавлена функция [getScopesForUser](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_rbac_resourceoperation_getscopesforintune_devices_user) к объекту [resourceOperation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_rbac_resourceoperation).|
|Изменение|Бета|Удалено свойство **manifest** из объекта [androidLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidlobapp).|
|Изменение|Бета|Добавлены свойства **assetTagTemplate**, **lockScreenFootnote**, **homeScreenDockIcons** и **homeScreenPages** к объекту [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration).|
|Изменение|Бета|Удалены свойства **deviceSharingAssetTagInformation**, **deviceSharingLockScreenFootnote**, **homeScreenLayoutDockIcons** и **homeScreenLayoutPages** из объекта [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration).|
|Изменение|Бета|Добавлено свойство **appsSingleAppModeBundleIds** к объекту [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration).|
|Изменение|Бета|Удалено свойство **manifest** из объекта [iosLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobapp).|
|Изменение|Бета|Добавлены свойства **createdDateTime**, **description**, **lastModifiedDateTime**, **displayName** и **version** к объекту [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration).|
|Изменение|Бета|Добавлены свойства **createdDateTime** и **lastModifiedDateTime** к объекту [managedAppPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy).|
|Изменение|Бета|Удалено свойство **deviceRegistrationState** из объекта [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devices_manageddevice).|
|Изменение|Бета|Добавлено свойство **manifest** к объекту [mobileAppContentFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile).|
|Изменение|Бета|Добавлены свойства **osDescription** и **userName** к объекту [mobileAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus).|
|Изменение|Бета|Удалено свойство **deviceType** из объекта [mobileAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus).|
|Изменение|Бета|Изменен тип следующих свойств объекта [mobileAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus):<br/>**mobileAppInstallStatusValue** (с Int32 на String)|
|Изменение|Бета|Добавлены свойства **targetedSecurityGroupIds** и **targetedSecurityGroupsCount** к объекту [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration).|
|Изменение|Бета|Удалено свойство **numberOfTargetedSecurityGroups** из объекта [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration).|
|Изменение|Бета|Добавлено свойство **id** к объекту [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devices_user).|
|Изменение|Бета|Удалены свойства **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** и **certificateValidityPeriodScale** из объекта [windows10CertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10certificateprofilebase).|
|Изменение|Бета|Удалены свойства **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** и **certificateValidityPeriodScale** из объекта [windows81CertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81certificateprofilebase).|
|Изменение|Бета|Удалено свойство **applyToWindows10Mobile** из объекта [windowsPhone81GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81generalconfiguration).|
|Изменение|Бета|Добавлены свойства навигации **enterpriseCerts**, **iosLobAppProvisioningConfigurations** и **symantecCert** к объекту [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement).|
|Изменение|Бета|Добавлено свойство навигации **userStatusOverview** к объекту [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy).|
|Изменение|Бета|Добавлено свойство навигации **userStatusOverview** к объекту [deviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration).|
|Изменение|Бета|Добавлены свойства навигации **groupAssignments**, **deviceStatuses** и **userStatuses** к объекту [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration).|
|Изменение|Бета|Изменен тип следующих свойств объекта [windows10VpnConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10vpnconfiguration):<br/>**identityCertificate** (с [windows10CertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10certificateprofilebase) на [windowsCertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowscertificateprofilebase))|
|Изменение|Бета|Добавлены свойства **deviceComplianceCheckinThresholdDays** и **isScheduledActionEnabled** к сложному типу [deviceManagementSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings).|
|Изменение|Бета|Удалены свойства **windowsCommercialId** и **windowsCommercialIdLastModifiedTime** из сложного типа [deviceManagementSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings).|
|Изменение|Бета|Добавлены свойства **bundleID**, **appName**, **publisher**, **enabled** и **showOnLockScreen** к сложному типу [iosNotificationSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings).|
|Изменение|Бета|Удалены свойства **bundleIdentifier**, **notificationsEnabled** и **showInLockScreen** из сложного типа [iosNotificationSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings).|



## <a name="january-2017"></a>Январь 2017 г.

### <a name="outlook-calendar"></a>Календарь Outlook

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|v1.0|Новое действие [findMeetingTimes](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_findmeetingtimes) для ресурса [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user).|
|Дополнение|v1.0|Новый сложный тип [attendeeBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/attendeebase), который состоит из свойства типа участников.|
|Дополнение|v1.0|Новые сложные типы:<br/>[attendeeAvailability](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/attendeeavailability)<br/>[locationConstraint](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/locationconstraint) <br/>[locationConstraintItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/locationconstraintitem)<br/>[meetingTimeSuggestion](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/meetingtimesuggestion)<br/>[meetingTimeSuggestionsResult](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/meetingtimesuggestionsresult)<br/>[timeConstraint](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/timeconstraint)<br/>[timeSlot](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/timeslot)|
|Изменение|1.0|Сложный тип [attendee](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/attendee) теперь является производным от attendeeBase, который, в свою очередь, является производным от [recipient](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/recipient). Он состоит из тех же свойств **status**, **type** и **emailAddress**, что и раньше, а также унаследованных свойств.|
|Дополнение|Бета|В ресурс [calendar](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/calendar) добавлено свойство hexColor.|

### <a name="intune-apis"></a>API Intune

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|Бета|Добавлены новые объекты: <br/>[appReportingOverviewStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appreportingoverviewstatus)<br/>[deviceComplianceDeviceOverview](https://developer.microsoft.com/en-us/graph/docs//api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview)<br/>[deviceConfigurationDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview)<br/>[deviceManagementExchangeOnpremisesPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_devicemanagementexchangeonpremisespolicy)<br/>[iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)<br/>[iosEducationDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)<br/>[iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)<br/>[onpremisesConditionalAccessSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_onpremisesconditionalaccesssettings)<br/>[sharedPCConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcconfiguration)<br/>[windows10EnterpriseModernAppManagementConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration)<br/>[windows10SecureAssessmentConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration)<br/>[windows10WindowsInformationProtectionConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10windowsinformationprotectionconfiguration)|
|Дополнение|Бета|Добавлены новые сложные типы: <br/> [appInstallationFailure](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure)<br/>[enterpriseCloudResource](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_enterprisecloudresource)<br/>[iosHomeScreenApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenapp)<br/>[iosHomeScreenFolder](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolder)<br/>[iosHomeScreenFolderPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolderpage)<br/>[iosHomeScreenItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenitem)<br/>[iosHomeScreenPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenpage)<br/>[iosNotificationSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings)<br/>[iPv6Range](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ipv6range)<br/>[sharedPCAccountManagerPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcaccountmanagerpolicy)<br/>[windowsInformationProtectionAppRule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionapprule)<br/>[windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruleapplockerpolicyfiletemplate)<br/>[windowsInformationProtectionAppRuleDesktopTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruledesktoptemplate)<br/>[windowsInformationProtectionAppRuleStoreAppTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionapprulestoreapptemplate)<br/>[windowsInformationProtectionAppRuleTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruletemplate)<br/>[windowsInformationProtectionCorporateNetworkLocation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectioncorporatenetworklocation)<br/>[windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectiondatarecoverycertificate)<br/>[windowsInformationProtectionProtectedLocation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocation)<br/>[windowsInformationProtectionProtectedLocationEnterpriseCloudResources](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterprisecloudresources)<br/>[windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseinternalproxyservers)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseipv4ranges)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseipv6ranges)<br/>[windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterprisenetworkdomainnames)<br/>[windowsInformationProtectionProtectedLocationEnterpriseProxyServers](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseproxyservers)<br/>[windowsInformationProtectionProtectedLocationNeutralResources](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationneutralresources)
|Удаление|Бета|Следующие сложные типы удалены и заменены на тип microsoft.graph.Json:<br/>managedAppDeploymentSummary <br/>managedAppSummary<br /> |
|Изменение|Бета|Для следующих объектов тип свойства appConfigComplianceStatus заменен на complianceStatus: <br/>[managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus)<br/>[managedDeviceMobileAppConfigurationUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationuserstatus)|
|Изменение|Бета|Для ресурса [managedAppStatusRaw](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedappstatusraw) тип свойства content изменен с managedAppSummary на Json.|
|Изменение|Бета|Из коллекции [managedAppRegistration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedappregistration) удалена функция getUsersWithFlaggedAppRegistration.|
|Изменение|Бета|Изменено свойство навигации **vppToken** объекта [iosVppApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_iosvppapp), теперь он не является включенной коллекцией.|
|Изменение|Бета|Добавлено свойство **deviceStatusOverview** к объектам [deviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) и [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy).|
|Изменение|Бета|Добавлено свойство **appReportingOverview** к одиночному объекту [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement).|
|Изменение|Бета|Добавлены свойства **deviceDisplayName** и **userPrincipalName** к объектам [deviceConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus), [deviceComplianceDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus) и [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus).|
|Изменение|Бета|Добавлено свойство **ruleName** к объекту [deviceComplianceScheduledActionForRule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancescheduledactionforrule).|
|Изменение|Бета|Добавлены свойства **devicesCount**, **userDisplayName** и **userPrincipalName** к объектам [deviceConfigurationUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuserstatus), [deviceComplianceUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuserstatus) и [managedDeviceMobileAppConfigurationUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationuserstatus).|
|Изменение|Бета|Добавлена коллекция [notificationMessageTemplates](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_notification_notificationmessagetemplate) к одиночному объекту [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagement).|
|Изменение|Бета|Добавлены свойства **isDefault**, **lastModifiedDateTime**, **locale**, **messageTemplate** и **subject** к объекту [localizedNotificationMessage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_localizednotificationmessage).|
|Изменение|Бета|Добавлены свойства **azureActiveDirectoryDeviceId**, **deviceCategory**, **deviceRegistrationState** и **managementAgent** к объекту [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_manageddevice).|
|Изменение|Бета|Добавлено свойство **lastModifiedDateTime** к объекту [mobileAppCategory](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcategory).|
|Изменение|Бета|Добавлены свойства **brandingOptions**, **defaultLocale**, **displayName**, **fromEmailAddress**, **lastModifiedDateTime**, **localizedNotificationMessages** к объекту [notificationMessageTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_notification_notificationmessagetemplate).|
|Изменение|Бета|Добавлены свойства **appsAllowTrustedAppsSideloading**, **appsBlockWindowsStoreOriginatedApps**, **developerUnlockSetting**, **edgeBlockAccessToAboutFlags**, **edgeBlockDeveloperTools**, **edgeBlockExtensions**, **edgeBlockInPrivateBrowsing**, **edgeFirstRunUrl**, **edgeHomepageUrls**, **gameDvrBlocked**, **settingsBlockAddProvisioningPackage**, **settingsBlockChangeLanguage**, **settingsBlockChangePowerSleep**, **settingsBlockChangeRegion**, **settingsBlockChangeSystemTime**, **settingsBlockEditDeviceName**, **settingsBlockRemoveProvisioningPackage**, **sharedUserAppDataAllowed**, **smartScreenBlockPromptOverride**, **smartScreenBlockPromptOverrideForFiles**, **storageRestrictAppDataToSystemVolume**, **storageRestrictAppInstallToSystemVolume**, **webRtcBlockLocalhostIpAddress**, **windowsStoreBlockAutoUpdate** и **windowsStoreEnablePrivateStoreOnly** к объекту [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration).|

## <a name="december-2016"></a>Декабрь 2016 г.

### <a name="delta-query"></a>Запрос на получение различий

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|Бета|В следующие объекты добавлена новая функция delta для выполнения [запроса на получение различий](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_overview):<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Примеры см. в следующих статьях:<br/>[Получение добавочных изменений групп (предварительная версия)](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_groups)<br/>[Получение добавочных изменений сообщений в папке (предварительная версия)](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_messages)<br/>[Получение добавочных изменений пользователей (предварительная версия)](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_users)|

### <a name="excel-apis"></a>API Excel

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|v1.0|Добавлены ресурс workbookPivotTable, действия refresh и refreshAll в сводных таблицах, ресурс workbookRangeView, действие visibleView в отфильтрованном диапазоне для возврата workbookRangeView пользователю, коллекция строк get и ресурс range из visibleView, функции columnsAfter, columnsBefore, resizedRange, rowsAbove и rowsBelow из ресурса range и новые свойства таблицы.|

### <a name="intune-apis"></a>API Intune

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|Бета|Добавлены API ресурсов и методов для Microsoft Intune. Это большой набор ресурсов и методов для поддержки общедоступной предварительной версии Intune на портале Azure. Сведения о службе Intune см. в статье [Документация по Intune](https://go.microsoft.com/fwlink/?linkid=836405). Сведения о ресурсах и API Intune см. в разделе [Работа с Intune в Microsoft Graph](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_graph_overview).|

## <a name="october-2016"></a>Октябрь 2016 г.

### <a name="authorization-provider"></a>Поставщик услуг авторизации

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|1.0 и бета-версия|Конечная точка авторизации 2.0 теперь поддерживает тип предоставления OAuth client_credentials, который можно использовать для [процессов управляющей программы и длительных процессов в бизнес-сценариях](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-client-creds/).|
|Дополнение|1.0 и бета-версия|Конечная точка авторизации 2.0 теперь поддерживает [разрешения, требующие согласия администратора](http://developer.microsoft.com/en-us/graph/docs/concepts/permissions_reference) ([конечная точка предоставления согласия администратора](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#admin-restricted-scopes)).|
|Дополнение|1.0 и бета-версия|Конечная точка авторизации 2.0 теперь поддерживает согласие администратора для всех пользователей клиента ([конечная точка предоставления согласия администратора](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#admin-restricted-scopes)).|

### <a name="invitation-apis"></a>API приглашений

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|Бета-версия|Добавлено свойство invitedUserType к типу объекта приглашений, определяющее тип приглашаемого пользователя (**Guest** или **Member**).|
|Удаление|Бета|Мы удалим свойство invitedToGroups для типа объекта invitation 11 ноября 2016 г. Это значит, что вы больше не сможете добавить приглашаемого пользователя в группу с помощью этого API. Это можно будет сделать с помощью [API добавления членов](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/group_post_members).|

## <a name="september-2016"></a>Сентябрь 2016 г.

### <a name="azure-ad-application-proxy"></a>Прокси приложения Azure AD

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета|Теперь API Azure AD Application Proxy доступны в конечной точке Microsoft Graph бета-версии. Эти API позволяют безопасно публиковать локальные приложения для пользователей, находящихся за пределами корпоративной сети, используя Azure AD в качестве общей системы управления доступом. Опубликованные API позволяют создавать приложения, которые могут получать и обновлять различные аспекты прокси приложения, например параметры _connectors_, _connectorGroups_ и _onPremisesPublishing_ приложения.|

### <a name="drive"></a>Drive

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета-версия|Добавлена коллекция _shared_, благодаря которой можно получать доступ к общим элементам driveItem с помощью идентификатора shareId или URL-адреса для совместного доступа.|
|Дополнение|Бета-версия|Добавлена функция _search_ к объекту drive, которая позволяет искать элементы не только в корневой папке диска.|


### <a name="driveitem"></a>DriveItem

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета-версия|Добавлена поддержка элемента _createUploadSession_, который позволяет отправлять файлы размером более 4 МБ в OneDrive, OneDrive для бизнеса и библиотеки документов SharePoint.|
|Дополнение|Бета-версия|Добавлено свойство _sharepointIds_, которое возвращает традиционные идентификаторы API SharePoint для элементов driveItem, хранящихся в SharePoint.|
|Дополнение|Бета-версия|Добавлены дополнительные свойства для _remoteItem_.|
|Дополнение|Бета-версия|Добавлено значение _quickXorHash_ для файлов в OneDrive для бизнеса.|
|Дополнение|Бета-версия|Добавлена область для объекта _createSharingLink_, которая позволяет создавать ссылки для совместного доступа в компании или анонимного совместного доступа.|

### <a name="extended-properties"></a>Расширенные свойства

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0|Теперь [расширенные свойства](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/extended-properties-overview) поддерживаются в следующих ресурсах: message, mailFolder, event, calendar, contact, contactFolder, group event, group calendar, group post.|

### <a name="groups"></a>Группы

Добавлена поддержка динамического членства в группах с помощью общедоступной ознакомительной версии API, включая дополнения, указанные в таблице ниже.

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета-версия|Добавленное свойство **membershipRule** содержит правила, которые определяют членов динамической группы.|
|Дополнение|Бета-версия|Добавленное свойство **membershipRuleProcessingState** определяет, включено ли динамическое членство для этой группы.|
|Дополнение|Бета-версия|Присвойте свойству **groupTypes** значение **DynamicMembership**, чтобы включить динамическое членство для этой группы.|
|Дополнение|Бета-версия|Добавлено свойство **preferredLanguage**, которое указывает предпочитаемый язык для группы Office 365.|
|Дополнение|Бета-версия|Добавлено свойство **theme**, которое позволяет указать цветовую тему группы Office 365.|

### <a name="hybrid-deployment-support"></a>Поддержка гибридного развертывания

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0|Приложения могут использовать API Почты, Календаря и Контактов Outlook версии 1.0 для доступа к локальным почтовым ящикам в гибридном развертывании Exchange 2016 с накопительным пакетом обновления 3 (CU3). Дополнительные сведения о поддержке REST API см. в разделах, посвященных соответствующему [гибридному развертыванию](https://developer.microsoft.com/en-us/graph/docs/overview/hybrid_rest_support). **Примечание.** Если вы используете эти наборы API версии 1.0, то теперь ваши приложения (включая рабочие) будут работать с локальными почтовыми ящиками, которые соответствуют требованиям для гибридных развертываний. Доступна только предварительная версия этой возможности.|

### <a name="identityriskevents"></a>IdentityRiskEvents

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Изменение|Бета|В рамках изменения схемы, при котором тип двух свойств расположений будет заменен новым сложным типом в конечной точке identityRiskEvents, в конечной точке identityRiskEvents изменены или добавлены следующие свойства:</br>**location** теперь относится не к Edm.String, а к signInLocation ComplexType;<br/>**previousLocation** теперь относится не к Edm.String, а к signInLocation ComplexType;<br/>**signInLocation** — новый элемент ComplexType, содержащий свойства city, state, countryOrRegion и geoCoordinates;<br/>**geoCoordinates** — новый элемент ComplexType, содержащий свойства latitude и longitude.|

### <a name="invitation-manager"></a>Диспетчер приглашений

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета|Теперь API диспетчера приглашений доступны в конечной точке Microsoft Graph бета-версии. С помощью API диспетчера приглашений вы можете создать приглашение для добавления внешнего пользователя в организацию. Кроме того, при приглашении пользователя вы можете добавить его в группу Office 365. Дополнительные сведения см. в статье [о диспетчере приглашений](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/invitation).|

### <a name="onedrive"></a>OneDrive

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0|Добавлен метод **CreateUploadSession** для **driveItem**, который позволяет отправлять большие файлы и возобновлять отправку.|
|Дополнение|v1.0|Добавлены свойства для отслеживания идентификаторов SharePoint в элементах из SharePoint (**sharepointIds**) и свойство для идентификации корневых папок (**root**).|
|Дополнение|1.0|Добавлена корневая коллекция **Shares**, которую можно использовать с идентификаторами shareId или ссылками для совместного доступа к общим элементам в OneDrive и SharePoint. Возвращает новый тип — sharedDriveItem.|
|Дополнение|1.0|Добавлен метод **Invite** для driveItem, который позволяет добавлять разрешения для элементов. |
|Дополнение|1.0|Добавлен метод **Search** для drive, который позволяет искать элементы на диске, а также общие элементы. |
|Дополнение|1.0|Добавлено свойство **processingMetadata** для свойства quickXorHash сложного типа hashes. |
|Дополнение|1.0|Добавлено свойство **quickXorHash** к сложному типу hashes. |

### <a name="outlook-calendar"></a>Календарь Outlook

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0|Добавлено свойство **onlineMeetingUrl** к ресурсу [event](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/event).|
|Дополнение|Бета-версия|Добавлено действие [forward](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/event_forward) к ресурсу event.|
|Дополнение|Бета-версия|К ресурсу [calendar](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/calendar) добавлены свойства, c помощью которых можно предоставлять общий доступ к календарю: **canEdit**, **canShare**, **canViewPrivateItems**, **isShared**, **isShareWithMe** и **owner**.|

### <a name="outlook-mail"></a>Почта Outlook

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0|Добавлен сложный тип [mailboxSettings](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/mailboxsettings), который включает свойства **automaticRepliesSetting**, **timeZone** и **language**.|
|Дополнение|1.0|Добавлено свойство **mailboxSettings** к ресурсу [user](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user).|
|Дополнение|Бета|Добавлена возможность создавать, отображать, получать и удалять один или несколько экземпляров объекта [mention](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/mention) в сообщении. С помощью объектов mention можно привлечь внимание других пользователей в сообщении.|
|Дополнение|Бета|Добавлена поддержка действия [getMailTips](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_getmailtips) для получения подсказок для определенных получателей. Добавлены следующие ресурсы: automaticRepliesMailTips, mailTips, mailTipsError.|

### <a name="query-parameters"></a>Параметры запроса

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Изменение|Бета|С 26 сентября 2016 г. поддерживаются параметры запроса без префиксов $. Префикс $ в параметрах запроса не является обязательным. Дополнительные сведения см. в записи блога [Поддержка параметров запросов без префиксов $ в Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).|

### <a name="sharepoint"></a>SharePoint

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета-версия|Доступ к сайтам и спискам SharePoint [по идентификатору](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/list_get) или [URL-адресу](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/baseitem_getbyurl).|
|Дополнение|Бета-версия|Возможность [отображать, создавать, получать и удалять экземпляры объектов listItem](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/listitem).|

### <a name="users"></a>Пользователи

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета|Добавлено нередактируемое свойство **refreshTokensValidFromDateTime**, которое указывает дату и время начала действия токенов обновления или токенов сеанса. Все токены, выпущенные до этого времени, недействительны, а при попытке их использования потребуется повторный вход в систему.|
|Дополнение|Бета-версия|Добавлено свойство **showInAddressList**, указывающее, должен ли глобальный список адресов Outlook содержать этого пользователя.|
|Дополнение|Бета-версия|Добавлено служебное действие **invalidateAllRefreshTokens**, которое аннулирует все токены обновления и токены сеанса пользователя, выпущенные для приложений, сбрасывая значения свойства **refreshTokensValidFromDateTime** и указывая для него текущую дату и время.|


### <a name="webhooks"></a>Веб-перехватчики

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета|В веб-перехватчики добавлены корневые элементы Drive в качестве ресурса, доступного для подписки.|

## <a name="august-2016"></a>Август 2016 г.

### <a name="contacts"></a>Контакты

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета|В рамках изменения схемы, при котором удаляются несколько свойств и добавляются соответствующие коллекции в конечную точку contacts, в эту конечную точку добавлены следующие свойства: _Websites Collection(ComplexType: Website)_,_Phones Collection (ComplexType: Phone)_, _PostalAddress Collection(ComplexType: PhysicalAddress)_. Дополнительные сведения см. в записи блога [Предстоящие изменения API Контактов и Людей](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/).|
|Удаление|Бета|В рамках изменения схемы, при котором удаляются несколько свойств и добавляются соответствующие коллекции в конечную точку contacts, из этой конечной точки удалены следующие свойства: _BusinessHomePage_,_HomePhones_, _MobilePhone1_, _BusinessPhones_, _HomeAddress_, _BusinessAddress_, _OtherAddress_. Дополнительные сведения см. в записи блога [Предстоящие изменения API Контактов и Людей](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/).|

### <a name="excel-apis"></a>API Excel

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0|REST API Excel стал общедоступным в Microsoft Graph. Теперь вы можете обеспечить глубокую и сложную интеграцию с книгами Excel в Office 365. Дополнительные сведения см. в записи блога [Настройка использования REST API для Excel в приложениях с помощью Microsoft Graph](http://dev.office.com/blogs/power-your-apps-with-the-new-excel-rest-api).|

### <a name="people"></a>Люди

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Изменение|Бета|Свойство _WebSite_ переименовано на _Websites_. Дополнительные сведения см. в записи [Предстоящие изменения API Контактов и Людей](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/).|

### <a name="privileged-identity-management"></a>Управление привилегированными пользователями (PIM)

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета|Теперь REST API управления привилегированными пользователями доступны в конечной точке Microsoft Graph (бета-версия). [Управление привилегированными пользователями](https://azure.microsoft.com/en-us/documentation/articles/active-directory-privileged-identity-management-configure/) обеспечивает активацию "точно в срок" для привилегированных ролей в организации Azure AD, например ролей глобального администратора, администратора выставления счетов и т. д. C помощью опубликованных API разработчики могут создавать приложения, которые получают и обновляют привилегированные роли и активируют роли для пользователей. Дополнительные сведения см. в статьях [Microsoft Graph: доступна бета-версия API для Azure AD Privileged Identity Management](http://dev.office.com/blogs/microsoft-graph-azure-ad-privileged-identity-management-apis-beta) и [Azure AD Privileged Identity Management](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/privilegedidentitymanagement_root).|

## <a name="july-2016"></a>Июль 2016 г.

### <a name="administrative-units"></a>Административные единицы

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета|Представлен новый API Administrative Units (предварительная версия). Административные единицы позволяют организациям делить Azure Active Directory на подразделения и делегировать административные обязанности этим подразделениям. Подразделения могут представлять регионы, отделы, места возникновения затрат и т. д. Теперь ими можно управлять с помощью API Microsoft Graph.|

## <a name="june-2016"></a>Июнь 2016 г.

### <a name="identityriskevents"></a>IdentityRiskEvents

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета|Представлен новый API IdentityRiskEvents (предварительная версия). Этот API работает в сочетании с защитой идентификации Azure Active Directory. Его можно использовать для запрашивания событий рисков, созданных функцией защиты идентификации. Дополнительные сведения см. в статье [Знакомство с предварительной версией нового API в Microsoft Graph: IdentityRiskEvents](http://dev.office.com/blogs/identityriskevents-api-preview).

### <a name="subscriptions"></a>Подписки

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета-версия|Области, предназначенные только для приложений, теперь поддерживаются для подписок _mail_ и _contacts_.|

## <a name="may-2016"></a>Май 2016 г.

### <a name="calendar"></a>Календарь

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Существенные изменения|Бета|Изменения в API findMeetingTimes. Дополнительные сведения см. в записи блога [Обновление API findMeetingTimes в Microsoft Graph](http://dev.office.com/microsoft-graph-findmeetingtimes-api-update). Это изменение вступило в силу 19 мая 2016 г.

### <a name="contact"></a>Контакт

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0|Добавлен абстрактный тип _extensions_ для поддержки открытого типа openTypeExtension в OData версии 4.|

### <a name="directory"></a>Каталог

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Существенные изменения|Бета|Свойство _settingTemplateId_ теперь называется _templateId_. Это изменение вступило в силу 19 мая 2016 г.|

### <a name="event"></a>Событие

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0|Добавлен абстрактный тип _extensions_ для поддержки открытого типа openTypeExtension в OData версии 4.|

### <a name="eventmessages"></a>EventMessages

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0|Добавлены типы _inferenceClassification_ и _extensions_ к объекту _eventMessages_.|
|Дополнение|Бета-версия|Добавлено свойство _responseRequested_ к _eventMessageRequest_.|

### <a name="messages"></a>Сообщения

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0|Добавлены типы _inferenceClassification_ и _extensions_ к объекту _message_.|
|Дополнение|Бета-версия|Добавлено свойство _wellknownname_ к объекту _contactFolder_.|Изменения в API _findMeetingTimes_. Дополнительные сведения см. в записи блога [Обновление API findMeetingTimes в Microsoft Graph](http://dev.office.com/microsoft-graph-findmeetingtimes-api-update). Это изменение вступило в силу 19 мая 2016 г.|

### <a name="post"></a>Запись

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0|Добавлен абстрактный тип _extensions_ для поддержки открытого типа openTypeExtension в OData версии 4.|

### <a name="user"></a>User

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0|Добавлен тип ресурса _inferenceClassification_.|
|Дополнение|Бета-версия|Добавлено свойство _timeZone_ к типу _mailboxsettings_.|
|Дополнение|Бета-версия|Добавлен API _findMeetingTimes_ для объекта _user_.|

## <a name="april-2016"></a>Апрель 2016 г.

### <a name="general"></a>Общие

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0 и бета-версия|Теперь _Accept-Encoding:gzip_ может учитываться.|
|Дополнение|1.0|Добавлена поддержка сегмента приведения в пути expand. Например: "https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event"|
|Дополнение|Бета|Добавлена поддержка запроса PATCH для структурных свойств. Например: "PATCH /me/mailboxSettings"|
|Дополнение|Бета|Теперь Azure Active Directory используется в качестве резервного ресурса для запросов /beta/users/id/photo, когда приложению Outlook не удается обслужить запрос (например, когда у пользователя нет лицензии на почтовый ящик или у клиента нет подписки на Exchange Online). ПРИМЕЧАНИЕ. Этот резервный ресурс доступен и для запросов GET, и для запросов PATCH.|
|Дополнение|Бета|Добавлена поддержка сегмента приведения в пути expand. Например: "https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event"|

### <a name="onedrive"></a>OneDrive

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Исправление|v1.0|Устранена неисправность, из-за которой при выполнении запросов createLink в OneDrive возникала ошибка 500: "Неподдерживаемый тип свойства расширения".|

## <a name="march-2016"></a>Март 2016 г.

### <a name="calendar"></a>Календарь

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета-версия|Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_.|
|Дополнение|Бета-версия|Добавлено свойство _suggestionHint_ к _meetingTimeCandidate_.|
|Дополнение|Бета-версия|Добавлено свойство _locationUri_ к _location_.|
|Дополнение|Бета-версия|Добавлены свойства _type_ и _postOfficeBox_ к _physicalAddress_.|
|Изменение|Бета-версия|У метода _findMeetingTimes_ появился новый параметр _ReturnSuggestionHints_.|
|Изменение|Бета-версия|Метод _findMeetingTimes_ теперь возвращает коллекцию объектов _meetingTimeCandidate_.|

### <a name="drive"></a>Drive

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0 и бета-версия|Добавлена функция _recent_ для вывода списка элементов, которые недавно использовал пользователь, вошедший в систему. Этот список включает элементы, находящиеся на диске пользователя, а также элементы на других дисках, к которым у пользователя есть доступ. Пример: GET /me/drive/recent.|
|Дополнение|1.0 и бета-версия|Добавлена функция _sharedWithMe_ для вывода списка элементов, доступ к которым предоставлен текущему пользователю. Пример: GET /me/drive/sharedWithMe.|

### <a name="driveitem"></a>DriveItem

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0 и бета-версия|Добавлен тип _remoteItem_, который позволяет предоставить ссылку на элемент на другом диске.|
|Дополнение|1.0 и бета-версия|Добавлен тип _sharingInvitation_, который позволяет предоставить сведения о приглашении к совместному использованию, связанном с этим разрешением.|
|Дополнение|1.0 и бета-версия|Добавлена функция _delta_, чтобы отслеживать изменения элементов на диске. Пример: GET /me/drive/items/{item-id}/delta|
|Дополнение|1.0 и бета-версия|Добавлен метод _copy_, который создает копию _driveItem_ (в том числе всех дочерних элементов) в новом родительском элементе или с новым именем. Пример: POST /me/drive/items/{item-id}/copy|
|Дополнение|1.0 и бета-версия|Атрибуты экземпляра _conflictBehavior_ теперь можно применять к _driveItem_.|
|Дополнение|Бета|Добавлена функция _invite_, которая позволяет отправить приглашение к совместному использованию для существующего элемента. Приглашение к совместному использованию создает уникальную ссылку для совместного доступа и отправляет ее получателю приглашения. Пример: POST /drive/items/{item-id}/invite

### <a name="event"></a>Событие

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета-версия|Добавлены новое свойство _onlineMeetingUrl_ и новый метод _cancel_.|

### <a name="event-messages"></a>Сообщения о событиях

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета-версия|Добавлены свойства _startDateTime_, _endDateTime_, _location_, _type_, _recurrence_, _isOutOfDate_, _conversationIndex_, _unsubscribe_, _unsubscribeData_, _unsubscribeEnabled_ и _flag_ к объекту _eventmessage_.|
|Дополнение|Бета-версия|Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_.|
|Дополнение|Бета-версия|Добавлен новый метод _unsubscribe_.|

### <a name="excel"></a>Excel

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета|Мы добавляем новые REST API Excel, которые позволяют считывать и изменять данные в рабочей книге Excel. Теперь вы можете создавать интеллектуальные приложения, с помощью которых пользователи смогут эффективно анализировать содержимое, хранящееся в рабочих книгах Excel. Используйте аналитические функции Excel, создавайте таблицы и визуально привлекательные диаграммы в своем приложении. Дополнительные сведения см. в статье [Работа с Excel в Microsoft Graph](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/excel).|

### <a name="general"></a>Общие

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0 и бета-версия|Улучшено сообщение об ошибке при сопоставлении псевдонима клиента и отклоненных токенов JWT (AAD).|
|Дополнение|1.0 и бета-версия|Сведения о расположении конечной точки службы авторизации теперь возвращаются в заголовке _www-authenticate_ при получении запроса с пустым токеном носителя.|
|Дополнение|1.0 и бета-версия|Исправлена возможность фильтрации по свойству id объекта. Пример: GET https://graph.microsoft.com/v1.0/users?$filter=id+eq+'x'<br/>Ранее в запросах POST требовалось добавлять microsoft.graph перед именем функции или действия. Например: POST https://graph.microsoft.com/v1.0/me/Microsoft.Graph.getMemberGroups.<br/>Теперь не требуется указывать префикс (хотя его по-прежнему можно указывать). Таким образом, указанный ниже запрос также будет работать. POST https://graph.microsoft.com/v1.0/me/getMemberGroups|
|Изменение|Бета|Удалены имена свойств подписок.|
|Дополнение|Бета|Мы добавили возможность находить (с помощью _directorySettingTemplates_) и переопределять поведение по умолчанию (путем создания _setting_ на основе шаблона) для объектов и связанных с ними функций. Изначально для управления поведением групп Office использовался только этот шаблон.|

### <a name="mail-folder"></a>Папка почты

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета-версия|Добавлены свойства _wellKnownName_ и _userConfigurations_.|
|Дополнение|Бета-версия|Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_.|

### <a name="messages"></a>Сообщения

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0|Добавлено свойство _mobilePhone_.|
|Дополнение|1.0 и бета-версия|Добавлено свойство _internetMessageId_. Идентификатор сообщения в формате, установленном документом [RFC2822](http://www.ietf.org/rfc/rfc2822.txt).|
|Изменение|Бета-версия|Свойство _mobilePhone1_ теперь называется _mobilePhone_.|
|Изменение|Бета-версия|У методов _createReply_ и _createReplyAll_ появились новые параметры — _Message_ и _comment_.|
|Изменение|Бета-версия|У метода _createForward_ появились новые параметры — _Message_, _ToRecipients_ и _comment_.|
|Изменение|Бета-версия|У методов _reply_, _replyAll_ и _forward_ появился новый параметр — _Message_.|

### <a name="permission"></a>Разрешение

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0 и бета-версия|Добавлено свойство _sharingInvitation_ для предоставления сведений о приглашении к совместному использованию, связанном с этим разрешением.|

### <a name="person"></a>Человек

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета-версия|Добавлены новые свойства: _birthday_, _personNotes_, _isFavorite_, _phones_, _permission_, _postalAddresses_, _websites_, _yomiCompany_, _department_, _profession_, _mailboxType_ и _personType_.|
|Дополнение|Бета-версия|Добавлены новые типы перечислений: _physicalAddressType_, _webSite_, _phone_ и _webSiteType_.|

### <a name="reference-attachment"></a>Вложение в виде ссылки

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета-версия|Добавлены новые свойства: _sourceUrl_, _providerType_, _thumbnailUrl_, _previewUrl_, _permission_ и _isFolder_.|
|Дополнение|Бета-версия|Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_.|
|Дополнение|Бета-версия|Добавлены новые типы перечислений — _referenceAttachmentProvider_ и _referenceAttachmentPermission_.|

### <a name="subscriptions"></a>Подписки

|**Тип изменения**|**Конечная точка**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0|Теперь веб-перехватчики общедоступны в конечной точке версии 1.0 благодаря ресурсу _/Subscriptions_. Вы можете создавать, считывать, продлевать и удалять подписки на уведомления о данных из чатов в Outlook и группах Office 365.|

### <a name="user"></a>Пользователь

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета-версия|Добавлено свойство _mailboxSettings_ и соответствующие типы.|

## <a name="february-2016"></a>Февраль 2016 г.

### <a name="driveitem"></a>DriveItem

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0 и бета-версия|Новое свойство _remoteItem_ для driveItem для учетных записей Майкрософт.|

### <a name="general"></a>Общие

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Изменение|1.0 и бета-версия|Конструкция-_/me/drive_ теперь работает как для учетных записей Майкрософт, так и для рабочих и учебных учетных записей.|
|Изменение|1.0 и бета-версия|Запросы Drive для учетных записей, хранилища OneDrive которых подготовлены по запросу, работают более надежно и в большем количестве сценариев, где для используемых по умолчанию сайтов SharePoint клиента применяются нестандартные имена.|
|Удаление|Бета|Из бета-версии схемы удалены различные нереализованные типы для более точного соответствия схеме версии 1.0.|

### <a name="subscriptions"></a>Подписки

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета|Проверка notificationUrl на создание подписок. Дополнительные сведения см. в статье [Обновление веб-перехватчиков Microsoft Graph — январь 2016 г.](http://dev.office.com/blogs/Microsoft-Graph-WebHooks-Update-January-2016)|
|Дополнение|Бета|Теперь можно удалять объекты подписки: DELETE https://graph.microsoft.com/beta/subscriptions/|

### <a name="users"></a>Пользователи

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Изменение|1.0 и бета-версия|Теперь для учетных записей Майкрософт возвращается _displayName_.|

## <a name="january-2016"></a>Январь 2016 г.

### <a name="contacts"></a>Контакты

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|1.0|В набор объектов личных контактов добавлено свойство mobilePhone.|

### <a name="directoryobjects"></a>directoryObjects

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Исправление|1.0 и бета-версия|Исправлены действия вызовов, привязанные к directoryObjects, при которых возникали сбои со следующим сообщением об ошибке:  Тип значения, возвращаемого в результате операции, невозможен для заданного набора объектов. Это относится к следующим действиям: _microsoft.graph.checkMemberObjects_, _microsoft.graph.getMemberObjects_, _microsoft.graph.checkMemberGroups_, _microsoft.graph.assignLicense_, _microsoft.graph.changePassword_.|

## <a name="december-2015"></a>Декабрь 2015 г.

### <a name="contacts"></a>Контакты

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета-версия|В набор объектов личных контактов добавлено свойство mobilePhone.|

### <a name="general"></a>Общие

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Исправление|1.0 и бета-версия|Исправлены запросы, в которых используются выражения $filter, указанные для одного и того же свойства несколько раз, при выполнении которых возникали сбои с кодом 500 и отображалось следующее сообщение об ошибке: "Элемент с тем же ключом уже был добавлен".|
|Исправление|1.0 и бета-версия|Исправлена ошибка, при которой не учитывался регистр имен и значений параметров действий.|
|Исправление|1.0 и бета-версия|Исправлена обработка запросов для полезных нагрузок, содержащих значения null для некоторых внедренных сложных свойств, при которых возникал сбой из-за ссылки на значение null.|
|Дополнение|1.0 и бета-версия|Добавлена возможность сортировать и фильтровать свойства сложных типов.|
|Дополнение|1.0 и бета-версия|Добавлено свойство authorization_uri в заголовок www-authenticate ответа 401. Вы можете использовать этот универсальный код ресурса для запуска потока получения токена.|
|Дополнение|1.0 и бета-версия|Улучшены сообщения об ошибках для пользователей и групп.|

### <a name="groups"></a>Группы

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Исправление|1.0 и бета-версия|Исправлен вызов следующих действий групп: _microsoft.graph.addFavorite_, _microsoft.graph.removeFavorite_ и _microsoft.graph.resetUnseenCount_.|

### <a name="messages"></a>Сообщения

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета-версия|К типу eventMessage добавлен подтип для свойств eventMessageRequest eventMessage, startDateTime, endDateTime, location, type, recurrence и isOutOfDate.|

### <a name="users"></a>Пользователи

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Исправление|1.0 и бета-версия|Устранена возможность выбирать определенные свойства других пользователей, когда на них ссылаются по их основному имени участника-пользователя. Например: https://graph.microsoft.com/v1.0/users/anotherUser@contoso.com?$select=aboutMe|
|Исправление|1.0 и бета-версия|Исправлен вызов функции _microsoft.graph.reminderView_, привязанной к пользователю, при котором возникал сбой и отображалось следующее сообщение об ошибке: "Не удалось найти свойство с именем businessPhones в типе Microsoft.OutlookServices.Reminder".|
|Исправление|1.0 и бета-версия|Устранена проблема, из-за которой при создании и обновлении пользователей (POST/PATCH /v1.0/users) возникала ошибка 400.|
