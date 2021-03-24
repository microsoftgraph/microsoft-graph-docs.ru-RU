---
title: Перечисление объектов macOSGeneralDeviceConfiguration
description: Список свойств и связей объектов macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b7fa467c7766ce4a05065f5ad9da8df74d3004d3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137226"
---
# <a name="list-macosgeneraldeviceconfigurations"></a><span data-ttu-id="aa6bd-103">Перечисление объектов macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="aa6bd-103">List macOSGeneralDeviceConfigurations</span></span>

<span data-ttu-id="aa6bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa6bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa6bd-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa6bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa6bd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa6bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa6bd-107">Список свойств и связей объектов [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa6bd-107">List properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa6bd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="aa6bd-108">Prerequisites</span></span>
<span data-ttu-id="aa6bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa6bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa6bd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa6bd-111">Permission type</span></span>|<span data-ttu-id="aa6bd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa6bd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa6bd-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa6bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa6bd-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa6bd-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aa6bd-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa6bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa6bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa6bd-116">Not supported.</span></span>|
|<span data-ttu-id="aa6bd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="aa6bd-117">Application</span></span>|<span data-ttu-id="aa6bd-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa6bd-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa6bd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa6bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="aa6bd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aa6bd-120">Request headers</span></span>
|<span data-ttu-id="aa6bd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aa6bd-121">Header</span></span>|<span data-ttu-id="aa6bd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aa6bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa6bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa6bd-123">Authorization</span></span>|<span data-ttu-id="aa6bd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa6bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa6bd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aa6bd-125">Accept</span></span>|<span data-ttu-id="aa6bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa6bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa6bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa6bd-127">Request body</span></span>
<span data-ttu-id="aa6bd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa6bd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa6bd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa6bd-129">Response</span></span>
<span data-ttu-id="aa6bd-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa6bd-130">If successful, this method returns a `200 OK` response code and a collection of [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa6bd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="aa6bd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa6bd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa6bd-132">Request</span></span>
<span data-ttu-id="aa6bd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa6bd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="aa6bd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa6bd-134">Response</span></span>
<span data-ttu-id="aa6bd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa6bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5369

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
      "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
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
      "emailInDomainSuffixes": [
        "Email In Domain Suffixes value"
      ],
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumCharacterSetCount": 0,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequiredType": "alphanumeric",
      "passwordRequired": true,
      "passwordMaximumAttemptCount": 11,
      "passwordMinutesUntilFailedLoginReset": 4,
      "keychainBlockCloudSync": true,
      "airPrintBlocked": true,
      "airPrintForceTrustedTLS": true,
      "airPrintBlockiBeaconDiscovery": true,
      "safariBlockAutofill": true,
      "cameraBlocked": true,
      "iTunesBlockMusicService": true,
      "spotlightBlockInternetResults": true,
      "keyboardBlockDictation": true,
      "definitionLookupBlocked": true,
      "appleWatchBlockAutoUnlock": true,
      "iTunesBlockFileSharing": true,
      "iCloudBlockDocumentSync": true,
      "iCloudBlockMail": true,
      "iCloudBlockAddressBook": true,
      "iCloudBlockCalendar": true,
      "iCloudBlockReminders": true,
      "iCloudBlockBookmarks": true,
      "iCloudBlockNotes": true,
      "airDropBlocked": true,
      "passwordBlockModification": true,
      "passwordBlockFingerprintUnlock": true,
      "passwordBlockAutoFill": true,
      "passwordBlockProximityRequests": true,
      "passwordBlockAirDropSharing": true,
      "softwareUpdatesEnforcedDelayInDays": 2,
      "updateDelayPolicy": "delayOSUpdateVisibility",
      "contentCachingBlocked": true,
      "iCloudBlockPhotoLibrary": true,
      "screenCaptureBlocked": true,
      "classroomAppBlockRemoteScreenObservation": true,
      "classroomAppForceUnpromptedScreenObservation": true,
      "classroomForceAutomaticallyJoinClasses": true,
      "classroomForceRequestPermissionToLeaveClasses": true,
      "classroomForceUnpromptedAppAndDeviceLock": true,
      "iCloudBlockActivityContinuation": true,
      "privacyAccessControls": [
        {
          "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem",
          "displayName": "Display Name value",
          "identifier": "Identifier value",
          "identifierType": "path",
          "codeRequirement": "Code Requirement value",
          "staticCodeValidation": true,
          "blockCamera": true,
          "blockMicrophone": true,
          "blockScreenCapture": true,
          "blockListenEvent": true,
          "speechRecognition": "enabled",
          "accessibility": "enabled",
          "addressBook": "enabled",
          "calendar": "enabled",
          "reminders": "enabled",
          "photos": "enabled",
          "mediaLibrary": "enabled",
          "fileProviderPresence": "enabled",
          "systemPolicyAllFiles": "enabled",
          "systemPolicySystemAdminFiles": "enabled",
          "systemPolicyDesktopFolder": "enabled",
          "systemPolicyDocumentsFolder": "enabled",
          "systemPolicyDownloadsFolder": "enabled",
          "systemPolicyNetworkVolumes": "enabled",
          "systemPolicyRemovableVolumes": "enabled",
          "postEvent": "enabled",
          "appleEventsAllowedReceivers": [
            {
              "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
              "codeRequirement": "Code Requirement value",
              "identifier": "Identifier value",
              "identifierType": "path",
              "allowed": true
            }
          ]
        }
      ]
    }
  ]
}
```




