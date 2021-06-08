---
title: Перечисление объектов iosManagedAppProtection
description: Перечисление свойств и связей объектов iosManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c1fc39b448964c769ad55fee1a5fce39f6e64b1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758082"
---
# <a name="list-iosmanagedappprotections"></a><span data-ttu-id="6ff89-103">Перечисление объектов iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="6ff89-103">List iosManagedAppProtections</span></span>

<span data-ttu-id="6ff89-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ff89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ff89-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ff89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ff89-106">Перечисление свойств и связей объектов [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="6ff89-106">List properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ff89-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6ff89-107">Prerequisites</span></span>
<span data-ttu-id="6ff89-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ff89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ff89-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ff89-110">Permission type</span></span>|<span data-ttu-id="6ff89-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ff89-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ff89-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ff89-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6ff89-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ff89-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6ff89-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ff89-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ff89-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ff89-115">Not supported.</span></span>|
|<span data-ttu-id="6ff89-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6ff89-116">Application</span></span>|<span data-ttu-id="6ff89-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ff89-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ff89-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ff89-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="6ff89-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6ff89-119">Request headers</span></span>
|<span data-ttu-id="6ff89-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ff89-120">Header</span></span>|<span data-ttu-id="6ff89-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6ff89-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ff89-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ff89-122">Authorization</span></span>|<span data-ttu-id="6ff89-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ff89-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ff89-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6ff89-124">Accept</span></span>|<span data-ttu-id="6ff89-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6ff89-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ff89-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ff89-126">Request body</span></span>
<span data-ttu-id="6ff89-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ff89-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ff89-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ff89-128">Response</span></span>
<span data-ttu-id="6ff89-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6ff89-129">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ff89-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6ff89-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ff89-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ff89-131">Request</span></span>
<span data-ttu-id="6ff89-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ff89-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="6ff89-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ff89-133">Response</span></span>
<span data-ttu-id="6ff89-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ff89-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2040

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
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
      "appDataEncryptionType": "afterDeviceRestart",
      "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
      "deployedAppCount": 0,
      "faceIdBlocked": true,
      "customBrowserProtocol": "Custom Browser Protocol value"
    }
  ]
}
```




