---
title: Перечисление объектов iosManagedAppProtection
description: Перечисление свойств и связей объектов iosManagedAppProtection.
ms.openlocfilehash: 61aad2322cbd74cd9e38331e4d12f738584a4434
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078375"
---
# <a name="list-iosmanagedappprotections"></a><span data-ttu-id="35739-103">Перечисление объектов iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="35739-103">List iosManagedAppProtections</span></span>

> <span data-ttu-id="35739-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35739-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35739-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35739-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35739-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="35739-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35739-107">Перечисление свойств и связей объектов [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="35739-107">List properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35739-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="35739-108">Prerequisites</span></span>
<span data-ttu-id="35739-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35739-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35739-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35739-111">Permission type</span></span>|<span data-ttu-id="35739-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35739-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35739-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35739-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35739-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="35739-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="35739-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35739-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35739-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35739-116">Not supported.</span></span>|
|<span data-ttu-id="35739-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35739-117">Application</span></span>|<span data-ttu-id="35739-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35739-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35739-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35739-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="35739-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35739-120">Request headers</span></span>
|<span data-ttu-id="35739-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35739-121">Header</span></span>|<span data-ttu-id="35739-122">Значение</span><span class="sxs-lookup"><span data-stu-id="35739-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35739-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="35739-123">Authorization</span></span>|<span data-ttu-id="35739-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="35739-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35739-125">Accept</span><span class="sxs-lookup"><span data-stu-id="35739-125">Accept</span></span>|<span data-ttu-id="35739-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35739-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35739-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35739-127">Request body</span></span>
<span data-ttu-id="35739-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35739-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35739-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="35739-129">Response</span></span>
<span data-ttu-id="35739-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="35739-130">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35739-131">Пример</span><span class="sxs-lookup"><span data-stu-id="35739-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="35739-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="35739-132">Request</span></span>
<span data-ttu-id="35739-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35739-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="35739-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="35739-134">Response</span></span>
<span data-ttu-id="35739-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="35739-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2870

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
      "minimumWipeOsVersion": "Minimum Wipe Os Version value",
      "minimumWipeAppVersion": "Minimum Wipe App Version value",
      "appActionIfDeviceComplianceRequired": "wipe",
      "appActionIfMaximumPinRetriesExceeded": "wipe",
      "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
      "isAssigned": true,
      "targetedAppManagementLevels": "unmanaged",
      "appDataEncryptionType": "afterDeviceRestart",
      "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
      "deployedAppCount": 0,
      "faceIdBlocked": true,
      "exemptedAppProtocols": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
      "allowedIosDeviceModels": "Allowed Ios Device Models value",
      "appActionIfIosDeviceModelNotAllowed": "wipe",
      "thirdPartyKeyboardsBlocked": true,
      "filterOpenInToOnlyManagedApps": true,
      "disableProtectionOfManagedOutboundOpenInData": true,
      "protectInboundDataFromUnknownSources": true
    }
  ]
}
```





