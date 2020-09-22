---
title: Get androidManagedAppProtection
description: Чтение свойств и связей объекта androidManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9656eac608ce13259baf50454f44ab4af9536a5e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985022"
---
# <a name="get-androidmanagedappprotection"></a><span data-ttu-id="50cc8-103">Get androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="50cc8-103">Get androidManagedAppProtection</span></span>

<span data-ttu-id="50cc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50cc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50cc8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50cc8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50cc8-106">Чтение свойств и связей объекта [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="50cc8-106">Read properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50cc8-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="50cc8-107">Prerequisites</span></span>
<span data-ttu-id="50cc8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50cc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50cc8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50cc8-110">Permission type</span></span>|<span data-ttu-id="50cc8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50cc8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50cc8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50cc8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50cc8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="50cc8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="50cc8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50cc8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50cc8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50cc8-115">Not supported.</span></span>|
|<span data-ttu-id="50cc8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50cc8-116">Application</span></span>|<span data-ttu-id="50cc8-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="50cc8-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50cc8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50cc8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50cc8-119">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="50cc8-119">Optional query parameters</span></span>
<span data-ttu-id="50cc8-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="50cc8-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50cc8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50cc8-121">Request headers</span></span>
|<span data-ttu-id="50cc8-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50cc8-122">Header</span></span>|<span data-ttu-id="50cc8-123">Значение</span><span class="sxs-lookup"><span data-stu-id="50cc8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50cc8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="50cc8-124">Authorization</span></span>|<span data-ttu-id="50cc8-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50cc8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50cc8-126">Accept</span><span class="sxs-lookup"><span data-stu-id="50cc8-126">Accept</span></span>|<span data-ttu-id="50cc8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="50cc8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50cc8-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="50cc8-128">Request body</span></span>
<span data-ttu-id="50cc8-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50cc8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50cc8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="50cc8-130">Response</span></span>
<span data-ttu-id="50cc8-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="50cc8-131">If successful, this method returns a `200 OK` response code and [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50cc8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="50cc8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="50cc8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="50cc8-133">Request</span></span>
<span data-ttu-id="50cc8-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50cc8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="50cc8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="50cc8-135">Response</span></span>
<span data-ttu-id="50cc8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50cc8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2143

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
    "managedBrowser": "microsoftEdge",
    "isAssigned": true,
    "screenCaptureBlocked": true,
    "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
    "encryptAppData": true,
    "deployedAppCount": 0,
    "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
    "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
    "customBrowserPackageId": "Custom Browser Package Id value",
    "customBrowserDisplayName": "Custom Browser Display Name value"
  }
}
```






