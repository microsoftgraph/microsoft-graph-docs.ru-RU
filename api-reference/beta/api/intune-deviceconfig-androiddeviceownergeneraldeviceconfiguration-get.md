---
title: Получение androidDeviceOwnerGeneralDeviceConfiguration
description: Чтение свойств и связей объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1e2ea1c39f3ac0cb760173fb9ce8552c4637bffa
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805847"
---
# <a name="get-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="38510-103">Получение androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="38510-103">Get androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="38510-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38510-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38510-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38510-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38510-106">Чтение свойств и связей объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="38510-106">Read properties and relationships of the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38510-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="38510-107">Prerequisites</span></span>
<span data-ttu-id="38510-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38510-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38510-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38510-110">Permission type</span></span>|<span data-ttu-id="38510-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38510-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38510-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38510-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38510-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38510-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="38510-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38510-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38510-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38510-115">Not supported.</span></span>|
|<span data-ttu-id="38510-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38510-116">Application</span></span>|<span data-ttu-id="38510-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38510-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38510-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38510-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38510-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="38510-119">Optional query parameters</span></span>
<span data-ttu-id="38510-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="38510-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38510-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38510-121">Request headers</span></span>
|<span data-ttu-id="38510-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38510-122">Header</span></span>|<span data-ttu-id="38510-123">Значение</span><span class="sxs-lookup"><span data-stu-id="38510-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38510-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38510-124">Authorization</span></span>|<span data-ttu-id="38510-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38510-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38510-126">Accept</span><span class="sxs-lookup"><span data-stu-id="38510-126">Accept</span></span>|<span data-ttu-id="38510-127">application/json</span><span class="sxs-lookup"><span data-stu-id="38510-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38510-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38510-128">Request body</span></span>
<span data-ttu-id="38510-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38510-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38510-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="38510-130">Response</span></span>
<span data-ttu-id="38510-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38510-131">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38510-132">Пример</span><span class="sxs-lookup"><span data-stu-id="38510-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="38510-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="38510-133">Request</span></span>
<span data-ttu-id="38510-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38510-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="38510-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="38510-135">Response</span></span>
<span data-ttu-id="38510-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38510-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3260

{
  "value": {
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
    "kioskModeBluetoothConfigurationEnabled": true,
    "kioskModeWiFiConfigurationEnabled": true,
    "microphoneForceMute": true,
    "networkEscapeHatchAllowed": true,
    "nfcBlockOutgoingBeam": true,
    "passwordBlockKeyguard": true,
    "passwordBlockKeyguardFeatures": [
      "camera"
    ],
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinimumLetterCharacters": 15,
    "passwordMinimumLowerCaseCharacters": 2,
    "passwordMinimumNonLetterCharacters": 2,
    "passwordMinimumNumericCharacters": 0,
    "passwordMinimumSymbolCharacters": 15,
    "passwordMinimumUpperCaseCharacters": 2,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordCountToBlock": 4,
    "passwordRequiredType": "required",
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "playStoreMode": "allowList",
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
}
```





