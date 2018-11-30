---
title: Перечисление объектов androidGeneralDeviceConfiguration
description: Перечисление свойств и связей объектов androidGeneralDeviceConfiguration.
ms.openlocfilehash: 3e0205bb65b52a9e57e52063ef5c6a47d4e6d205
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027767"
---
# <a name="list-androidgeneraldeviceconfigurations"></a><span data-ttu-id="1a779-103">Перечисление объектов androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a779-103">List androidGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="1a779-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1a779-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a779-105">Перечисление свойств и связей объектов [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a779-105">List properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a779-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1a779-106">Prerequisites</span></span>
<span data-ttu-id="1a779-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a779-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a779-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a779-109">Permission type</span></span>|<span data-ttu-id="1a779-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a779-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a779-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a779-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1a779-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a779-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1a779-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a779-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a779-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a779-114">Not supported.</span></span>|
|<span data-ttu-id="1a779-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a779-115">Application</span></span>|<span data-ttu-id="1a779-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a779-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a779-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a779-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1a779-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a779-118">Request headers</span></span>
|<span data-ttu-id="1a779-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a779-119">Header</span></span>|<span data-ttu-id="1a779-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1a779-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a779-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a779-121">Authorization</span></span>|<span data-ttu-id="1a779-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1a779-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a779-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1a779-123">Accept</span></span>|<span data-ttu-id="1a779-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1a779-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a779-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a779-125">Request body</span></span>
<span data-ttu-id="1a779-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a779-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a779-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a779-127">Response</span></span>
<span data-ttu-id="1a779-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a779-128">If successful, this method returns a `200 OK` response code and a collection of [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a779-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1a779-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="1a779-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a779-130">Request</span></span>
<span data-ttu-id="1a779-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a779-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="1a779-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="1a779-132">Response</span></span>
<span data-ttu-id="1a779-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1a779-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3618

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
      "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  ]
}
```



