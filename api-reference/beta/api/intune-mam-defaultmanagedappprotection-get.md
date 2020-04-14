---
title: Get defaultManagedAppProtection
description: Чтение свойств и связей объекта defaultManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9cacdefe6f9f4ec93ddbafb03026fc7078afd8d8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444566"
---
# <a name="get-defaultmanagedappprotection"></a><span data-ttu-id="48522-103">Get defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="48522-103">Get defaultManagedAppProtection</span></span>

<span data-ttu-id="48522-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48522-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48522-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48522-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48522-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48522-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48522-107">Чтение свойств и связей объекта [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="48522-107">Read properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48522-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="48522-108">Prerequisites</span></span>
<span data-ttu-id="48522-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48522-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48522-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48522-111">Permission type</span></span>|<span data-ttu-id="48522-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48522-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48522-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48522-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48522-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="48522-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="48522-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48522-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48522-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48522-116">Not supported.</span></span>|
|<span data-ttu-id="48522-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="48522-117">Application</span></span>|<span data-ttu-id="48522-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="48522-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48522-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48522-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48522-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="48522-120">Optional query parameters</span></span>
<span data-ttu-id="48522-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="48522-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48522-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48522-122">Request headers</span></span>
|<span data-ttu-id="48522-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48522-123">Header</span></span>|<span data-ttu-id="48522-124">Значение</span><span class="sxs-lookup"><span data-stu-id="48522-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48522-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="48522-125">Authorization</span></span>|<span data-ttu-id="48522-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48522-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48522-127">Accept</span><span class="sxs-lookup"><span data-stu-id="48522-127">Accept</span></span>|<span data-ttu-id="48522-128">application/json</span><span class="sxs-lookup"><span data-stu-id="48522-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48522-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48522-129">Request body</span></span>
<span data-ttu-id="48522-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48522-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48522-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="48522-131">Response</span></span>
<span data-ttu-id="48522-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="48522-132">If successful, this method returns a `200 OK` response code and [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48522-133">Пример</span><span class="sxs-lookup"><span data-stu-id="48522-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="48522-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="48522-134">Request</span></span>
<span data-ttu-id="48522-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48522-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="48522-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="48522-136">Response</span></span>
<span data-ttu-id="48522-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48522-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4930

{
  "value": {
    "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "77064c51-4c51-7706-514c-0677514c0677",
    "version": "Version value",
    "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
    "periodOnlineBeforeAccessCheck": "PT35.0018757S",
    "allowedInboundDataTransferSources": "managedApps",
    "allowedOutboundDataTransferDestinations": "managedApps",
    "organizationalCredentialsRequired": true,
    "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
    "dataBackupBlocked": true,
    "deviceComplianceRequired": true,
    "managedBrowserToOpenLinksRequired": true,
    "saveAsBlocked": true,
    "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
    "pinRequired": true,
    "maximumPinRetries": 1,
    "simplePinBlocked": true,
    "minimumPinLength": 0,
    "pinCharacterSet": "alphanumericAndSymbol",
    "periodBeforePinReset": "PT3M29.6631862S",
    "allowedDataStorageLocations": [
      "sharePoint"
    ],
    "contactSyncBlocked": true,
    "printBlocked": true,
    "fingerprintBlocked": true,
    "disableAppPinIfDevicePinIsSet": true,
    "minimumRequiredOsVersion": "Minimum Required Os Version value",
    "minimumWarningOsVersion": "Minimum Warning Os Version value",
    "minimumRequiredAppVersion": "Minimum Required App Version value",
    "minimumWarningAppVersion": "Minimum Warning App Version value",
    "minimumWipeOsVersion": "Minimum Wipe Os Version value",
    "minimumWipeAppVersion": "Minimum Wipe App Version value",
    "appActionIfDeviceComplianceRequired": "wipe",
    "appActionIfMaximumPinRetriesExceeded": "wipe",
    "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
    "allowedOutboundClipboardSharingExceptionLength": 14,
    "notificationRestriction": "blockOrganizationalData",
    "previousPinBlockCount": 5,
    "managedBrowser": "microsoftEdge",
    "maximumAllowedDeviceThreatLevel": "secured",
    "mobileThreatDefenseRemediationAction": "wipe",
    "blockDataIngestionIntoOrganizationDocuments": true,
    "allowedDataIngestionLocations": [
      "sharePoint"
    ],
    "appActionIfUnableToAuthenticateUser": "wipe",
    "appDataEncryptionType": "afterDeviceRestart",
    "screenCaptureBlocked": true,
    "encryptAppData": true,
    "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
    "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "deployedAppCount": 0,
    "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
    "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
    "exemptedAppProtocols": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "exemptedAppPackages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "faceIdBlocked": true,
    "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
    "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
    "allowedIosDeviceModels": "Allowed Ios Device Models value",
    "appActionIfIosDeviceModelNotAllowed": "wipe",
    "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
    "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
    "thirdPartyKeyboardsBlocked": true,
    "filterOpenInToOnlyManagedApps": true,
    "disableProtectionOfManagedOutboundOpenInData": true,
    "protectInboundDataFromUnknownSources": true,
    "requiredAndroidSafetyNetDeviceAttestationType": "basicIntegrity",
    "appActionIfAndroidSafetyNetDeviceAttestationFailed": "wipe",
    "requiredAndroidSafetyNetAppsVerificationType": "enabled",
    "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe",
    "customBrowserProtocol": "Custom Browser Protocol value",
    "customBrowserPackageId": "Custom Browser Package Id value",
    "customBrowserDisplayName": "Custom Browser Display Name value",
    "minimumRequiredCompanyPortalVersion": "Minimum Required Company Portal Version value",
    "minimumWarningCompanyPortalVersion": "Minimum Warning Company Portal Version value",
    "minimumWipeCompanyPortalVersion": "Minimum Wipe Company Portal Version value",
    "allowedAndroidDeviceModels": [
      "Allowed Android Device Models value"
    ],
    "appActionIfAndroidDeviceModelNotAllowed": "wipe"
  }
}
```



