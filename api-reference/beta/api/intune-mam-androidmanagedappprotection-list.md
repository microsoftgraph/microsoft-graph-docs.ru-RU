---
title: Перечисление объектов androidManagedAppProtection
description: Перечисление свойств и связей объектов androidManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa59dd37e66fe148792df58d285f87ad4d0e6d70
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571167"
---
# <a name="list-androidmanagedappprotections"></a><span data-ttu-id="96278-103">Перечисление объектов androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="96278-103">List androidManagedAppProtections</span></span>

> <span data-ttu-id="96278-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96278-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96278-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="96278-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96278-106">Перечисление свойств и связей объектов [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="96278-106">List properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96278-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="96278-107">Prerequisites</span></span>
<span data-ttu-id="96278-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="96278-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="96278-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96278-110">Permission type</span></span>|<span data-ttu-id="96278-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96278-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96278-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96278-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96278-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="96278-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="96278-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96278-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96278-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96278-115">Not supported.</span></span>|
|<span data-ttu-id="96278-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96278-116">Application</span></span>|<span data-ttu-id="96278-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96278-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96278-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96278-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="96278-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96278-119">Request headers</span></span>
|<span data-ttu-id="96278-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96278-120">Header</span></span>|<span data-ttu-id="96278-121">Значение</span><span class="sxs-lookup"><span data-stu-id="96278-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96278-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96278-122">Authorization</span></span>|<span data-ttu-id="96278-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96278-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96278-124">Accept</span><span class="sxs-lookup"><span data-stu-id="96278-124">Accept</span></span>|<span data-ttu-id="96278-125">application/json</span><span class="sxs-lookup"><span data-stu-id="96278-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96278-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96278-126">Request body</span></span>
<span data-ttu-id="96278-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96278-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96278-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="96278-128">Response</span></span>
<span data-ttu-id="96278-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="96278-129">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96278-130">Пример</span><span class="sxs-lookup"><span data-stu-id="96278-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="96278-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="96278-131">Request</span></span>
<span data-ttu-id="96278-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96278-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="96278-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="96278-133">Response</span></span>
<span data-ttu-id="96278-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96278-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3247

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
      "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe"
    }
  ]
}
```




