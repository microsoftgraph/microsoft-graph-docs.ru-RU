---
title: Get macOSGeneralDeviceConfiguration
description: Чтение свойств и связей объекта macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 423c28adb18629007e4f604b29e1fc94ab380c68
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177865"
---
# <a name="get-macosgeneraldeviceconfiguration"></a><span data-ttu-id="ea52d-103">Get macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea52d-103">Get macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="ea52d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea52d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea52d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea52d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea52d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea52d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea52d-107">Чтение свойств и связей объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea52d-107">Read properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea52d-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ea52d-108">Prerequisites</span></span>
<span data-ttu-id="ea52d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea52d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea52d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea52d-111">Permission type</span></span>|<span data-ttu-id="ea52d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea52d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea52d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea52d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea52d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea52d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ea52d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea52d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea52d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea52d-116">Not supported.</span></span>|
|<span data-ttu-id="ea52d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea52d-117">Application</span></span>|<span data-ttu-id="ea52d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea52d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea52d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea52d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea52d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ea52d-120">Optional query parameters</span></span>
<span data-ttu-id="ea52d-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ea52d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea52d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea52d-122">Request headers</span></span>
|<span data-ttu-id="ea52d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea52d-123">Header</span></span>|<span data-ttu-id="ea52d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ea52d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea52d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea52d-125">Authorization</span></span>|<span data-ttu-id="ea52d-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea52d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea52d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ea52d-127">Accept</span></span>|<span data-ttu-id="ea52d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ea52d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea52d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea52d-129">Request body</span></span>
<span data-ttu-id="ea52d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea52d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea52d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea52d-131">Response</span></span>
<span data-ttu-id="ea52d-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ea52d-132">If successful, this method returns a `200 OK` response code and [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea52d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ea52d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea52d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea52d-134">Request</span></span>
<span data-ttu-id="ea52d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea52d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ea52d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea52d-136">Response</span></span>
<span data-ttu-id="ea52d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea52d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4994

{
  "value": {
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
    "softwareUpdatesForceDelayed": true,
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
}
```



