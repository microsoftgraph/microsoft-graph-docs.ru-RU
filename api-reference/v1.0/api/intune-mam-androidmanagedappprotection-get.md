---
title: Get androidManagedAppProtection
description: Чтение свойств и связей объекта androidManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 656b09610fae79a25274b98cba55cd07b92b29dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919297"
---
# <a name="get-androidmanagedappprotection"></a><span data-ttu-id="d16bc-103">Get androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="d16bc-103">Get androidManagedAppProtection</span></span>

> <span data-ttu-id="d16bc-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d16bc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d16bc-105">Чтение свойств и связей объекта [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d16bc-105">Read properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d16bc-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d16bc-106">Prerequisites</span></span>
<span data-ttu-id="d16bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d16bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d16bc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d16bc-109">Permission type</span></span>|<span data-ttu-id="d16bc-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d16bc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d16bc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d16bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d16bc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d16bc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d16bc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d16bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d16bc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d16bc-114">Not supported.</span></span>|
|<span data-ttu-id="d16bc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d16bc-115">Application</span></span>|<span data-ttu-id="d16bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d16bc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d16bc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d16bc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d16bc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d16bc-118">Optional query parameters</span></span>
<span data-ttu-id="d16bc-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d16bc-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d16bc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d16bc-120">Request headers</span></span>
|<span data-ttu-id="d16bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d16bc-121">Header</span></span>|<span data-ttu-id="d16bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d16bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d16bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d16bc-123">Authorization</span></span>|<span data-ttu-id="d16bc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d16bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d16bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d16bc-125">Accept</span></span>|<span data-ttu-id="d16bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d16bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d16bc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d16bc-127">Request body</span></span>
<span data-ttu-id="d16bc-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d16bc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d16bc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d16bc-129">Response</span></span>
<span data-ttu-id="d16bc-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d16bc-130">If successful, this method returns a `200 OK` response code and [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d16bc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d16bc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d16bc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d16bc-132">Request</span></span>
<span data-ttu-id="d16bc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d16bc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="d16bc-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="d16bc-134">Response</span></span>
<span data-ttu-id="d16bc-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d16bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



