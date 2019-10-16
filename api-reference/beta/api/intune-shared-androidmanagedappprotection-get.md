---
title: Get androidManagedAppProtection
description: Чтение свойств и связей объекта androidManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c0a2968bc14c90d5efd819370b261d971f6d8f13
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537158"
---
# <a name="get-androidmanagedappprotection"></a><span data-ttu-id="43d51-103">Get androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="43d51-103">Get androidManagedAppProtection</span></span>

> <span data-ttu-id="43d51-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43d51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43d51-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43d51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43d51-106">Чтение свойств и связей объекта [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="43d51-106">Read properties and relationships of the [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43d51-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="43d51-107">Prerequisites</span></span>
<span data-ttu-id="43d51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43d51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43d51-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43d51-110">Permission type</span></span>|<span data-ttu-id="43d51-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43d51-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43d51-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43d51-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="43d51-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="43d51-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="43d51-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="43d51-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="43d51-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="43d51-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="43d51-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="43d51-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="43d51-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43d51-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43d51-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43d51-118">Not supported.</span></span>|
|<span data-ttu-id="43d51-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="43d51-119">Application</span></span>||
| <span data-ttu-id="43d51-120">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="43d51-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="43d51-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="43d51-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="43d51-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="43d51-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="43d51-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="43d51-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43d51-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43d51-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43d51-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="43d51-125">Optional query parameters</span></span>
<span data-ttu-id="43d51-126">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="43d51-126">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43d51-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43d51-127">Request headers</span></span>
|<span data-ttu-id="43d51-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43d51-128">Header</span></span>|<span data-ttu-id="43d51-129">Значение</span><span class="sxs-lookup"><span data-stu-id="43d51-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43d51-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43d51-130">Authorization</span></span>|<span data-ttu-id="43d51-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43d51-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43d51-132">Accept</span><span class="sxs-lookup"><span data-stu-id="43d51-132">Accept</span></span>|<span data-ttu-id="43d51-133">application/json</span><span class="sxs-lookup"><span data-stu-id="43d51-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43d51-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43d51-134">Request body</span></span>
<span data-ttu-id="43d51-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43d51-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43d51-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="43d51-136">Response</span></span>
<span data-ttu-id="43d51-137">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="43d51-137">If successful, this method returns a `200 OK` response code and [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43d51-138">Пример</span><span class="sxs-lookup"><span data-stu-id="43d51-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="43d51-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="43d51-139">Request</span></span>
<span data-ttu-id="43d51-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43d51-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="43d51-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="43d51-141">Response</span></span>
<span data-ttu-id="43d51-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43d51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3296

{
  "value": {
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
}
```






