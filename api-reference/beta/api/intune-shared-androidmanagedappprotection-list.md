---
title: Перечисление объектов androidManagedAppProtection
description: Перечисление свойств и связей объектов androidManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8e4a1b48da2b6f8e1bc7a2455b4a7af17c9d28ab
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940203"
---
# <a name="list-androidmanagedappprotections"></a><span data-ttu-id="28a43-103">Перечисление объектов androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="28a43-103">List androidManagedAppProtections</span></span>

> <span data-ttu-id="28a43-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28a43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28a43-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28a43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28a43-106">Перечисление свойств и связей объектов [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="28a43-106">List properties and relationships of the [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28a43-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="28a43-107">Prerequisites</span></span>
<span data-ttu-id="28a43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28a43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28a43-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28a43-110">Permission type</span></span>|<span data-ttu-id="28a43-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="28a43-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28a43-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28a43-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="28a43-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="28a43-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="28a43-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="28a43-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="28a43-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="28a43-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="28a43-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="28a43-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="28a43-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28a43-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28a43-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28a43-118">Not supported.</span></span>|
|<span data-ttu-id="28a43-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28a43-119">Application</span></span>||
| <span data-ttu-id="28a43-120">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="28a43-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="28a43-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="28a43-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="28a43-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="28a43-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="28a43-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="28a43-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28a43-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28a43-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="28a43-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="28a43-125">Request headers</span></span>
|<span data-ttu-id="28a43-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28a43-126">Header</span></span>|<span data-ttu-id="28a43-127">Значение</span><span class="sxs-lookup"><span data-stu-id="28a43-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28a43-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28a43-128">Authorization</span></span>|<span data-ttu-id="28a43-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28a43-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28a43-130">Accept</span><span class="sxs-lookup"><span data-stu-id="28a43-130">Accept</span></span>|<span data-ttu-id="28a43-131">application/json</span><span class="sxs-lookup"><span data-stu-id="28a43-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28a43-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="28a43-132">Request body</span></span>
<span data-ttu-id="28a43-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28a43-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28a43-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="28a43-134">Response</span></span>
<span data-ttu-id="28a43-135">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="28a43-135">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28a43-136">Пример</span><span class="sxs-lookup"><span data-stu-id="28a43-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="28a43-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="28a43-137">Request</span></span>
<span data-ttu-id="28a43-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28a43-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="28a43-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="28a43-139">Response</span></span>
<span data-ttu-id="28a43-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28a43-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3448

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
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
      "isAssigned": true,
      "targetedAppManagementLevels": "unmanaged",
      "screenCaptureBlocked": true,
      "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
      "encryptAppData": true,
      "deployedAppCount": 0,
      "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
      "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
      "exemptedAppPackages": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
      "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
      "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
      "requiredAndroidSafetyNetDeviceAttestationType": "basicIntegrity",
      "appActionIfAndroidSafetyNetDeviceAttestationFailed": "wipe",
      "requiredAndroidSafetyNetAppsVerificationType": "enabled",
      "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe",
      "customBrowserPackageId": "Custom Browser Package Id value",
      "customBrowserDisplayName": "Custom Browser Display Name value"
    }
  ]
}
```








