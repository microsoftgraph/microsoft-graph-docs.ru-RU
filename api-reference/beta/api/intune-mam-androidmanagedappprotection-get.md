---
title: Get androidManagedAppProtection
description: Чтение свойств и связей объекта androidManagedAppProtection.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2f03fef824797898761c1b162a05b37cdf166c78
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400097"
---
# <a name="get-androidmanagedappprotection"></a><span data-ttu-id="18a67-103">Get androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="18a67-103">Get androidManagedAppProtection</span></span>

> <span data-ttu-id="18a67-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="18a67-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="18a67-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18a67-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18a67-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18a67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18a67-107">Чтение свойств и связей объекта [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="18a67-107">Read properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18a67-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="18a67-108">Prerequisites</span></span>
<span data-ttu-id="18a67-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="18a67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="18a67-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18a67-111">Permission type</span></span>|<span data-ttu-id="18a67-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18a67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18a67-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18a67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18a67-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="18a67-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="18a67-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18a67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18a67-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18a67-116">Not supported.</span></span>|
|<span data-ttu-id="18a67-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18a67-117">Application</span></span>|<span data-ttu-id="18a67-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18a67-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18a67-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18a67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18a67-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="18a67-120">Optional query parameters</span></span>
<span data-ttu-id="18a67-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="18a67-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18a67-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18a67-122">Request headers</span></span>
|<span data-ttu-id="18a67-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18a67-123">Header</span></span>|<span data-ttu-id="18a67-124">Значение</span><span class="sxs-lookup"><span data-stu-id="18a67-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18a67-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="18a67-125">Authorization</span></span>|<span data-ttu-id="18a67-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="18a67-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18a67-127">Accept</span><span class="sxs-lookup"><span data-stu-id="18a67-127">Accept</span></span>|<span data-ttu-id="18a67-128">application/json</span><span class="sxs-lookup"><span data-stu-id="18a67-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18a67-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18a67-129">Request body</span></span>
<span data-ttu-id="18a67-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18a67-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18a67-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="18a67-131">Response</span></span>
<span data-ttu-id="18a67-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="18a67-132">If successful, this method returns a `200 OK` response code and [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18a67-133">Пример</span><span class="sxs-lookup"><span data-stu-id="18a67-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="18a67-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="18a67-134">Request</span></span>
<span data-ttu-id="18a67-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18a67-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="18a67-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="18a67-136">Response</span></span>
<span data-ttu-id="18a67-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="18a67-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2773

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
    "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe"
  }
}
```




