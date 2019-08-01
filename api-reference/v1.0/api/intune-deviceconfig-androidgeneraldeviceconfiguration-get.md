---
title: Get androidGeneralDeviceConfiguration
description: Чтение свойств и связей объекта androidGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6c71d5fe036bbbfae93b52d9d1dba9a1a96d38a6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019627"
---
# <a name="get-androidgeneraldeviceconfiguration"></a><span data-ttu-id="986e1-103">Get androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="986e1-103">Get androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="986e1-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="986e1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="986e1-105">Чтение свойств и связей объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="986e1-105">Read properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="986e1-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="986e1-106">Prerequisites</span></span>
<span data-ttu-id="986e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="986e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="986e1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="986e1-109">Permission type</span></span>|<span data-ttu-id="986e1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="986e1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="986e1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="986e1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="986e1-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="986e1-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="986e1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="986e1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="986e1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="986e1-114">Not supported.</span></span>|
|<span data-ttu-id="986e1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="986e1-115">Application</span></span>|<span data-ttu-id="986e1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="986e1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="986e1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="986e1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="986e1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="986e1-118">Optional query parameters</span></span>
<span data-ttu-id="986e1-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="986e1-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="986e1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="986e1-120">Request headers</span></span>
|<span data-ttu-id="986e1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="986e1-121">Header</span></span>|<span data-ttu-id="986e1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="986e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="986e1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="986e1-123">Authorization</span></span>|<span data-ttu-id="986e1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="986e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="986e1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="986e1-125">Accept</span></span>|<span data-ttu-id="986e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="986e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="986e1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="986e1-127">Request body</span></span>
<span data-ttu-id="986e1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="986e1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="986e1-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="986e1-129">Response</span></span>
<span data-ttu-id="986e1-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="986e1-130">If successful, this method returns a `200 OK` response code and [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="986e1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="986e1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="986e1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="986e1-132">Request</span></span>
<span data-ttu-id="986e1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="986e1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="986e1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="986e1-134">Response</span></span>
<span data-ttu-id="986e1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="986e1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3414

{
  "value": {
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
}
```



