---
title: Перечисление объектов iosGeneralDeviceConfiguration
description: Перечисление свойств и связей объектов iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b16ab25554a20dafaab7e6ce0cc6eadf772f646
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756332"
---
# <a name="list-iosgeneraldeviceconfigurations"></a><span data-ttu-id="09ed4-103">Перечисление объектов iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="09ed4-103">List iosGeneralDeviceConfigurations</span></span>

<span data-ttu-id="09ed4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09ed4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09ed4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09ed4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09ed4-106">Перечисление свойств и связей объектов [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09ed4-106">List properties and relationships of the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09ed4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="09ed4-107">Prerequisites</span></span>
<span data-ttu-id="09ed4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09ed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09ed4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09ed4-110">Permission type</span></span>|<span data-ttu-id="09ed4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09ed4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09ed4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09ed4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="09ed4-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09ed4-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09ed4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09ed4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09ed4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09ed4-115">Not supported.</span></span>|
|<span data-ttu-id="09ed4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="09ed4-116">Application</span></span>|<span data-ttu-id="09ed4-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09ed4-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09ed4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09ed4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="09ed4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="09ed4-119">Request headers</span></span>
|<span data-ttu-id="09ed4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09ed4-120">Header</span></span>|<span data-ttu-id="09ed4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="09ed4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09ed4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="09ed4-122">Authorization</span></span>|<span data-ttu-id="09ed4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09ed4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09ed4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="09ed4-124">Accept</span></span>|<span data-ttu-id="09ed4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09ed4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09ed4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09ed4-126">Request body</span></span>
<span data-ttu-id="09ed4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09ed4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09ed4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="09ed4-128">Response</span></span>
<span data-ttu-id="09ed4-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="09ed4-129">If successful, this method returns a `200 OK` response code and a collection of [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09ed4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="09ed4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="09ed4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="09ed4-131">Request</span></span>
<span data-ttu-id="09ed4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09ed4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="09ed4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="09ed4-133">Response</span></span>
<span data-ttu-id="09ed4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09ed4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8922

{
  "value": [
    {
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
  ]
}
```




