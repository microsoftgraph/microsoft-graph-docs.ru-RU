---
title: Перечисление объектов androidManagedAppProtection
description: Перечисление свойств и связей объектов androidManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fcaeab1b111b26e92a6b27ba3a5c5493f7d4fd3e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566845"
---
# <a name="list-androidmanagedappprotections"></a><span data-ttu-id="a49f7-103">Перечисление объектов androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="a49f7-103">List androidManagedAppProtections</span></span>

> <span data-ttu-id="a49f7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a49f7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a49f7-105">Перечисление свойств и связей объектов [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="a49f7-105">List properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a49f7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a49f7-106">Prerequisites</span></span>
<span data-ttu-id="a49f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a49f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a49f7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a49f7-109">Permission type</span></span>|<span data-ttu-id="a49f7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a49f7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a49f7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a49f7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a49f7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a49f7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a49f7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a49f7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a49f7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a49f7-114">Not supported.</span></span>|
|<span data-ttu-id="a49f7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a49f7-115">Application</span></span>|<span data-ttu-id="a49f7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a49f7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a49f7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a49f7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="a49f7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a49f7-118">Request headers</span></span>
|<span data-ttu-id="a49f7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a49f7-119">Header</span></span>|<span data-ttu-id="a49f7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a49f7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a49f7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a49f7-121">Authorization</span></span>|<span data-ttu-id="a49f7-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a49f7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a49f7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a49f7-123">Accept</span></span>|<span data-ttu-id="a49f7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a49f7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a49f7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a49f7-125">Request body</span></span>
<span data-ttu-id="a49f7-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a49f7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a49f7-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a49f7-127">Response</span></span>
<span data-ttu-id="a49f7-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a49f7-128">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a49f7-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a49f7-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a49f7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a49f7-130">Request</span></span>
<span data-ttu-id="a49f7-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a49f7-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="a49f7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a49f7-132">Response</span></span>
<span data-ttu-id="a49f7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a49f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2065

{
  "value": [
    {
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
  ]
}
```



