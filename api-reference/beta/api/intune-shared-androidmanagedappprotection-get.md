---
title: Get androidManagedAppProtection
description: Чтение свойств и связей объекта androidManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 74e002023664a4496acc387de36ba474c01fe7bb
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864678"
---
# <a name="get-androidmanagedappprotection"></a><span data-ttu-id="b70e4-103">Get androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="b70e4-103">Get androidManagedAppProtection</span></span>

<span data-ttu-id="b70e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b70e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b70e4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b70e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b70e4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b70e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b70e4-107">Чтение свойств и связей объекта [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b70e4-107">Read properties and relationships of the [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b70e4-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b70e4-108">Prerequisites</span></span>
<span data-ttu-id="b70e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b70e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b70e4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b70e4-111">Permission type</span></span>|<span data-ttu-id="b70e4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b70e4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b70e4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b70e4-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b70e4-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="b70e4-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="b70e4-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b70e4-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="b70e4-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="b70e4-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b70e4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b70e4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b70e4-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b70e4-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b70e4-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b70e4-119">Not supported.</span></span>|
|<span data-ttu-id="b70e4-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b70e4-120">Application</span></span>||
| <span data-ttu-id="b70e4-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="b70e4-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="b70e4-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b70e4-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="b70e4-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="b70e4-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b70e4-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b70e4-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b70e4-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b70e4-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b70e4-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b70e4-126">Optional query parameters</span></span>
<span data-ttu-id="b70e4-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b70e4-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b70e4-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b70e4-128">Request headers</span></span>
|<span data-ttu-id="b70e4-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b70e4-129">Header</span></span>|<span data-ttu-id="b70e4-130">Значение</span><span class="sxs-lookup"><span data-stu-id="b70e4-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b70e4-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b70e4-131">Authorization</span></span>|<span data-ttu-id="b70e4-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b70e4-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b70e4-133">Accept</span><span class="sxs-lookup"><span data-stu-id="b70e4-133">Accept</span></span>|<span data-ttu-id="b70e4-134">application/json</span><span class="sxs-lookup"><span data-stu-id="b70e4-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b70e4-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b70e4-135">Request body</span></span>
<span data-ttu-id="b70e4-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b70e4-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b70e4-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b70e4-137">Response</span></span>
<span data-ttu-id="b70e4-138">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b70e4-138">If successful, this method returns a `200 OK` response code and [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b70e4-139">Пример</span><span class="sxs-lookup"><span data-stu-id="b70e4-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="b70e4-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b70e4-140">Request</span></span>
<span data-ttu-id="b70e4-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b70e4-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="b70e4-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b70e4-142">Response</span></span>
<span data-ttu-id="b70e4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b70e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







