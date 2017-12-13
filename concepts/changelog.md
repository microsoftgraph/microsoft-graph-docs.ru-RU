# <a name="changelog-for-microsoft-graph"></a>Журнал изменений Microsoft Graph

Этот журнал содержит сведения об изменениях Microsoft Graph, в том числе API Microsoft Graph для конечных точек версии 1.0 и бета-версии.  

Дополнительные сведения об известных проблемах с API Microsoft Graph см. в статье [Известные проблемы](known_issues.md).

## <a name="november-2017"></a>Ноябрь 2017 г.

### <a name="webhooks"></a>Веб-перехватчики

| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Существенные изменения | Бета-версия и версия 1.0 | Сокращен [максимальный период действия подписки](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type) с использованием [веб-перехватчиков](../api-reference/v1.0/resources/webhooks.md) для элементов в корне диска. Новое значение — допустимый максимальный срок действия для элементов в корне диска. | 

### <a name="reports-apis"></a>API отчетов
| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета-версия    | Добавлена поддержка JSON для следующих API:<br>[getEmailActivityUserDetail](../api-reference/beta/api/reportroot_getemailactivityuserdetail.md)<br>[getEmailActivityCounts](../api-reference/beta/api/reportroot_getemailactivitycounts.md)<br>[getEmailActivityUserCounts](../api-reference/beta/api/reportroot_getemailactivityusercounts.md)<br>[getEmailAppUsageUserDetail](../api-reference/beta/api/reportroot_getemailappusageuserdetail.md)<br>[getEmailAppUsageAppsUserCounts](../api-reference/beta/api/reportroot_getemailappusageappsusercounts.md)<br>[getEmailAppUsageUserCounts](../api-reference/beta/api/reportroot_getemailappusageusercounts.md)<br>[getEmailAppUsageVersionsUserCounts](../api-reference/beta/api/reportroot_getemailappusageversionsusercounts.md)<br>[getMailboxUsageDetail](../api-reference/beta/api/reportroot_getmailboxusagedetail.md)<br>[getMailboxUsageMailboxCounts](../api-reference/beta/api/reportroot_getmailboxusagemailboxcounts.md)<br>[getMailboxUsageQuotaStatusMailboxCounts](../api-reference/beta/api/reportroot_getmailboxusagequotastatusmailboxcounts.md)<br>[getMailboxUsageStorage](../api-reference/beta/api/reportroot_getmailboxusagestorage.md)<br>[getOffice365ActivationsUserDetail](../api-reference/beta/api/reportroot_getoffice365activationsuserdetail.md)<br>[getOffice365ActivationCounts](../api-reference/beta/api/reportroot_getoffice365activationcounts.md)<br>[getOffice365ActivationsUserCounts](../api-reference/beta/api/reportroot_getoffice365activationsusercounts.md)<br>[getOffice365ActiveUserDetail](../api-reference/beta/api/reportroot_getoffice365activeuserdetail.md)<br>[getOffice365ActiveUserCounts](../api-reference/beta/api/reportroot_getoffice365activeusercounts.md)<br>[getOffice365ServicesUserCounts](../api-reference/beta/api/reportroot_getoffice365servicesusercounts.md)<br>[getOffice365GroupsActivityDetail](../api-reference/beta/api/reportroot_getoffice365groupsactivitydetail.md)<br> [getOffice365GroupsActivityCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivitycounts.md)<br>[getOffice365GroupsActivityGroupCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivitygroupcounts.md)<br>[getOffice365GroupsActivityStorage](../api-reference/beta/api/reportroot_getoffice365groupsactivitystorage.md)<br>[getOffice365GroupsActivityFileCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivityfilecounts.md)<br>[getOneDriveActivityUserDetail](../api-reference/beta/api/reportroot_getonedriveactivityuserdetail.md)<br>[getOneDriveActivityUserCounts](../api-reference/beta/api/reportroot_getonedriveactivityusercounts.md)<br>[getOneDriveActivityFileCounts](../api-reference/beta/api/reportroot_getonedriveactivityfilecounts.md)<br>[getOneDriveUsageAccountDetail](../api-reference/beta/api/reportroot_getonedriveusageaccountdetail.md)<br>[getOneDriveUsageAccountCounts](../api-reference/beta/api/reportroot_getonedriveusageaccountcounts.md)<br>[getOneDriveUsageFileCounts](../api-reference/beta/api/reportroot_getonedriveusagefilecounts.md)<br>[getOneDriveUsageStorage](../api-reference/beta/api/reportroot_getonedriveusagestorage.md)<br>[getSharePointActivityUserDetail](../api-reference/beta/api/reportroot_getsharepointactivityuserdetail.md)<br>[getSharePointActivityFileCounts](../api-reference/beta/api/reportroot_getsharepointactivityfilecounts.md)<br>[getSharePointActivityUserCounts](../api-reference/beta/api/reportroot_getsharepointactivityusercounts.md)<br>[getSharePointActivityPages](../api-reference/beta/api/reportroot_getsharepointactivitypages.md)<br>[getSharePointSiteUsageDetail](../api-reference/beta/api/reportroot_getsharepointsiteusagedetail.md)<br>[getSharePointSiteUsageFileCounts](../api-reference/beta/api/reportroot_getsharepointsiteusagefilecounts.md)<br>[getSharePointSiteUsageSiteCounts](../api-reference/beta/api/reportroot_getsharepointsiteusagesitecounts.md)<br>[getSharePointSiteUsageStorage](../api-reference/beta/api/reportroot_getsharepointsiteusagestorage.md)<br>[getSharePointSiteUsagePages](../api-reference/beta/api/reportroot_getsharepointsiteusagepages.md)<br>[getSkypeForBusinessActivityUserDetail](../api-reference/beta/api/reportroot_getskypeforbusinessactivityuserdetail.md)<br>[getSkypeForBusinessActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessactivitycounts.md)<br>[getSkypeForBusinessActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessactivityusercounts.md)<br>[getSkypeForBusinessDeviceUsageUserDetail](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusageuserdetail.md)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusagedistributionusercounts.md)<br>[getSkypeForBusinessDeviceUsageUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusageusercounts.md)<br>[getSkypeForBusinessOrganizerActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivitycounts.md)<br>[getSkypeForBusinessOrganizerActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivityusercounts.md)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivityminutecounts.md)<br>[getSkypeForBusinessParticipantActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivitycounts.md)<br>[getSkypeForBusinessParticipantActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivityusercounts.md)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivityminutecounts.md)<br>[getSkypeForBusinessPeerToPeerActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivitycounts.md)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivityusercounts.md)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivityminutecounts.md)<br>[getYammerActivityUserDetail](../api-reference/beta/api/reportroot_getyammeractivityuserdetail.md)<br>[getYammerActivityCounts](../api-reference/beta/api/reportroot_getyammeractivitycounts.md)<br>[getYammerActivityUserCounts](../api-reference/beta/api/reportroot_getyammeractivityusercounts.md)<br>[getYammerDeviceUsageUserDetail](../api-reference/beta/api/reportroot_getyammerdeviceusageuserdetail.md)<br>[getYammerDeviceUsageDistributionUserCounts](../api-reference/beta/api/reportroot_getyammerdeviceusagedistributionusercounts.md)<br>[getYammerDeviceUsageUserCounts](../api-reference/beta/api/reportroot_getyammerdeviceusageusercounts.md)<br>[getYammerGroupsActivityDetail](../api-reference/beta/api/reportroot_getyammergroupsactivitydetail.md)<br>[getYammerGroupsActivityGroupCounts](../api-reference/beta/api/reportroot_getyammergroupsactivitygroupcounts.md)<br>[getYammerGroupsActivityCounts](../api-reference/beta/api/reportroot_getyammergroupsactivitycounts.md) |

## <a name="october-2017"></a>Октябрь 2017 г.

### <a name="azure-ad-apis"></a>API Azure AD

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
|Дополнение|Бета-версия|Добавлены объект [identityProvider](../api-reference/beta/resources/identityprovider.md) и операции [create](../api-reference/beta/api/identityprovider_post_identityproviders.md), [list](../api-reference/beta/api/identityprovider_list.md), [get](../api-reference/beta/api/identityprovider_get.md), [update](../api-reference/beta/api/identityprovider_update.md) и [delete](../api-reference/beta/api/identityprovider_delete.md).|


