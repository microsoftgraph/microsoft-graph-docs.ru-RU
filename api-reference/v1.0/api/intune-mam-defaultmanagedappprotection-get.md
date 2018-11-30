---
title: Get defaultManagedAppProtection
description: Чтение свойств и связей объекта defaultManagedAppProtection.
ms.openlocfilehash: c6c51fc592534074588dac3bf783637c6dc7b3c2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027106"
---
# <a name="get-defaultmanagedappprotection"></a><span data-ttu-id="0c4b1-103">Get defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="0c4b1-103">Get defaultManagedAppProtection</span></span>

> <span data-ttu-id="0c4b1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0c4b1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c4b1-105">Чтение свойств и связей объекта [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c4b1-105">Read properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0c4b1-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0c4b1-106">Prerequisites</span></span>
<span data-ttu-id="0c4b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c4b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c4b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c4b1-109">Permission type</span></span>|<span data-ttu-id="0c4b1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c4b1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c4b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c4b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0c4b1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c4b1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0c4b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c4b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c4b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c4b1-114">Not supported.</span></span>|
|<span data-ttu-id="0c4b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c4b1-115">Application</span></span>|<span data-ttu-id="0c4b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c4b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c4b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c4b1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c4b1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0c4b1-118">Optional query parameters</span></span>
<span data-ttu-id="0c4b1-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0c4b1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0c4b1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c4b1-120">Request headers</span></span>
|<span data-ttu-id="0c4b1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c4b1-121">Header</span></span>|<span data-ttu-id="0c4b1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0c4b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c4b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c4b1-123">Authorization</span></span>|<span data-ttu-id="0c4b1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0c4b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c4b1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0c4b1-125">Accept</span></span>|<span data-ttu-id="0c4b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c4b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c4b1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c4b1-127">Request body</span></span>
<span data-ttu-id="0c4b1-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c4b1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c4b1-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c4b1-129">Response</span></span>
<span data-ttu-id="0c4b1-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0c4b1-130">If successful, this method returns a `200 OK` response code and [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c4b1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0c4b1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0c4b1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c4b1-132">Request</span></span>
<span data-ttu-id="0c4b1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c4b1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="0c4b1-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c4b1-134">Response</span></span>
<span data-ttu-id="0c4b1-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0c4b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2264

{
  "value": {
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
}
```



