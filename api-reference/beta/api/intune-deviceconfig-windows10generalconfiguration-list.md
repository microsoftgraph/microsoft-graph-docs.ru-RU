---
title: Перечисление объектов windows10GeneralConfiguration
description: Перечисление свойств и связей объектов windows10GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ceab79259c12f7dde24d08bc39e99a16e341fdbd
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783108"
---
# <a name="list-windows10generalconfigurations"></a>Перечисление объектов windows10GeneralConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Перечисление свойств и связей объектов [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 16638

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
      "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "taskManagerBlockEndTask": true,
      "energySaverOnBatteryThresholdPercentage": 7,
      "energySaverPluggedInThresholdPercentage": 7,
      "powerLidCloseActionOnBattery": "noAction",
      "powerLidCloseActionPluggedIn": "noAction",
      "powerButtonActionOnBattery": "noAction",
      "powerButtonActionPluggedIn": "noAction",
      "powerSleepButtonActionOnBattery": "noAction",
      "powerSleepButtonActionPluggedIn": "noAction",
      "powerHybridSleepOnBattery": "enabled",
      "powerHybridSleepPluggedIn": "enabled",
      "windows10AppsForceUpdateSchedule": {
        "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
        "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
        "recurrence": "daily",
        "runImmediatelyIfAfterStartDateTime": true
      },
      "enableAutomaticRedeployment": true,
      "microsoftAccountSignInAssistantSettings": "disabled",
      "authenticationAllowSecondaryDevice": true,
      "authenticationWebSignIn": "enabled",
      "authenticationPreferredAzureADTenantDomainName": "Authentication Preferred Azure ADTenant Domain Name value",
      "cryptographyAllowFipsAlgorithmPolicy": true,
      "displayAppListWithGdiDPIScalingTurnedOn": [
        "Display App List With Gdi DPIScaling Turned On value"
      ],
      "displayAppListWithGdiDPIScalingTurnedOff": [
        "Display App List With Gdi DPIScaling Turned Off value"
      ],
      "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
      "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
      "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
      "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
      "enterpriseCloudPrintDiscoveryMaxLimit": 5,
      "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
      "experienceDoNotSyncBrowserSettings": "blockedWithUserOverride",
      "messagingBlockSync": true,
      "messagingBlockMMS": true,
      "messagingBlockRichCommunicationServices": true,
      "printerNames": [
        "Printer Names value"
      ],
      "printerDefaultName": "Printer Default Name value",
      "printerBlockAddition": true,
      "searchBlockDiacritics": true,
      "searchDisableAutoLanguageDetection": true,
      "searchDisableIndexingEncryptedItems": true,
      "searchEnableRemoteQueries": true,
      "searchDisableUseLocation": true,
      "searchDisableLocation": true,
      "searchDisableIndexerBackoff": true,
      "searchDisableIndexingRemovableDrive": true,
      "searchEnableAutomaticIndexSizeManangement": true,
      "searchBlockWebResults": true,
      "findMyFiles": "enabled",
      "securityBlockAzureADJoinedDevicesAutoEncryption": true,
      "diagnosticsDataSubmissionMode": "none",
      "oneDriveDisableFileSync": true,
      "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
      "edgeTelemetryForMicrosoft365Analytics": "intranet",
      "inkWorkspaceAccess": "enabled",
      "inkWorkspaceAccessState": "blocked",
      "inkWorkspaceBlockSuggestedApps": true,
      "smartScreenEnableAppInstallControl": true,
      "smartScreenAppInstallControl": "anywhere",
      "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
      "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
      "bluetoothAllowedServices": [
        "Bluetooth Allowed Services value"
      ],
      "bluetoothBlockAdvertising": true,
      "bluetoothBlockPromptedProximalConnections": true,
      "bluetoothBlockDiscoverableMode": true,
      "bluetoothBlockPrePairing": true,
      "edgeBlockAutofill": true,
      "edgeBlocked": true,
      "edgeCookiePolicy": "allow",
      "edgeBlockDeveloperTools": true,
      "edgeBlockSendingDoNotTrackHeader": true,
      "edgeBlockExtensions": true,
      "edgeBlockInPrivateBrowsing": true,
      "edgeBlockJavaScript": true,
      "edgeBlockPasswordManager": true,
      "edgeBlockAddressBarDropdown": true,
      "edgeBlockCompatibilityList": true,
      "edgeClearBrowsingDataOnExit": true,
      "edgeAllowStartPagesModification": true,
      "edgeDisableFirstRunPage": true,
      "edgeBlockLiveTileDataCollection": true,
      "edgeSyncFavoritesWithInternetExplorer": true,
      "edgeFavoritesListLocation": "Edge Favorites List Location value",
      "edgeBlockEditFavorites": true,
      "edgeNewTabPageURL": "Edge New Tab Page URL value",
      "edgeHomeButtonConfiguration": {
        "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
      },
      "edgeHomeButtonConfigurationEnabled": true,
      "edgeOpensWith": "startPage",
      "edgeBlockSideloadingExtensions": true,
      "edgeRequiredExtensionPackageFamilyNames": [
        "Edge Required Extension Package Family Names value"
      ],
      "edgeBlockPrinting": true,
      "edgeFavoritesBarVisibility": "hide",
      "edgeBlockSavingHistory": true,
      "edgeBlockFullScreenMode": true,
      "edgeBlockWebContentOnNewTabPage": true,
      "edgeBlockTabPreloading": true,
      "edgeBlockPrelaunch": true,
      "edgeShowMessageWhenOpeningInternetExplorerSites": "disabled",
      "edgePreventCertificateErrorOverride": true,
      "edgeKioskModeRestriction": "digitalSignage",
      "edgeKioskResetAfterIdleTimeInMinutes": 4,
      "cellularBlockDataWhenRoaming": true,
      "cellularBlockVpn": true,
      "cellularBlockVpnWhenRoaming": true,
      "cellularData": "required",
      "defenderRequireRealTimeMonitoring": true,
      "defenderRequireBehaviorMonitoring": true,
      "defenderRequireNetworkInspectionSystem": true,
      "defenderScanDownloads": true,
      "defenderScheduleScanEnableLowCpuPriority": true,
      "defenderDisableCatchupQuickScan": true,
      "defenderDisableCatchupFullScan": true,
      "defenderScanScriptsLoadedInInternetExplorer": true,
      "defenderBlockEndUserAccess": true,
      "defenderSignatureUpdateIntervalInHours": 6,
      "defenderMonitorFileActivity": "disable",
      "defenderDaysBeforeDeletingQuarantinedMalware": 12,
      "defenderScanMaxCpu": 2,
      "defenderScanArchiveFiles": true,
      "defenderScanIncomingMail": true,
      "defenderScanRemovableDrivesDuringFullScan": true,
      "defenderScanMappedNetworkDrivesDuringFullScan": true,
      "defenderScanNetworkFiles": true,
      "defenderRequireCloudProtection": true,
      "defenderCloudBlockLevel": "high",
      "defenderCloudExtendedTimeout": 12,
      "defenderCloudExtendedTimeoutInSeconds": 5,
      "defenderPromptForSampleSubmission": "alwaysPrompt",
      "defenderScheduledQuickScanTime": "11:58:49.3840000",
      "defenderScanType": "disabled",
      "defenderSystemScanSchedule": "everyday",
      "defenderScheduledScanTime": "11:59:10.9990000",
      "defenderPotentiallyUnwantedAppAction": "block",
      "defenderPotentiallyUnwantedAppActionSetting": "enable",
      "defenderSubmitSamplesConsentType": "alwaysPrompt",
      "defenderBlockOnAccessProtection": true,
      "defenderDetectedMalwareActions": {
        "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
        "lowSeverity": "clean",
        "moderateSeverity": "clean",
        "highSeverity": "clean",
        "severeSeverity": "clean"
      },
      "defenderFileExtensionsToExclude": [
        "Defender File Extensions To Exclude value"
      ],
      "defenderFilesAndFoldersToExclude": [
        "Defender Files And Folders To Exclude value"
      ],
      "defenderProcessesToExclude": [
        "Defender Processes To Exclude value"
      ],
      "lockScreenAllowTimeoutConfiguration": true,
      "lockScreenBlockActionCenterNotifications": true,
      "lockScreenBlockCortana": true,
      "lockScreenBlockToastNotifications": true,
      "lockScreenTimeoutInSeconds": 10,
      "lockScreenActivateAppsWithVoice": "enabled",
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordMinimumCharacterSetCount": 0,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequired": true,
      "passwordRequireWhenResumeFromIdleState": true,
      "passwordRequiredType": "alphanumeric",
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordMinimumAgeInDays": 8,
      "privacyAdvertisingId": "blocked",
      "privacyAutoAcceptPairingAndConsentPrompts": true,
      "privacyDisableLaunchExperience": true,
      "privacyBlockInputPersonalization": true,
      "privacyBlockPublishUserActivities": true,
      "privacyBlockActivityFeed": true,
      "activateAppsWithVoice": "enabled",
      "startBlockUnpinningAppsFromTaskbar": true,
      "startMenuAppListVisibility": "collapse",
      "startMenuHideChangeAccountSettings": true,
      "startMenuHideFrequentlyUsedApps": true,
      "startMenuHideHibernate": true,
      "startMenuHideLock": true,
      "startMenuHidePowerButton": true,
      "startMenuHideRecentJumpLists": true,
      "startMenuHideRecentlyAddedApps": true,
      "startMenuHideRestartOptions": true,
      "startMenuHideShutDown": true,
      "startMenuHideSignOut": true,
      "startMenuHideSleep": true,
      "startMenuHideSwitchAccount": true,
      "startMenuHideUserTile": true,
      "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
      "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
      "startMenuMode": "fullScreen",
      "startMenuPinnedFolderDocuments": "hide",
      "startMenuPinnedFolderDownloads": "hide",
      "startMenuPinnedFolderFileExplorer": "hide",
      "startMenuPinnedFolderHomeGroup": "hide",
      "startMenuPinnedFolderMusic": "hide",
      "startMenuPinnedFolderNetwork": "hide",
      "startMenuPinnedFolderPersonalFolder": "hide",
      "startMenuPinnedFolderPictures": "hide",
      "startMenuPinnedFolderSettings": "hide",
      "startMenuPinnedFolderVideos": "hide",
      "settingsBlockSettingsApp": true,
      "settingsBlockSystemPage": true,
      "settingsBlockDevicesPage": true,
      "settingsBlockNetworkInternetPage": true,
      "settingsBlockPersonalizationPage": true,
      "settingsBlockAccountsPage": true,
      "settingsBlockTimeLanguagePage": true,
      "settingsBlockEaseOfAccessPage": true,
      "settingsBlockPrivacyPage": true,
      "settingsBlockUpdateSecurityPage": true,
      "settingsBlockAppsPage": true,
      "settingsBlockGamingPage": true,
      "windowsSpotlightBlockConsumerSpecificFeatures": true,
      "windowsSpotlightBlocked": true,
      "windowsSpotlightBlockOnActionCenter": true,
      "windowsSpotlightBlockTailoredExperiences": true,
      "windowsSpotlightBlockThirdPartyNotifications": true,
      "windowsSpotlightBlockWelcomeExperience": true,
      "windowsSpotlightBlockWindowsTips": true,
      "windowsSpotlightConfigureOnLockScreen": "disabled",
      "networkProxyApplySettingsDeviceWide": true,
      "networkProxyDisableAutoDetect": true,
      "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
      "networkProxyServer": {
        "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
        "address": "Address value",
        "exceptions": [
          "Exceptions value"
        ],
        "useForLocalAddresses": true
      },
      "accountsBlockAddingNonMicrosoftAccountEmail": true,
      "antiTheftModeBlocked": true,
      "bluetoothBlocked": true,
      "cameraBlocked": true,
      "connectedDevicesServiceBlocked": true,
      "certificatesBlockManualRootCertificateInstallation": true,
      "copyPasteBlocked": true,
      "cortanaBlocked": true,
      "deviceManagementBlockFactoryResetOnMobile": true,
      "deviceManagementBlockManualUnenroll": true,
      "safeSearchFilter": "strict",
      "edgeBlockPopups": true,
      "edgeBlockSearchSuggestions": true,
      "edgeBlockSearchEngineCustomization": true,
      "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
      "edgeSendIntranetTrafficToInternetExplorer": true,
      "edgeRequireSmartScreen": true,
      "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
      "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
      "edgeSearchEngine": {
        "@odata.type": "microsoft.graph.edgeSearchEngineBase"
      },
      "edgeHomepageUrls": [
        "Edge Homepage Urls value"
      ],
      "edgeBlockAccessToAboutFlags": true,
      "smartScreenBlockPromptOverride": true,
      "smartScreenBlockPromptOverrideForFiles": true,
      "webRtcBlockLocalhostIpAddress": true,
      "internetSharingBlocked": true,
      "settingsBlockAddProvisioningPackage": true,
      "settingsBlockRemoveProvisioningPackage": true,
      "settingsBlockChangeSystemTime": true,
      "settingsBlockEditDeviceName": true,
      "settingsBlockChangeRegion": true,
      "settingsBlockChangeLanguage": true,
      "settingsBlockChangePowerSleep": true,
      "locationServicesBlocked": true,
      "microsoftAccountBlocked": true,
      "microsoftAccountBlockSettingsSync": true,
      "nfcBlocked": true,
      "resetProtectionModeBlocked": true,
      "screenCaptureBlocked": true,
      "storageBlockRemovableStorage": true,
      "storageRequireMobileDeviceEncryption": true,
      "usbBlocked": true,
      "voiceRecordingBlocked": true,
      "wiFiBlockAutomaticConnectHotspots": true,
      "wiFiBlocked": true,
      "wiFiBlockManualConfiguration": true,
      "wiFiScanInterval": 0,
      "wirelessDisplayBlockProjectionToThisDevice": true,
      "wirelessDisplayBlockUserInputFromReceiver": true,
      "wirelessDisplayRequirePinForPairing": true,
      "windowsStoreBlocked": true,
      "appsAllowTrustedAppsSideloading": "blocked",
      "windowsStoreBlockAutoUpdate": true,
      "developerUnlockSetting": "blocked",
      "sharedUserAppDataAllowed": true,
      "appsBlockWindowsStoreOriginatedApps": true,
      "windowsStoreEnablePrivateStoreOnly": true,
      "storageRestrictAppDataToSystemVolume": true,
      "storageRestrictAppInstallToSystemVolume": true,
      "gameDvrBlocked": true,
      "experienceBlockDeviceDiscovery": true,
      "experienceBlockErrorDialogWhenNoSIM": true,
      "experienceBlockTaskSwitcher": true,
      "logonBlockFastUserSwitching": true,
      "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
      "appManagementMSIAllowUserControlOverInstall": true,
      "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
      "dataProtectionBlockDirectMemoryAccess": true,
      "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
        "App Management Package Family Names To Launch After Log On value"
      ],
      "uninstallBuiltInApps": true,
      "configureTimeZone": "Configure Time Zone value"
    }
  ]
}
```