### <a name="microsoft-intune-apis"></a>API Microsoft Intune
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidDeviceComplianceLocalActionLockDeviceWithPasscode](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androiddevicecompliancelocalactionlockdevicewithpasscode)<br/>[iosLobAppProvisioningConfigurationAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfigurationassignment)<br/>[iosVppEBookAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_books_iosvppebookassignment)<br/>[managedDeviceMobileAppConfigurationAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationassignment)<br/>[managedEBookAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_books_managedebookassignment)<br/>[managedMobileApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_managedmobileapp)<br/>[mobileAppAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileappassignment)<br/>[termsAndConditionsAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_companyterms_termsandconditionsassignment)<br/>[vppToken](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_vpptoken)<br/>[windows10PFXImportCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10pfximportcertificateprofile)<br/>[windowsAssignedAccessProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsassignedaccessprofile)<br/>[windowsDomainJoinConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsdomainjoinconfiguration)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[iosLobAppAssignmentSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_ioslobappassignmentsettings)<br/>[iosSingleSignOnSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iossinglesignonsettings)<br/>[iosStoreAppAssignmentSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_iosstoreappassignmentsettings)<br/>[iosVppAppAssignmentSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_iosvppappassignmentsettings)<br/>[mobileAppAssignmentSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileappassignmentsettings)<br/>[proxiedDomain](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_proxieddomain)<br/>[windowsInformationProtectionProxiedDomainCollection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionproxieddomaincollection)<br/>[windowsStoreForBusinessAppAssignmentSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessappassignmentsettings)<br/>|
|Дополнение|Бета-версия|Добавлено действие [assign](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_apps_mobileapp_assign.md) для объекта [mobileApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileapp). |
|Дополнение|Бета-версия|Добавлено действие [assign](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign.md) к объекту [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration). |
|Дополнение|Бета-версия|Добавлено действие [assign](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_apps_manageddevicemobileappconfiguration_assign.md) для объекта [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration). |
|Дополнение|Бета-версия|Добавлено действие [assign](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_deviceconfig_devicecompliancepolicy_assign.md) для объекта [deviceCompliancePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy). |
|Дополнение|Бета-версия|Добавлено действие [assignedAccessMultiModeProfiles](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_deviceconfig_deviceconfiguration_assignedaccessmultimodeprofiles.md) для объекта [deviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration). |
|Дополнение|Бета-версия|Добавлено действие [syncLicenses](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_onboarding_vpptoken_synclicenses.md) для объекта [vppToken](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_vpptoken). |
|Дополнение|Бета-версия|Добавлено действие [targetApps](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_mam_managedapppolicy_targetapps.md) для объекта [managedAppPolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy). |
|Дополнение|Бета-версия|Добавлено действие [targetApps](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_mam_managedappprotection_targetapps.md) для объекта [managedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_managedappprotection). |
|Дополнение|Бета-версия|Добавлено действие [targetApps](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_targetapps.md) для объекта [targetedManagedAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration). |
|Дополнение|Бета|Добавлено действие [assign](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_books_managedebook_assign.md) для объекта [managedEBook](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_books_managedebook). |
|Удаление|Бета-версия|Удалены следующие объекты:<br/>**cloudPkiSubscription**<br/>|
|Удаление|Бета-версия|Удалены следующие сложные типы:<br/>**cloudPkiAdministratorCredentials**<br/>**windowsNetworkIsolationCloudResource**<br/>**windowsNetworkIsolationCloudResourceCollection**<br/>**windowsNetworkIsolationIPRangeCollection**<br/>**windowsNetworkIsolationResourceCollection**<br/>|
|Изменение|Бета-версия|Добавлено свойство **gracePeriodInMinutes** для объекта [androidDeviceComplianceLocalActionBase](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androiddevicecompliancelocalactionbase).|
|Изменение|Бета-версия|Удалено свойство **enableSplitTunneling** объекта [androidForWorkVpnConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkvpnconfiguration).|
|Изменение|Бета-версия|Добавлены свойства **versionName** и **versionCode** для объекта [androidLobApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_androidlobapp).|
|Изменение|Бета-версия|Добавлены свойства **minimumRequiredPatchVersion** и **minimumWarningPatchVersion** для объекта [androidManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection).|
|Изменение|Бета-версия|Добавлены свойства **minimumRequiredPatchVersion** и **minimumWarningPatchVersion** для объекта [defaultManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection).|
|Изменение|Бета-версия|Добавлено свойство **target** для объекта [deviceCompliancePolicyAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicyassignment).|
|Изменение|Бета-версия|Добавлено свойство **singleSignOnSettings** для объекта [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration).|
|Изменение|Бета-версия|Добавлены свойства **versionNumber** и **buildNumber** для объекта [iosLobApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_ioslobapp).|
|Изменение|Бета-версия|Добавлено свойство **bundleId** для объекта [iosVppApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_iosvppapp).|
|Изменение|Бета-версия|Добавлено свойство **preSharedKey** для объекта [iosWiFiConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswificonfiguration).|
|Изменение|Бета-версия|Добавлены свойства **versionName** и **versionCode** для объекта [managedAndroidLobApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp).|
|Изменение|Бета-версия|Добавлено свойство **periodBeforePinReset** для объекта [managedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_managedappprotection).|
|Изменение|Бета-версия|Добавлены свойства **subscriberCarrier**, **meid**, **totalStorageSpaceInBytes** и **freeStorageSpaceInBytes** для объекта [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice).|
|Изменение|Бета-версия|Удалено свойство **enrollmentType** объекта [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice).|
|Изменение|Бета-версия|Добавлены свойства **versionNumber** и **buildNumber** для объекта [managedIOSLobApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp).|
|Изменение|Бета-версия|Добавлено свойство **displayVersion** для объекта [mobileAppInstallStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus).|
|Изменение|Бета-версия|Удалены свойства **defaultDeviceEnrollmentRestrictions**, **defaultDeviceEnrollmentWindowsHelloForBusinessSettings** и **defaultDeviceEnrollmentLimit** объекта [organization](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_organization).|
|Изменение|Бета-версия|Добавлено свойство **isAssigned** для объекта [targetedManagedAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration).|
|Изменение|Бета-версия|Добавлено свойство **isAssigned** для объекта [targetedManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappprotection).|
|Изменение|Бета-версия|Добавлены свойства **activeFirewallRequired**, **uacRequired**, **defenderEnabled**, **defenderVersion**, **signatureOutOfDate** и **rtpEnabled** объекта [windows10CompliancePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10compliancepolicy).|
|Изменение|Бета-версия|Добавлены свойства **assignedAccessSingleModeUserName**, **assignedAccessSingleModeAppUserModelId**, **microsoftAccountSignInAssistantSettings**, **authenticationAllowSecondaryDevice**, **cryptographyAllowFipsAlgorithmPolicy**, **securityBlockAzureADJoinedDevicesAutoEncryption**, **systemTelemetryProxyServer**, **inkWorkspaceAccess**, **inkWorkspaceBlockSuggestedApps**, **defenderCloudBlockLevel** и **defenderCloudExtendedTimeout** объекта [windows10GeneralConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration).|
|Изменение|Бета-версия|Добавлены свойства **protectedApps**, **enterpriseProxiedDomains** и **isAssigned** для объекта [windowsInformationProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection).|
|Изменение|Бета-версия|Добавлено свойство **productVersion** для объекта [windowsMobileMSI](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi).|
|Изменение|Бета-версия|Добавлено свойство навигации **apps** для объекта [androidManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection).|
|Изменение|Бета-версия|Добавлено свойство навигации **apps** для объекта [defaultManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection).|
|Изменение|Бета-версия|Добавлено свойство навигации **vppTokens** для объекта [deviceAppManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignments** для объекта [deviceCompliancePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy).|
|Изменение|Бета-версия|Удалено свойство навигации **deviceCompliancePolicy** объекта [deviceCompliancePolicyAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicyassignment).|
|Изменение|Бета-версия|Добавлено свойство навигации **deviceCompliancePolicy** для объекта [deviceCompliancePolicyGroupAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicygroupassignment).|
|Изменение|Бета-версия|Добавлено свойство навигации **identityCertificateForClientAuthentication** для объекта [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignments** для объекта [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration).|
|Изменение|Бета-версия|Добавлено свойство навигации **apps** для объекта [iosManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignments** для объекта [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignments** для объекта [managedEBook](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_books_managedebook).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignments** для объекта [mobileApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileapp).|
|Изменение|Бета-версия|Добавлено свойство навигации **apps** для объекта [targetedManagedAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignments** для объекта [termsAndConditions](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_companyterms_termsandconditions).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignedAccessMultiModeProfiles** для объекта [windows10GeneralConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration).|
|Изменение|Бета-версия|Добавлено свойство навигации **protectedAppLockerFiles** для объекта [windowsInformationProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection).|
|Изменение|Бета-версия|Добавлены свойства **port** и **forceTls** для сложного типа [airPrintDestination](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_airprintdestination).|
|Изменение|Бета-версия|Изменен тип следующих свойств сложного типа [deviceCompliancePolicySettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate):<br/>вместо Int32 **errorCode** теперь используется Int64.<br/>|
|Изменение|Бета-версия|Изменен тип следующих свойств сложного типа [deviceConfigurationSettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate):<br/>вместо Int32 **errorCode** теперь используется Int64.<br/>|
|Изменение|Бета-версия|Изменен тип следующих свойств сложного типа [windowsNetworkIsolationPolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsnetworkisolationpolicy):<br/>вместо **enterpriseCloudResources** [windowsNetworkIsolationCloudResourceCollection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsNetworkIsolationCloudResourceCollection.md) теперь используется коллекция объектов [proxiedDomain](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_proxieddomain);<br/>вместо [windowsNetworkIsolationResourceCollection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsNetworkIsolationResourceCollection.md) **enterpriseInternalProxyServers** теперь используется коллекция строк;<br/>вместо **enterpriseIPRanges** [windowsNetworkIsolationIPRangeCollection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsNetworkIsolationIPRangeCollection.md) теперь используется коллекция объектов [ipRange](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iprange);<br/>вместо **enterpriseNetworkDomainNames** [windowsNetworkIsolationResourceCollection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsNetworkIsolationResourceCollection.md) теперь используется коллекция строк;<br/>вместо **enterpriseProxyServers** [windowsNetworkIsolationResourceCollection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsNetworkIsolationResourceCollection.md) теперь используется коллекция строк;<br/>вместо **neutralDomainResources** [windowsNetworkIsolationResourceCollection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsNetworkIsolationResourceCollection.md) теперь используется коллекция строк.<br/>|

### <a name="microsoft-teams-apis"></a>API Microsoft Teams

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета-версия|Добавлен новый объект [team](../api-reference/beta/resources/team.md).|
|Дополнение|Бета-версия|Добавлены операции [create](../api-reference/beta/api/team_put_teams.md), [get](../api-reference/beta/api/team_get.md) и [update](../api-reference/beta/api/team_update.md) для объекта [team](../api-reference/beta/resources/team.md).|

### <a name="outlook-messages"></a>Сообщения Outlook

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Это улучшение поведения связано с получением общей почтовой папки или содержимого сообщений в ней, если кто-то предоставил вошедшему пользователю доступ к почтовой папке или делегировал ему почтовый ящик пользователя. В таких случаях приложение может указать ИД пользователя или имя участника-пользователя, чтобы [получить эту общую почтовую папку](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/mailfolder_get) или [получить сообщения из этого общего календаря](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/user_list_messages), при условии что вошедший пользователь предоставил приложению делегированные разрешения. |


### <a name="outlook-user-choices"></a>Настройки пользователей Outlook

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
|Дополнение | Бета-версия | Добавлено новое свойство **workingHours** для объекта [mailboxSettings](../api-reference/beta/resources/mailboxsettings.md). Сведения о поддерживаемых вариантах использования см. в описании [типа ресурса workingHours](../api-reference/beta/resources/workinghours.md).|
|Дополнение | Бета-версия | Добавлены следующие сложные типы: <br> [workingHours](../api-reference/beta/resources/workinghours.md) <br> [timeZoneBase](../api-reference/beta/resources/timezonebase.md) <br> [customTimeZone](../api-reference/beta/resources/customtimezone.md) <br> [standardTimeZoneOffset](../api-reference/beta/resources/standardtimezoneoffset.md) <br> [daylightTimeZoneOffset](../api-reference/beta/resources/daylighttimezoneoffset.md)|


### <a name="reports-apis"></a>API отчетов
| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Изменение      | Бета-версия    | Добавлены API [getEmailActivityUserDetail](../api-reference/beta/api/reportroot_getemailactivityuserdetail.md), [getEmailActivityCounts](../api-reference/beta/api/reportroot_getemailactivitycounts.md) и [getEmailActivityUserCounts](../api-reference/beta/api/reportroot_getemailactivityusercounts.md). Они заменили API EmailActivity. |
| Изменение      | Бета-версия    | Добавлены API [getEmailAppUsageUserDetail](../api-reference/beta/api/reportroot_getemailappusageuserdetail.md), [getEmailAppUsageAppsUserCounts](../api-reference/beta/api/reportroot_getemailappusageappsusercounts.md), [getEmailAppUsageUserCounts](../api-reference/beta/api/reportroot_getemailappusageusercounts.md) и [getEmailAppUsageVersionsUserCounts](../api-reference/beta/api/reportroot_getemailappusageversionsusercounts.md). Они заменили API EmailAppUsage. |
| Изменение      | Бета-версия    | Добавлены API [getMailboxUsageDetail](../api-reference/beta/api/reportroot_getmailboxusagedetail.md), [getMailboxUsageMailboxCounts](../api-reference/beta/api/reportroot_getmailboxusagemailboxcounts.md), [getMailboxUsageQuotaStatusMailboxCounts](../api-reference/beta/api/reportroot_getmailboxusagequotastatusmailboxcounts.md) и [getMailboxUsageStorage](../api-reference/beta/api/reportroot_getmailboxusagestorage.md). Они заменили API MailboxUsage. |
| Изменение      | Бета-версия    | Добавлены API [getOffice365ActivationsUserDetail](../api-reference/beta/api/reportroot_getoffice365activationsuserdetail.md), [getOffice365ActivationCounts](../api-reference/beta/api/reportroot_getoffice365activationcounts.md) и [getOffice365ActivationsUserCounts](../api-reference/beta/api/reportroot_getoffice365activationsusercounts.md). Они заменили API Office365Activations. |
| Изменение      | Бета-версия    | Добавлены API [getOffice365ActiveUserDetail](../api-reference/beta/api/reportroot_getoffice365activeuserdetail.md), [getOffice365ActiveUserCounts](../api-reference/beta/api/reportroot_getoffice365activeusercounts.md) и [getOffice365ServicesUserCounts](../api-reference/beta/api/reportroot_getoffice365servicesusercounts.md). Они заменили API Office365ActiveUser. |
| Изменение      | Бета-версия    | Добавлены API [getOffice365GroupsActivityDetail](../api-reference/beta/api/reportroot_getoffice365groupsactivitydetail.md), [getOffice365GroupsActivityCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivitycounts.md), [getOffice365GroupsActivityGroupCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivitygroupcounts.md), [getOffice365GroupsActivityStorage](../api-reference/beta/api/reportroot_getoffice365groupsactivitystorage.md) и [getOffice365GroupsActivityFileCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivityfilecounts.md). Они заменили API Office365GroupsActivity. |
| Изменение      | Бета-версия    | Добавлены API [getOneDriveActivityUserDetail](../api-reference/beta/api/reportroot_getonedriveactivityuserdetail.md), [getOneDriveActivityUserCounts](../api-reference/beta/api/reportroot_getonedriveactivityusercounts.md) и [getOneDriveActivityFileCounts](../api-reference/beta/api/reportroot_getonedriveactivityfilecounts.md). Они заменили API OneDriveActivity. |
| Изменение      | Бета-версия    | Добавлены API [getOneDriveUsageAccountDetail](../api-reference/beta/api/reportroot_getonedriveusageaccountdetail.md), [getOneDriveUsageAccountCounts](../api-reference/beta/api/reportroot_getonedriveusageaccountcounts.md), [getOneDriveUsageFileCounts](../api-reference/beta/api/reportroot_getonedriveusagefilecounts.md) и [getOneDriveUsageStorage](../api-reference/beta/api/reportroot_getonedriveusagestorage.md). Они заменили API OneDriveUsage. |
| Изменение      | Бета-версия    | Добавлены API [getSharePointActivityUserDetail](../api-reference/beta/api/reportroot_getsharepointactivityuserdetail.md), [getSharePointActivityFileCounts](../api-reference/beta/api/reportroot_getsharepointactivityfilecounts.md), [getSharePointActivityUserCounts](../api-reference/beta/api/reportroot_getsharepointactivityusercounts.md) и [getSharePointActivityPages](../api-reference/beta/api/reportroot_getsharepointactivitypages.md). Они заменили API SharePointActivity. |
| Изменение      | Бета-версия    | Добавлены API [getSharePointSiteUsageDetail](../api-reference/beta/api/reportroot_getsharepointsiteusagedetail.md), [getSharePointSiteUsageFileCounts](../api-reference/beta/api/reportroot_getsharepointsiteusagefilecounts.md), [getSharePointSiteUsageSiteCounts](../api-reference/beta/api/reportroot_getsharepointsiteusagesitecounts.md), [getSharePointSiteUsageStorage](../api-reference/beta/api/reportroot_getsharepointsiteusagestorage.md) и [getSharePointSiteUsagePages](../api-reference/beta/api/reportroot_getsharepointsiteusagepages.md). Они заменили API SharePointSiteUsage. |
| Изменение      | Бета-версия    | Добавлены API [getSkypeForBusinessActivityUserDetail](../api-reference/beta/api/reportroot_getskypeforbusinessactivityuserdetail.md), [getSkypeForBusinessActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessactivitycounts.md) и [getSkypeForBusinessActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessactivityusercounts.md). Они заменили API SfbActivity. |
| Изменение      | Бета-версия    | Добавлены API [getSkypeForBusinessDeviceUsageUserDetail](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusageuserdetail.md), [getSkypeForBusinessDeviceUsageDistributionUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusagedistributionusercounts.md) и [getSkypeForBusinessDeviceUsageUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusageusercounts.md). Они заменили API SfbDeviceUsage. |
| Изменение      | Бета-версия    | Добавлены API [getSkypeForBusinessOrganizerActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivitycounts.md), [getSkypeForBusinessOrganizerActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivityusercounts.md) и [getSkypeForBusinessOrganizerActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivityminutecounts.md). Они заменили API SfbOrganizerActivity. |
| Изменение      | Бета-версия    | Добавлены API [getSkypeForBusinessParticipantActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivitycounts.md), [getSkypeForBusinessParticipantActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivityusercounts.md) и [getSkypeForBusinessParticipantActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivityminutecounts.md). Они заменили API SfbParticipantActivity. |
| Изменение      | Бета-версия    | Добавлены API [getSkypeForBusinessPeerToPeerActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivitycounts.md), [getSkypeForBusinessPeerToPeerActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivityusercounts.md) и [getSkypeForBusinessPeerToPeerActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivityminutecounts.md). Они заменили API SfbP2PActivity. |
| Изменение      | Бета-версия    | Добавлены API [getYammerActivityUserDetail](../api-reference/beta/api/reportroot_getyammeractivityuserdetail.md), [getYammerActivityCounts](../api-reference/beta/api/reportroot_getyammeractivitycounts.md) и [getYammerActivityUserCounts](../api-reference/beta/api/reportroot_getyammeractivityusercounts.md). Они заменили API YammerActivity. |
| Изменение      | Бета-версия    | Добавлены API [getYammerDeviceUsageUserDetail](../api-reference/beta/api/reportroot_getyammerdeviceusageuserdetail.md), [getYammerDeviceUsageDistributionUserCounts](../api-reference/beta/api/reportroot_getyammerdeviceusagedistributionusercounts.md) и [getYammerDeviceUsageUserCounts](../api-reference/beta/api/reportroot_getyammerdeviceusageusercounts.md). Они заменили API YammerDeviceUsage. |
| Изменение      | Бета-версия    | Добавлены API [getYammerGroupsActivityDetail](../api-reference/beta/api/reportroot_getyammergroupsactivitydetail.md), [getYammerGroupsActivityGroupCounts](../api-reference/beta/api/reportroot_getyammergroupsactivitygroupcounts.md) и [getYammerGroupsActivityCounts](../api-reference/beta/api/reportroot_getyammergroupsactivitycounts.md). Они заменили API YammerGroupsActivity. |



## <a name="september-2017"></a>Сентябрь 2017 г.

### <a name="intune-apis"></a>API Intune

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета    | Добавлены новые объекты:<br/>[activeDirectoryWindowsAutopilotDeploymentProfile](../api-reference/beta/resources/intune_enrollment_activedirectorywindowsautopilotdeploymentprofile.md)<br/>[azureADWindowsAutopilotDeploymentProfile](../api-reference/beta/resources/intune_enrollment_azureadwindowsautopilotdeploymentprofile.md)<br/>[deviceEnrollmentConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentconfiguration.md)<br/>[deviceEnrollmentLimitConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentlimitconfiguration.md)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)<br/>[deviceManagementPartner](../api-reference/beta/resources/intune_onboarding_devicemanagementpartner.md)<br/>[enrollmentConfigurationAssignment](../api-reference/beta/resources/intune_onboarding_enrollmentconfigurationassignment.md)<br/>[windows10EnrollmentCompletionPageConfiguration](../api-reference/beta/resources/intune_onboarding_windows10enrollmentcompletionpageconfiguration.md)<br/>[windows10NetworkBoundaryConfiguration](../api-reference/beta/resources/intune_deviceconfig_windows10networkboundaryconfiguration.md)<br/>[windowsAutopilotDeploymentProfile](../api-reference/beta/resources/intune_enrollment_windowsautopilotdeploymentprofile.md)<br/>[windowsAutopilotDeviceIdentity](../api-reference/beta/resources/intune_enrollment_windowsautopilotdeviceidentity.md)<br/>[windowsAutopilotSettings](../api-reference/beta/resources/intune_enrollment_windowsautopilotsettings.md)<br/> |
| Дополнение    | Бета    | Добавлены новые сложные типы:<br/>[adminConsent](../api-reference/beta/resources/intune_devices_adminconsent.md)<br/>[allDevicesAssignmentTarget](../api-reference/beta/resources/intune_onboarding_alldevicesassignmenttarget.md)<br/>[allLicensedUsersAssignmentTarget](../api-reference/beta/resources/intune_onboarding_alllicensedusersassignmenttarget.md)<br/>[deviceAndAppManagementAssignmentTarget](../api-reference/beta/resources/intune_onboarding_deviceandappmanagementassignmenttarget.md)<br/>[deviceEnrollmentPlatformRestriction](../api-reference/beta/resources/intune_onboarding_deviceenrollmentplatformrestriction.md)<br/>[deviceHealthAttestationState](../api-reference/beta/resources/intune_devices_devicehealthattestationstate.md)<br/>[exclusionGroupAssignmentTarget](../api-reference/beta/resources/intune_onboarding_exclusiongroupassignmenttarget.md)<br/>[groupAssignmentTarget](../api-reference/beta/resources/intune_onboarding_groupassignmenttarget.md)<br/>[outOfBoxExperienceSettings](../api-reference/beta/resources/intune_enrollment_outofboxexperiencesettings.md)<br/>[windowsFirewallNetworkProfile](../api-reference/beta/resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)<br/>[windowsNetworkIsolationCloudResource](../api-reference/beta/resources/intune_deviceconfig_windowsnetworkisolationcloudresource.md)<br/>[windowsNetworkIsolationCloudResourceCollection](../api-reference/beta/resources/intune_deviceconfig_windowsnetworkisolationcloudresourcecollection.md)<br/>[windowsNetworkIsolationIPRangeCollection](../api-reference/beta/resources/intune_deviceconfig_windowsnetworkisolationiprangecollection.md)<br/>[windowsNetworkIsolationPolicy](../api-reference/beta/resources/intune_deviceconfig_windowsnetworkisolationpolicy.md)<br/>[windowsNetworkIsolationResourceCollection](../api-reference/beta/resources/intune_deviceconfig_windowsnetworkisolationresourcecollection.md)<br/> |
| Дополнение    | Бета    | Добавлено действие [sync](../api-reference/beta/api/intune_enrollment_windowsautopilotsettings_sync.md) для объекта [windowsAutopilotSettings](../api-reference/beta/resources/intune_enrollment_windowsautopilotsettings.md). |
| Дополнение    | Бета    | Добавлено действие [assign](../api-reference/beta/api/intune_enrollment_windowsautopilotdeploymentprofile_assign.md) для объекта [windowsAutopilotDeploymentProfile](../api-reference/beta/resources/intune_enrollment_windowsautopilotdeploymentprofile.md). |
| Дополнение    | Бета    | Добавлено действие [localActions](../api-reference/beta/api/intune_deviceconfig_devicecompliancepolicy_localactions.md) для объекта [deviceCompliancePolicy](../api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy.md). |
| Дополнение    | Бета    | Добавлено действие [setPriority](../api-reference/beta/api/intune_onboarding_deviceenrollmentconfiguration_setpriority.md) для объекта [deviceEnrollmentConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentconfiguration.md). |
| Дополнение    | Бета    | Добавлено действие [assign](../api-reference/beta/api/intune_onboarding_deviceenrollmentconfiguration_assign.md) для объекта [deviceEnrollmentConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentconfiguration.md). |
| Дополнение    | Бета    | Добавлено действие uploadDepToken для коллекции [depOnboardingSetting](../api-reference/beta/resources/intune_onboarding_deponboardingsetting.md). |
| Дополнение    | Бета    | Добавлено действие syncWithAppleDeviceEnrollmentProgram для коллекции [depOnboardingSetting](../api-reference/beta/resources/intune_onboarding_deponboardingsetting.md). |
| Дополнение    | Бета    | Добавлено действие updateMobileAppIdentifierDeployments для объекта [managedAppProtection](../api-reference/beta/resources/intune_mam_managedappprotection.md). |
| Дополнение    | Бета    | Добавлено действие assign для объекта [targetedManagedAppProtection](../api-reference/beta/resources/intune_mam_targetedmanagedappprotection.md). |
| Дополнение    | Бета    | Добавлено действие assign для объекта [targetedManagedAppConfiguration](../api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration.md). |
| Дополнение    | Бета    | Добавлено действие assign для объекта [windowsInformationProtection](../api-reference/beta/resources/intune_mam_windowsinformationprotection.md). |
| Дополнение    | Бета    | Добавлена функция getEncryptionPublicKey для коллекции [depOnboardingSetting](../api-reference/beta/resources/intune_onboarding_deponboardingsetting.md). |
| Изменение      | Бета    | Добавлены свойства **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders**, **requireCompanyPortalAppIntegrity** и **conditionStatementId** для объекта [androidCompliancePolicy](../api-reference/beta/resources/intune_deviceconfig_androidcompliancepolicy.md). |
| Изменение      | Бета    | Добавлены свойства **requireAppVerify**, **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders** и **requireCompanyPortalAppIntegrity** для объекта [androidForWorkCompliancePolicy](../api-reference/beta/resources/intune_deviceconfig_androidforworkcompliancepolicy.md). |
| Изменение      | Бета    | Добавлены свойства **blockCrossProfileCopyPaste** и **requireAppVerify** для объекта [androidForWorkGeneralDeviceConfiguration](../api-reference/beta/resources/intune_deviceconfig_androidforworkgeneraldeviceconfiguration.md). |
| Изменение      | Бета    | Добавлены свойства **kioskModeApps** и **requireAppVerify** для объекта [androidGeneralDeviceConfiguration](../api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md). |
| Изменение      | Бета    | Удалено свойство **kioskModeManagedApps** объекта [androidGeneralDeviceConfiguration](../api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md). |
| Изменение      | Бета    | Удалены свойства **cloudPkiProvider**, **createdDateTime**, **description**, **lastModifiedDateTime**, **displayName**, **syncStatus**, **lastSyncError**, **lastSyncDateTime**, **credentials**, **trustedRootCertificate** и **version** объекта [cloudPkiSubscription](../api-reference/beta/resources/intune_deviceconfig_cloudpkisubscription.md). |
| Изменение      | Бета    | Удалены свойства **assignmentStatus**, **assignmentProgress** и **assignmentErrorMessage** объекта [deviceConfiguration](../api-reference/beta/resources/intune_deviceconfig_deviceconfiguration.md). |
| Изменение      | Бета    | Добавлено свойство **adminConsent** для объекта [deviceManagement](../api-reference/beta/resources/intune_androidforwork_devicemanagement.md). |
| Изменение      | Бета    | Добавлены свойства **vppTokenOrganizationName**, **vppTokenAccountType** и **vppTokenAppleId** для объекта [iosVppApp](../api-reference/beta/resources/intune_apps_iosvppapp.md). |
| Изменение      | Бета    | Добавлены свойства **deviceEnrollmentType**, **wiFiMacAddress** и **deviceHealthAttestationState** для объекта [managedDevice](../api-reference/beta/resources/intune_deviceconfig_manageddevice.md). |
| Изменение      | Бета    | Добавлено свойство **legacyAppConfiguration** для объекта [managedDeviceMobileAppConfiguration](../api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration.md). |
| Изменение      | Бета    | Добавлено свойство **notApplicableCount** для объекта [managedDeviceMobileAppConfigurationDeviceSummary](../api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md). |
| Изменение      | Бета    | Добавлено свойство **notApplicableCount** для объекта [managedDeviceMobileAppConfigurationUserSummary](../api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationusersummary.md). |
| Изменение      | Бета    | Добавлены свойства **firewallBlockStatefulFTP**, **firewallIdleTimeoutForSecurityAssociationInSeconds**, **firewallPreSharedKeyEncodingMethod**, **firewallIPSecExemptionsAllowNeighborDiscovery**, **firewallIPSecExemptionsAllowICMP**, **firewallIPSecExemptionsAllowRouterDiscovery**, **firewallIPSecExemptionsAllowDHCP**, **firewallCertificateRevocationListCheckMethod**, **firewallMergeKeyingModuleSettings**, **firewallPacketQueueingMethod**, **firewallProfileDomain**, **firewallProfilePublic**, **firewallProfilePrivate**, **defenderAttackSurfaceReductionExcludedPaths**, **defenderOfficeAppsOtherProcessInjectionType**, **defenderOfficeAppsExecutableContentCreationOrLaunchType**, **defenderOfficeAppsLaunchChildProcessType**, **defenderOfficeMacroCodeAllowWin32ImportsType**, **defenderScriptObfuscatedMacroCodeType**, **defenderScriptDownloadedPayloadExecutionType**, **defenderEmailContentExecutionType**, **defenderGuardMyFoldersType**, **defenderGuardedFoldersAllowedAppPaths**, **defenderAdditionalGuardedFolders**, **defenderNetworkProtectionType**, **defenderExploitProtectionXml**, **defenderExploitProtectionXmlFileName**, **defenderSecurityCenterBlockExploitProtectionOverride**, **appLockerApplicationControl**, **applicationGuardBlockClipboardSharing**, **applicationGuardAllowPrintToPDF**, **applicationGuardAllowPrintToXPS**, **applicationGuardAllowPrintToLocalPrinters**, **applicationGuardAllowPrintToNetworkPrinters** и **bitLockerDisableWarningForOtherDiskEncryption** для объекта [windows10EndpointProtectionConfiguration](../api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md). |
| Изменение      | Бета    | Добавлены свойства **displayAppListWithGdiDPIScalingTurnedOn**, **displayAppListWithGdiDPIScalingTurnedOff**, **messagingBlockSync**, **messagingBlockMMS** и **messagingBlockRichCommunicationServices** для объекта [windows10GeneralConfiguration](../api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration.md). |
| Изменение      | Бета    | Удалено свойство **bluetoothDeviceName** объекта [windows10GeneralConfiguration](../api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration.md). |
| Изменение      | Бета    | Удалены свойства **deviceAccountBlockExchangeServices**, **deviceAccountEmailAddress**, **deviceAccountExchangeServerAddress**, **deviceAccountRequirePasswordRotation** и **deviceAccountSessionInitiationProtocolAddress** объекта [windows10TeamGeneralConfiguration](../api-reference/beta/resources/intune_deviceconfig_windows10teamgeneralconfiguration.md). |
| Изменение      | Бета    | Добавлено свойство навигации **localActions** для объекта [androidCompliancePolicy](../api-reference/beta/resources/intune_deviceconfig_androidcompliancepolicy.md). |
| Изменение      | Бета    | Добавлены свойства навигации **windowsAutopilotSettings**, **windowsAutopilotDeviceIdentities**, **windowsAutopilotDeploymentProfiles**, **deviceEnrollmentConfigurations**, **deviceManagementPartners** и **depOnboardingSettings** для объекта [deviceManagement](../api-reference/beta/resources/intune_androidforwork_devicemanagement.md). |
| Изменение      | Бета    | Удалено свойство навигации **cloudPkiSubscriptions** объекта [deviceManagement](../api-reference/beta/resources/intune_androidforwork_devicemanagement.md). |
| Изменение      | Бета    | Добавлено свойство навигации **assignments** для объекта [targetedManagedAppConfiguration](../api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration.md). |
| Изменение      | Бета    | Добавлено свойство навигации **assignments** для объекта [targetedManagedAppProtection](../api-reference/beta/resources/intune_mam_targetedmanagedappprotection.md). |
| Изменение      | Бета    | Добавлено свойство навигации **assignments** для объекта [windowsInformationProtection](../api-reference/beta/resources/intune_mam_windowsinformationprotection.md). |

### <a name="onedrive"></a>OneDrive

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлено свойство **system** для ресурса [Drive][]. |
| Дополнение        | 1.0        | Добавлена связь **list** для ресурса [Drive][]. |
| Дополнение        | 1.0        | Добавлена связь **listItem** для ресурса [DriveItem][]. |
| Дополнение        | 1.0        | Добавлены связи **list** и **listItem** для ресурса [SharedDriveItem][]. |
| Дополнение        | 1.0        | Добавлены новые сложные типы: [FolderView][]  |
| Дополнение        | 1.0        | Добавлено свойство **view** для сложного типа [Folder][]. |
| Дополнение        | 1.0        | Добавлено свойство **driveType** для сложного типа [ItemReference][]. |
| Дополнение        | 1.0        | Добавлены свойства **audioBitsPerSample**, **audioChannels**, **audioFormat**, **audioSamplesPerSecond**, **fourCC** и **frameRate** для сложного типа [Video][]. |
| Дополнение        | Бета        | Добавлено свойство **system** для ресурса [Drive][Drive-beta]. |
| Дополнение        | Бета        | Добавлена связь **activities** для ресурса [Drive][Drive-beta]. |
| Дополнение        | Бета        | Добавлено свойство **publication** для ресурса [DriveItem][DriveItem-beta]. |
| Дополнение        | Бета        | Добавлены связи **activities** и **versions** для ресурса [DriveItem][DriveItem-beta]. |
| Дополнение        | Бета        | Добавлены новые объекты: [DriveItemVersion][DriveItemVersion-beta], [ItemActivity][ItemActivity-beta]. |
| Дополнение        | Бета        | Добавлены новые сложные типы: [CommentAction][CommentAction-beta], [CreateAction][CreateAction-beta], [DeleteAction][DeleteAction-beta], [EditAction][EditAction-beta], [ItemActionSet][ItemActionSet-beta], [ItemActivityTimeSet][ItemActivityTimeSet-beta], [MentionAction][MentionAction-beta], [MoveAction][MoveAction-beta], [PublicationFacet][PublicationFacet-beta], [RenameAction][RenameAction-beta], [RestoreAction][RestoreAction-beta], [ShareAction][ShareAction-beta] и [VersionAction][VersionAction-beta]. |
| Дополнение        | Бета        | Добавлено свойство **driveType** для сложного типа [ItemReference][ItemReference-beta]. |
| Удаление        | Бета        | Удалено свойство **tenantId** сложного типа [SharepointIds][SharepointIds-beta]. |
| Дополнение        | 1.0        | Добавлены свойства **audioBitsPerSample**, **audioChannels**, **audioFormat**, **audioSamplesPerSecond**, **fourCC** и **frameRate** для сложного типа [Video][Video-beta]. |
| Дополнение        | Бета        | Добавлены действия [CheckIn][CheckIn-beta] и [CheckOut][CheckOut-beta] для ресурса [DriveItem][DriveItem-beta]. |
| Дополнение        | Бета        | Добавлены свойства **expirationDateTime**, **password**, **message** и **recipients** для действия [CreateLink][CreateLink-beta] ресурса [DriveItem][DriveItem-beta]. |

[Drive]: ../api-reference/v1.0/resources/drive.md
[DriveItem]: ../api-reference/v1.0/resources/driveitem.md
[SharedDriveItem]: ../api-reference/v1.0/resources/shareddriveitem.md
[FolderView]: ../api-reference/v1.0/resources/folderview.md
[Folder]: ../api-reference/v1.0/resources/folder.md
[ItemReference]: ../api-reference/v1.0/resources/itemreference.md
[Video]: ../api-reference/v1.0/resources/video.md
[Drive-beta]: ../api-reference/beta/resources/drive.md
[DriveItem-beta]: ../api-reference/beta/resources/driveitem.md
[DriveItemVersion-beta]: ../api-reference/beta/resources/driveitemversion.md
[ItemActivity-beta]: ../api-reference/beta/resources/itemactivity.md
[CommentAction-beta]: ../api-reference/beta/resources/commentaction.md
[CreateAction-beta]: ../api-reference/beta/resources/createaction.md
[DeleteAction-beta]: ../api-reference/beta/resources/deleteaction.md
[EditAction-beta]: ../api-reference/beta/resources/editaction.md
[ItemActionSet-beta]: ../api-reference/beta/resources/itemactionset.md
[ItemActivityTimeSet-beta]: ../api-reference/beta/resources/itemactivitytimeset.md
[MentionAction-beta]: ../api-reference/beta/resources/mentionaction.md
[MoveAction-beta]: ../api-reference/beta/resources/moveaction.md
[PublicationFacet-beta]: ../api-reference/beta/resources/publicationfacet.md
[RenameAction-beta]: ../api-reference/beta/resources/renameaction.md
[RestoreAction-beta]: ../api-reference/beta/resources/restoreaction.md
[ShareAction-beta]: ../api-reference/beta/resources/shareaction.md
[VersionAction-beta]: ../api-reference/beta/resources/versionaction.md
[ItemReference-beta]: ../api-reference/beta/resources/itemreference.md
[SharepointIds-beta]: ../api-reference/beta/resources/sharepointids.md
[Video-beta]: ../api-reference/beta/resources/video.md
[CheckIn-beta]: ../api-reference/beta/api/driveitem_checkin.md
[CheckOut-beta]: ../api-reference/beta/api/driveitem_checkout.md
[CreateLink-beta]: ../api-reference/beta/api/driveitem_createlink.md


### <a name="outlook-calendar"></a>Календарь Outlook

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | Бета          | Добавлены функции [findRoomLists](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/user_findroomlists) и [findRooms](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/user_findrooms) для объекта [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/user). |
| Дополнение        | Бета          | Добавлено свойство **locations** для объекта [event](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/event), позволяющее организовать событие, в котором могут участвовать пользователи из нескольких расположений. |
| Дополнение        | Бета          | Добавлено свойство **locationType** для сложного типа [location](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/location). |
| Дополнение        | Бета          | Добавлены свойства **uniqueId** и **uniqueIdType** для сложного типа [location](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/location). В настоящее время эти свойства предназначены только для внутреннего использования. |
| Изменение          | 1.0 и бета-версия | Это улучшение поведения связано с получением общего календаря или содержимого событий в нем, если кто-то предоставил вошедшему пользователю доступ к календарю или делегировал ему почтовый ящик пользователя. В таких случаях приложение может указать ИД пользователя или имя участника-пользователя, чтобы [получить этот общий календарь](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/calendar_get) или [получить события из этого общего календаря](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/user_list_events), при условии что вошедший пользователь предоставил приложению делегированные разрешения. |

### <a name="outlook-contacts"></a>Контакты Outlook

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Это улучшение поведения связано с получением общей папки контактов или содержимого контактов в ней, если кто-то предоставил вошедшему пользователю доступ к папке контактов или делегировал ему почтовый ящик пользователя. В таких случаях приложение может указать ИД пользователя или имя участника-пользователя, чтобы [получить эту общую папку контактов](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/contactfolder_get) или [получить контакты из этой общей папки](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/user_list_contacts), при условии что вошедший пользователь предоставил приложению делегированные разрешения. |

### <a name="outlook-mail"></a>Почта Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлено свойство **internetMessageHeaders** для объекта [message](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/message). |
| Дополнение        | Бета        | Добавлен сложный тип [internetMessageHeader](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/internetmessageheader). |
| Дополнение        | Бета        | Добавлено свойство навигации **messageRules** для объекта [mailFolder](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/mailfolder). **messageRules** — это набор экземпляров [messageRule](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/messagerule). |
| Дополнение        | Бета        | Добавлены объект [messageRule](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/messagerule) и сложные типы [messageRuleActions](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/messageruleactions), [messageRulePredicates](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/messagerulepredicates) и [sizeRange](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/sizerange). |
| Дополнение        | Бета        | Добавлены следующие операции CRUD для правил обработки сообщений: [create](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/mailfolder_post_messagerules), [list](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/mailfolder_list_messagerules), [get](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/messagerule_get), [update](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/messagerule_update) и [delete](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/messagerule_delete). |


### <a name="outlook-user-choices"></a>Настройки пользователей Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлено новое свойство навигации **masterCategories** для объекта [outlookUser](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/outlookuser). **masterCategories** — это коллекция объектов [outlookCategory](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/outlookCategory). |
| Дополнение        | Бета        | Добавлен объект [outlookCategory](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/outlookCategory). |
| Дополнение        | Бета        | Добавлены следующие операции CRUD для объекта [outlookCategory](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/outlookCategory): [создание](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/outlookuser_post_mastercategories), [получение](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/outlookcategory_get), [обновление](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/outlookcategory_update) и [удаление](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/outlookcategory_delete). |
| Дополнение        | Бета        | Добавлена новая функция [supportedLanguages](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/outlookuser_supportedlanguages) для объекта [outlookUser](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/outlookuser). |
| Дополнение        | Бета        | Добавлена новая функция [supportedTimeZones](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/outlookuser_supportedtimezones) для объекта [outlookUser](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/outlookuser). |


### <a name="sharepoint-lists"></a>Списки SharePoint

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлены новые объекты: [ColumnDefinition][], [ColumnLink][], [ContentType][], [List][], [ListItem][]. |
| Дополнение        | 1.0        | Добавлены связи **columns**, **contentTypes**, **items** и **lists** для ресурса [Site][]. |
| Дополнение        | 1.0        | Добавлены новые сложные типы: [BooleanColumn][], [CalculatedColumn][], [ChoiceColumn][], [ContentTypeInfo][], [ContentTypeOrder][], [CurrencyColumn][], [DateTimeColumn][], [DefaultColumnValue][], [ListInfo][], [LookupColumn][], [NumberColumn][], [PersonOrGroupColumn][], [SystemFacet][], [TextColumn][]. |
| Дополнение        | Бета        | Добавлены новые объекты: [BaseItemVersion][BaseItemVersion-beta], [ColumnLink][ColumnLink-beta], [ContentType][ContentType-beta], [ListItemVersion][ListItemVersion-beta]. |
| Дополнение        | Бета        | Добавлены свойства **columnGroup**, **currency**, **defaultValue** и **displayName** для объекта [ColumnDefinition][ColumnDefinition-beta]. |
| Дополнение        | Бета        | Добавлены свойства **displayName** и **system** для ресурса [List][List-beta]. |
| Дополнение        | Бета        | Добавлены связи **activities** и **contentTypes** для ресурса [List][List-beta]. |
| Дополнение        | Бета        | Добавлено свойство **contentType** для ресурса [ListItem][ListItem-beta]. |
| Дополнение        | Бета        | Добавлены связи **activities** и **versions** для ресурса [ListItem][ListItem-beta]. |
| Дополнение        | Бета        | Добавлена связь **contentTypes** для ресурса [Site][Site-beta]. |
| Дополнение        | Бета        | Добавлено свойство **outputType** для типа [BooleanColumn][BooleanColumn-beta]. |
| Дополнение        | Бета        | Добавлены новые сложные типы: [ContentTypeInfo][ContentTypeInfo-beta], [ContentTypeOrder][ContentTypeOrder-beta], [CurrencyColumn][CurrencyColumn-beta] и [SystemFacet][SystemFacet-beta]. |
| Дополнение        | Бета        | Добавлено свойство **contentTypesEnabled** для сложного типа [ListInfo][ListInfo-beta]. |
| Дополнение        | Бета        | Добавлено свойство **allowUnlimitedLength** для сложного типа [LookupColumn][LookupColumn-beta]. |
| Изменение          | Бета        | Имя свойства **allowMultipleValue** изменено на **allowMultipleValues** для сложного типа [LookupColumn][LookupColumn-beta]. |
| Изменение          | Бета        | Имя свойства **chooseFrom** изменено на **chooseFromType** для сложного типа [PersonOrGroupColumn][PersonOrGroupColumn-beta]. |
| Удаление        | Бета        | Удалено свойство **locale** сложного типа [NumberColumn][NumberColumn-beta]. |
| Удаление        | Бета        | Удалено свойство **enforceUniqueValues** сложного типа [PersonOrGroupColumn][PersonOrGroupColumn-beta]. |

[BaseItemVersion-beta]: ../api-reference/beta/resources/baseitemversion.md
[BooleanColumn-beta]:  ../api-reference/beta/resources/booleanColumn.md
[BooleanColumn]: ../api-reference/v1.0/resources/booleancolumn.md
[CalculatedColumn]: ../api-reference/v1.0/resources/calculatedcolumn.md
[ChoiceColumn]: ../api-reference/v1.0/resources/choicecolumn.md
[ColumnDefinition-beta]: ../api-reference/beta/resources/columndefinition.md
[ColumnDefinition]: ../api-reference/v1.0/resources/columndefinition.md
[ColumnLink-beta]: ../api-reference/beta/resources/columnLink.md
[ColumnLink]: ../api-reference/v1.0/resources/columnLink.md
[ContentType-beta]: ../api-reference/beta/resources/contentType.md
[ContentType]: ../api-reference/v1.0/resources/contentType.md
[ContentTypeInfo-beta]: ../api-reference/beta/resources/contentTypeInfo.md
[ContentTypeInfo]: ../api-reference/v1.0/resources/contentTypeInfo.md
[ContentTypeOrder-beta]: ../api-reference/beta/resources/contentTypeOrder.md
[ContentTypeOrder]: ../api-reference/v1.0/resources/contentTypeOrder.md
[CurrencyColumn-beta]: ../api-reference/beta/resources/currencycolumn.md
[CurrencyColumn]: ../api-reference/v1.0/resources/currencycolumn.md
[DateTimeColumn]: ../api-reference/v1.0/resources/datetimecolumn.md
[DefaultColumnValue]: ../api-reference/v1.0/resources/defaultColumnValue.md
[List-beta]: ../api-reference/beta/resources/list.md
[List]: ../api-reference/v1.0/resources/list.md
[ListInfo-beta]: ../api-reference/beta/resources/listinfo.md
[ListInfo]: ../api-reference/v1.0/resources/listinfo.md
[ListItem-beta]: ../api-reference/beta/resources/listitem.md
[ListItem]: ../api-reference/v1.0/resources/listitem.md
[ListItemVersion-beta]: ../api-reference/beta/resources/listitemversion.md
[LookupColumn-beta]: ../api-reference/beta/resources/lookupColumn.md
[LookupColumn]: ../api-reference/v1.0/resources/lookupcolumn.md
[NumberColumn-beta]: ../api-reference/beta/resources/numberColumn.md
[NumberColumn]: ../api-reference/v1.0/resources/numbercolumn.md
[PersonOrGroupColumn-beta]: ../api-reference/beta/resources/personOrGroupColumn.md
[PersonOrGroupColumn]: ../api-reference/v1.0/resources/personorgroupcolumn.md
[Site-beta]: ../api-reference/beta/resources/site.md
[Site]: ../api-reference/v1.0/resources/site.md
[SystemFacet-beta]: ../api-reference/beta/resources/systemfacet.md
[SystemFacet]: ../api-reference/v1.0/resources/systemFacet.md
[TextColumn]: ../api-reference/v1.0/resources/textcolumn.md


### <a name="sharepoint-sites"></a>Сайты SharePoint

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлены свойства **dataLocationCode** и **root** для сложного типа [SiteCollection][SiteCollection-beta]. |

[SiteCollection-beta]: ../api-reference/beta/resources/sitecollection.md


## <a name="august-2017"></a>Август 2017 г.

### <a name="group-lifecycle-policy"></a>Политика жизненного цикла группы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлена сущность [groupLifecyclePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/grouplifecyclepolicy). |
| Дополнение        | Бета        | Добавлены следующие API для политики жизненного цикла группы, а именно для: [создания](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/grouplifecyclepolicy_post_grouplifecyclepolicies), [перечисления](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/grouplifecyclepolicy_list), [получения](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/grouplifecyclepolicy_get), [обновления](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/grouplifecyclepolicy_update), [удаления](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/grouplifecyclepolicy_delete), [добавления группы](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/grouplifecyclepolicy_addgroup), [удаления группы](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/grouplifecyclepolicy_removegroup) и [возобновления группы](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/grouplifecyclepolicy_renewgroup). |
| Дополнение        | Бета        | Добавлена функция [List groupLifecylePolicies](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/group_list_grouplifecyclepolicies.md) для объекта [group](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/group). |

### <a name="intune-apis"></a>API Intune
| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета-версия    | Добавлен новый объект:<br/>[windowsPrivacyDataAccessControlItem](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsprivacydataaccesscontrolitem)<br/> |
| Дополнение    | Бета    | Добавлены новые сложные типы:<br/>[configurationManagerClientEnabledFeatures](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devices_configurationmanagerclientenabledfeatures)<br/>[windowsDefenderScanActionResult](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devices_windowsdefenderscanactionresult)<br/> |
| Дополнение    | Бета-версия    | Добавлено действие [windowsDefenderScan](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_devices_manageddevice_windowsdefenderscan.md) для [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Дополнение    | Бета-версия    | Добавлено действие [windowsDefenderUpdateSignatures](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_devices_manageddevice_windowsdefenderupdatesignatures.md) для [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Дополнение    | Бета-версия    | Добавлено действие [windowsPrivacyAccessControls](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_deviceconfig_deviceconfiguration_windowsprivacyaccesscontrols.md) для [deviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) |
| Изменение      | Бета-версия    | Добавлены свойства **automaticallyUpdateApps** и **countryOrRegion** для объекта [appleVolumePurchaseProgramToken](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_applevolumepurchaseprogramtoken) |
| Изменение      | Бета-версия    | Добавлено свойство **enableAuthenticationViaCompanyPortal** для объекта [depEnrollmentProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_corpenrollment_depenrollmentprofile) |
| Изменение      | Бета-версия    | Добавлено свойство **notificationMessageCCList** для объекта [deviceComplianceActionItem](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceactionitem) |
| Изменение      | Бета-версия    | Добавлено свойство **notApplicableCount** для объекта [deviceComplianceDeviceOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview) |
| Изменение      | Бета-версия    | Добавлено свойство **notApplicableCount** для объекта [deviceComplianceUserOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview) |
| Изменение      | Бета-версия    | Добавлено свойство **notApplicableCount** для объекта [deviceConfigurationDeviceOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview) |
| Изменение      | Бета-версия    | Добавлено свойство **notApplicableCount** для объекта [deviceConfigurationUserOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview) |
| Изменение      | Бета-версия    | Добавлено свойство **configurationManagerClientEnabledFeatures** для объекта [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Изменение      | Бета-версия    | Удалено свойство **intuneBrand** для объекта [organization](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_organization) |
| Изменение      | Бета-версия    | Добавлены свойства **smartScreenEnableInShell**, **smartScreenBlockOverrideForFiles**, **applicationGuardEnabled**, **applicationGuardBlockFileTransfer**, **applicationGuardBlockNonEnterpriseContent**, **applicationGuardAllowPersistence** и **applicationGuardForceAuditing** для объекта [windows10EndpointProtectionConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration) |
| Изменение      | Бета-версия    | Добавлены свойства **searchBlockDiacritics**, **searchDisableAutoLanguageDetection**, **searchDisableIndexingEncryptedItems**, **searchEnableRemoteQueries**, **searchDisableUseLocation**, **searchDisableIndexerBackoff**, **searchDisableIndexingRemovableDrive**, **searchEnableAutomaticIndexSizeManangement**, **smartScreenEnableAppInstallControl** и **privacyAdvertisingId** для объекта [windows10GeneralConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) |
| Изменение      | Бета-версия    | Удалено свойство **settingsDeviceName** для объекта [windows10TeamGeneralConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10teamgeneralconfiguration) |
| Изменение      | Бета-версия    | Удалено свойство **restartMode** для объекта [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration) |
| Изменение      | Бета-версия    | Добавлены свойства навигации **detectedApps** и **managedDevices** для объекта [deviceManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) |
| Изменение      | Бета-версия    | Добавлено свойство навигации **privacyAccessControls** для объекта [windows10GeneralConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) |
| Изменение      | Бета-версия    | Добавлено свойство **secureByDefault** для сложного типа [deviceManagementSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) |
| Изменение      | Бета-версия    | Добавлено свойство **restartMode** для сложного типа [windowsUpdateScheduledInstall](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdatescheduledinstall) |

### <a name="onenote"></a>OneNote

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Добавлено свойство навигации [onenote](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/onenote) для **site**. |
| Дополнение        | Бета          | Добавлены целевые параметры *siteCollectionId* и *siteId* для операций копирования. Пример: [CopyNotebook](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/notebook_copynotebook). |

### <a name="people"></a>Люди 

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | В версии 1.0 добавлены [API People](../api-reference/v1.0/resources/person.md). Дополнительные сведения об API People см. в статье, посвященной [получению релевантных сведений о пользователях](people_example.md). |

### <a name="user"></a>Пользователь

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлено свойство **employeeId** для [user](../api-reference/beta/resources/user.md). |

## <a name="july-2017"></a>Июль 2017 г.

### <a name="group-settings"></a>Параметры группы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлена поддержка параметров группы.<br/>Новые типы ресурсов: [groupSetting](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/groupsetting.md), [groupSettingTemplate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/groupsettingtemplate.md), [settingValue](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/settingvalue.md) и [settingTemplateValue](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/settingtemplatevalue.md). |
| Изменение          | 1.0        | Добавлено свойство **classification** и свойство навигации **settings** для [group](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/group.md). |

### <a name="intune-apis"></a>API Intune

| Тип&nbsp;изменения | Версия | Описание                              |
| :--------------- | :------ | :--------------------------------------- |
| Дополнение         | Бета-версия    | Добавлено действие [assign](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_apps_iosmobileappconfiguration_assign) для объекта [iosMobileAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_iosmobileappconfiguration). |
| Дополнение         | Бета-версия    | Добавлено действие [syncDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_devices_manageddevice_syncdevice) для объекта [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
| Изменение           | Бета-версия    | Добавлены свойства **appsInstallAllowList**, **appsLaunchBlockList** и **appsHideList** для объекта [androidGeneralDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration). |
| Изменение           | Бета-версия    | Добавлено свойство **disableAppEncryptionIfDeviceEncryptionIsEnabled** для объекта [androidManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection). |
| Изменение           | Бета-версия    | Добавлено свойство **disableAppEncryptionIfDeviceEncryptionIsEnabled** для объекта [defaultManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection). |
| Изменение           | Бета-версия    | Добавлено свойство **complianceGracePeriodExpirationDateTime** для объекта [deviceComplianceDeviceStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus). |
| Изменение           | Бета-версия    | Добавлено свойство **complianceGracePeriodExpirationDateTime** для объекта [deviceComplianceSettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate). |
| Изменение           | Бета-версия    | Добавлено свойство **complianceGracePeriodExpirationDateTime** для объекта [deviceConfigurationDeviceStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus). |
| Изменение           | Бета-версия    | Добавлено свойство **subscriptions** для объекта [deviceManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement). |
| Изменение           | Бета-версия    | Добавлено свойство **version** для объекта [deviceManagementExchangeConnector](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_devicemanagementexchangeconnector). |
| Изменение           | Бета-версия    | Добавлено свойство **utcTimeOffsetInMinutes** для объекта [iosUpdateConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdateconfiguration). |
| Изменение           | Бета-версия    | Добавлено свойство **complianceGracePeriodExpirationDateTime** для объекта [iosUpdateDeviceStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdatedevicestatus). |
| Изменение           | Бета-версия    | Добавлено свойство **preSharedKey** для объекта [macOSWiFiConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoswificonfiguration). |
| Изменение           | Бета-версия    | Добавлены свойства **phoneNumber**, **androidSecurityPatchLevel** и **userDisplayName** для объекта [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
| Изменение           | Бета-версия    | Добавлены свойства **userName**, **deviceModel**, **platform** и **complianceGracePeriodExpirationDateTime** для объекта [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus). |
| Изменение           | Бета-версия    | Добавлено свойство **userPrincipalName** для объекта [mobileAppInstallStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus). |
| Изменение           | Бета-версия    | Добавлено свойство **overrideDefaultRule** для объекта [onPremisesConditionalAccessSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_onpremisesconditionalaccesssettings). |
| Изменение           | Бета-версия    | Добавлено свойство **userPrincipalName** для объекта [userAppInstallStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_userappinstallstatus). |
| Изменение           | Бета-версия    | Добавлены свойства **connectAppBlockAutoLaunch**, **deviceAccountBlockExchangeServices**, **deviceAccountEmailAddress**, **deviceAccountExchangeServerAddress**, **deviceAccountRequirePasswordRotation**, **deviceAccountSessionInitiationProtocolAddress**, **settingsBlockMyMeetingsAndFiles**, **settingsBlockSessionResume**, **settingsBlockSigninSuggestions**, **settingsDefaultVolume**, **settingsScreenTimeoutInMinutes**, **settingsSessionTimeoutInMinutes** и **settingsSleepTimeoutInMinutes** для объекта [windows10TeamGeneralConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10teamgeneralconfiguration). |
| Изменение           | Бета-версия    | Добавлено свойство навигации **deploymentSummary** для объекта [defaultManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection). |
| Изменение           | Бета-версия    | Добавлены свойства **settingName**, **userId**, **userName**, **userEmail** и **currentValue** к сложному типу [deviceCompliancePolicySettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate). |
| Изменение           | Бета    | Для сложного типа [deviceConfigurationSettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) добавлены свойства **settingName**, **userId**, **userName**, **userEmail** и **currentValue** |
| Изменение           | Бета-версия    | Добавлено свойство **unknownCount** к сложному типу [deviceOperatingSystemSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devices_deviceoperatingsystemsummary). |



## <a name="june-2017"></a>Июнь 2017 г.

### <a name="project-rome"></a>Project Rome

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлены следующие ресурсы и API:<br/>[Действие](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/projectrome_activity)<br/>[Создание или замена действия](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/projectrome_put_activity)<br/>[Удаление действия](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/projectrome_delete_activity)<br/>[Элемент журнала](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/projectrome_historyitem)<br/>[Создание или замена элемента журнала](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/projectrome_put_historyitem)<br/>[Удаление элемента журнала](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/projectrome_delete_historyitem) |

### <a name="outlook-calendar"></a>Календарь Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Повышен уровень для следующих 4 свойств [calendar](https://graph.microsoft.io/ru-RU/docs/api-reference/v1.0/resources/calendar) до версии 1.0: **canEdit**, **canShare**, **canViewPrivateItems** и **owner**. |


### <a name="intune-apis"></a>Интерфейсы API Intune

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета    | Добавлены новые объекты:<br/>[defaultDeviceCompliancePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_defaultdevicecompliancepolicy);<br/>[deviceConfigurationUserStateSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuserstatesummary);<br/>[deviceManagementScriptDeviceState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptdevicestate);<br/>[deviceManagementScriptRunSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptrunsummary);<br/>[deviceManagementScriptUserState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptuserstate);<br/>[iosUpdateDeviceStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdatedevicestatus);<br/>[windowsManagedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanageddevice);<br/>[windowsManagementAppHealthState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapphealthstate);<br/>[windowsManagementAppHealthSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapphealthsummary).<br/> |
| Дополнение    | Бета    | Добавлены новые сложные типы:<br/>[bitLockerFixedDrivePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerfixeddrivepolicy);<br/>[bitLockerRecoveryOptions](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerrecoveryoptions);<br/>[bitLockerRemovableDrivePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerremovabledrivepolicy);<br/>[deleteUserFromSharedAppleDeviceActionResult](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devicefe_deleteuserfromsharedappledeviceactionresult);<br/>[iosNetworkUsageRule](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnetworkusagerule).<br/> |
| Удаление    | Бета-версия    | Удалены следующие объекты:<br/>**deviceManagementScriptState**.<br/> |
| Удаление    | Бета-версия    | Удалено действие wipeByDeviceTag для [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devicefe_user). |
| Изменение      | Бета-версия    | Добавлены свойства **innerAuthenticationProtocolForEapTtls**, **innerAuthenticationProtocolForPeap** и **outerIdentityPrivacyTemporaryValue** для объекта [androidEnterpriseWiFiConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidenterprisewificonfiguration). |
| Изменение      | Бета-версия    | Удалены свойства **nonEapAuthenticationMethodForEapTtls**, **nonEapAuthenticationMethodForPeap** и **enableOuterIdentityPrivacy** для объекта [androidEnterpriseWiFiConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidenterprisewificonfiguration). |
| Изменение      | Бета-версия    | Добавлено свойство **deployedAppCount** для объекта [androidManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection). |
| Изменение      | Бета-версия    | Удалены свойства **instanceDisplayName** и **settingPlatform** для объекта [complianceSettingStateSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/complianceSettingStateSummary). |
| Изменение      | Бета-версия    | Добавлено свойство **deployedAppCount** для объекта [defaultManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection). |
| Изменение      | Бета    | Добавлено свойство **excludeGroup** для объекта [deviceCompliancePolicyGroupAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicygroupassignment) |
| Изменение      | Бета-версия    | Удалены свойства **instanceDisplayName** и **settingPlatform** для объекта [deviceCompliancePolicySettingStateSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary). |
| Изменение      | Бета-версия    | Удалено свойство **devicePlatform** для объекта [deviceComplianceSettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate). |
| Изменение      | Бета-версия    | Добавлены свойства **assignmentStatus**, **assignmentProgress** и **assignmentErrorMessage** для объекта [deviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration). |
| Изменение      | Бета-версия    | Добавлено свойство **intuneBrand** для объекта [deviceManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement). |
| Изменение      | Бета-версия    | Добавлены свойства **enforceSignatureCheck** и **fileName** для объекта [deviceManagementScript](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript). |
| Изменение      | Бета-версия    | Добавлены свойства **innerAuthenticationProtocolForEapTtls** и **outerIdentityPrivacyTemporaryValue** для объекта [iosEnterpriseWiFiConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosenterprisewificonfiguration). |
| Изменение      | Бета-версия    | Удалены свойства **nonEapAuthenticationMethodForEapTtls** и **enableOuterIdentityPrivacy** для объекта [iosEnterpriseWiFiConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosenterprisewificonfiguration). |
| Изменение      | Бета-версия    | Добавлены свойства **classroomAppForceUnpromptedScreenObservation**, **keyboardBlockDictation**, **networkUsageRules** и **wiFiConnectOnlyToConfiguredNetworks** для объекта [iosGeneralDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration). |
| Изменение      | Бета-версия    | Добавлено свойство **deployedAppCount** для объекта [iosManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection). |
| Изменение      | Бета-версия    | Добавлено свойство **preSharedKey** для объекта [iosWiFiConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswificonfiguration). |
| Изменение      | Бета-версия    | Добавлены свойства **innerAuthenticationProtocolForEapTtls** и **outerIdentityPrivacyTemporaryValue** для объекта [macOSEnterpriseWiFiConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosenterprisewificonfiguration). |
| Изменение      | Бета-версия    | Удалены свойства **nonEapAuthenticationMethodForEapTtls** и **enableOuterIdentityPrivacy** для объекта [macOSEnterpriseWiFiConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosenterprisewificonfiguration). |
| Изменение      | Бета-версия    | Удалены свойства **lastModifiedTime** и **deployedAppCount** для объекта [managedAppPolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy). |
| Изменение      | Бета-версия    | Добавлено свойство **serialNumber** для объекта [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
| Изменение      | Бета-версия    | Удалено свойство **managementAgents** для объекта [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
| Изменение      | Бета-версия    | Добавлено свойство **deployedAppCount** для объекта [targetedManagedAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration). |
| Изменение      | Бета-версия    | Добавлены свойства **bitLockerFixedDrivePolicy** и **bitLockerRemovableDrivePolicy** для объекта [windows10EndpointProtectionConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration). |
| Изменение      | Бета-версия    | Добавлены свойства **enterpriseCloudPrintDiscoveryEndPoint**, **enterpriseCloudPrintOAuthAuthority**, **enterpriseCloudPrintOAuthClientIdentifier**, **enterpriseCloudPrintResourceIdentifier**, **enterpriseCloudPrintDiscoveryMaxLimit**, **enterpriseCloudPrintMopriaDiscoveryResourceIdentifier**, **edgeBlockAddressBarDropdown**, **edgeBlockCompatibilityList**, **edgeClearBrowsingDataOnExit**, **edgeAllowStartPagesModification**, **edgeDisableFirstRunPage**, **edgeBlockLiveTileDataCollection** и **edgeSyncFavoritesWithInternetExplorer** для объекта [windows10GeneralConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration). |
| Изменение      | Бета-версия    | Добавлено свойство **availableVersion** для объекта [windowsManagementApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp). |
| Изменение      | Бета-версия    | Удалены свойства **onboardingStatus**, **deployedVersion** и **lastModifiedTime** для объекта [windowsManagementApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp). |
| Изменение      | Бета-версия    | Добавлено свойство **packageIdentityName** для объекта [windowsStoreForBusinessApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessapp). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **mobileAppIdentifierDeployments** и **deploymentSummary** для объекта [androidManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **mobileAppIdentifierDeployments** для объекта [defaultManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **deviceConfigurationUserStateSummaries** и **iosUpdateStatuses** для объекта [deviceManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement). |
| Изменение      | Бета-версия    | Удалено свойство навигации **complianceSettingStateSummaries** для объекта [deviceManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **runSummary**, **deviceRunStates** и **userRunStates** для объекта [deviceManagementScript](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript). |
| Изменение      | Бета-версия    | Удалено свойство навигации **runStates** для объекта [deviceManagementScript](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **mobileAppIdentifierDeployments** и **deploymentSummary** для объекта [iosManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection). |
| Изменение      | Бета-версия    | Удалены свойства навигации **mobileAppIdentifierDeployments** и **deploymentSummary** для объекта [managedAppPolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **mobileAppIdentifierDeployments** и **deploymentSummary** для объекта [targetedManagedAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **healthSummary** и **healthStates** для объекта [windowsManagementApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp). |
| Изменение      | Бета-версия    | Добавлены свойства **applicationId**, **appName**, **platformId**, **userFailures** и **deviceFailures** для сложного типа [appInstallationFailure](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure). |
| Изменение      | Бета-версия    | Добавлены свойства **encryptionMethod**, **startupAuthenticationRequired**, **startupAuthenticationBlockWithoutTpmChip**, **startupAuthenticationTpmUsage**, **startupAuthenticationTpmPinUsage**, **startupAuthenticationTpmKeyUsage**, **startupAuthenticationTpmPinAndKeyUsage**, **recoveryOptions** и **prebootRecoveryEnableMessageAndUrl** для сложного типа [bitLockerSystemDrivePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockersystemdrivepolicy). |
| Изменение      | Бета-версия    | Удалены свойства **settingName**, **userId**, **userName**, **userEmail** и **currentValue** для сложного типа [deviceCompliancePolicySettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate). |
| Изменение      | Бета-версия    | Удалены свойства **settingName**, **userId**, **userName**, **userEmail** и **currentValue** для сложного типа [deviceConfigurationSettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate). |
| Изменение      | Бета-версия    | Добавлены свойства **windowsCommercialId** и **windowsCommercialIdLastModifiedTime** для сложного типа [deviceManagementSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings). |
| Изменение      | Бета-версия    | Добавлено свойство **address** для сложного типа [vpnServer](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_vpnserver). |


## <a name="may-2017"></a>Май 2017 г.

### <a name="application-api-changes"></a>Изменения в API приложений

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версии        | Обновление API приложений. Это первый набор изменений, включающий изменение структуры и переименование свойств объекта [application](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/application).<br/>**Новые объекты:** [api](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/api]), [informationalUrl](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/informationalUrl), [installedClient](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/installedclient), [permissionScope](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/permissionscope), [preauthorizedApplication](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/preauthorizedapplication), [web](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/web).<br/>**Удаленные свойства:** addIns, appRoles, availableToOtherOrganizations, knownClientApplications, oauth2AllowUrlPathMatching, recordConsentConditions.<br/>**Переименованные свойства:** с appId на id, с identifierUris на applicationAliases, с availableToOtherTenants на orgRestrictions, с mainLogo на logo, с oauth2Permissions на publishedPermissionsScopes, с publicClient на allowPublicClient, с replyUrls на redirectUrls.<br/>**Новые свойства:** tags. |

### <a name="remove-deprecated-planner-api"></a>Удаление устаревшего API Планировщика
| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Удаление        | Бета-версия        | Удалены следующие объекты:<br/>**task**<br/>**plan**<br/>**bucket**<br/>**taskDetails**<br/>**planDetails**<br/>**taskBoardTaskFormat**<br/>**planTaskBoard** |

### <a name="project-rome"></a>Project Rome

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлена поддержка Project Rome, в том числе [получения списка устройств](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/user_list_devices), [отправки команды устройству](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/send_device_command) и [проверки состояния команды](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/get_device_command_status). |
| Дополнение        | Бета-версия        | Добавлена поддержка ресурсов [activity](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/projectrome_activity) и [historyItem](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/projectrome_historyitem) для объектов user, включая [создание или замену activity](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/projectrome_put_activity) и [создание или замену historyItem](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/projectrome_put_historyitem). |

### <a name="administrative-units-property-changes"></a>Изменения свойств административных единиц

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета        | Тип свойства roleMemberInfo объекта [scopedRoleMembership](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/scopedrolemembership) изменен на [identity](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/identity). |
| Изменение          | Бета        | Свойство навигации scopedAdministratorOf объекта [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/user) заменено на scopedRoleMemberOf. |
| Изменение          | Бета        | Свойство навигации scopedAdministrators объекта [administrativeUnit](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/administrativeunit) заменено на scopedRoleMembers. |
| Изменение          | Бета        | Свойство навигации scopedAdministrators объекта [directoryRole](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/directoryrole) заменено на scopedMembers. |

### <a name="add-users-and-groups-webhook-support-in-preview"></a>Добавлена поддержка пользователей и групп в веб-перехватчиках в бета-версии

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
| Изменение        | Бета       | Добавлена поддержка пользователей и групп в [веб-перехватчиках](https://developer.microsoft.com/graph/docs/api-reference/beta/resources/webhooks).

### <a name="add-delta-query-to-v10"></a>Добавлена поддержка запросов изменений в версии 1.0

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлена поддержка функции delta в версии 1.0. Она позволяет выполнять [запрос изменений](https://developer.microsoft.com/ru-RU/graph/docs/concepts/delta_query_overview) для следующих объектов:<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Примеры см. в следующих статьях:<br/>[Получение добавочных изменений для групп](https://developer.microsoft.com/ru-RU/graph/docs/concepts/delta_query_groups)<br/>[Получение добавочных изменений для сообщений в папке](https://developer.microsoft.com/ru-RU/graph/docs/concepts/delta_query_messages)<br/>[Получение добавочных изменений для пользователей](https://developer.microsoft.com/ru-RU/graph/docs/concepts/delta_query_users) |
| Изменение          | Бета        | Добавлена возможность дополнительной фильтрации запросов (по идентификатору) для [пользователей](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/user_delta) и [групп](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/group_delta). |

### <a name="added-user-resource-support-for-deleted-items"></a>Добавлена поддержка работы с удаленными элементами для ресурса user

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлена поддержка [восстановления и окончательного удаления пользователей](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/directory). |

### <a name="added-onpremisesprovisioningerror"></a>Добавлен объект OnPremisesProvisioningError

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Новый объект: [OnPremisesProvisioningError](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/onpremisesprovisioningerror) |
| Изменение          | Бета        | В объекты [user](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/user), [group](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/group) и [orgcontact](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/orgcontact) добавлено свойство OnPremisesProvisioningError. |

### <a name="added-deleteddatetime-property"></a>Добавлено свойство deletedDateTime

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Изменение|Бета|В объект [user](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/user) добавлено свойство deletedDateTime.
|Изменение|Бета|В объект [group](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/group) добавлено свойство deletedDateTime.
|Изменение|Бета|В объект [application](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/application) добавлено свойство deletedDateTime.

### <a name="added-domain-operations-to-v10"></a>Добавлены операции с доменами в версии 1.0

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлены операции с [доменами](https://graph.microsoft.io/ru-RU/docs/api-reference/v1.0/resources/domain).<br/>Новые объекты:</br>[domain](https://graph.microsoft.io/ru-RU/docs/api-reference/v1.0/resources/domain);<br/>[domainDnsRecord](https://graph.microsoft.io/ru-RU/docs/api-reference/v1.0/resources/domaindnsrecord);<br/>[domainDnsCnameRecord](https://graph.microsoft.io/ru-RU/docs/api-reference/v1.0/resources/domainDnsCnameRecord);<br/>[domainDnsMxRecord](https://graph.microsoft.io/ru-RU/docs/api-reference/v1.0/resources/domainDnsMxRecord);<br/>[domainDnsSrvRecord](https://graph.microsoft.io/ru-RU/docs/api-reference/v1.0/resources/domainDnsSrvRecord);<br/>[domainDnsTxtRecord](https://graph.microsoft.io/ru-RU/docs/api-reference/v1.0/resources/domainDnsTxtRecord);<br/>[domainDnsUnavailableRecord](https://graph.microsoft.io/ru-RU/docs/api-reference/v1.0/resources/domainDnsUnavailableRecord).<br/>Новые действия:</br>[verify](https://graph.microsoft.io/ru-RU/docs/api-reference/v1.0/api/domain_verify) |

### <a name="added-contracts-to-v10"></a>Добавлены контракты в версии 1.0

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Новый объект:</br>[contract](https://graph.microsoft.io/ru-RU/docs/api-reference/v1.0/resources/contract) |

### <a name="added-licensedetails-to-v10"></a>Добавлен объект licenseDetails в версии 1.0

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Новый объект:</br>[licenseDetails](https://graph.microsoft.io/ru-RU/docs/api-reference/v1.0/resources/licensedetails) |
| Изменение          | 1.0        | Добавлено свойство навигации [licensedetails](https://graph.microsoft.io/ru-RU/docs/api-reference/v1.0/api/user_list_licensedetails) для объекта [user](https://graph.microsoft.io/ru-RU/docs/api-reference/v1.0/resources/user). |


### <a name="drive-api"></a>API Диска

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:----------|:--------------|
| Дополнение | 1.0 | Добавлен тип ресурса **baseItem**, состоящий из базовых свойств объекта **driveItem**.
| Дополнение | 1.0 и бета | В объект **thumbnail** добавлено свойство **sourceItemId**. <br/> В объект **sharepointIds** добавлено свойство **siteUrl**. <br/> В объект **shared** добавлены свойства **sharedBy** и **sharedDateTime**. <br/> В объект **remoteItem** добавлено свойство **shared**. <br/> В объекты**drive** и **itemReference** добавлено свойство **sharepointIds**. <br/> В объект **fileSystemInfo** добавлено свойство **lastAccessedDateTime**. <br/> В объект **sharedDriveItem** добавлены свойства навигации **driveItem** и **site**. <br/> В объект **baseItem** добавлено свойство **parentReference**.
| Изменение | 1.0 и бета | Объекты **driveItem** и **sharedDriveItem** теперь наследуются от объекта **baseItem**. <br/> Тип **identity** отмечен как открытый.
| Изменение | Бета | В объект **sharingLink** добавлены свойства **configuratorUrl** и **webHtml**. <br/> Добавлены тип ресурса **folderView** и свойство **view** для типа ресурса **folder**. <br/> В объект **driveItem** добавлено свойство навигации **listItem**. <br/> В объект **drive** добавлено свойство навигации **list**.


### <a name="extensions-open-extensions"></a>Расширения (открытые расширения)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0          | Поддержка [openTypeExtension](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/opentypeextension) в ресурсах [device](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/device), [group](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/group), [organization](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/organization) и [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user). |
| Дополнение        | 1.0 и бета-версия | Если пользователь вошел с помощью личной учетной записи Майкрософт, открытые расширения поддерживаются в ресурсах event, post, group, message, contact и user. (При использовании рабочей или учебной учетной записи открытые расширения также поддерживаются в ресурсах device, group, organization и user.) |
| Дополнение        | 1.0 и бета | Поддержка параметра `$expand` для [получения открытых расширений](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/opentypeextension_get) в ресурсах [device](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/device), [group](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/group), [organization](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/organization), [post](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/post) и [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user). |
| Дополнение        | Бета          | Поддержка параметра `$expand` для [получения открытых расширений](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/opentypeextension_get) в объекте [administrativeUnit](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/administrativeunit). |


### <a name="extensions-schema-extensions"></a>Расширения (расширения схемы) 

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0          | Новый ресурс [schemaExtension](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/schemaextension) и методы CRUD для управления определениями расширений для следующих ресурсов: [contact](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/contact), [device](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/device), [event](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/event), [group](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/group), [message](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/message), [organization](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/organization), [post](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/post) и [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user). Обратите внимание, что объект [administrativeUnit](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/administrativeunit) по-прежнему поддерживается только в бета-версии. |
| Дополнение        | 1.0          | Существующие методы POST, GET и PATCH ресурсов [contact](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/contact), [device](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/device), [event](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/event), [group](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/group), [message](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/message), [organization](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/organization), [post](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/post) и [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user) теперь поддерживают добавление, получение, обновление и удаление пользовательских данных, хранящихся в виде расширений схемы в соответствующих экземплярах ресурсов. |
| Дополнение        | 1.0 и бета-версия | Теперь вы можете использовать параметр `$filter` для поиска экземпляров ресурсов, свойства которых совпадают с определенным значениями свойств расширений, например имени. Эта возможность рассматривается подробнее в этом [примере](https://devx.microsoft-tst.com/ru-RU/graph/docs/concepts/extensibility_schema_groups#5-get-a-group-and-its-extension-data). |
| Изменение          | 1.0 и бета | [Удаление определения расширения схемы](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/schemaextension_delete) больше не влияет на доступ к пользовательским данным, добавленным на основе этого определения. |
| Изменение          | 1.0 и бета | Теперь вы можете задать для сложного типа расширения схемы значение null, чтобы удалить расширение схемы из экземпляра ресурса. |


### <a name="group"></a>Группа

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:----------|:--------------|
| Дополнение | 1.0 и бета | Добавлены свойства навигации **drives** и **sites** для объекта **group**.

### <a name="insights-apis"></a>API Insights

|**Тип изменения**|**Версия**|**Описание**| 
|:-------------|:-----------|:--------------|
|Дополнение|Бета|Добавлен [API Shared](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/insights_shared).<br />Новые ресурсы:<br />[sharingDetail](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/insights_sharingdetail) <br />[insightIdentity](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/insights_insightidentity) <br />
|Дополнение|Бета|Добавлен [API Used](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/insights_used).<br />Новые ресурсы:<br />[usageDetails](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/insights_usagedetails) <br />
|Изменение|Бета|Новое свойство **Type** в<br />ресурсе [resourceVisualization](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/insights_resourcevisualization). <br />
|Удаление|Бета-версия|Удалены следующие объекты:<br/>**workingWith**<br/>**trendingAround**<br/>|

### <a name="intune-apis"></a>API Intune

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета    | Добавлены новые объекты:<br/>[androidForWorkMobileAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_androidforworkmobileappconfiguration)<br/>[cartToClassAssociation](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_carttoclassassociation)<br/>[deviceCompliancePolicySettingStateSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary)<br/>[eBookInstallSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_books_ebookinstallsummary)<br/>[eBookVppGroupAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_books_ebookvppgroupassignment)<br/>[iosUpdateConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdateconfiguration)<br/>[remoteAssistancePartner](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner)<br/>[windows10EndpointProtectionConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration)<br/>[windowsDeviceMalwareState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsdevicemalwarestate)<br/>[windowsInformationProtectionAppLearningSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_wip_windowsinformationprotectionapplearningsummary)<br/>[windowsMalwareInformation](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsmalwareinformation)<br/>[windowsProtectionState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsprotectionstate)<br/> |
| Дополнение    | Бета    | Добавлены новые сложные типы:<br/>[androidPermissionAction](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_androidpermissionaction)<br/>[bitLockerSystemDrivePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockersystemdrivepolicy)<br/>[defenderDetectedMalwareActions](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_defenderdetectedmalwareactions)<br/>[settingSource](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_settingsource)<br/> |
| Дополнение    | Бета    | Добавлено действие [assign](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_books_managedebook_assign) для объекта [managedEBook](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_books_managedebook). |
| Дополнение    | Бета    | Добавлено действие [beginOnboarding](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_remoteassistance_remoteassistancepartner_beginonboarding) для объекта [remoteAssistancePartner](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner). |
| Дополнение    | Бета    | Добавлено действие [disconnect](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_remoteassistance_remoteassistancepartner_disconnect) для объекта [remoteAssistancePartner](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner). |
| Удаление    | Бета-версия    | Удалены следующие объекты:<br/>**outlookTask**<br/>**outlookTaskFolder**<br/>**outlookTaskGroup**<br/>**outlookUser**<br/>**windowsManagementAppHealthState**<br/> |
| Удаление    | Бета-версия    | Удалены следующие сложные типы:<br/>**applePushNotificationCertificateSetting**<br/>**eventCreationOptions**<br/> |
| Изменение      | Бета    | Добавлены свойства **workProfilePasswordBlockFingerprintUnlock**, **workProfilePasswordBlockTrustAgents**, **workProfilePasswordExpirationDays**, **workProfilePasswordMinimumLength**, **workProfilePasswordMinutesOfInactivityBeforeScreenTimeout**, **workProfilePasswordPreviousPasswordBlockCount**, **workProfilePasswordSignInFailureCountBeforeFactoryReset**, **workProfilePasswordRequiredType** и **workProfileRequirePassword** для объекта [androidForWorkGeneralDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkgeneraldeviceconfiguration). |
| Изменение      | Бета    | Добавлено свойство **subjectAlternativeNameFormatString** для объекта [androidForWorkPkcsCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkpkcscertificateprofile). |
| Изменение      | Бета    | Добавлены свойства **subjectNameFormatString** и **subjectAlternativeNameFormatString** для объекта [androidForWorkScepCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile). |
| Изменение      | Бета    | Добавлено свойство **kioskModeManagedApps** для объекта [androidGeneralDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration). |
| Изменение      | Бета    | Удалено свойство **kioskModeManagedAppId** для объекта [androidGeneralDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration). |
| Изменение      | Бета    | Добавлено свойство **subjectAlternativeNameFormatString** для объекта [androidPkcsCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidpkcscertificateprofile). |
| Изменение      | Бета    | Добавлены свойства **subjectNameFormatString** и **subjectAlternativeNameFormatString** для объекта [androidScepCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidscepcertificateprofile). |
| Изменение      | Бета    | Удалено свойство **hexColor** для объекта [calendar](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/calendar). |
| Изменение      | Бета    | Для объекта [complianceSettingStateSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_compliancesettingstatesummary) добавлены свойства **setting** и **platformType** |
| Изменение      | Бета    | Удалено свойство **windowsManagementAppEnabled** для объекта [deviceAppManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement). |
| Изменение      | Бета    | Добавлены свойства **userName**, **deviceModel** и **platform** для объекта [deviceComplianceDeviceStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus). |
| Изменение      | Бета    | Добавлены свойства **userPrincipalName** и **deviceModel** для объекта [deviceComplianceSettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate). |
| Изменение      | Бета    | Для объекта [deviceComplianceSettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) добавлены свойства **platformType**, **setting**, **userId** и **userEmail** |
| Изменение      | Бета    | Для объекта [deviceCompliancePolicyDeviceStateSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary) добавлено свойство **inGracePeriodCount** |
| Изменение      | Бета    | Добавлены свойства **userName**, **deviceModel** и **platform** для объекта [deviceConfigurationDeviceStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus). |
| Изменение      | Бета    | Удалено свойство **creationOptions** для объекта [event](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/event). |
| Изменение      | Бета    | Удалено свойство **isDelegated** для объекта [eventMessage](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/eventMessage). |
| Изменение      | Бета    | Удалены свойства **unseenConversationsCount** и **unseenMessagesCount** для объекта [group](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/group). |
| Изменение      | Бета    | Добавлены свойства **settingXml** и **settings** для объекта [iosMobileAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_iosmobileappconfiguration). |
| Изменение      | Бета    | Добавлено свойство **subjectAlternativeNameFormatString** для объекта [iosPkcsCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iospkcscertificateprofile). |
| Изменение      | Бета    | Добавлено свойство **subjectAlternativeNameFormatString** для объекта [iosScepCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosscepcertificateprofile). |
| Изменение      | Бета    | Добавлено свойство **systemIntegrityProtectionEnabled** для объекта [macOSCompliancePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscompliancepolicy). |
| Изменение      | Бета    | Добавлено свойство **subjectAlternativeNameFormatString** для объекта [macOSScepCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosscepcertificateprofile). |
| Изменение      | Бета    | Для объекта [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) добавлены свойства **complianceGracePeriodExpirationDateTime**, **userPrincipalName** и **imei** |
| Изменение      | Бета    | Удалены свойства **settingXml** и **settings** для объекта [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration). |
| Изменение      | Бета    | Добавлены свойства **useSharedComputerActivation**, **updateChannel**, **officePlatformArchitecture** и **localesToInstall** для объекта [officeSuiteApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp). |
| Изменение      | Бета    | Удалено свойство **applePushNotificationCertificateSetting** для объекта [organization](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_organization). |
| Изменение      | Бета    | Изменены следующие свойства объекта [post](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/post):<br/>свойство **sender** сделано обязательным.<br/> |
| Изменение      | Бета    | Добавлены свойства **compliantUserCount**, **nonCompliantUserCount**, **remediatedUserCount**, **errorUserCount**, **unknownUserCount**, **conflictUserCount** и **notApplicableUserCount** для объекта [softwareUpdateStatusSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_softwareupdatestatussummary). |
| Изменение      | Бета    | Добавлены свойства **bluetoothAllowedServices**, **bluetoothBlockPrePairing**, **cellularData**, **defenderDetectedMalwareActions**, **defenderPotentiallyUnwantedAppAction**, **lockScreenAllowTimeoutConfiguration**, **lockScreenBlockCortana**, **lockScreenBlockToastNotifications**, **lockScreenTimeoutInSeconds**, **passwordBlockSimple**, **privacyAutoAcceptPairingAndConsentPrompts**, **privacyBlockInputPersonalization**, **startMenuHideChangeAccountSettings**, **startMenuHideHibernate**, **startMenuHideLock**, **startMenuHideShutDown**, **startMenuHideSignOut**, **startMenuHideSleep**, **startMenuHideSwitchAccount**, **settingsBlockAppsPage**, **settingsBlockGamingPage**, **windowsSpotlightBlockConsumerSpecificFeatures**, **windowsSpotlightBlocked**, **windowsSpotlightBlockOnActionCenter**, **windowsSpotlightBlockTailoredExperiences**, **windowsSpotlightBlockThirdPartyNotifications**, **windowsSpotlightBlockWelcomeExperience**, **windowsSpotlightBlockWindowsTips**, **windowsSpotlightConfigureOnLockScreen** и **connectedDevicesServiceBlocked** для объекта [windows10GeneralConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration). |
| Изменение      | Бета    | Удалены свойства **automaticUpdateMode**, **automaticUpdateSchedule**, **automaticUpdateTime**, **prereleaseFeatures**, **experienceBlockWindowsSpotlight**, **experienceBlockWindowsTips** и **experienceBlockConsumerSpecificFeatures** для объекта [windows10GeneralConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration). |
| Изменение      | Бета    | Добавлено свойство **subjectAlternativeNameFormatString** для объекта [windows10PkcsCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10pkcscertificateprofile). |
| Изменение      | Бета    | Добавлены свойства **subjectNameFormatString** и **subjectAlternativeNameFormatString** для объекта [windows81SCEPCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81scepcertificateprofile). |
| Изменение      | Бета    | Добавлены свойства **indexingEncryptedStoresOrItemsBlocked** и **smbAutoEncryptedFileExtensions** для объекта [windowsInformationProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection). |
| Изменение      | Бета    | Изменены следующие свойства объекта [windowsInformationProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection):<br/>свойство **rightsManagementServicesTemplateId** сделано необязательным.<br/> |
| Изменение      | Бета    | Изменены следующие свойства объекта [windowsMobileMSI](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi):<br/>свойство **productCode** сделано необязательным.<br/> |
| Изменение      | Бета    | Добавлены свойства **subjectNameFormatString** и **subjectAlternativeNameFormatString** для объекта [windowsPhone81SCEPCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81scepcertificateprofile). |
| Изменение      | Бета    | Добавлено свойство навигации **mobileAppConfigurations** для объекта [deviceAppManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement). |
| Изменение      | Бета    | Для объекта [deviceManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) добавлены свойства **cartToClassAssociations**, **deviceCompliancePolicySettingStateSummaries**, **remoteAssistancePartners**, **windowsInformationProtectionAppLearningSummaries** и **windowsMalwareInformation** |
| Изменение      | Бета    | Добавлены свойство навигации **eBook** для объекта [eBookGroupAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_books_ebookgroupassignment). |
| Изменение      | Бета    | Добавлено свойство навигации **windowsProtectionState** для объекта [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
| Изменение      | Бета    | Добавлено свойство навигации **installSummary** для объекта [managedEBook](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_books_managedebook). |
| Изменение      | Бета    | Удалено свойство навигации **outlook** для объекта [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_user). |
| Изменение      | Бета    | Удалено свойство навигации **healthStates** для объекта [windowsManagementApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapp). |
| Изменение      | Бета    | Добавлено свойство **androidForWorkRestrictions** для сложного типа [defaultDeviceEnrollmentRestrictions](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_defaultdeviceenrollmentrestrictions). |
| Изменение      | Бета    | Добавлены свойства **userPrincipalName** и **sources** для сложного типа [deviceCompliancePolicySettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate). |
| Изменение      | Бета    | Добавлены свойства **userPrincipalName** и **sources** для сложного типа [deviceConfigurationSettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate). |
| Изменение      | Бета    | Для сложного типа [deviceConfigurationSettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) добавлены свойства **settingName**, **userId**, **userName**, **userEmail** и **currentValue** |
| Изменение      | Бета    | Удалено свойство **archiveFolder** для сложного типа [mailboxSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/mailboxSettings). |


### <a name="outlook-calendar"></a>Календарь Outlook

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Для метода **findMeetingTimes** добавлено значение перечисления **unrestricted**, указываемое в качестве свойства **activityDomain** в составе параметра **timeConstraint**. Это позволяет методу **findMeetingTimes** искать интервалы времени, соответствующие типу планируемого мероприятия. Дополнительные сведения см. в разделе [request body](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/user_findmeetingtimes#request-body). |
| Дополнение        | Бета-версия          | Содержание объекта **event** теперь можно получать в виде обычного текста, а не только в формате HTML. Дополнительные сведения см. в описаниях событий [get](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/event_get) и [list](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/user_list_events). |

### <a name="outlook-mail"></a>Почта Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версия        | Содержание объекта **message** теперь можно получать в виде обычного текста, а не только в формате HTML. Дополнительные сведения см. в описаниях событий [get](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/message_get) и [list](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/user_list_messages). |


### <a name="outlook-tasks"></a>Задачи Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | В объект [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/user) добавлено новое свойство навигации **outlook** для доступа к задачам Outlook. |
| Дополнение        | Бета        | Новые объекты [outlookuser](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/outlookuser), [outlookTaskGroup](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/outlooktaskgroup), [outlookTaskFolder](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/outlooktaskfolder) и [outlookTask](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/outlooktask), а также их методы поддерживают доступ к задачам Outlook. |
| Дополнение        | Бета        | Задачи Outlook поддерживают вложения (ресурсы [attachment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/attachment), [fileAttachment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/fileattachment), [itemAttachment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/itemattachment) и [referenceAttachment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/referenceattachment)). |
| Дополнение        | Бета        | Задачи Outlook поддерживают [расширенные свойства](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/extended-properties-overview) (ресурсы [singleValueLegacyExtendedProperty](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/singlevaluelegacyextendedproperty) и [multiValueLegacyExtendedProperty](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/multivaluelegacyextendedproperty)). |

### <a name="planner-apis"></a>API Планировщика

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен [API Планировщика](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/planner_overview).<br />Новые ресурсы:<br />[plannerPlan](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/plannerPlan); <br />[plannerTask](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/plannerTask); <br />[plannerPlanDetails](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/plannerPlanDetails); <br />[plannerTaskDetails](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/plannerTaskDetails); <br />[plannerBucket](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/plannerBucket); <br />[plannerAssignedToTaskBoardTaskFormat](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/plannerassignedtotaskboardtaskformat); <br />[plannerBucketTaskBoardTaskFormat](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/plannerBuckettaskboardtaskformat); <br />[plannerProgressTaskBoardTaskFormat](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/plannerprogresstaskboardtaskformat) |

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

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версия        | Обновления API административных единиц будут предоставлены в бета-версиях. Первый набор изменений будет применен 3 мая 2017 г. Изменения включают в себя следующие переименования:<br />сложный тип - **roleMemberInfo** для объекта scopedRoleMembership теперь зовется **identity**;<br />свойство навигации - **scopedAdministratorOf** для объекта user теперь зовется **scopedRoleMemberOf**;<br />свойство навигации - **scopedAdministrators** для объекта administrativeUnit теперь зовется **scopedRoleMembers**;<br />свойство навигации - **scopedAdministrators** для объекта directoryRole теперь зовется **scopedMembers**. |

### <a name="application-and-serviceprincipal-api-changes"></a>Изменения в API application и servicePrincipal

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версия        | API [application](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/application) и [servicePrincipal](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/serviceprincipal) будут обновлены в бета-версии. Первый набор изменений будет применен 15 мая 2017 г. Изменения включают переименование и реструктуризацию свойств. Некоторые свойства (например, appRoles и addIns) будут доступны только после применения изменений. Прежде чем выйдет версия 1.0 с изменениями, будут выпущены бета-версии. |

### <a name="added-preview-support-for-cloud-solution-provider-developers"></a>Добавлена поддержка бета-версий для разработчиков, присоединившихся к программе Cloud Solution Provider

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Приложения, разрешение на использование которых было заранее предоставлено согласно программе Cloud Solution Provider, теперь могут вызывать Microsoft Graph. Описание см. в новой [статье об авторизации](https://graph.microsoft.io/ru-RU/docs/concepts/auth_cloudsolutionprovider). |

### <a name="added-onpremises-properties-to-user-entity"></a>Добавлены свойства onPremises к объекту user

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | К объекту [user](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/user) добавлены новые свойства для onPremises: onPremisesDomainName, OnPremisesSamAccountName и onPremisesUserPrincipalName. |

### <a name="new-planner-apis-and-an-update-to-the-group-visibility-property"></a>Новые API Планировщика и обновление свойства видимости группы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версия        | Добавлено значение **HiddenMembership** для свойства видимости объекта [Group](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/group). |
| Дополнение        | Бета-версия        | Добавлен новый [API Планировщика](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/planner_overview).<br />Новые ресурсы:<br />[plannerPlan](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/plannerPlan); <br />[plannerTask](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/plannerTask); <br />[plannerPlanDetails](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/plannerPlanDetails); <br />[plannerTaskDetails](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/plannerTaskDetails); <br />[plannerBucket](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/plannerBucket); <br />[plannerAssignedToTaskBoardTaskFormat](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/plannerassignedtotaskboardtaskformat); <br />[plannerBucketTaskBoardTaskFormat](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/plannerBuckettaskboardtaskformat); <br />[plannerProgressTaskBoardTaskFormat](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/plannerprogresstaskboardtaskformat). |

### <a name="intune-apis"></a>API Intune
| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлены новые объекты:<br/>[androidForWorkCompliancePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkcompliancepolicy);<br/>[deviceComplianceSettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate);<br/>[deviceInstallState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_books_deviceinstallstate);<br/>[deviceManagementScript](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscript)<br/>[deviceManagementScriptGroupAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscriptgroupassignment)<br/>[deviceManagementScriptState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscriptstate)<br/>[eBookGroupAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_books_ebookgroupassignment);<br/>[iosVppEBook](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_books_iosvppebook);<br/>[managedEBook](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_books_managedebook);<br/>[userInstallStateSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_books_userinstallstatesummary);<br/>[windowsManagementApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapp)<br/>[windowsManagementAppHealthState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapphealthstate)<br/> |
| Дополнение        | Бета        | Добавлены новые сложные типы:<br/>[dailySchedule](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_dailyschedule)<br/>[hourlySchedule](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_hourlyschedule)<br/>[iosBookmark](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosbookmark);<br/>[iosWebContentFilterAutoFilter](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterautofilter);<br/>[iosWebContentFilterBase](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterbase);<br/>[iosWebContentFilterSpecificWebsitesAccess](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterspecificwebsitesaccess);<br/>[runSchedule](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_runschedule)<br/>[sharedAppleDeviceUser](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedappledeviceuser)<br/>[windows10NetworkProxyServer](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10networkproxyserver).<br/> |
| Дополнение        | Бета-версия        | Добавлено действие [requestRemoteAssistance](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_requestremoteassistance) к объекту [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
| Дополнение        | Бета-версия        | Добавлено действие [cleanWindowsDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_cleanwindowsdevice) к объекту [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
| Дополнение        | Бета-версия        | Добавлено действие [logoutSharedAppleDeviceActiveUser](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_logoutsharedappledeviceactiveuser) к объекту [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
| Дополнение        | Бета-версия        | Добавлено действие [deleteUserFromSharedAppleDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_deleteuserfromsharedappledevice) к объекту [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
| Дополнение        | Бета-версия        | Добавлено действие [assign](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_deviceconfig_devicemanagementscript_assign) к объекту [deviceManagementScript](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscript). |
| Дополнение        | Бета-версия        | Добавлено действие [syncLicenses](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_onboarding_applevolumepurchaseprogramtoken_synclicenses) к объекту [appleVolumePurchaseProgramToken](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_applevolumepurchaseprogramtoken). |
| Дополнение        | Бета-версия        | Добавлена функция **getTopMobileApps** для коллекции [mobileApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileapp). |
| Дополнение        | Бета-версия        | Добавлена функция [downloadApplePushNotificationCertificateSigningRequest](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_deviceconfig_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest) к объекту [applePushNotificationCertificate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_applepushnotificationcertificate). |
| Дополнение        | Бета-версия        | Добавлена функция [getDeviceComplianceSettingStates](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_deviceconfig_devicemanagement_getdevicecompliancesettingstates) к объекту [deviceManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement). |
| Дополнение        | Бета-версия        | Добавлена функция [deviceConfigurationUserActivity](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity) к объекту [reportRoot](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_reportroot). |
| Дополнение        | Бета-версия        | Добавлена функция [deviceConfigurationDeviceActivity](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity) к объекту [reportRoot](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_reportroot). |
| Удаление        | Бета-версия        | Удалены следующие сложные типы:<br/>**enterpriseCloudResource**;<br/>**windowsInformationProtectionAppRule**;<br/>**windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate**;<br/>**windowsInformationProtectionAppRuleDesktopTemplate**;<br/>**windowsInformationProtectionAppRuleStoreAppTemplate**;<br/>**windowsInformationProtectionAppRuleTemplate**;<br/>**windowsInformationProtectionCorporateNetworkLocation**;<br/>**windowsInformationProtectionProtectedLocation**;<br/>**windowsInformationProtectionProtectedLocationEnterpriseCloudResources**;<br/>**windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers**;<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges**;<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges**;<br/>**windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames**;<br/>**windowsInformationProtectionProtectedLocationEnterpriseProxyServers**;<br/>**windowsInformationProtectionProtectedLocationNeutralResources**.<br/> |
| Изменение          | Бета-версия        | Добавлено свойство **deviceSharingAllowed** к объекту [androidGeneralDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration). |
| Изменение          | Бета-версия        | Удалено **deviceSharingBlocked** свойство из объекта [androidGeneralDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration). |
| Изменение          | Бета-версия        | Добавлено свойство **minimumRequiredSdkVersion** к объекту [defaultManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection). |
| Изменение          | Бета-версия        | Добавлено свойство **windowsManagementAppEnabled** к объекту [deviceAppManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement). |
| Изменение          | Бета-версия        | Добавлено свойство **notificationTemplateId** к объекту [deviceComplianceActionItem](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceactionitem). |
| Изменение          | Бета-версия        | Добавлено свойство **excludeGroup** к объекту [deviceConfigurationGroupAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationgroupassignment) |
| Изменение          | Бета-версия        | Изменены следующие свойства объекта [iosCustomConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscustomconfiguration):<br/>**payloadFileName** теперь можно не указывать.<br/> |
| Изменение          | Бета-версия        | Добавлено свойство **contentFilterSettings** к объекту [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration). |
| Изменение          | Бета-версия        | Добавлены свойства **cellularBlockPersonalHotspot** и **passcodeBlockFingerprintModification** к объекту [iosGeneralDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration). |
| Изменение          | Бета-версия        | Добавлено свойство **minimumRequiredSdkVersion** к объекту [iosManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection). |
| Изменение          | Бета-версия        | Изменены следующие свойства объекта [macOSCustomConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscustomconfiguration):<br/>**payloadFileName** теперь можно не указывать.<br/> |
| Изменение          | Бета-версия        | Добавлены свойства **disableAppPinIfDevicePinIsSet**, **minimumRequiredOsVersion**, **minimumWarningOsVersion**, **minimumRequiredAppVersion** и **minimumWarningAppVersion** к объекту [managedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_managedappprotection). |
| Изменение          | Бета-версия        | Добавлены свойства **remoteAssistanceSessionUrl**, **isEncrypted**, **model** и **manufacturer** к объекту [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
| Изменение          | Бета-версия        | Изменены следующие свойства объекта [getMobileAppCount](https://developer.microsoft.com/ru-RU/graph/docs/docs/api-reference/beta/api/intune_apps_mobileapp_getmobileappcount):<br/>для **bindingParameter** вместо **mobileApp** теперь используется **коллекция** *mobileApp*;<br/>для свойства **status** вместо типа GUID теперь используется String.<br/> |
| Изменение          | Бета-версия        | Добавлено свойство **vpnConfigurationId** к объекту [mobileAppGroupAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileappgroupassignment). |
| Изменение          | Бета-версия        | Удалено свойство **fromEmailAddress** из объекта [notificationMessageTemplate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_notificationmessagetemplate). |
| Изменение          | Бета-версия        | Добавлено свойство **excludedApps** к объекту [officeSuiteApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp). |
| Изменение          | Бета-версия        | Удалено свойство **excludedOfficeApps** из объекта [officeSuiteApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp). |
| Изменение          | Бета-версия        | Добавлено свойство **enabled** к объекту [sharedPCConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcconfiguration). |
| Изменение          | Бета-версия        | Добавлены свойства **networkProxyApplySettingsDeviceWide**, **networkProxyDisableAutoDetect**, **networkProxyAutomaticConfigurationUrl**, **networkProxyServer**, **bluetoothDeviceName**, **wiFiScanInterval**, **wirelessDisplayBlockProjectionToThisDevice**, **wirelessDisplayBlockUserInputFromReceiver**, **wirelessDisplayRequirePinForPairing**, **experienceBlockDeviceDiscovery**, **experienceBlockErrorDialogWhenNoSIM**, **experienceBlockTaskSwitcher**, **startMenuPinnedFolderDocuments**, **startMenuPinnedFolderDownloads**, **startMenuPinnedFolderFileExplorer**, **startMenuPinnedFolderHomeGroup**, **startMenuPinnedFolderMusic**, **startMenuPinnedFolderNetwork**, **startMenuPinnedFolderPersonalFolder**, **startMenuPinnedFolderPictures**, **startMenuPinnedFolderSettings**, **startMenuPinnedFolderVideos**, **startMenuAppListVisibility**, **startMenuHideFrequentlyUsedApps**, **startMenuHideRecentJumpLists**, **startMenuHideRecentlyAddedApps**, **startMenuHideRestartOptions**, **startMenuHideUserTile**, **startMenuHidePowerButton**, **startMenuLayoutEdgeAssetsXml**, **personalizationDesktopImageUrl** и **personalizationLockScreenImageUrl** к объекту [windows10GeneralConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration). |
| Изменение          | Бета-версия        | Изменен тип следующих свойств объекта [windowsMobileMSI](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi):<br/>**productCode** теперь относится не к Guid, а к String.<br/> |
| Изменение          | Бета-версия        | Изменены следующие свойства объекта [windowsPhone81AppX](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx):<br/>**phoneProductIdentifier** больше не обязательно указывать;<br/>**phonePublisherId** больше не обязательно указывать.<br/> |
| Изменение          | Бета-версия        | Изменены следующие свойства объекта [windowsPhone81AppXBundle](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appxbundle):<br/>**appXPackageInformationList** больше не обязательно указывать.<br/> |
| Изменение          | Бета-версия        | Добавлены свойства **productKey** и **licenseType** к объекту [windowsStoreForBusinessApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessapp). |
| Изменение          | Бета-версия        | Добавлено свойство **previewBuildSetting** к объекту [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration). |
| Изменение          | Бета-версия        | Добавлены свойства навигации **windowsManagementApp** и **managedEBooks** к объекту [deviceAppManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement). |
| Изменение          | Бета-версия        | Добавлены свойства навигации **deviceManagementScripts**, **managedDeviceOverview** и **cloudPkiSubscriptions** к объекту [deviceManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement). |
| Изменение          | Бета-версия        | Добавлены свойства **osMinimumVersion** и **osMaximumVersion** к сложному типу [deviceEnrollmentPlatformRestrictions](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_deviceenrollmentplatformrestrictions). |
| Изменение          | Бета-версия        | Добавлены свойства **isSharedDevice** и **sharedDeviceCachedUsers** к сложному типу [hardwareInformation](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_hardwareinformation). |
| Изменение          | Бета-версия        | Изменены следующие свойства сложного типа [omaSettingBase64](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_omasettingbase64):<br/>**fileName** больше не обязательно указывать.<br/> |
| Изменение          | Бета-версия        | Изменены следующие свойства сложного типа [omaSettingStringXml](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_omasettingstringxml):<br/>**fileName** больше не обязательно указывать.<br/> |

## <a name="march-2017"></a>Март 2017 г.

### <a name="intune-apis"></a>API Intune

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета    | Добавлены новые объекты:<br/>[androidForWorkApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_androidforworkapp);<br/>[androidForWorkAppConfigurationSchema](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationschema);<br/>[androidForWorkSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings);<br/>[androidForWorkVpnConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkvpnconfiguration);<br/>[applePushNotificationCertificate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_applepushnotificationcertificate)<br/>[complianceSettingStateSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_compliancesettingstatesummary);<br/>[deviceCompliancePolicyDeviceStateSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary);<br/>[deviceCompliancePolicyState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicystate);<br/>[deviceConfigurationDeviceStateSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatesummary);<br/>[deviceConfigurationState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationstate);<br/>[enterpriseCodeSigningCertificate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_enterprisecodesigningcertificate);<br/>[iosEduDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosedudeviceconfiguration);<br/>[managedDeviceCertificateState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevicecertificatestate)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicesummary);<br/>[managedDeviceMobileAppConfigurationUserSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationusersummary);<br/>[mdmWindowsInformationProtectionPolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_mdmwindowsinformationprotectionpolicy);<br/>[mobileAppInstallSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallsummary);<br/>[mobileAppProvisioningConfigGroupAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileappprovisioningconfiggroupassignment);<br/>[mobileThreatDefenseConnector](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_mobilethreatdefenseconnector);<br/>[officeSuiteApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp);<br/>[settingStateDeviceSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_settingstatedevicesummary);<br/>[softwareUpdateStatusSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_softwareupdatestatussummary);<br/>[symantecCodeSigningCertificate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_symanteccodesigningcertificate);<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration);<br/>[windowsInformationProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection);<br/>[windowsInformationProtectionAppLockerFile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionapplockerfile);<br/>[windowsInformationProtectionPolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionpolicy);<br/>[windowsMobileMSI](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi).<br/> |
| Дополнение    | Бета    | Добавлены новые сложные типы:<br/>[androidForWorkAppConfigurationExample](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationexample);<br/>[androidForWorkAppConfigurationExampleJson](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationexamplejson);<br/>[androidForWorkAppConfigurationSchemaItem](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationschemaitem);<br/>[deviceCompliancePolicySettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate);<br/>[deviceConfigurationSettingState](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate);<br/>[deviceExchangeAccessStateSummary](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceexchangeaccessstatesummary)<br/>[edgeSearchEngine](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchengine);<br/>[edgeSearchEngineBase](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchenginebase);<br/>[edgeSearchEngineCustom](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchenginecustom);<br/>[excludedApps](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_excludedapps);<br/>[iosEduCertificateSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducertificatesettings);<br/>[ipRange](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iprange);<br/>[windowsInformationProtectionApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionapp);<br/>[windowsInformationProtectionCloudResource](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioncloudresource);<br/>[windowsInformationProtectionCloudResourceCollection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioncloudresourcecollection);<br/>[windowsInformationProtectionDesktopApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondesktopapp);<br/>[windowsInformationProtectionIPRangeCollection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioniprangecollection);<br/>[windowsInformationProtectionResourceCollection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionresourcecollection);<br/>[windowsInformationProtectionStoreApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionstoreapp).<br/> |
| Дополнение    | Бета-версия    | Добавлено действие [requestSignupUrl](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_requestsignupurl) к объекту [androidForWorkSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings). |
| Дополнение    | Бета-версия    | Добавлено действие [completeSignup](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_completesignup) к объекту [androidForWorkSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings). |
| Дополнение    | Бета-версия    | Добавлено действие [syncApps](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_syncapps) к объекту [androidForWorkSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings). |
| Дополнение    | Бета-версия    | Добавлено действие [unbind](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_unbind) к объекту [androidForWorkSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings). |
| Дополнение    | Бета-версия    | Добавлено действие [assign](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign) к объекту [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration). |
| Дополнение    | Бета-версия    | Добавлено действие [recoverPasscode](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_recoverpasscode) к объекту [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
| Дополнение    | Бета-версия    | Добавлено действие [removeApplePushNotificationCertificate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_onboarding_organization_removeapplepushnotificationcertificate) к объекту [organization](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_organization). |
| Дополнение    | Бета-версия    | Добавлено действие [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_mam_iosmanagedappprotection_updatemobileappidentifierdeployments) к объекту [iosManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection). |
| Дополнение    | Бета-версия    | Добавлено действие [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_mam_androidmanagedappprotection_updatemobileappidentifierdeployments) к объекту [androidManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection). |
| Дополнение    | Бета-версия    | Добавлено действие [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_updatemobileappidentifierdeployments) к объекту [targetedManagedAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration). |
| Дополнение    | Бета-версия    | Добавлено действие [updateTargetedSecurityGroups](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_mam_iosmanagedappprotection_updatetargetedsecuritygroups) к объекту [iosManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection). |
| Дополнение    | Бета-версия    | Добавлено действие [updateTargetedSecurityGroups](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_mam_androidmanagedappprotection_updatetargetedsecuritygroups) к объекту [androidManagedAppProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection). |
| Дополнение    | Бета-версия    | Добавлено действие [updateTargetedSecurityGroups](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_mam_windowsinformationprotection_updatetargetedsecuritygroups) к объекту [windowsInformationProtection](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection). |
| Дополнение    | Бета-версия    | Добавлено действие [updateTargetedSecurityGroups](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_mam_windowsinformationprotection_updatetargetedsecuritygroups) к объекту [windowsInformationProtectionPolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionpolicy). |
| Дополнение    | Бета-версия    | Добавлено действие [updateTargetedSecurityGroups](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_mam_mdmwindowsinformationprotectionpolicy_updatetargetedsecuritygroups) к объекту [mdmWindowsInformationProtectionPolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_mdmwindowsinformationprotectionpolicy). |
| Дополнение    | Бета-версия    | Добавлено действие [wipeManagedAppRegistrationByDeviceTag](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_mam_user_wipemanagedappregistrationbydevicetag) к объекту [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_user). |
| Дополнение    | Бета-версия    | Добавлена функция [getTopMobileApps](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_apps_mobileapp_gettopmobileapps) к объекту [mobileApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileapp). |
| Дополнение    | Бета-версия    | Добавлена функция [verifyWindowsEnrollmentAutoDiscovery](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_corpenrollment_devicemanagement_verifywindowsenrollmentautodiscovery) к объекту [deviceManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement). |
| Удаление    | Бета-версия    | Удалены следующие объекты:<br/>**appProvisioningConfigGroupAssignment**;<br/>**defaultManagedAppConfiguration**;<br/>**enterpriseCertificate**;<br/>**managedDeviceMobileAppProvisioningConfigurationDeviceStatus**;<br/>**symantecCertificate**;<br/>**windows10WindowsInformationProtectionConfiguration**.<br/> |
| Удаление    | Бета-версия    | Удалены следующие сложные типы:<br/>**mobileAppInstallSummary**;<br/>**windowsArchitecture**;<br/>**windowsDeviceType**.<br/> |
| Изменение      | Бета-версия    | Добавлено свойство **webBrowserBlockPopups** к объекту [androidGeneralDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration). |
| Изменение      | Бета-версия    | Удалено свойство **webBrowserAllowPopups** из объекта [androidGeneralDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration). |
| Изменение      | Бета-версия    | Добавлено свойство **appIdentifier** к объекту [androidStoreApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_androidstoreapp). |
| Изменение      | Бета-версия    | Удалены свойства **applicationCount**, **failedApplicationCount** и **appInstallFailures** из объекта [appReportingOverviewStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/appReportingOverviewStatus). |
| Изменение      | Бета-версия    | Добавлены свойства **sharedIPadMaximumUserCount** и **enableSharedIPad** к объекту [depEnrollmentProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_corpenrollment_depenrollmentprofile). |
| Изменение      | Бета-версия    | Добавлены свойства **shareTokenWithSchoolDataSyncService** и **lastSyncErrorCode** к объекту [depOnboardingSetting](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_deponboardingsetting). |
| Изменение      | Бета-версия    | Добавлены свойства **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** и **configurationVersion** к объекту [deviceComplianceDeviceOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview). |
| Изменение      | Бета-версия    | Удалены свойства **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** и **policyRevision** из объекта [deviceComplianceDeviceOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview). |
| Изменение      | Бета-версия    | Добавлены свойства **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** и **configurationVersion** к объекту [deviceComplianceUserOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview). |
| Изменение      | Бета-версия    | Удалены свойства **numberOfPendingUsers**, **numberOfSucceededUsers**, **numberOfErrorUsers**, **numberOfFailedUsers**, **lastUpdateTime** и **policyRevision** из объекта [deviceComplianceUserOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview). |
| Изменение      | Бета-версия    | Добавлены свойства **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** и **configurationVersion** к объекту [deviceConfigurationDeviceOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview). |
| Изменение      | Бета-версия    | Удалены свойства **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** и **policyRevision** из объекта [deviceConfigurationDeviceOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview). |
| Изменение      | Бета-версия    | Добавлены свойства **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** и **configurationVersion** к объекту [deviceConfigurationUserOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview). |
| Изменение      | Бета-версия    | Удалены свойства **numberOfPendingUsers**, **numberOfSucceededUsers**, **numberOfErrorUsers**, **numberOfFailedUsers**, **lastUpdateTime** и **policyRevision** из объекта [deviceConfigurationUserOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview). |
| Изменение      | Бета-версия    | Добавлено свойство **subscriptionState** к объекту [deviceManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement). |
| Изменение      | Бета-версия    | Добавлено свойство **managedEmailProfileRequired** к объекту [iosCompliancePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscompliancepolicy). |
| Изменение      | Бета-версия    | Добавлено свойство **appsSingleAppModeList** к объекту [iosGeneralDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration). |
| Изменение      | Бета-версия    | Удалено свойство **appsSingleAppModeBundleIds** из объекта [iosGeneralDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration). |
| Изменение      | Бета-версия    | Добавлено свойство **expirationDateTime** к объекту [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration). |
| Изменение      | Бета-версия    | Удалено свойство **expiration** из объекта [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration). |
| Изменение      | Бета-версия    | Добавлены свойства **passwordMinimumCharacterSetCount**, **osMinimumVersion**, **osMaximumVersion**, **deviceThreatProtectionEnabled**, **deviceThreatProtectionRequiredSecurityLevel** и **storageRequireEncryption** к объекту [macOSCompliancePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscompliancepolicy). |
| Изменение      | Бета-версия    | Удалено свойство **manifest** из объекта [managedAndroidLobApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp). |
| Изменение      | Бета-версия    | Добавлены свойства **isSupervised**, **exchangeLastSuccessfulSyncDateTime**, **exchangeAccessState** и **exchangeAccessStateReason** к объекту [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
| Изменение      | Бета-версия    | Добавлено свойство **deviceExchangeAccessStateSummary** к объекту [managedDeviceOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddeviceoverview). |
| Изменение      | Бета-версия    | Удалено свойство **manifest** из объекта [managedIOSLobApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp). |
| Изменение      | Бета-версия    | Удалено свойство **installSummary** из объекта [mobileApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileapp). |
| Изменение      | Бета-версия    | Добавлено свойство **uploadState** к объекту [mobileAppContentFile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile). |
| Изменение      | Бета-версия    | Изменены следующие свойства объекта [mobileAppContentFile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile):<br/>**azureStorageUriExpirationDateTime** больше не обязательно указывать.<br/> |
| Изменение      | Бета-версия    | Добавлены свойства **initiatedByUserPrincipalName**, **deviceOwnerUserPrincipalName**, **deviceIMEI** и **actionState** к объекту [remoteActionAudit](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_remoteactionaudit). |
| Изменение      | Бета-версия    | Добавлены свойства **oneDriveDisableFileSync**, **safeSearchFilter**, **edgeSearchEngine**, **settingsBlockSettingsApp**, **settingsBlockSystemPage**, **settingsBlockDevicesPage**, **settingsBlockNetworkInternetPage**, **settingsBlockPersonalizationPage**, **settingsBlockAccountsPage**, **settingsBlockTimeLanguagePage**, **settingsBlockEaseOfAccessPage**, **settingsBlockPrivacyPage**, **settingsBlockUpdateSecurityPage**, **experienceBlockWindowsSpotlight**, **experienceBlockWindowsTips**, **experienceBlockConsumerSpecificFeatures**, **startMenuLayoutXml**, **startMenuMode**, **logonBlockFastUserSwitching** и **startBlockUnpinningAppsFromTaskbar** к объекту [windows10GeneralConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration). |
| Изменение      | Бета-версия    | Добавлены свойства **allowPrinting**, **allowScreenCapture** и **allowTextSuggestion** к объекту [windows10SecureAssessmentConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration). |
| Изменение      | Бета-версия    | Удалены свойства **blockPrinting**, **blockScreenCapture** и **blockTextSuggestion** из объекта [windows10SecureAssessmentConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration). |
| Изменение      | Бета-версия    | Добавлено свойство **identityName** к объекту [windowsAppX](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsappx). |
| Изменение      | Бета-версия    | Изменен тип следующих свойств объекта [windowsAppX](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsappx):<br/>**applicableArchitectures** теперь относится не к [windowsArchitecture](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/windowsArchitecture), а к String.<br/> |
| Изменение      | Бета-версия    | Добавлено свойство **identityName** к объекту [windowsPhone81AppX](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx). |
| Изменение      | Бета-версия    | Изменен тип следующих свойств объекта [windowsPhone81AppX](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx):<br/>**applicableArchitectures** теперь относится не к [windowsArchitecture](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/windowsArchitecture), а к String.<br/> |
| Изменение      | Бета-версия    | Добавлены свойства **identityName**, **identityPublisherHash** и **identityResourceIdentifier** к объекту [windowsUniversalAppX](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx). |
| Изменение      | Бета-версия    | Изменен тип следующих свойств объекта [windowsUniversalAppX](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx):<br/>**applicableArchitectures** теперь относится не к [windowsArchitecture](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/windowsArchitecture), а к String;<br/>**applicableDeviceTypes** теперь относится не к [windowsDeviceType](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/windowsDeviceType), а к String.<br/> |
| Изменение      | Бета-версия    | Добавлено свойство **restartMode** к объекту [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [androidForWorkScepCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [androidScepCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidscepcertificateprofile). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **enterpriseCodeSigningCertificates**, **symantecCodeSigningCertificate**, **sideLoadingKeys**, **managedAppPolicies**, **iosManagedAppProtections**, **androidManagedAppProtections**, **defaultManagedAppProtections**, **targetedManagedAppConfigurations**, **mdmWindowsInformationProtectionPolicies**, **windowsInformationProtectionPolicies**, **managedAppRegistrations** и **managedAppStatuses** к объекту [deviceAppManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement). |
| Изменение      | Бета-версия    | Удалены свойства навигации **appReportingOverview**, **enterpriseCerts** и **symantecCert** из объекта [deviceAppManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **deviceSettingStateSummaries** к объекту [deviceCompliancePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **deviceSettingStateSummaries** к объекту [deviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **termsAndConditions**, **androidForWorkSettings**, **androidForWorkAppConfigurationSchemas**, **applePushNotificationCertificate**, **softwareUpdateStatusSummary**, **deviceCompliancePolicyDeviceStateSummary**, **complianceSettingStateSummaries**, **deviceConfigurationDeviceStateSummaries** и **mobileThreatDefenseConnectors** к объекту [deviceManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement). |
| Изменение      | Бета-версия    | Удалены свойства навигации **teacherRootCertificates**, **teacherIdentityCertificate**, **studentRootCertificates** и **studentIdentityCertificate** из объекта [iosEducationDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration). |
| Изменение      | Бета-версия    | Изменен тип следующих свойств объекта [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration):<br/>**deviceStatuses** теперь относится не к коллекции [managedDeviceMobileAppProvisioningConfigurationDeviceStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/managedDeviceMobileAppProvisioningConfigurationDeviceStatus), а к коллекции [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus).<br/>**groupAssignments** теперь относится не к коллекции [appProvisioningConfigGroupAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/appProvisioningConfigGroupAssignment), а к коллекции [mobileAppProvisioningConfigGroupAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileappprovisioningconfiggroupassignment).<br/> |
| Изменение      | Бета-версия    | Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [iosScepCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosscepcertificateprofile). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [macOSScepCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosscepcertificateprofile). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **deviceConfigurationStates** и **deviceCompliancePolicyStates** к объекту [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **deviceStatusSummary** и **userStatusSummary** к объекту [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **installSummary** к объекту [mobileApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileapp). |
| Изменение      | Бета-версия    | Удалено свойство навигации **sideLoadingKeys** из объекта [organization](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_organization). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [windows81SCEPCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81scepcertificateprofile). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [windowsPhone81SCEPCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81scepcertificateprofile). |
| Изменение      | Бета-версия    | Удалены свойства **applicationId**, **appName**, **platformId**, **userFailures** и **deviceFailures** из сложного типа [appInstallationFailure](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure). |
| Изменение      | Бета-версия    | Добавлено свойство **displayName** к сложному типу [iosHomeScreenFolderPage](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolderpage). |
| Изменение      | Бета-версия    | Добавлено свойство **displayName** к сложному типу [iosHomeScreenPage](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenpage). |
| Изменение      | Бета-версия    | Добавлены свойства **subjectName**, **description**, **expirationDateTime** и **certificate** к сложному типу [windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondatarecoverycertificate). |
| Изменение      | Бета-версия    | Удалены свойства **dataRecoveryCertificate** и **certificateFileName** из сложного типа [windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondatarecoverycertificate). |
| Изменение      | Бета-версия    | Добавлено свойство **displayName** к сложному типу [windowsPackageInformation](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation). |
| Изменение      | Бета-версия    | Изменен тип следующих свойств сложного типа [windowsPackageInformation](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation):<br/>**applicableArchitecture** теперь относится не к [windowsArchitecture](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/windowsArchitecture), а к String.<br/> |
| Изменение      | Бета-версия    | Изменены следующие свойства сложного типа [windowsPackageInformation](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation):<br/>свойство **applicableArchitecture** сделано обязательным.<br/> |

### <a name="add-contracts-to-microsoft-graph"></a>Добавление контрактов в Microsoft Graph

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Новый ресурс:</br>[contract](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/contract). |

### <a name="add-domain-operations-to-microsoft-graph"></a>Добавление операций с доменами в Microsoft Graph

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены функции к объектам [domain](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/domain).<br/>Новые объекты:</br>[domain](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/domain);<br/>[domainDnsRecord](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/domaindnsrecord);<br/>[domainDnsCnameRecord](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/domainDnsCnameRecord);<br/>[domainDnsMxRecord](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/domainDnsMxRecord);<br/>[domainDnsSrvRecord](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/domainDnsSrvRecord);<br/>[domainDnsTxtRecord](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/domainDnsTxtRecord);<br/>[domainDnsUnavailableRecord](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/domainDnsUnavailableRecord).<br/>Новые действия:</br>[forceDelete](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/api/domain_forcedelete);</br>[verify](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/api/domain_verify). |

### <a name="add-custom-data-to-microsoft-graph-using-schema-extensions"></a>Добавление пользовательских данных в Microsoft Graph с помощью расширений схемы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавление данных приложения в Microsoft Graph с помощью [расширений схемы](https://developer.microsoft.com/ru-RU/graph/docs/concepts/extensibility_overview#schema-extensions-preview)  поддерживается для следующих ресурсов:<br/>administrative unit;<br/>calendar event;<br/>device;<br/>group;<br/>message;<br/>organization;<br/>personal contact;<br/>post;<br/>user.<br/>Пример приведен в следующей статье:<br/>[Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)](https://developer.microsoft.com/ru-RU/graph/docs/concepts/extensibility_schema_groups). |
| Дополнение        | Бета        | Предоставлен альтернативный способ создания определения расширения схемы без подтвержденного личного домена .com. Подробности см. в разделе [Расширения схемы](https://developer.microsoft.com/ru-RU/graph/docs/concepts/extensibility_overview#schema-extensions-preview). |

### <a name="add-custom-data-to-microsoft-graph-using-open-extensions"></a>Добавление пользовательских данных в Microsoft Graph с помощью открытых расширений

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Вместо термина "расширения данных Office 365" теперь используется "открытые расширения". |
| Дополнение        | Бета-версия          | Добавлены ресурсы, которые поддерживают [открытые расширения](https://developer.microsoft.com/ru-RU/graph/docs/concepts/extensibility_overview#open-extensions): <br/>administrative unit;<br/>device;<br/>group;<br/>organization;<br/>user.<br/>Пример приведен в следующей статье:<br/>[Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](https://developer.microsoft.com/ru-RU/graph/docs/concepts/extensibility_open_users). |

### <a name="directory-apis"></a>API каталогов

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлена поддержка [восстановления и окончательного удаления групп](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/directory).<br/>Новый объект: каталог со свойством навигации deleteditems. |
| Дополнение        | Бета        | Новый объект:</br>[Конечная точка](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/endpoint) |
| Изменение          | Бета        | Новое свойство навигации [endpoints](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/api/group_list_endpoints) для ресурса [group](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/group) |
| Дополнение        | Бета        | Новый объект:</br>[licenseDetails](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/licensedetails) |
| Изменение          | Бета        | Добавлено свойство навигации [licensedetails](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/api/user_list_licensedetails) для объекта [user](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/user). |

### <a name="reports-apis"></a>API отчетов

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Представлена предварительная версия нового API для функций создания отчетов в Office 365. С его помощью можно получать отчеты об использовании служб Office 365 сотрудниками компании. Например, вы можете определить, кто использует службу по максимуму, а кому вообще не нужна лицензия Office 365. Дополнительные сведения см. в статье о ресурсе [report](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/report). |

### <a name="directory-apis"></a>API каталогов

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Новый объект:</br>[contract](https://graph.microsoft.io/ru-RU/docs/api-reference/beta/resources/contract). |

## <a name="february-2017"></a>Февраль 2017 г.

### <a name="intune-apis"></a>API Intune

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета    | Добавлены новые объекты:<br/>[androidForWorkCertificateProfileBase](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkcertificateprofilebase)<br/>[androidForWorkEasEmailProfileBase](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkeasemailprofilebase)<br/>[androidForWorkEnterpriseWiFiConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkenterprisewificonfiguration)<br/>[androidForWorkGmailEasConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkgmaileasconfiguration)<br/>[androidForWorkNineWorkEasConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworknineworkeasconfiguration)<br/>[androidForWorkPkcsCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkpkcscertificateprofile)<br/>[androidForWorkScepCertificateProfile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile)<br/>[androidForWorkTrustedRootCertificate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworktrustedrootcertificate)<br/>[androidForWorkWiFiConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkwificonfiguration)<br/>[appleDeviceFeaturesConfigurationBase](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_appledevicefeaturesconfigurationbase)<br/>[appProvisioningConfigGroupAssignment](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_appprovisioningconfiggroupassignment)<br/>[deviceComplianceUserOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview)<br/>[deviceConfigurationUserOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview)<br/>[enterpriseCertificate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_enterprisecertificate)<br/>[iosEducationDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)<br/>[macOSDeviceFeaturesConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosdevicefeaturesconfiguration)<br/>[managedAndroidLobApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp)<br/>[managedDeviceMobileAppProvisioningConfigurationDeviceStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappprovisioningconfigurationdevicestatus)<br/>[managedIOSLobApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp)<br/>[managedMobileLobApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_managedmobilelobapp)<br/>[symantecCertificate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_symanteccertificate)<br/>[windowsAppX](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsappx)<br/>[windowsCertificateProfileBase](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowscertificateprofilebase)<br/>[windowsPhone81AppX](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx)<br/>[windowsPhone81AppXBundle](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appxbundle)<br/>[windowsPhoneXAP](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsphonexap)<br/>[windowsUniversalAppX](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx)<br/> |
| Дополнение    | Бета    | Добавлены новые сложные типы:<br/>[airPrintDestination](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_airprintdestination)<br/>[windowsArchitecture](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsarchitecture)<br/>[windowsDeviceType](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsdevicetype)<br/>[windowsMinimumOperatingSystem](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowsminimumoperatingsystem)<br/>[windowsPackageInformation](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation)<br/> |
| Дополнение    | Бета    | Добавлено действие [assign](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign) к объекту [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration). |
| Дополнение    | Бета    | Добавлено действие [scheduleActionsForRules](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_deviceconfig_devicecompliancepolicy_scheduleactionsforrules) к объекту [deviceCompliancePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy). |
| Дополнение    | Бета    | Добавлено действие [updateTargetedSecurityGroups](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_updatetargetedsecuritygroups) к объекту [targetedManagedAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration). |
| Дополнение    | Бета    | Добавлена функция [getScopesForUser](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/intune_rbac_resourceoperation_getscopesforintune_devices_user) к объекту [resourceOperation](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_rbac_resourceoperation). |
| Изменение      | Бета    | Удалено свойство **manifest** из объекта [androidLobApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_androidlobapp). |
| Изменение      | Бета    | Добавлены свойства **assetTagTemplate**, **lockScreenFootnote**, **homeScreenDockIcons** и **homeScreenPages** к объекту [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration). |
| Изменение      | Бета    | Удалены свойства **deviceSharingAssetTagInformation**, **deviceSharingLockScreenFootnote**, **homeScreenLayoutDockIcons** и **homeScreenLayoutPages** из объекта [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration). |
| Изменение      | Бета    | Добавлено свойство **appsSingleAppModeBundleIds** к объекту [iosGeneralDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration). |
| Изменение      | Бета    | Удалено свойство **manifest** из объекта [iosLobApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_ioslobapp). |
| Изменение      | Бета    | Добавлены свойства **createdDateTime**, **description**, **lastModifiedDateTime**, **displayName** и **version** к объекту [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration). |
| Изменение      | Бета    | Добавлены свойства **createdDateTime** и **lastModifiedDateTime** к объекту [managedAppPolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy). |
| Изменение      | Бета    | Удалено свойство **deviceRegistrationState** из объекта [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devices_manageddevice). |
| Изменение      | Бета    | Добавлено свойство **manifest** к объекту [mobileAppContentFile](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile). |
| Изменение      | Бета    | Добавлены свойства **osDescription** и **userName** к объекту [mobileAppInstallStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus). |
| Изменение      | Бета    | Удалено свойство **deviceType** из объекта [mobileAppInstallStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus). |
| Изменение      | Бета    | Изменен тип следующих свойств объекта [mobileAppInstallStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus):<br/>**mobileAppInstallStatusValue** (с Int32 на String) |
| Изменение      | Бета    | Добавлены свойства **targetedSecurityGroupIds** и **targetedSecurityGroupsCount** к объекту [targetedManagedAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration). |
| Изменение      | Бета    | Удалено свойство **numberOfTargetedSecurityGroups** из объекта [targetedManagedAppConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration). |
| Изменение      | Бета    | Добавлено свойство **id** к объекту [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_devices_user). |
| Изменение      | Бета    | Удалены свойства **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** и **certificateValidityPeriodScale** из объекта [windows10CertificateProfileBase](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10certificateprofilebase). |
| Изменение      | Бета    | Удалены свойства **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** и **certificateValidityPeriodScale** из объекта [windows81CertificateProfileBase](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81certificateprofilebase). |
| Изменение      | Бета    | Удалено свойство **applyToWindows10Mobile** из объекта [windowsPhone81GeneralConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81generalconfiguration). |
| Изменение      | Бета    | Добавлены свойства навигации **enterpriseCerts**, **iosLobAppProvisioningConfigurations** и **symantecCert** к объекту [deviceAppManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement). |
| Изменение      | Бета    | Добавлено свойство навигации **userStatusOverview** к объекту [deviceCompliancePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy). |
| Изменение      | Бета    | Добавлено свойство навигации **userStatusOverview** к объекту [deviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration). |
| Изменение      | Бета    | Добавлены свойства навигации **groupAssignments**, **deviceStatuses** и **userStatuses** к объекту [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration). |
| Изменение      | Бета    | Изменен тип следующих свойств объекта [windows10VpnConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10vpnconfiguration):<br/>**identityCertificate** (с [windows10CertificateProfileBase](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10certificateprofilebase) на [windowsCertificateProfileBase](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowscertificateprofilebase)) |
| Изменение      | Бета    | Добавлены свойства **deviceComplianceCheckinThresholdDays** и **isScheduledActionEnabled** к сложному типу [deviceManagementSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings). |
| Изменение      | Бета    | Удалены свойства **windowsCommercialId** и **windowsCommercialIdLastModifiedTime** из сложного типа [deviceManagementSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings). |
| Изменение      | Бета    | Добавлены свойства **bundleID**, **appName**, **publisher**, **enabled** и **showOnLockScreen** к сложному типу [iosNotificationSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings). |
| Изменение      | Бета    | Удалены свойства **bundleIdentifier**, **notificationsEnabled** и **showInLockScreen** из сложного типа [iosNotificationSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings). |



## <a name="january-2017"></a>Январь 2017 г.

### <a name="outlook-calendar"></a>Календарь Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | v1.0        | Новое действие [findMeetingTimes](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/user_findmeetingtimes) для ресурса [user](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user). |
| Дополнение        | v1.0        | Новый сложный тип [attendeeBase](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/attendeebase), который состоит из свойства типа участников. |
| Дополнение        | v1.0        | Новые сложные типы:<br/>[attendeeAvailability](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/attendeeavailability)<br/>[locationConstraint](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/locationconstraint) <br/>[locationConstraintItem](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/locationconstraintitem)<br/>[meetingTimeSuggestion](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/meetingtimesuggestion)<br/>[meetingTimeSuggestionsResult](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/meetingtimesuggestionsresult)<br/>[timeConstraint](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/timeconstraint)<br/>[timeSlot](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/timeslot) |
| Изменение          | 1.0        | Сложный тип [attendee](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/attendee) теперь является производным от attendeeBase, который, в свою очередь, является производным от [recipient](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/recipient). Он состоит из тех же свойств **status**, **type** и **emailAddress**, что и раньше, а также унаследованных свойств. |
| Дополнение        | Бета        | В ресурс [calendar](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/calendar) добавлено свойство hexColor. |

### <a name="intune-apis"></a>API Intune

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлены новые объекты: <br/>[appReportingOverviewStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_appreportingoverviewstatus)<br/>[deviceComplianceDeviceOverview](https://developer.microsoft.com/ru-RU/graph/docs//api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview)<br/>[deviceConfigurationDeviceOverview](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview)<br/>[deviceManagementExchangeOnpremisesPolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_devicemanagementexchangeonpremisespolicy)<br/>[iosDeviceFeaturesConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)<br/>[iosEducationDeviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)<br/>[iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)<br/>[onpremisesConditionalAccessSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_onpremisesconditionalaccesssettings)<br/>[sharedPCConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcconfiguration)<br/>[windows10EnterpriseModernAppManagementConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration)<br/>[windows10SecureAssessmentConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration)<br/>[windows10WindowsInformationProtectionConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10windowsinformationprotectionconfiguration) |
|Дополнение|Бета|Добавлены новые сложные типы: <br/> [appInstallationFailure](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure)<br/>[enterpriseCloudResource](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_enterprisecloudresource)<br/>[iosHomeScreenApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenapp)<br/>[iosHomeScreenFolder](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolder)<br/>[iosHomeScreenFolderPage](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolderpage)<br/>[iosHomeScreenItem](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenitem)<br/>[iosHomeScreenPage](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenpage)<br/>[iosNotificationSettings](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings)<br/>[iPv6Range](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_ipv6range)<br/>[sharedPCAccountManagerPolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcaccountmanagerpolicy)<br/>[windowsInformationProtectionAppRule](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionapprule)<br/>[windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruleapplockerpolicyfiletemplate)<br/>[windowsInformationProtectionAppRuleDesktopTemplate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruledesktoptemplate)<br/>[windowsInformationProtectionAppRuleStoreAppTemplate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionapprulestoreapptemplate)<br/>[windowsInformationProtectionAppRuleTemplate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruletemplate)<br/>[windowsInformationProtectionCorporateNetworkLocation](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectioncorporatenetworklocation)<br/>[windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectiondatarecoverycertificate)<br/>[windowsInformationProtectionProtectedLocation](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocation)<br/>[windowsInformationProtectionProtectedLocationEnterpriseCloudResources](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterprisecloudresources)<br/>[windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseinternalproxyservers)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseipv4ranges)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseipv6ranges)<br/>[windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterprisenetworkdomainnames)<br/>[windowsInformationProtectionProtectedLocationEnterpriseProxyServers](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseproxyservers)<br/>[windowsInformationProtectionProtectedLocationNeutralResources](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationneutralresources)
|Удаление|Бета|Следующие сложные типы удалены и заменены на тип microsoft.graph.Json:<br/>managedAppDeploymentSummary <br/>managedAppSummary<br /> |
|Изменение|Бета|Для следующих объектов тип свойства appConfigComplianceStatus заменен на complianceStatus: <br/>[managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus)<br/>[managedDeviceMobileAppConfigurationUserStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationuserstatus)|
|Изменение|Бета|Для ресурса [managedAppStatusRaw](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_managedappstatusraw) тип свойства content изменен с managedAppSummary на Json.|
|Изменение|Бета|Из коллекции [managedAppRegistration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_mam_managedappregistration) удалена функция getUsersWithFlaggedAppRegistration.|
|Изменение|Бета|Изменено свойство навигации **vppToken** объекта [iosVppApp](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_iosvppapp), теперь он не является включенной коллекцией.|
|Изменение|Бета|Добавлено свойство **deviceStatusOverview** к объектам [deviceConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) и [deviceCompliancePolicy](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy).|
|Изменение|Бета|Добавлено свойство **appReportingOverview** к одиночному объекту [deviceAppManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement).|
|Изменение|Бета|Добавлены свойства **deviceDisplayName** и **userPrincipalName** к объектам [deviceConfigurationDeviceStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus), [deviceComplianceDeviceStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus) и [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus).|
|Изменение|Бета|Добавлено свойство **ruleName** к объекту [deviceComplianceScheduledActionForRule](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancescheduledactionforrule).|
|Изменение|Бета|Добавлены свойства **devicesCount**, **userDisplayName** и **userPrincipalName** к объектам [deviceConfigurationUserStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuserstatus), [deviceComplianceUserStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuserstatus) и [managedDeviceMobileAppConfigurationUserStatus](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationuserstatus).|
|Изменение|Бета|Добавлена коллекция [notificationMessageTemplates](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_notification_notificationmessagetemplate) к одиночному объекту [deviceManagement](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagement).|
|Изменение|Бета|Добавлены свойства **isDefault**, **lastModifiedDateTime**, **locale**, **messageTemplate** и **subject** к объекту [localizedNotificationMessage](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_localizednotificationmessage).|
|Изменение|Бета|Добавлены свойства **azureActiveDirectoryDeviceId**, **deviceCategory**, **deviceRegistrationState** и **managementAgent** к объекту [managedDevice](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_onboarding_manageddevice).|
|Изменение|Бета|Добавлено свойство **lastModifiedDateTime** к объекту [mobileAppCategory](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_apps_mobileappcategory).|
|Изменение|Бета|Добавлены свойства **brandingOptions**, **defaultLocale**, **displayName**, **fromEmailAddress**, **lastModifiedDateTime**, **localizedNotificationMessages** к объекту [notificationMessageTemplate](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_notification_notificationmessagetemplate).|
|Изменение|Бета|Добавлены свойства **appsAllowTrustedAppsSideloading**, **appsBlockWindowsStoreOriginatedApps**, **developerUnlockSetting**, **edgeBlockAccessToAboutFlags**, **edgeBlockDeveloperTools**, **edgeBlockExtensions**, **edgeBlockInPrivateBrowsing**, **edgeFirstRunUrl**, **edgeHomepageUrls**, **gameDvrBlocked**, **settingsBlockAddProvisioningPackage**, **settingsBlockChangeLanguage**, **settingsBlockChangePowerSleep**, **settingsBlockChangeRegion**, **settingsBlockChangeSystemTime**, **settingsBlockEditDeviceName**, **settingsBlockRemoveProvisioningPackage**, **sharedUserAppDataAllowed**, **smartScreenBlockPromptOverride**, **smartScreenBlockPromptOverrideForFiles**, **storageRestrictAppDataToSystemVolume**, **storageRestrictAppInstallToSystemVolume**, **webRtcBlockLocalhostIpAddress**, **windowsStoreBlockAutoUpdate** и **windowsStoreEnablePrivateStoreOnly** к объекту [windows10GeneralConfiguration](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration).|

## <a name="december-2016"></a>Декабрь 2016 г.

### <a name="delta-query"></a>Запрос на получение различий

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | В следующие объекты добавлена новая функция delta для выполнения [запроса на получение различий](https://developer.microsoft.com/ru-RU/graph/docs/concepts/delta_query_overview):<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Примеры см. в следующих статьях:<br/>[Получение добавочных изменений групп (предварительная версия)](https://developer.microsoft.com/ru-RU/graph/docs/concepts/delta_query_groups)<br/>[Получение добавочных изменений сообщений в папке (предварительная версия)](https://developer.microsoft.com/ru-RU/graph/docs/concepts/delta_query_messages)<br/>[Получение добавочных изменений пользователей (предварительная версия)](https://developer.microsoft.com/ru-RU/graph/docs/concepts/delta_query_users) |

### <a name="excel-apis"></a>API Excel

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | v1.0        | Добавлены ресурс workbookPivotTable, действия refresh и refreshAll в сводных таблицах, ресурс workbookRangeView, действие visibleView в отфильтрованном диапазоне для возврата workbookRangeView пользователю, коллекция строк get и ресурс range из visibleView, функции columnsAfter, columnsBefore, resizedRange, rowsAbove и rowsBelow из ресурса range и новые свойства таблицы. |

### <a name="intune-apis"></a>API Intune

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлены API ресурсов и методов для Microsoft Intune. Это большой набор ресурсов и методов для поддержки общедоступной предварительной версии Intune на портале Azure. Сведения о службе Intune см. в статье [Документация по Intune](https://go.microsoft.com/fwlink/?linkid=836405). Сведения о ресурсах и API Intune см. в разделе [Работа с Intune в Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/intune_graph_overview). |

## <a name="october-2016"></a>Октябрь 2016 г.

### <a name="authorization-provider"></a>Поставщик услуг авторизации

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Конечная точка авторизации 2.0 теперь поддерживает тип предоставления OAuth client_credentials, который можно использовать для [процессов управляющей программы и длительных процессов в бизнес-сценариях](https://azure.microsoft.com/ru-RU/documentation/articles/active-directory-v2-protocols-oauth-client-creds/). |
| Дополнение        | 1.0 и бета-версия | Конечная точка авторизации 2.0 теперь поддерживает [разрешения, требующие согласия администратора](http://developer.microsoft.com/ru-RU/graph/docs/concepts/permissions_reference) ([конечная точка предоставления согласия администратора](https://azure.microsoft.com/ru-RU/documentation/articles/active-directory-v2-scopes/#admin-restricted-scopes)). |
| Дополнение        | 1.0 и бета-версия | Конечная точка авторизации 2.0 теперь поддерживает согласие администратора для всех пользователей клиента ([конечная точка предоставления согласия администратора](https://azure.microsoft.com/ru-RU/documentation/articles/active-directory-v2-scopes/#admin-restricted-scopes)). |

### <a name="invitation-apis"></a>API приглашений

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлено свойство invitedUserType к типу объекта приглашений, определяющее тип приглашаемого пользователя (**Guest** или **Member**). |
| Удаление        | Бета        | Мы удалим свойство invitedToGroups для типа объекта invitation 11 ноября 2016 г. Это значит, что вы больше не сможете добавить приглашаемого пользователя в группу с помощью этого API. Это можно будет сделать с помощью [API добавления членов](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/group_post_members). |

## <a name="september-2016"></a>Сентябрь 2016 г.

### <a name="azure-ad-application-proxy"></a>Прокси приложения Azure AD

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Теперь API Azure AD Application Proxy доступны в конечной точке Microsoft Graph бета-версии. Эти API позволяют безопасно публиковать локальные приложения для пользователей, находящихся за пределами корпоративной сети, используя Azure AD в качестве общей системы управления доступом. Опубликованные API позволяют создавать приложения, которые могут получать и обновлять различные аспекты прокси приложения, например параметры _connectors_, _connectorGroups_ и _onPremisesPublishing_ приложения. |

### <a name="drive"></a>Drive

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлена коллекция _shared_, благодаря которой можно получать доступ к общим элементам driveItem с помощью идентификатора shareId или URL-адреса для совместного доступа. |
| Дополнение        | Бета-версия        | Добавлена функция _search_ к объекту drive, которая позволяет искать элементы не только в корневой папке диска. |


### <a name="driveitem"></a>DriveItem

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлена поддержка элемента _createUploadSession_, который позволяет отправлять файлы размером более 4 МБ в OneDrive, OneDrive для бизнеса и библиотеки документов SharePoint. |
| Дополнение        | Бета-версия        | Добавлено свойство _sharepointIds_, которое возвращает традиционные идентификаторы API SharePoint для элементов driveItem, хранящихся в SharePoint. |
| Дополнение        | Бета-версия        | Добавлены дополнительные свойства для _remoteItem_. |
| Дополнение        | Бета-версия        | Добавлено значение _quickXorHash_ для файлов в OneDrive для бизнеса. |
| Дополнение        | Бета-версия        | Добавлена область для объекта _createSharingLink_, которая позволяет создавать ссылки для совместного доступа в компании или анонимного совместного доступа. |

### <a name="extended-properties"></a>Расширенные свойства

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Теперь [расширенные свойства](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/extended-properties-overview) поддерживаются в следующих ресурсах: message, mailFolder, event, calendar, contact, contactFolder, group event, group calendar, group post. |

### <a name="groups"></a>Группы

Добавлена поддержка динамического членства в группах с помощью общедоступной ознакомительной версии API, включая дополнения, указанные в таблице ниже.

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавленное свойство **membershipRule** содержит правила, которые определяют членов динамической группы. |
| Дополнение        | Бета-версия        | Добавленное свойство **membershipRuleProcessingState** определяет, включено ли динамическое членство для этой группы. |
| Дополнение        | Бета-версия        | Присвойте свойству **groupTypes** значение **DynamicMembership**, чтобы включить динамическое членство для этой группы. |
| Дополнение        | Бета-версия        | Добавлено свойство **preferredLanguage**, которое указывает предпочитаемый язык для группы Office 365. |
| Дополнение        | Бета-версия        | Добавлено свойство **theme**, которое позволяет указать цветовую тему группы Office 365. |

### <a name="hybrid-deployment-support"></a>Поддержка гибридного развертывания

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Приложения могут использовать API Почты, Календаря и Контактов Outlook версии 1.0 для доступа к локальным почтовым ящикам в гибридном развертывании Exchange 2016 с накопительным пакетом обновления 3 (CU3). Дополнительные сведения о поддержке REST API см. в разделах, посвященных соответствующему [гибридному развертыванию](https://developer.microsoft.com/ru-RU/graph/docs/overview/hybrid_rest_support). **Примечание.** Если вы используете эти наборы API версии 1.0, то теперь ваши приложения (включая рабочие) будут работать с локальными почтовыми ящиками, которые соответствуют требованиям для гибридных развертываний. Доступна только предварительная версия этой возможности. |

### <a name="identityriskevents"></a>IdentityRiskEvents

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета        | В рамках изменения схемы, при котором тип двух свойств расположений будет заменен новым сложным типом в конечной точке identityRiskEvents, в конечной точке identityRiskEvents изменены или добавлены следующие свойства:</br>**location** теперь относится не к Edm.String, а к signInLocation ComplexType;<br/>**previousLocation** теперь относится не к Edm.String, а к signInLocation ComplexType;<br/>**signInLocation** — новый элемент ComplexType, содержащий свойства city, state, countryOrRegion и geoCoordinates;<br/>**geoCoordinates** — новый элемент ComplexType, содержащий свойства latitude и longitude. |

### <a name="invitation-manager"></a>Диспетчер приглашений

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Теперь API диспетчера приглашений доступны в конечной точке Microsoft Graph бета-версии. С помощью API диспетчера приглашений вы можете создать приглашение для добавления внешнего пользователя в организацию. Кроме того, при приглашении пользователя вы можете добавить его в группу Office 365. Дополнительные сведения см. в статье [о диспетчере приглашений](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/invitation). |

### <a name="onedrive"></a>OneDrive

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен метод **CreateUploadSession** для **driveItem**, который позволяет отправлять большие файлы и возобновлять отправку. |
| Дополнение        | v1.0        | Добавлены свойства для отслеживания идентификаторов SharePoint в элементах из SharePoint (**sharepointIds**) и свойство для идентификации корневых папок (**root**). |
| Дополнение        | 1.0        | Добавлена корневая коллекция **Shares**, которую можно использовать с идентификаторами shareId или ссылками для совместного доступа к общим элементам в OneDrive и SharePoint. Возвращает новый тип — sharedDriveItem. |
| Дополнение        | 1.0        | Добавлен метод **Invite** для driveItem, который позволяет добавлять разрешения для элементов. |
| Дополнение        | 1.0        | Добавлен метод **Search** для drive, который позволяет искать элементы на диске, а также общие элементы. |
| Дополнение        | 1.0        | Добавлено свойство **processingMetadata** для свойства quickXorHash сложного типа hashes. |
| Дополнение        | 1.0        | Добавлено свойство **quickXorHash** к сложному типу hashes. |

### <a name="outlook-calendar"></a>Календарь Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлено свойство **onlineMeetingUrl** к ресурсу [event](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/event). |
| Дополнение        | Бета-версия        | Добавлено действие [forward](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/event_forward) к ресурсу event. |
| Дополнение        | Бета-версия        | К ресурсу [calendar](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/calendar) добавлены свойства, c помощью которых можно предоставлять общий доступ к календарю: **canEdit**, **canShare**, **canViewPrivateItems**, **isShared**, **isShareWithMe** и **owner**. |

### <a name="outlook-mail"></a>Почта Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен сложный тип [mailboxSettings](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/mailboxsettings), который включает свойства **automaticRepliesSetting**, **timeZone** и **language**. |
| Дополнение        | 1.0        | Добавлено свойство **mailboxSettings** к ресурсу [user](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user). |
| Дополнение        | Бета        | Добавлена возможность создавать, отображать, получать и удалять один или несколько экземпляров объекта [mention](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/mention) в сообщении. С помощью объектов mention можно привлечь внимание других пользователей в сообщении. |
| Дополнение        | Бета        | Добавлена поддержка действия [getMailTips](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/user_getmailtips) для получения подсказок для определенных получателей. Добавлены следующие ресурсы: automaticRepliesMailTips, mailTips, mailTipsError. |

### <a name="query-parameters"></a>Параметры запроса

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета        | С 26 сентября 2016 г. поддерживаются параметры запроса без префиксов $. Префикс $ в параметрах запроса не является обязательным. Дополнительные сведения см. в записи блога [Поддержка параметров запросов без префиксов $ в Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph). |

### <a name="sharepoint"></a>SharePoint

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Доступ к сайтам и спискам SharePoint [по идентификатору](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/list_get) или [URL-адресу](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/api/baseitem_getbyurl). |
| Дополнение        | Бета-версия        | Возможность [отображать, создавать, получать и удалять экземпляры объектов listItem](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/listitem). |

### <a name="users"></a>Пользователи

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлено нередактируемое свойство **refreshTokensValidFromDateTime**, которое указывает дату и время начала действия токенов обновления или токенов сеанса. Все токены, выпущенные до этого времени, недействительны, а при попытке их использования потребуется повторный вход в систему. |
| Дополнение        | Бета-версия        | Добавлено свойство **showInAddressList**, указывающее, должен ли глобальный список адресов Outlook содержать этого пользователя. |
| Дополнение        | Бета-версия        | Добавлено служебное действие **invalidateAllRefreshTokens**, которое аннулирует все токены обновления и токены сеанса пользователя, выпущенные для приложений, сбрасывая значения свойства **refreshTokensValidFromDateTime** и указывая для него текущую дату и время. |


### <a name="webhooks"></a>Веб-перехватчики

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | В веб-перехватчики добавлены корневые элементы Drive в качестве ресурса, доступного для подписки. |

## <a name="august-2016"></a>Август 2016 г.

### <a name="contacts"></a>Контакты

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | В рамках изменения схемы, при котором удаляются несколько свойств и добавляются соответствующие коллекции в конечную точку contacts, в эту конечную точку добавлены следующие свойства: _Websites Collection(ComplexType: Website)_,_Phones Collection (ComplexType: Phone)_, _PostalAddress Collection(ComplexType: PhysicalAddress)_. Дополнительные сведения см. в записи блога [Предстоящие изменения API Контактов и Людей](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/). |
| Удаление        | Бета        | В рамках изменения схемы, при котором удаляются несколько свойств и добавляются соответствующие коллекции в конечную точку contacts, из этой конечной точки удалены следующие свойства: _BusinessHomePage_,_HomePhones_, _MobilePhone1_, _BusinessPhones_, _HomeAddress_, _BusinessAddress_, _OtherAddress_. Дополнительные сведения см. в записи блога [Предстоящие изменения API Контактов и Людей](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/). |

### <a name="excel-apis"></a>API Excel

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | REST API Excel стал общедоступным в Microsoft Graph. Теперь вы можете обеспечить глубокую и сложную интеграцию с книгами Excel в Office 365. Дополнительные сведения см. в записи блога [Настройка использования REST API для Excel в приложениях с помощью Microsoft Graph](http://dev.office.com/blogs/power-your-apps-with-the-new-excel-rest-api). |

### <a name="people"></a>Люди

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета        | Свойство _WebSite_ переименовано на _Websites_. Дополнительные сведения см. в записи [Предстоящие изменения API Контактов и Людей](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/). |

### <a name="privileged-identity-management"></a>Управление привилегированными пользователями (PIM)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Теперь REST API управления привилегированными пользователями доступны в конечной точке Microsoft Graph (бета-версия). [Управление привилегированными пользователями](https://azure.microsoft.com/ru-RU/documentation/articles/active-directory-privileged-identity-management-configure/) обеспечивает активацию "точно в срок" для привилегированных ролей в организации Azure AD, например ролей глобального администратора, администратора выставления счетов и т. д. C помощью опубликованных API разработчики могут создавать приложения, которые получают и обновляют привилегированные роли и активируют роли для пользователей. Дополнительные сведения см. в статьях [Microsoft Graph: доступна бета-версия API для Azure AD Privileged Identity Management](http://dev.office.com/blogs/microsoft-graph-azure-ad-privileged-identity-management-apis-beta) и [Azure AD Privileged Identity Management](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/privilegedidentitymanagement_root). |

## <a name="july-2016"></a>Июль 2016 г.

### <a name="administrative-units"></a>Административные единицы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Представлен новый API Administrative Units (предварительная версия). Административные единицы позволяют организациям делить Azure Active Directory на подразделения и делегировать административные обязанности этим подразделениям. Подразделения могут представлять регионы, отделы, места возникновения затрат и т. д. Теперь ими можно управлять с помощью API Microsoft Graph. |

## <a name="june-2016"></a>Июнь 2016 г.

### <a name="identityriskevents"></a>IdentityRiskEvents

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета|Представлен новый API IdentityRiskEvents (предварительная версия). Этот API работает в сочетании с защитой идентификации Azure Active Directory. Его можно использовать для запрашивания событий рисков, созданных функцией защиты идентификации. Дополнительные сведения см. в статье [Знакомство с предварительной версией нового API в Microsoft Graph: IdentityRiskEvents](http://dev.office.com/blogs/identityriskevents-api-preview).

### <a name="subscriptions"></a>Подписки

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Области, предназначенные только для приложений, теперь поддерживаются для подписок _mail_ и _contacts_. |

## <a name="may-2016"></a>Май 2016 г.

### <a name="calendar"></a>Календарь

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Существенные изменения|Бета|Изменения в API findMeetingTimes. Дополнительные сведения см. в записи блога [Обновление API findMeetingTimes в Microsoft Graph](http://dev.office.com/microsoft-graph-findmeetingtimes-api-update). Это изменение вступило в силу 19 мая 2016 г.

### <a name="contact"></a>Контакт

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен абстрактный тип _extensions_ для поддержки открытого типа openTypeExtension в OData версии 4. |

### <a name="directory"></a>Каталог

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Существенные изменения | Бета        | Свойство _settingTemplateId_ теперь называется _templateId_. Это изменение вступило в силу 19 мая 2016 г. |

### <a name="event"></a>Событие

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен абстрактный тип _extensions_ для поддержки открытого типа openTypeExtension в OData версии 4. |

### <a name="eventmessages"></a>EventMessages

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлены типы _inferenceClassification_ и _extensions_ к объекту _eventMessages_. |
| Дополнение        | Бета-версия        | Добавлено свойство _responseRequested_ к _eventMessageRequest_. |

### <a name="messages"></a>Сообщения

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлены типы _inferenceClassification_ и _extensions_ к объекту _message_. |
| Дополнение        | Бета-версия        | Добавлено свойство _wellknownname_ для объекта _contactFolder_. |

### <a name="post"></a>Запись

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен абстрактный тип _extensions_ для поддержки открытого типа openTypeExtension в OData версии 4. |

### <a name="user"></a>User

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен тип ресурса _inferenceClassification_. |
| Дополнение        | Бета-версия        | Добавлено свойство _timeZone_ к типу _mailboxsettings_.   |
| Дополнение        | Бета-версия        | Добавлен API _findMeetingTimes_ для объекта _user_.   |

## <a name="april-2016"></a>Апрель 2016 г.

### <a name="general"></a>Общие

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Теперь _Accept-Encoding:gzip_ может учитываться. |
| Дополнение        | 1.0          | Добавлена поддержка сегмента приведения в пути expand. Например: "https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event" |
| Дополнение        | Бета          | Добавлена поддержка запроса PATCH для структурных свойств. Например: "PATCH /me/mailboxSettings" |
| Дополнение        | Бета          | Теперь Azure Active Directory используется в качестве резервного ресурса для запросов /beta/users/id/photo, когда приложению Outlook не удается обслужить запрос (например, когда у пользователя нет лицензии на почтовый ящик или у клиента нет подписки на Exchange Online). ПРИМЕЧАНИЕ. Этот резервный ресурс доступен и для запросов GET, и для запросов PATCH. |
| Дополнение        | Бета          | Добавлена поддержка сегмента приведения в пути expand. Например: "https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event" |

### <a name="onedrive"></a>OneDrive

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Исправление             | v1.0        | Устранена неисправность, из-за которой при выполнении запросов createLink в OneDrive возникала ошибка 500: "Неподдерживаемый тип свойства расширения". |

## <a name="march-2016"></a>Март 2016 г.

### <a name="calendar"></a>Календарь

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_. |
| Дополнение        | Бета-версия        | Добавлено свойство _suggestionHint_ к _meetingTimeCandidate_. |
| Дополнение        | Бета-версия        | Добавлено свойство _locationUri_ к _location_. |
| Дополнение        | Бета-версия        | Добавлены свойства _type_ и _postOfficeBox_ к _physicalAddress_. |
| Изменение          | Бета-версия        | У метода _findMeetingTimes_ появился новый параметр _ReturnSuggestionHints_. |
| Изменение          | Бета-версия        | Метод _findMeetingTimes_ теперь возвращает коллекцию объектов _meetingTimeCandidate_. |

### <a name="drive"></a>Drive

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Добавлена функция _recent_ для вывода списка элементов, которые недавно использовал пользователь, вошедший в систему. Этот список включает элементы, находящиеся на диске пользователя, а также элементы на других дисках, к которым у пользователя есть доступ. Пример: GET /me/drive/recent. |
| Дополнение        | 1.0 и бета-версия | Добавлена функция _sharedWithMe_ для вывода списка элементов, доступ к которым предоставлен текущему пользователю. Пример: GET /me/drive/sharedWithMe. |

### <a name="driveitem"></a>DriveItem

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Добавлен тип _remoteItem_, который позволяет предоставить ссылку на элемент на другом диске. |
| Дополнение        | 1.0 и бета-версия | Добавлен тип _sharingInvitation_, который позволяет предоставить сведения о приглашении к совместному использованию, связанном с этим разрешением. |
| Дополнение        | 1.0 и бета-версия | Добавлена функция _delta_, чтобы отслеживать изменения элементов на диске. Пример: GET /me/drive/items/{item-id}/delta |
| Дополнение        | 1.0 и бета-версия | Добавлен метод _copy_, который создает копию _driveItem_ (в том числе всех дочерних элементов) в новом родительском элементе или с новым именем. Пример: POST /me/drive/items/{item-id}/copy |
| Дополнение        | 1.0 и бета-версия | Атрибуты экземпляра _conflictBehavior_ теперь можно применять к _driveItem_. |
|Дополнение|Бета|Добавлена функция _invite_, которая позволяет отправить приглашение к совместному использованию для существующего элемента. Приглашение к совместному использованию создает уникальную ссылку для совместного доступа и отправляет ее получателю приглашения. Пример: POST /drive/items/{item-id}/invite

### <a name="event"></a>Событие

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены новое свойство _onlineMeetingUrl_ и новый метод _cancel_. |

### <a name="event-messages"></a>Сообщения о событиях

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены свойства _startDateTime_, _endDateTime_, _location_, _type_, _recurrence_, _isOutOfDate_, _conversationIndex_, _unsubscribe_, _unsubscribeData_, _unsubscribeEnabled_ и _flag_ к объекту _eventmessage_. |
| Дополнение        | Бета-версия        | Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_. |
| Дополнение        | Бета-версия        | Добавлен новый метод _unsubscribe_.          |

### <a name="excel"></a>Excel

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Мы добавляем новые REST API Excel, которые позволяют считывать и изменять данные в рабочей книге Excel. Теперь вы можете создавать интеллектуальные приложения, с помощью которых пользователи смогут эффективно анализировать содержимое, хранящееся в рабочих книгах Excel. Используйте аналитические функции Excel, создавайте таблицы и визуально привлекательные диаграммы в своем приложении. Дополнительные сведения см. в статье [Работа с Excel в Microsoft Graph](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/beta/resources/excel). |

### <a name="general"></a>Общие

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Улучшено сообщение об ошибке при сопоставлении псевдонима клиента и отклоненных токенов JWT (AAD). |
| Дополнение        | 1.0 и бета-версия | Сведения о расположении конечной точки службы авторизации теперь возвращаются в заголовке _www-authenticate_ при получении запроса с пустым токеном носителя. |
| Дополнение        | 1.0 и бета-версия | Исправлена возможность фильтрации по свойству id объекта. Пример: GET https://graph.microsoft.com/v1.0/users?$filter=id+eq+'x'<br/>Ранее в запросах POST требовалось добавлять microsoft.graph перед именем функции или действия. Например: POST https://graph.microsoft.com/v1.0/me/Microsoft.Graph.getMemberGroups.<br/>Теперь не требуется указывать префикс (хотя его по-прежнему можно указывать). Таким образом, указанный ниже запрос также будет работать. POST https://graph.microsoft.com/v1.0/me/getMemberGroups |
| Изменение          | Бета          | Удалены имена свойств подписок.  |
| Дополнение        | Бета          | Мы добавили возможность находить (с помощью _directorySettingTemplates_) и переопределять поведение по умолчанию (путем создания _setting_ на основе шаблона) для объектов и связанных с ними функций. Изначально для управления поведением групп Office использовался только этот шаблон. |

### <a name="mail-folder"></a>Папка почты

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены свойства _wellKnownName_ и _userConfigurations_. |
| Дополнение        | Бета-версия        | Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_. |

### <a name="messages"></a>Сообщения

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0          | Добавлено свойство _mobilePhone_.            |
| Дополнение        | 1.0 и бета-версия | Добавлено свойство _internetMessageId_. Идентификатор сообщения в формате, установленном документом [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). |
| Изменение          | Бета-версия          | Свойство _mobilePhone1_ теперь называется _mobilePhone_. |
| Изменение          | Бета-версия          | У методов _createReply_ и _createReplyAll_ появились новые параметры — _Message_ и _comment_. |
| Изменение          | Бета-версия          | У метода _createForward_ появились новые параметры — _Message_, _ToRecipients_ и _comment_. |
| Изменение          | Бета-версия          | У методов _reply_, _replyAll_ и _forward_ появился новый параметр — _Message_. |

### <a name="permission"></a>Разрешение

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Добавлено свойство _sharingInvitation_ для предоставления сведений о приглашении к совместному использованию, связанном с этим разрешением. |

### <a name="person"></a>Человек

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены новые свойства: _birthday_, _personNotes_, _isFavorite_, _phones_, _permission_, _postalAddresses_, _websites_, _yomiCompany_, _department_, _profession_, _mailboxType_ и _personType_. |
| Дополнение        | Бета-версия        | Добавлены новые типы перечислений: _physicalAddressType_, _webSite_, _phone_ и _webSiteType_. |

### <a name="reference-attachment"></a>Вложение в виде ссылки

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены новые свойства: _sourceUrl_, _providerType_, _thumbnailUrl_, _previewUrl_, _permission_ и _isFolder_. |
| Дополнение        | Бета-версия        | Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_. |
| Дополнение        | Бета-версия        | Добавлены новые типы перечислений — _referenceAttachmentProvider_ и _referenceAttachmentPermission_. |

### <a name="subscriptions"></a>Подписки

| **Тип изменения** | **Конечная точка** | **Описание**                          |
| :-------------- | :----------- | :--------------------------------------- |
| Дополнение        | 1.0         | Теперь веб-перехватчики общедоступны в конечной точке версии 1.0 благодаря ресурсу _/Subscriptions_. Вы можете создавать, считывать, продлевать и удалять подписки на уведомления о данных из чатов в Outlook и группах Office 365. |

### <a name="user"></a>Пользователь

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлено свойство _mailboxSettings_ и соответствующие типы. |

## <a name="february-2016"></a>Февраль 2016 г.

### <a name="driveitem"></a>DriveItem

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Новое свойство _remoteItem_ для driveItem для учетных записей Майкрософт. |

### <a name="general"></a>Общие

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Конструкция-_/me/drive_ теперь работает как для учетных записей Майкрософт, так и для рабочих и учебных учетных записей. |
| Изменение          | 1.0 и бета-версия | Запросы Drive для учетных записей, хранилища OneDrive которых подготовлены по запросу, работают более надежно и в большем количестве сценариев, где для используемых по умолчанию сайтов SharePoint клиента применяются нестандартные имена. |
| Удаление        | Бета          | Из бета-версии схемы удалены различные нереализованные типы для более точного соответствия схеме версии 1.0. |

### <a name="subscriptions"></a>Подписки

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Проверка notificationUrl на создание подписок. Дополнительные сведения см. в статье [Обновление веб-перехватчиков Microsoft Graph — январь 2016 г.](http://dev.office.com/blogs/Microsoft-Graph-WebHooks-Update-January-2016) |
| Дополнение        | Бета        | Теперь можно удалять объекты подписки: DELETE https://graph.microsoft.com/beta/subscriptions/ |

### <a name="users"></a>Пользователи

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Теперь для учетных записей Майкрософт возвращается _displayName_. |

## <a name="january-2016"></a>Январь 2016 г.

### <a name="contacts"></a>Контакты

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | В набор объектов личных контактов добавлено свойство mobilePhone. |

### <a name="directoryobjects"></a>directoryObjects

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Исправление             | 1.0 и бета-версия | Исправлены действия вызовов, привязанные к directoryObjects, при которых возникали сбои со следующим сообщением об ошибке:  Тип значения, возвращаемого в результате операции, невозможен для заданного набора объектов. Это относится к следующим действиям: _microsoft.graph.checkMemberObjects_, _microsoft.graph.getMemberObjects_, _microsoft.graph.checkMemberGroups_, _microsoft.graph.assignLicense_, _microsoft.graph.changePassword_. |

## <a name="december-2015"></a>Декабрь 2015 г.

### <a name="contacts"></a>Контакты

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | В набор объектов личных контактов добавлено свойство mobilePhone. |

### <a name="general"></a>Общие

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Исправление             | 1.0 и бета-версия | Исправлены запросы, в которых используются выражения $filter, указанные для одного и того же свойства несколько раз, при выполнении которых возникали сбои с кодом 500 и отображалось следующее сообщение об ошибке: "Элемент с тем же ключом уже был добавлен". |
| Исправление             | 1.0 и бета-версия | Исправлена ошибка, при которой не учитывался регистр имен и значений параметров действий. |
| Исправление             | 1.0 и бета-версия | Исправлена обработка запросов для полезных нагрузок, содержащих значения null для некоторых внедренных сложных свойств, при которых возникал сбой из-за ссылки на значение null. |
| Дополнение        | 1.0 и бета-версия | Добавлена возможность сортировать и фильтровать свойства сложных типов. |
| Дополнение        | 1.0 и бета-версия | Добавлено свойство authorization_uri в заголовок www-authenticate ответа 401. Вы можете использовать этот универсальный код ресурса для запуска потока получения токена. |
| Дополнение        | 1.0 и бета-версия | Улучшены сообщения об ошибках для пользователей и групп. |

### <a name="groups"></a>Группы

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Исправление             | 1.0 и бета-версия | Исправлен вызов следующих действий групп: _microsoft.graph.addFavorite_, _microsoft.graph.removeFavorite_ и _microsoft.graph.resetUnseenCount_. |

### <a name="messages"></a>Сообщения

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | К типу eventMessage добавлен подтип для свойств eventMessageRequest eventMessage, startDateTime, endDateTime, location, type, recurrence и isOutOfDate. |

### <a name="users"></a>Пользователи

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Исправление             | 1.0 и бета-версия | Устранена возможность выбирать определенные свойства других пользователей, когда на них ссылаются по их основному имени участника-пользователя. Например: https://graph.microsoft.com/v1.0/users/anotherUser@contoso.com?$select=aboutMe |
| Исправление             | 1.0 и бета-версия | Исправлен вызов функции _microsoft.graph.reminderView_, привязанной к пользователю, при котором возникал сбой и отображалось следующее сообщение об ошибке: "Не удалось найти свойство с именем businessPhones в типе Microsoft.OutlookServices.Reminder". |
| Исправление             | 1.0 и бета-версия | Устранена проблема, из-за которой при создании и обновлении пользователей (POST/PATCH /v1.0/users) возникала ошибка 400. |
