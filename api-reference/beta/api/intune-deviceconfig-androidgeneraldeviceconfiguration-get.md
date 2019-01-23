---
title: Get androidGeneralDeviceConfiguration
description: Чтение свойств и связей объекта androidGeneralDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 749274db88e8fbf8089a5d713bac073fb0bc239c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404906"
---
# <a name="get-androidgeneraldeviceconfiguration"></a><span data-ttu-id="0d32a-103">Get androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0d32a-103">Get androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="0d32a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0d32a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0d32a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d32a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d32a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d32a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d32a-107">Чтение свойств и связей объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d32a-107">Read properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d32a-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0d32a-108">Prerequisites</span></span>
<span data-ttu-id="0d32a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0d32a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0d32a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d32a-111">Permission type</span></span>|<span data-ttu-id="0d32a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d32a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d32a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d32a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d32a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d32a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0d32a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d32a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d32a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d32a-116">Not supported.</span></span>|
|<span data-ttu-id="0d32a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d32a-117">Application</span></span>|<span data-ttu-id="0d32a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d32a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d32a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d32a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0d32a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0d32a-120">Optional query parameters</span></span>
<span data-ttu-id="0d32a-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0d32a-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d32a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d32a-122">Request headers</span></span>
|<span data-ttu-id="0d32a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d32a-123">Header</span></span>|<span data-ttu-id="0d32a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0d32a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d32a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d32a-125">Authorization</span></span>|<span data-ttu-id="0d32a-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0d32a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d32a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0d32a-127">Accept</span></span>|<span data-ttu-id="0d32a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0d32a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d32a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d32a-129">Request body</span></span>
<span data-ttu-id="0d32a-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d32a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d32a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d32a-131">Response</span></span>
<span data-ttu-id="0d32a-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0d32a-132">If successful, this method returns a `200 OK` response code and [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d32a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0d32a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d32a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d32a-134">Request</span></span>
<span data-ttu-id="0d32a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d32a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0d32a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d32a-136">Response</span></span>
<span data-ttu-id="0d32a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0d32a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3552

{
  "value": {
    "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
    "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "appsBlockClipboardSharing": true,
    "appsBlockCopyPaste": true,
    "appsBlockYouTube": true,
    "bluetoothBlocked": true,
    "cameraBlocked": true,
    "cellularBlockDataRoaming": true,
    "cellularBlockMessaging": true,
    "cellularBlockVoiceRoaming": true,
    "cellularBlockWiFiTethering": true,
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
    "diagnosticDataBlockSubmission": true,
    "locationServicesBlocked": true,
    "googleAccountBlockAutoSync": true,
    "googlePlayStoreBlocked": true,
    "kioskModeBlockSleepButton": true,
    "kioskModeBlockVolumeButtons": true,
    "dateAndTimeBlockChanges": true,
    "kioskModeApps": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "nfcBlocked": true,
    "passwordBlockFingerprintUnlock": true,
    "passwordBlockTrustAgents": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "passwordRequiredType": "alphabetic",
    "passwordRequired": true,
    "powerOffBlocked": true,
    "factoryResetBlocked": true,
    "screenCaptureBlocked": true,
    "deviceSharingAllowed": true,
    "storageBlockGoogleBackup": true,
    "storageBlockRemovableStorage": true,
    "storageRequireDeviceEncryption": true,
    "storageRequireRemovableStorageEncryption": true,
    "voiceAssistantBlocked": true,
    "voiceDialingBlocked": true,
    "webBrowserBlockPopups": true,
    "webBrowserBlockAutofill": true,
    "webBrowserBlockJavaScript": true,
    "webBrowserBlocked": true,
    "webBrowserCookieSettings": "blockAlways",
    "wiFiBlocked": true,
    "appsInstallAllowList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "appsLaunchBlockList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "appsHideList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "securityRequireVerifyApps": true
  }
}
```




