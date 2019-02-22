---
title: Список Андроиддевицеовнерженералдевицеконфигуратионс
description: Список свойств и связей объектов androidDeviceOwnerGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d36484c740d9ced29bf9bea0403639ae3dc9483b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146461"
---
# <a name="list-androiddeviceownergeneraldeviceconfigurations"></a><span data-ttu-id="e23d6-103">Список Андроиддевицеовнерженералдевицеконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="e23d6-103">List androidDeviceOwnerGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="e23d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e23d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e23d6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e23d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e23d6-106">Список свойств и связей объектов [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e23d6-106">List properties and relationships of the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e23d6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e23d6-107">Prerequisites</span></span>
<span data-ttu-id="e23d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e23d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e23d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e23d6-110">Permission type</span></span>|<span data-ttu-id="e23d6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e23d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e23d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e23d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e23d6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e23d6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e23d6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e23d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e23d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e23d6-115">Not supported.</span></span>|
|<span data-ttu-id="e23d6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e23d6-116">Application</span></span>|<span data-ttu-id="e23d6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e23d6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e23d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e23d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e23d6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e23d6-119">Request headers</span></span>
|<span data-ttu-id="e23d6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e23d6-120">Header</span></span>|<span data-ttu-id="e23d6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e23d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e23d6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e23d6-122">Authorization</span></span>|<span data-ttu-id="e23d6-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e23d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e23d6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e23d6-124">Accept</span></span>|<span data-ttu-id="e23d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e23d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e23d6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e23d6-126">Request body</span></span>
<span data-ttu-id="e23d6-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e23d6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e23d6-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e23d6-128">Response</span></span>
<span data-ttu-id="e23d6-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e23d6-129">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e23d6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e23d6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e23d6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e23d6-131">Request</span></span>
<span data-ttu-id="e23d6-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e23d6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="e23d6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e23d6-133">Response</span></span>
<span data-ttu-id="e23d6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e23d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3014

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
      "id": "edad943d-943d-edad-3d94-aded3d94aded",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
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
      "dataRoamingBlocked": true,
      "dateTimeConfigurationBlocked": true,
      "factoryResetDeviceAdministratorEmails": [
        "Factory Reset Device Administrator Emails value"
      ],
      "factoryResetBlocked": true,
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
      "microphoneForceMute": true,
      "networkEscapeHatchAllowed": true,
      "nfcBlockOutgoingBeam": true,
      "passwordBlockKeyguard": true,
      "passwordBlockKeyguardFeatures": [
        "camera"
      ],
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordCountToBlock": 4,
      "passwordRequiredType": "required",
      "passwordSignInFailureCountBeforeFactoryReset": 12,
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
      "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
      "vpnAlwaysOnLockdownMode": true,
      "wifiBlockEditConfigurations": true,
      "wifiBlockEditPolicyDefinedConfigurations": true
    }
  ]
}
```




