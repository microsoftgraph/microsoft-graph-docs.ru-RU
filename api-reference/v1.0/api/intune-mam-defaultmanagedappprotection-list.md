---
title: Перечисление объектов defaultManagedAppProtection
description: Перечисление свойств и связей объектов defaultManagedAppProtection.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 167c8eb1d85a912e9f259d6a9a7942122ad853be
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363880"
---
# <a name="list-defaultmanagedappprotections"></a><span data-ttu-id="dd185-103">Перечисление объектов defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="dd185-103">List defaultManagedAppProtections</span></span>

> <span data-ttu-id="dd185-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd185-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd185-105">Перечисление свойств и связей объектов [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dd185-105">List properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd185-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dd185-106">Prerequisites</span></span>
<span data-ttu-id="dd185-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd185-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd185-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd185-109">Permission type</span></span>|<span data-ttu-id="dd185-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd185-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd185-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd185-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dd185-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd185-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dd185-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd185-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd185-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd185-114">Not supported.</span></span>|
|<span data-ttu-id="dd185-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd185-115">Application</span></span>|<span data-ttu-id="dd185-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd185-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd185-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd185-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="dd185-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd185-118">Request headers</span></span>
|<span data-ttu-id="dd185-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd185-119">Header</span></span>|<span data-ttu-id="dd185-120">Значение</span><span class="sxs-lookup"><span data-stu-id="dd185-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd185-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd185-121">Authorization</span></span>|<span data-ttu-id="dd185-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd185-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd185-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dd185-123">Accept</span></span>|<span data-ttu-id="dd185-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dd185-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd185-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd185-125">Request body</span></span>
<span data-ttu-id="dd185-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd185-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd185-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd185-127">Response</span></span>
<span data-ttu-id="dd185-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dd185-128">If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd185-129">Пример</span><span class="sxs-lookup"><span data-stu-id="dd185-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd185-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd185-130">Request</span></span>
<span data-ttu-id="dd185-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd185-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="dd185-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd185-132">Response</span></span>
<span data-ttu-id="dd185-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd185-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




