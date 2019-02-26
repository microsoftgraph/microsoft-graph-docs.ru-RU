---
title: Get androidGeneralDeviceConfiguration
description: Чтение свойств и связей объекта androidGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 78a33a821c174f8ddda0d42bb3ec61fe5d213fb3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140154"
---
# <a name="get-androidgeneraldeviceconfiguration"></a><span data-ttu-id="dc95f-103">Get androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="dc95f-103">Get androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="dc95f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc95f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc95f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc95f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc95f-106">Чтение свойств и связей объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dc95f-106">Read properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc95f-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="dc95f-107">Prerequisites</span></span>
<span data-ttu-id="dc95f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dc95f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dc95f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc95f-110">Permission type</span></span>|<span data-ttu-id="dc95f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc95f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc95f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc95f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc95f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc95f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dc95f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc95f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc95f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc95f-115">Not supported.</span></span>|
|<span data-ttu-id="dc95f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc95f-116">Application</span></span>|<span data-ttu-id="dc95f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc95f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc95f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc95f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dc95f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dc95f-119">Optional query parameters</span></span>
<span data-ttu-id="dc95f-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dc95f-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc95f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc95f-121">Request headers</span></span>
|<span data-ttu-id="dc95f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc95f-122">Header</span></span>|<span data-ttu-id="dc95f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="dc95f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc95f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc95f-124">Authorization</span></span>|<span data-ttu-id="dc95f-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dc95f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc95f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="dc95f-126">Accept</span></span>|<span data-ttu-id="dc95f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dc95f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc95f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc95f-128">Request body</span></span>
<span data-ttu-id="dc95f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc95f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc95f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc95f-130">Response</span></span>
<span data-ttu-id="dc95f-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dc95f-131">If successful, this method returns a `200 OK` response code and [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc95f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="dc95f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc95f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc95f-133">Request</span></span>
<span data-ttu-id="dc95f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc95f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="dc95f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc95f-135">Response</span></span>
<span data-ttu-id="dc95f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dc95f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




