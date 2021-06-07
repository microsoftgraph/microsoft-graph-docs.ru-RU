---
title: Get iosGeneralDeviceConfiguration
description: Чтение свойств и связей объекта iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a346f34c6c9f48cbe05bb21009b368b6f8f63de1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757075"
---
# <a name="get-iosgeneraldeviceconfiguration"></a><span data-ttu-id="3fade-103">Get iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3fade-103">Get iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="3fade-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fade-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3fade-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3fade-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fade-106">Чтение свойств и связей объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3fade-106">Read properties and relationships of the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fade-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3fade-107">Prerequisites</span></span>
<span data-ttu-id="3fade-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fade-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fade-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fade-110">Permission type</span></span>|<span data-ttu-id="3fade-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fade-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fade-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fade-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3fade-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fade-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3fade-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fade-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fade-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fade-115">Not supported.</span></span>|
|<span data-ttu-id="3fade-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="3fade-116">Application</span></span>|<span data-ttu-id="3fade-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fade-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fade-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fade-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3fade-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3fade-119">Optional query parameters</span></span>
<span data-ttu-id="3fade-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3fade-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3fade-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fade-121">Request headers</span></span>
|<span data-ttu-id="3fade-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3fade-122">Header</span></span>|<span data-ttu-id="3fade-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3fade-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fade-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fade-124">Authorization</span></span>|<span data-ttu-id="3fade-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fade-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fade-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3fade-126">Accept</span></span>|<span data-ttu-id="3fade-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3fade-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fade-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3fade-128">Request body</span></span>
<span data-ttu-id="3fade-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3fade-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fade-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fade-130">Response</span></span>
<span data-ttu-id="3fade-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3fade-131">If successful, this method returns a `200 OK` response code and [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fade-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3fade-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fade-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fade-133">Request</span></span>
<span data-ttu-id="3fade-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fade-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3fade-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fade-135">Response</span></span>
<span data-ttu-id="3fade-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3fade-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8470

{
  "value": {
    "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
    "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "accountBlockModification": true,
    "activationLockAllowWhenSupervised": true,
    "airDropBlocked": true,
    "airDropForceUnmanagedDropTarget": true,
    "airPlayForcePairingPasswordForOutgoingRequests": true,
    "appleWatchBlockPairing": true,
    "appleWatchForceWristDetection": true,
    "appleNewsBlocked": true,
    "appsSingleAppModeList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "appsVisibilityList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "appsVisibilityListType": "appsInListCompliant",
    "appStoreBlockAutomaticDownloads": true,
    "appStoreBlocked": true,
    "appStoreBlockInAppPurchases": true,
    "appStoreBlockUIAppInstallation": true,
    "appStoreRequirePassword": true,
    "bluetoothBlockModification": true,
    "cameraBlocked": true,
    "cellularBlockDataRoaming": true,
    "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
    "cellularBlockPerAppDataModification": true,
    "cellularBlockPersonalHotspot": true,
    "cellularBlockVoiceRoaming": true,
    "certificatesBlockUntrustedTlsCertificates": true,
    "classroomAppBlockRemoteScreenObservation": true,
    "classroomAppForceUnpromptedScreenObservation": true,
    "compliantAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "compliantAppListType": "appsInListCompliant",
    "configurationProfileBlockChanges": true,
    "definitionLookupBlocked": true,
    "deviceBlockEnableRestrictions": true,
    "deviceBlockEraseContentAndSettings": true,
    "deviceBlockNameModification": true,
    "diagnosticDataBlockSubmission": true,
    "diagnosticDataBlockSubmissionModification": true,
    "documentsBlockManagedDocumentsInUnmanagedApps": true,
    "documentsBlockUnmanagedDocumentsInManagedApps": true,
    "emailInDomainSuffixes": [
      "Email In Domain Suffixes value"
    ],
    "enterpriseAppBlockTrust": true,
    "enterpriseAppBlockTrustModification": true,
    "faceTimeBlocked": true,
    "findMyFriendsBlocked": true,
    "gamingBlockGameCenterFriends": true,
    "gamingBlockMultiplayer": true,
    "gameCenterBlocked": true,
    "hostPairingBlocked": true,
    "iBooksStoreBlocked": true,
    "iBooksStoreBlockErotica": true,
    "iCloudBlockActivityContinuation": true,
    "iCloudBlockBackup": true,
    "iCloudBlockDocumentSync": true,
    "iCloudBlockManagedAppsSync": true,
    "iCloudBlockPhotoLibrary": true,
    "iCloudBlockPhotoStreamSync": true,
    "iCloudBlockSharedPhotoStream": true,
    "iCloudRequireEncryptedBackup": true,
    "iTunesBlockExplicitContent": true,
    "iTunesBlockMusicService": true,
    "iTunesBlockRadio": true,
    "keyboardBlockAutoCorrect": true,
    "keyboardBlockDictation": true,
    "keyboardBlockPredictive": true,
    "keyboardBlockShortcuts": true,
    "keyboardBlockSpellCheck": true,
    "kioskModeAllowAssistiveSpeak": true,
    "kioskModeAllowAssistiveTouchSettings": true,
    "kioskModeAllowAutoLock": true,
    "kioskModeAllowColorInversionSettings": true,
    "kioskModeAllowRingerSwitch": true,
    "kioskModeAllowScreenRotation": true,
    "kioskModeAllowSleepButton": true,
    "kioskModeAllowTouchscreen": true,
    "kioskModeAllowVoiceOverSettings": true,
    "kioskModeAllowVolumeButtons": true,
    "kioskModeAllowZoomSettings": true,
    "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
    "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
    "kioskModeRequireAssistiveTouch": true,
    "kioskModeRequireColorInversion": true,
    "kioskModeRequireMonoAudio": true,
    "kioskModeRequireVoiceOver": true,
    "kioskModeRequireZoom": true,
    "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
    "lockScreenBlockControlCenter": true,
    "lockScreenBlockNotificationView": true,
    "lockScreenBlockPassbook": true,
    "lockScreenBlockTodayView": true,
    "mediaContentRatingAustralia": {
      "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingCanada": {
      "@odata.type": "microsoft.graph.mediaContentRatingCanada",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingFrance": {
      "@odata.type": "microsoft.graph.mediaContentRatingFrance",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingGermany": {
      "@odata.type": "microsoft.graph.mediaContentRatingGermany",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingIreland": {
      "@odata.type": "microsoft.graph.mediaContentRatingIreland",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingJapan": {
      "@odata.type": "microsoft.graph.mediaContentRatingJapan",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingNewZealand": {
      "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingUnitedKingdom": {
      "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingUnitedStates": {
      "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "networkUsageRules": [
      {
        "@odata.type": "microsoft.graph.iosNetworkUsageRule",
        "managedApps": [
          {
            "@odata.type": "microsoft.graph.appListItem",
            "name": "Name value",
            "publisher": "Publisher value",
            "appStoreUrl": "https://example.com/appStoreUrl/",
            "appId": "App Id value"
          }
        ],
        "cellularDataBlockWhenRoaming": true,
        "cellularDataBlocked": true
      }
    ],
    "mediaContentRatingApps": "allBlocked",
    "messagesBlocked": true,
    "notificationsBlockSettingsModification": true,
    "passcodeBlockFingerprintUnlock": true,
    "passcodeBlockFingerprintModification": true,
    "passcodeBlockModification": true,
    "passcodeBlockSimple": true,
    "passcodeExpirationDays": 6,
    "passcodeMinimumLength": 5,
    "passcodeMinutesOfInactivityBeforeLock": 5,
    "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
    "passcodeMinimumCharacterSetCount": 0,
    "passcodePreviousPasscodeBlockCount": 2,
    "passcodeSignInFailureCountBeforeWipe": 4,
    "passcodeRequiredType": "alphanumeric",
    "passcodeRequired": true,
    "podcastsBlocked": true,
    "safariBlockAutofill": true,
    "safariBlockJavaScript": true,
    "safariBlockPopups": true,
    "safariBlocked": true,
    "safariCookieSettings": "blockAlways",
    "safariManagedDomains": [
      "Safari Managed Domains value"
    ],
    "safariPasswordAutoFillDomains": [
      "Safari Password Auto Fill Domains value"
    ],
    "safariRequireFraudWarning": true,
    "screenCaptureBlocked": true,
    "siriBlocked": true,
    "siriBlockedWhenLocked": true,
    "siriBlockUserGeneratedContent": true,
    "siriRequireProfanityFilter": true,
    "spotlightBlockInternetResults": true,
    "voiceDialingBlocked": true,
    "wallpaperBlockModification": true,
    "wiFiConnectOnlyToConfiguredNetworks": true
  }
}
```




