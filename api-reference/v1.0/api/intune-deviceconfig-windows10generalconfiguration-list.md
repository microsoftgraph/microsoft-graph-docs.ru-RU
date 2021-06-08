---
title: Перечисление объектов windows10GeneralConfiguration
description: Перечисление свойств и связей объектов windows10GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b1bdb2193d1931b15ac6279ef96784d4b7ae6874
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758152"
---
# <a name="list-windows10generalconfigurations"></a><span data-ttu-id="c75ef-103">Перечисление объектов windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="c75ef-103">List windows10GeneralConfigurations</span></span>

<span data-ttu-id="c75ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c75ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c75ef-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c75ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c75ef-106">Перечисление свойств и связей объектов [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c75ef-106">List properties and relationships of the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c75ef-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c75ef-107">Prerequisites</span></span>
<span data-ttu-id="c75ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c75ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c75ef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c75ef-110">Permission type</span></span>|<span data-ttu-id="c75ef-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c75ef-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c75ef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c75ef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c75ef-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c75ef-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c75ef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c75ef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c75ef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c75ef-115">Not supported.</span></span>|
|<span data-ttu-id="c75ef-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c75ef-116">Application</span></span>|<span data-ttu-id="c75ef-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c75ef-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c75ef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c75ef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c75ef-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c75ef-119">Request headers</span></span>
|<span data-ttu-id="c75ef-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c75ef-120">Header</span></span>|<span data-ttu-id="c75ef-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c75ef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c75ef-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c75ef-122">Authorization</span></span>|<span data-ttu-id="c75ef-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c75ef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c75ef-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c75ef-124">Accept</span></span>|<span data-ttu-id="c75ef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c75ef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c75ef-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c75ef-126">Request body</span></span>
<span data-ttu-id="c75ef-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c75ef-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c75ef-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c75ef-128">Response</span></span>
<span data-ttu-id="c75ef-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c75ef-129">If successful, this method returns a `200 OK` response code and a collection of [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c75ef-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c75ef-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c75ef-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c75ef-131">Request</span></span>
<span data-ttu-id="c75ef-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c75ef-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="c75ef-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c75ef-133">Response</span></span>
<span data-ttu-id="c75ef-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c75ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10959

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
      "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
      "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
      "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
      "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
      "enterpriseCloudPrintDiscoveryMaxLimit": 5,
      "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
      "searchBlockDiacritics": true,
      "searchDisableAutoLanguageDetection": true,
      "searchDisableIndexingEncryptedItems": true,
      "searchEnableRemoteQueries": true,
      "searchDisableIndexerBackoff": true,
      "searchDisableIndexingRemovableDrive": true,
      "searchEnableAutomaticIndexSizeManangement": true,
      "diagnosticsDataSubmissionMode": "none",
      "oneDriveDisableFileSync": true,
      "smartScreenEnableAppInstallControl": true,
      "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
      "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
      "bluetoothAllowedServices": [
        "Bluetooth Allowed Services value"
      ],
      "bluetoothBlockAdvertising": true,
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
      "cellularBlockDataWhenRoaming": true,
      "cellularBlockVpn": true,
      "cellularBlockVpnWhenRoaming": true,
      "defenderRequireRealTimeMonitoring": true,
      "defenderRequireBehaviorMonitoring": true,
      "defenderRequireNetworkInspectionSystem": true,
      "defenderScanDownloads": true,
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
      "defenderPromptForSampleSubmission": "alwaysPrompt",
      "defenderScheduledQuickScanTime": "11:58:49.3840000",
      "defenderScanType": "disabled",
      "defenderSystemScanSchedule": "everyday",
      "defenderScheduledScanTime": "11:59:10.9990000",
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
      "privacyAdvertisingId": "blocked",
      "privacyAutoAcceptPairingAndConsentPrompts": true,
      "privacyBlockInputPersonalization": true,
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
      "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true
    }
  ]
}
```




