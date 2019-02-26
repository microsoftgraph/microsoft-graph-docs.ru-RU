---
title: Перечисление объектов iosManagedAppProtection
description: Перечисление свойств и связей объектов iosManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bcb31258ad79cd575c73b8adde41821caac220b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260489"
---
# <a name="list-iosmanagedappprotections"></a><span data-ttu-id="48593-103">Перечисление объектов iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="48593-103">List iosManagedAppProtections</span></span>

> <span data-ttu-id="48593-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48593-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48593-105">Перечисление свойств и связей объектов [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="48593-105">List properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48593-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="48593-106">Prerequisites</span></span>
<span data-ttu-id="48593-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="48593-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="48593-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48593-109">Permission type</span></span>|<span data-ttu-id="48593-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48593-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48593-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48593-111">Delegated (work or school account)</span></span>|<span data-ttu-id="48593-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="48593-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="48593-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48593-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48593-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48593-114">Not supported.</span></span>|
|<span data-ttu-id="48593-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48593-115">Application</span></span>|<span data-ttu-id="48593-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48593-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48593-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48593-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="48593-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48593-118">Request headers</span></span>
|<span data-ttu-id="48593-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48593-119">Header</span></span>|<span data-ttu-id="48593-120">Значение</span><span class="sxs-lookup"><span data-stu-id="48593-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48593-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="48593-121">Authorization</span></span>|<span data-ttu-id="48593-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="48593-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48593-123">Accept</span><span class="sxs-lookup"><span data-stu-id="48593-123">Accept</span></span>|<span data-ttu-id="48593-124">application/json</span><span class="sxs-lookup"><span data-stu-id="48593-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48593-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48593-125">Request body</span></span>
<span data-ttu-id="48593-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48593-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48593-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="48593-127">Response</span></span>
<span data-ttu-id="48593-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="48593-128">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48593-129">Пример</span><span class="sxs-lookup"><span data-stu-id="48593-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="48593-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="48593-130">Request</span></span>
<span data-ttu-id="48593-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48593-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="48593-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="48593-132">Response</span></span>
<span data-ttu-id="48593-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="48593-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1933

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
      "isAssigned": true,
      "appDataEncryptionType": "afterDeviceRestart",
      "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
      "deployedAppCount": 0,
      "faceIdBlocked": true
    }
  ]
}
```



