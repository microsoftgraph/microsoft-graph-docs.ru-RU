---
title: Перечисление объектов defaultManagedAppProtection
description: Перечисление свойств и связей объектов defaultManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2e678b6293230ec32211c20483e6d788142d3de0
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162050"
---
# <a name="list-defaultmanagedappprotections"></a><span data-ttu-id="1148e-103">Перечисление объектов defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="1148e-103">List defaultManagedAppProtections</span></span>

<span data-ttu-id="1148e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1148e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1148e-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1148e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1148e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1148e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1148e-107">Перечисление свойств и связей объектов [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="1148e-107">List properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1148e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1148e-108">Prerequisites</span></span>
<span data-ttu-id="1148e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1148e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1148e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1148e-111">Permission type</span></span>|<span data-ttu-id="1148e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1148e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1148e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1148e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1148e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1148e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1148e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1148e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1148e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1148e-116">Not supported.</span></span>|
|<span data-ttu-id="1148e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1148e-117">Application</span></span>|<span data-ttu-id="1148e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1148e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1148e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1148e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="1148e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1148e-120">Request headers</span></span>
|<span data-ttu-id="1148e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1148e-121">Header</span></span>|<span data-ttu-id="1148e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1148e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1148e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1148e-123">Authorization</span></span>|<span data-ttu-id="1148e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1148e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1148e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1148e-125">Accept</span></span>|<span data-ttu-id="1148e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1148e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1148e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1148e-127">Request body</span></span>
<span data-ttu-id="1148e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1148e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1148e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1148e-129">Response</span></span>
<span data-ttu-id="1148e-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1148e-130">If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1148e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1148e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1148e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1148e-132">Request</span></span>
<span data-ttu-id="1148e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1148e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="1148e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1148e-134">Response</span></span>
<span data-ttu-id="1148e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1148e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 6001

{
  "value": [
    {
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
      "maximumRequiredOsVersion": "Maximum Required Os Version value",
      "maximumWarningOsVersion": "Maximum Warning Os Version value",
      "maximumWipeOsVersion": "Maximum Wipe Os Version value",
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
      "dialerRestrictionLevel": "managedApps",
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
      "appActionIfAndroidDeviceModelNotAllowed": "wipe",
      "customDialerAppProtocol": "Custom Dialer App Protocol value",
      "customDialerAppPackageId": "Custom Dialer App Package Id value",
      "customDialerAppDisplayName": "Custom Dialer App Display Name value",
      "biometricAuthenticationBlocked": true,
      "requiredAndroidSafetyNetEvaluationType": "hardwareBacked",
      "blockAfterCompanyPortalUpdateDeferralInDays": 11,
      "warnAfterCompanyPortalUpdateDeferralInDays": 10,
      "wipeAfterCompanyPortalUpdateDeferralInDays": 10,
      "deviceLockRequired": true,
      "appActionIfDeviceLockNotSet": "wipe"
    }
  ]
}
```




