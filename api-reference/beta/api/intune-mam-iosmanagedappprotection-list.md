---
title: Перечисление объектов iosManagedAppProtection
description: Перечисление свойств и связей объектов iosManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5625cca8c03cbf8ea7c9c9963b186bffc70357c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887664"
---
# <a name="list-iosmanagedappprotections"></a><span data-ttu-id="ede44-103">Перечисление объектов iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="ede44-103">List iosManagedAppProtections</span></span>

> <span data-ttu-id="ede44-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ede44-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ede44-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ede44-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ede44-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ede44-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ede44-107">Перечисление свойств и связей объектов [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="ede44-107">List properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ede44-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ede44-108">Prerequisites</span></span>
<span data-ttu-id="ede44-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ede44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ede44-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ede44-111">Permission type</span></span>|<span data-ttu-id="ede44-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ede44-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ede44-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ede44-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ede44-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ede44-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ede44-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ede44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ede44-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ede44-116">Not supported.</span></span>|
|<span data-ttu-id="ede44-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ede44-117">Application</span></span>|<span data-ttu-id="ede44-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ede44-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ede44-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ede44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="ede44-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ede44-120">Request headers</span></span>
|<span data-ttu-id="ede44-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ede44-121">Header</span></span>|<span data-ttu-id="ede44-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ede44-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ede44-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ede44-123">Authorization</span></span>|<span data-ttu-id="ede44-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ede44-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ede44-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ede44-125">Accept</span></span>|<span data-ttu-id="ede44-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ede44-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ede44-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ede44-127">Request body</span></span>
<span data-ttu-id="ede44-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ede44-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ede44-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ede44-129">Response</span></span>
<span data-ttu-id="ede44-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ede44-130">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ede44-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ede44-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ede44-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ede44-132">Request</span></span>
<span data-ttu-id="ede44-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ede44-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="ede44-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ede44-134">Response</span></span>
<span data-ttu-id="ede44-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ede44-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





