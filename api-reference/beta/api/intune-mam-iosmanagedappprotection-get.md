---
title: Получение объекта iosManagedAppProtection
description: Чтение свойств и связей объекта iosManagedAppProtection.
author: tfitzmac
ms.openlocfilehash: b913d26ae7022cff368984b65fbbf6eaa85aaad2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310208"
---
# <a name="get-iosmanagedappprotection"></a><span data-ttu-id="5cce9-103">Получение объекта iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="5cce9-103">Get iosManagedAppProtection</span></span>

> <span data-ttu-id="5cce9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5cce9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5cce9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cce9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5cce9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5cce9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5cce9-107">Чтение свойств и связей объекта [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="5cce9-107">Read properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5cce9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5cce9-108">Prerequisites</span></span>
<span data-ttu-id="5cce9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cce9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cce9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cce9-111">Permission type</span></span>|<span data-ttu-id="5cce9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cce9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cce9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cce9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5cce9-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cce9-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5cce9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cce9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cce9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cce9-116">Not supported.</span></span>|
|<span data-ttu-id="5cce9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5cce9-117">Application</span></span>|<span data-ttu-id="5cce9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cce9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cce9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cce9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5cce9-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5cce9-120">Optional query parameters</span></span>
<span data-ttu-id="5cce9-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5cce9-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5cce9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cce9-122">Request headers</span></span>
|<span data-ttu-id="5cce9-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5cce9-123">Header</span></span>|<span data-ttu-id="5cce9-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5cce9-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cce9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5cce9-125">Authorization</span></span>|<span data-ttu-id="5cce9-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5cce9-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cce9-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5cce9-127">Accept</span></span>|<span data-ttu-id="5cce9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5cce9-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cce9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5cce9-129">Request body</span></span>
<span data-ttu-id="5cce9-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5cce9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cce9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cce9-131">Response</span></span>
<span data-ttu-id="5cce9-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5cce9-132">If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cce9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5cce9-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="5cce9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cce9-134">Request</span></span>
<span data-ttu-id="5cce9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cce9-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="5cce9-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cce9-136">Response</span></span>
<span data-ttu-id="5cce9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5cce9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2736

{
  "value": {
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
}
```





