---
title: Перечисление объектов defaultManagedAppProtection
description: Перечисление свойств и связей объектов defaultManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bf7a1f8bef68cee9b57614d43c02aa957515b5e7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758124"
---
# <a name="list-defaultmanagedappprotections"></a><span data-ttu-id="4bd08-103">Перечисление объектов defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="4bd08-103">List defaultManagedAppProtections</span></span>

<span data-ttu-id="4bd08-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bd08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4bd08-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4bd08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bd08-106">Перечисление свойств и связей объектов [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4bd08-106">List properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bd08-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4bd08-107">Prerequisites</span></span>
<span data-ttu-id="4bd08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bd08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bd08-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bd08-110">Permission type</span></span>|<span data-ttu-id="4bd08-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bd08-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bd08-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bd08-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4bd08-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bd08-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4bd08-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bd08-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bd08-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bd08-115">Not supported.</span></span>|
|<span data-ttu-id="4bd08-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4bd08-116">Application</span></span>|<span data-ttu-id="4bd08-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bd08-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bd08-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bd08-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="4bd08-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4bd08-119">Request headers</span></span>
|<span data-ttu-id="4bd08-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4bd08-120">Header</span></span>|<span data-ttu-id="4bd08-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4bd08-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bd08-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bd08-122">Authorization</span></span>|<span data-ttu-id="4bd08-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bd08-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bd08-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4bd08-124">Accept</span></span>|<span data-ttu-id="4bd08-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4bd08-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bd08-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4bd08-126">Request body</span></span>
<span data-ttu-id="4bd08-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4bd08-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bd08-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bd08-128">Response</span></span>
<span data-ttu-id="4bd08-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4bd08-129">If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bd08-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4bd08-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bd08-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bd08-131">Request</span></span>
<span data-ttu-id="4bd08-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bd08-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="4bd08-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bd08-133">Response</span></span>
<span data-ttu-id="4bd08-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4bd08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2422

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
  ]
}
```




