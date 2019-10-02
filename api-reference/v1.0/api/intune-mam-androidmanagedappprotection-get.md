---
title: Get androidManagedAppProtection
description: Чтение свойств и связей объекта androidManagedAppProtection.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b1a63ea33922e2e4d624e1917adc077f8b201b57
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363992"
---
# <a name="get-androidmanagedappprotection"></a><span data-ttu-id="48cd8-103">Get androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="48cd8-103">Get androidManagedAppProtection</span></span>

> <span data-ttu-id="48cd8-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48cd8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48cd8-105">Чтение свойств и связей объекта [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="48cd8-105">Read properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48cd8-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="48cd8-106">Prerequisites</span></span>
<span data-ttu-id="48cd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48cd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48cd8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48cd8-109">Permission type</span></span>|<span data-ttu-id="48cd8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48cd8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48cd8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48cd8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="48cd8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="48cd8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="48cd8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48cd8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48cd8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48cd8-114">Not supported.</span></span>|
|<span data-ttu-id="48cd8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48cd8-115">Application</span></span>|<span data-ttu-id="48cd8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48cd8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48cd8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48cd8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48cd8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="48cd8-118">Optional query parameters</span></span>
<span data-ttu-id="48cd8-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="48cd8-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48cd8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48cd8-120">Request headers</span></span>
|<span data-ttu-id="48cd8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48cd8-121">Header</span></span>|<span data-ttu-id="48cd8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="48cd8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48cd8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48cd8-123">Authorization</span></span>|<span data-ttu-id="48cd8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48cd8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48cd8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="48cd8-125">Accept</span></span>|<span data-ttu-id="48cd8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48cd8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48cd8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48cd8-127">Request body</span></span>
<span data-ttu-id="48cd8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48cd8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48cd8-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="48cd8-129">Response</span></span>
<span data-ttu-id="48cd8-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="48cd8-130">If successful, this method returns a `200 OK` response code and [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48cd8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="48cd8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="48cd8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="48cd8-132">Request</span></span>
<span data-ttu-id="48cd8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48cd8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="48cd8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="48cd8-134">Response</span></span>
<span data-ttu-id="48cd8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48cd8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1967

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
    "isAssigned": true,
    "screenCaptureBlocked": true,
    "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
    "encryptAppData": true,
    "deployedAppCount": 0,
    "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
    "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
  }
}
```




