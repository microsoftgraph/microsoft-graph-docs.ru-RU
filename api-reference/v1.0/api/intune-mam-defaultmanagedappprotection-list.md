---
title: Перечисление объектов defaultManagedAppProtection
description: Перечисление свойств и связей объектов defaultManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7eb1c8fb0c82f66c8da357cad66a867fb3bfa3b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877646"
---
# <a name="list-defaultmanagedappprotections"></a><span data-ttu-id="bcd77-103">Перечисление объектов defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="bcd77-103">List defaultManagedAppProtections</span></span>

> <span data-ttu-id="bcd77-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bcd77-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bcd77-105">Перечисление свойств и связей объектов [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="bcd77-105">List properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bcd77-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bcd77-106">Prerequisites</span></span>
<span data-ttu-id="bcd77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcd77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcd77-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcd77-109">Permission type</span></span>|<span data-ttu-id="bcd77-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcd77-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcd77-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcd77-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bcd77-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcd77-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bcd77-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcd77-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcd77-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcd77-114">Not supported.</span></span>|
|<span data-ttu-id="bcd77-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcd77-115">Application</span></span>|<span data-ttu-id="bcd77-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcd77-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcd77-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcd77-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="bcd77-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcd77-118">Request headers</span></span>
|<span data-ttu-id="bcd77-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bcd77-119">Header</span></span>|<span data-ttu-id="bcd77-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bcd77-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcd77-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcd77-121">Authorization</span></span>|<span data-ttu-id="bcd77-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bcd77-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcd77-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bcd77-123">Accept</span></span>|<span data-ttu-id="bcd77-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bcd77-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcd77-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bcd77-125">Request body</span></span>
<span data-ttu-id="bcd77-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bcd77-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcd77-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcd77-127">Response</span></span>
<span data-ttu-id="bcd77-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bcd77-128">If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcd77-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bcd77-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="bcd77-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcd77-130">Request</span></span>
<span data-ttu-id="bcd77-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcd77-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="bcd77-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="bcd77-132">Response</span></span>
<span data-ttu-id="bcd77-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bcd77-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2380

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
      "faceIdBlocked": true
    }
  ]
}
```



