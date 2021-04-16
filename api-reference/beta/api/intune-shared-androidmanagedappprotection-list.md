---
title: Перечисление объектов androidManagedAppProtection
description: Перечисление свойств и связей объектов androidManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ae8fcf08efe266dc34947fb6e7ad6b8c8fb2a36a
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864650"
---
# <a name="list-androidmanagedappprotections"></a><span data-ttu-id="31b35-103">Перечисление объектов androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="31b35-103">List androidManagedAppProtections</span></span>

<span data-ttu-id="31b35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31b35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31b35-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31b35-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31b35-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31b35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31b35-107">Перечисление свойств и связей объектов [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="31b35-107">List properties and relationships of the [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31b35-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="31b35-108">Prerequisites</span></span>
<span data-ttu-id="31b35-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31b35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31b35-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31b35-111">Permission type</span></span>|<span data-ttu-id="31b35-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="31b35-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31b35-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31b35-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="31b35-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="31b35-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="31b35-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="31b35-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="31b35-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="31b35-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="31b35-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="31b35-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="31b35-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31b35-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31b35-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31b35-119">Not supported.</span></span>|
|<span data-ttu-id="31b35-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="31b35-120">Application</span></span>||
| <span data-ttu-id="31b35-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="31b35-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="31b35-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="31b35-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="31b35-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="31b35-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="31b35-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="31b35-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31b35-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31b35-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="31b35-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="31b35-126">Request headers</span></span>
|<span data-ttu-id="31b35-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31b35-127">Header</span></span>|<span data-ttu-id="31b35-128">Значение</span><span class="sxs-lookup"><span data-stu-id="31b35-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31b35-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31b35-129">Authorization</span></span>|<span data-ttu-id="31b35-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31b35-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31b35-131">Accept</span><span class="sxs-lookup"><span data-stu-id="31b35-131">Accept</span></span>|<span data-ttu-id="31b35-132">application/json</span><span class="sxs-lookup"><span data-stu-id="31b35-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31b35-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31b35-133">Request body</span></span>
<span data-ttu-id="31b35-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31b35-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31b35-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="31b35-135">Response</span></span>
<span data-ttu-id="31b35-136">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="31b35-136">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31b35-137">Пример</span><span class="sxs-lookup"><span data-stu-id="31b35-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="31b35-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="31b35-138">Request</span></span>
<span data-ttu-id="31b35-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31b35-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="31b35-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="31b35-140">Response</span></span>
<span data-ttu-id="31b35-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31b35-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







