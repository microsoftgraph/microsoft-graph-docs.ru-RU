---
title: Get androidDeviceOwnerGeneralDeviceConfiguration
description: Чтение свойств и связей объекта AndroidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b79f8fda6e0539602fecc032fc1888ebdcf67ef2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138719"
---
# <a name="get-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="398ce-103">Get androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="398ce-103">Get androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="398ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="398ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="398ce-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="398ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="398ce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="398ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="398ce-107">Чтение свойств и связей [объекта AndroidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="398ce-107">Read properties and relationships of the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="398ce-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="398ce-108">Prerequisites</span></span>
<span data-ttu-id="398ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="398ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="398ce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="398ce-111">Permission type</span></span>|<span data-ttu-id="398ce-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="398ce-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="398ce-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="398ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="398ce-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="398ce-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="398ce-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="398ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="398ce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="398ce-116">Not supported.</span></span>|
|<span data-ttu-id="398ce-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="398ce-117">Application</span></span>|<span data-ttu-id="398ce-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="398ce-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="398ce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="398ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="398ce-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="398ce-120">Optional query parameters</span></span>
<span data-ttu-id="398ce-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="398ce-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="398ce-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="398ce-122">Request headers</span></span>
|<span data-ttu-id="398ce-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="398ce-123">Header</span></span>|<span data-ttu-id="398ce-124">Значение</span><span class="sxs-lookup"><span data-stu-id="398ce-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="398ce-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="398ce-125">Authorization</span></span>|<span data-ttu-id="398ce-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="398ce-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="398ce-127">Accept</span><span class="sxs-lookup"><span data-stu-id="398ce-127">Accept</span></span>|<span data-ttu-id="398ce-128">application/json</span><span class="sxs-lookup"><span data-stu-id="398ce-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="398ce-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="398ce-129">Request body</span></span>
<span data-ttu-id="398ce-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="398ce-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="398ce-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="398ce-131">Response</span></span>
<span data-ttu-id="398ce-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="398ce-132">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="398ce-133">Пример</span><span class="sxs-lookup"><span data-stu-id="398ce-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="398ce-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="398ce-134">Request</span></span>
<span data-ttu-id="398ce-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="398ce-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="398ce-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="398ce-136">Response</span></span>
<span data-ttu-id="398ce-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="398ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7876

{
  "value": {
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
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "playStoreMode": "allowList",
    "safeBootBlocked": true,
    "screenCaptureBlocked": true,
    "securityAllowDebuggingFeatures": true,
    "securityRequireVerifyApps": true,
    "statusBarBlocked": true,
    "stayOnModes": [
      "ac"
    ],
    "storageAllowUsb": true,
    "storageBlockExternalMedia": true,
    "storageBlockUsbFileTransfer": true,
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
    "workProfilePasswordRequiredType": "required"
  }
}
```




