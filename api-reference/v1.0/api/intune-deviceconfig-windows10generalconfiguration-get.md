---
title: Get windows10GeneralConfiguration
description: Чтение свойств и связей объекта windows10GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6563890dffb9ba7dec4037cc67377f7ff11f94e4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759235"
---
# <a name="get-windows10generalconfiguration"></a><span data-ttu-id="14058-103">Get windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="14058-103">Get windows10GeneralConfiguration</span></span>

<span data-ttu-id="14058-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14058-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14058-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14058-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14058-106">Чтение свойств и связей объекта [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14058-106">Read properties and relationships of the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14058-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="14058-107">Prerequisites</span></span>
<span data-ttu-id="14058-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14058-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14058-110">Permission type</span></span>|<span data-ttu-id="14058-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14058-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14058-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14058-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14058-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14058-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14058-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14058-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14058-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14058-115">Not supported.</span></span>|
|<span data-ttu-id="14058-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="14058-116">Application</span></span>|<span data-ttu-id="14058-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14058-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14058-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14058-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14058-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="14058-119">Optional query parameters</span></span>
<span data-ttu-id="14058-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="14058-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14058-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14058-121">Request headers</span></span>
|<span data-ttu-id="14058-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14058-122">Header</span></span>|<span data-ttu-id="14058-123">Значение</span><span class="sxs-lookup"><span data-stu-id="14058-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14058-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="14058-124">Authorization</span></span>|<span data-ttu-id="14058-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14058-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14058-126">Accept</span><span class="sxs-lookup"><span data-stu-id="14058-126">Accept</span></span>|<span data-ttu-id="14058-127">application/json</span><span class="sxs-lookup"><span data-stu-id="14058-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14058-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14058-128">Request body</span></span>
<span data-ttu-id="14058-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="14058-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14058-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="14058-130">Response</span></span>
<span data-ttu-id="14058-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="14058-131">If successful, this method returns a `200 OK` response code and [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14058-132">Пример</span><span class="sxs-lookup"><span data-stu-id="14058-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="14058-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="14058-133">Request</span></span>
<span data-ttu-id="14058-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14058-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="14058-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="14058-135">Response</span></span>
<span data-ttu-id="14058-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14058-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10479

{
  "value": {
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
}
```




