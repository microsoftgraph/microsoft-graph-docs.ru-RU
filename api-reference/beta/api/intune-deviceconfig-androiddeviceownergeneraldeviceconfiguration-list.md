---
title: Перечисление объектов androidDeviceOwnerGeneralDeviceConfigurations
description: Список свойств и связей объектов androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c457f96c752c82f40bffa085f37e1144a314cb41
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670977"
---
# <a name="list-androiddeviceownergeneraldeviceconfigurations"></a>Перечисление объектов androidDeviceOwnerGeneralDeviceConfigurations

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

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
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного `200 OK` выполнения этот метод возвращает код отклика и коллекцию объектов [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в теле отклика.

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
Content-Length: 11343

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
      "id": "edad943d-943d-edad-3d94-aded3d94aded",
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
      "azureAdSharedDeviceDataClearApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "accountsBlockModification": true,
      "appsAllowInstallFromUnknownSources": true,
      "appsAutoUpdatePolicy": "userChoice",
      "appsDefaultPermissionPolicy": "prompt",
      "appsRecommendSkippingFirstUseHints": true,
      "bluetoothBlockConfiguration": true,
      "bluetoothBlockContactSharing": true,
      "cameraBlocked": true,
      "cellularBlockWiFiTethering": true,
      "certificateCredentialConfigurationDisabled": true,
      "crossProfilePoliciesAllowCopyPaste": true,
      "crossProfilePoliciesAllowDataSharing": "crossProfileDataSharingBlocked",
      "crossProfilePoliciesShowWorkContactsInPersonalProfile": true,
      "microsoftLauncherConfigurationEnabled": true,
      "microsoftLauncherCustomWallpaperEnabled": true,
      "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
      "microsoftLauncherCustomWallpaperAllowUserModification": true,
      "microsoftLauncherFeedEnabled": true,
      "microsoftLauncherFeedAllowUserModification": true,
      "microsoftLauncherDockPresenceConfiguration": "show",
      "microsoftLauncherDockPresenceAllowUserModification": true,
      "microsoftLauncherSearchBarPlacementConfiguration": "top",
      "enrollmentProfile": "dedicatedDevice",
      "dataRoamingBlocked": true,
      "dateTimeConfigurationBlocked": true,
      "detailedHelpText": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
        "localizedMessages": [
          {
            "@odata.type": "microsoft.graph.keyValuePair",
            "name": "Name value",
            "value": "Value value"
          }
        ],
        "defaultMessage": "Default Message value"
      },
      "deviceOwnerLockScreenMessage": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
        "localizedMessages": [
          {
            "@odata.type": "microsoft.graph.keyValuePair",
            "name": "Name value",
            "value": "Value value"
          }
        ],
        "defaultMessage": "Default Message value"
      },
      "securityCommonCriteriaModeEnabled": true,
      "factoryResetDeviceAdministratorEmails": [
        "Factory Reset Device Administrator Emails value"
      ],
      "factoryResetBlocked": true,
      "globalProxy": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
        "proxyAutoConfigURL": "Proxy Auto Config URL value"
      },
      "googleAccountsBlocked": true,
      "kioskCustomizationDeviceSettingsBlocked": true,
      "kioskCustomizationPowerButtonActionsBlocked": true,
      "kioskCustomizationStatusBar": "notificationsAndSystemInfoEnabled",
      "kioskCustomizationSystemErrorWarnings": true,
      "kioskCustomizationSystemNavigation": "navigationEnabled",
      "kioskModeScreenSaverConfigurationEnabled": true,
      "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
      "kioskModeScreenSaverDisplayTimeInSeconds": 8,
      "kioskModeScreenSaverStartDelayInSeconds": 7,
      "kioskModeScreenSaverDetectMediaDisabled": true,
      "kioskModeApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
      "kioskModeExitCode": "Kiosk Mode Exit Code value",
      "kioskModeVirtualHomeButtonEnabled": true,
      "kioskModeVirtualHomeButtonType": "swipeUp",
      "kioskModeBluetoothConfigurationEnabled": true,
      "kioskModeWiFiConfigurationEnabled": true,
      "kioskModeFlashlightConfigurationEnabled": true,
      "kioskModeMediaVolumeConfigurationEnabled": true,
      "kioskModeShowDeviceInfo": true,
      "kioskModeManagedSettingsEntryDisabled": true,
      "kioskModeDebugMenuEasyAccessEnabled": true,
      "kioskModeShowAppNotificationBadge": true,
      "kioskModeScreenOrientation": "portrait",
      "kioskModeIconSize": "smallest",
      "kioskModeFolderIcon": "darkSquare",
      "kioskModeWifiAllowedSsids": [
        "Kiosk Mode Wifi Allowed Ssids value"
      ],
      "kioskModeAppOrderEnabled": true,
      "kioskModeAppsInFolderOrderedByName": true,
      "kioskModeGridHeight": 3,
      "kioskModeGridWidth": 2,
      "kioskModeLockHomeScreen": true,
      "kioskModeManagedFolders": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
          "folderName": "Folder Name value",
          "folderIdentifier": "Folder Identifier value",
          "items": [
            {
              "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
              "label": "Label value",
              "link": "Link value"
            }
          ]
        }
      ],
      "kioskModeAppPositions": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
          "position": 8,
          "item": {
            "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
            "label": "Label value",
            "link": "Link value"
          }
        }
      ],
      "kioskModeManagedHomeScreenAutoSignout": true,
      "kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds": 7,
      "kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds": 8,
      "kioskModeManagedHomeScreenPinComplexity": "simple",
      "kioskModeManagedHomeScreenPinRequired": true,
      "kioskModeManagedHomeScreenPinRequiredToResume": true,
      "kioskModeManagedHomeScreenSignInBackground": "Kiosk Mode Managed Home Screen Sign In Background value",
      "kioskModeManagedHomeScreenSignInBrandingLogo": "Kiosk Mode Managed Home Screen Sign In Branding Logo value",
      "kioskModeManagedHomeScreenSignInEnabled": true,
      "kioskModeUseManagedHomeScreenApp": "singleAppMode",
      "microphoneForceMute": true,
      "networkEscapeHatchAllowed": true,
      "nfcBlockOutgoingBeam": true,
      "passwordBlockKeyguard": true,
      "passwordBlockKeyguardFeatures": [
        "camera"
      ],
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinimumLetterCharacters": 15,
      "passwordMinimumLowerCaseCharacters": 2,
      "passwordMinimumNonLetterCharacters": 2,
      "passwordMinimumNumericCharacters": 0,
      "passwordMinimumSymbolCharacters": 15,
      "passwordMinimumUpperCaseCharacters": 2,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordCountToBlock": 4,
      "passwordRequiredType": "required",
      "passwordRequireUnlock": "daily",
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "playStoreMode": "allowList",
      "screenCaptureBlocked": true,
      "securityDeveloperSettingsEnabled": true,
      "securityRequireVerifyApps": true,
      "shortHelpText": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
        "localizedMessages": [
          {
            "@odata.type": "microsoft.graph.keyValuePair",
            "name": "Name value",
            "value": "Value value"
          }
        ],
        "defaultMessage": "Default Message value"
      },
      "statusBarBlocked": true,
      "stayOnModes": [
        "ac"
      ],
      "storageAllowUsb": true,
      "storageBlockExternalMedia": true,
      "storageBlockUsbFileTransfer": true,
      "systemUpdateFreezePeriods": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerSystemUpdateFreezePeriod",
          "startMonth": 10,
          "startDay": 8,
          "endMonth": 8,
          "endDay": 6
        }
      ],
      "systemUpdateWindowStartMinutesAfterMidnight": 11,
      "systemUpdateWindowEndMinutesAfterMidnight": 9,
      "systemUpdateInstallType": "postpone",
      "systemWindowsBlocked": true,
      "usersBlockAdd": true,
      "usersBlockRemove": true,
      "volumeBlockAdjustment": true,
      "vpnAlwaysOnLockdownMode": true,
      "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
      "wifiBlockEditConfigurations": true,
      "wifiBlockEditPolicyDefinedConfigurations": true,
      "personalProfileAppsAllowInstallFromUnknownSources": true,
      "personalProfileCameraBlocked": true,
      "personalProfileScreenCaptureBlocked": true,
      "personalProfilePlayStoreMode": "blockedApps",
      "personalProfilePersonalApplications": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "workProfilePasswordExpirationDays": 1,
      "workProfilePasswordMinimumLength": 0,
      "workProfilePasswordMinimumNumericCharacters": 11,
      "workProfilePasswordMinimumNonLetterCharacters": 13,
      "workProfilePasswordMinimumLetterCharacters": 10,
      "workProfilePasswordMinimumLowerCaseCharacters": 13,
      "workProfilePasswordMinimumUpperCaseCharacters": 13,
      "workProfilePasswordMinimumSymbolCharacters": 10,
      "workProfilePasswordPreviousPasswordCountToBlock": 15,
      "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
      "workProfilePasswordRequiredType": "required",
      "workProfilePasswordRequireUnlock": "daily"
    }
  ]
}
```




