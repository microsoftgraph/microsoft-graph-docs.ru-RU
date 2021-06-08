---
title: Get defaultManagedAppProtection
description: Чтение свойств и связей объекта defaultManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7f77abbb38915799497859ae5f9ee3c3f008fed2
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758117"
---
# <a name="get-defaultmanagedappprotection"></a><span data-ttu-id="5adbe-103">Get defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="5adbe-103">Get defaultManagedAppProtection</span></span>

<span data-ttu-id="5adbe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5adbe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5adbe-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5adbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5adbe-106">Чтение свойств и связей объекта [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="5adbe-106">Read properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5adbe-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5adbe-107">Prerequisites</span></span>
<span data-ttu-id="5adbe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5adbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5adbe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5adbe-110">Permission type</span></span>|<span data-ttu-id="5adbe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5adbe-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5adbe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5adbe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5adbe-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5adbe-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5adbe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5adbe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5adbe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5adbe-115">Not supported.</span></span>|
|<span data-ttu-id="5adbe-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5adbe-116">Application</span></span>|<span data-ttu-id="5adbe-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5adbe-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5adbe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5adbe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5adbe-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5adbe-119">Optional query parameters</span></span>
<span data-ttu-id="5adbe-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5adbe-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5adbe-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5adbe-121">Request headers</span></span>
|<span data-ttu-id="5adbe-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5adbe-122">Header</span></span>|<span data-ttu-id="5adbe-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5adbe-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5adbe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5adbe-124">Authorization</span></span>|<span data-ttu-id="5adbe-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5adbe-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5adbe-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5adbe-126">Accept</span></span>|<span data-ttu-id="5adbe-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5adbe-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5adbe-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5adbe-128">Request body</span></span>
<span data-ttu-id="5adbe-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5adbe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5adbe-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5adbe-130">Response</span></span>
<span data-ttu-id="5adbe-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5adbe-131">If successful, this method returns a `200 OK` response code and [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5adbe-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5adbe-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5adbe-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5adbe-133">Request</span></span>
<span data-ttu-id="5adbe-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5adbe-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="5adbe-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5adbe-135">Response</span></span>
<span data-ttu-id="5adbe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5adbe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2304

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
    "managedBrowser": "microsoftEdge",
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




