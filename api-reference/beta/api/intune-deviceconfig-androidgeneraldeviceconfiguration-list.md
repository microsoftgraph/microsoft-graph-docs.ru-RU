---
title: Перечисление объектов androidGeneralDeviceConfiguration
description: Перечисление свойств и связей объектов androidGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0d8ba32deed7098c721cba7595692aebdee140f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983816"
---
# <a name="list-androidgeneraldeviceconfigurations"></a><span data-ttu-id="adb72-103">Перечисление объектов androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="adb72-103">List androidGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="adb72-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="adb72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adb72-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adb72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="adb72-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="adb72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="adb72-107">Перечисление свойств и связей объектов [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="adb72-107">List properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="adb72-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="adb72-108">Prerequisites</span></span>
<span data-ttu-id="adb72-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adb72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adb72-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adb72-111">Permission type</span></span>|<span data-ttu-id="adb72-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="adb72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adb72-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adb72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="adb72-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="adb72-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="adb72-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adb72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adb72-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adb72-116">Not supported.</span></span>|
|<span data-ttu-id="adb72-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="adb72-117">Application</span></span>|<span data-ttu-id="adb72-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adb72-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adb72-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="adb72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="adb72-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="adb72-120">Request headers</span></span>
|<span data-ttu-id="adb72-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="adb72-121">Header</span></span>|<span data-ttu-id="adb72-122">Значение</span><span class="sxs-lookup"><span data-stu-id="adb72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adb72-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="adb72-123">Authorization</span></span>|<span data-ttu-id="adb72-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="adb72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adb72-125">Accept</span><span class="sxs-lookup"><span data-stu-id="adb72-125">Accept</span></span>|<span data-ttu-id="adb72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="adb72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adb72-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="adb72-127">Request body</span></span>
<span data-ttu-id="adb72-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="adb72-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adb72-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="adb72-129">Response</span></span>
<span data-ttu-id="adb72-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="adb72-130">If successful, this method returns a `200 OK` response code and a collection of [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adb72-131">Пример</span><span class="sxs-lookup"><span data-stu-id="adb72-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="adb72-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="adb72-132">Request</span></span>
<span data-ttu-id="adb72-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adb72-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="adb72-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="adb72-134">Response</span></span>
<span data-ttu-id="adb72-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="adb72-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3766

{
  "value": [
    {
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
  ]
}
```





