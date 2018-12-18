---
title: Get defaultManagedAppProtection
description: Чтение свойств и связей объекта defaultManagedAppProtection.
author: tfitzmac
ms.openlocfilehash: 1932ee08cc3ea879dc207dade7010fc029d49afa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341624"
---
# <a name="get-defaultmanagedappprotection"></a><span data-ttu-id="e27a8-103">Get defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="e27a8-103">Get defaultManagedAppProtection</span></span>

> <span data-ttu-id="e27a8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e27a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e27a8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e27a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e27a8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e27a8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e27a8-107">Чтение свойств и связей объекта [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="e27a8-107">Read properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e27a8-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e27a8-108">Prerequisites</span></span>
<span data-ttu-id="e27a8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e27a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e27a8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e27a8-111">Permission type</span></span>|<span data-ttu-id="e27a8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e27a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e27a8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e27a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e27a8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e27a8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e27a8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e27a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e27a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e27a8-116">Not supported.</span></span>|
|<span data-ttu-id="e27a8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e27a8-117">Application</span></span>|<span data-ttu-id="e27a8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e27a8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e27a8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e27a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e27a8-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e27a8-120">Optional query parameters</span></span>
<span data-ttu-id="e27a8-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e27a8-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e27a8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e27a8-122">Request headers</span></span>
|<span data-ttu-id="e27a8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e27a8-123">Header</span></span>|<span data-ttu-id="e27a8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e27a8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e27a8-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e27a8-125">Authorization</span></span>|<span data-ttu-id="e27a8-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e27a8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e27a8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e27a8-127">Accept</span></span>|<span data-ttu-id="e27a8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e27a8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e27a8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e27a8-129">Request body</span></span>
<span data-ttu-id="e27a8-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e27a8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e27a8-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e27a8-131">Response</span></span>
<span data-ttu-id="e27a8-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e27a8-132">If successful, this method returns a `200 OK` response code and [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e27a8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e27a8-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="e27a8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e27a8-134">Request</span></span>
<span data-ttu-id="e27a8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e27a8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="e27a8-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e27a8-136">Response</span></span>
<span data-ttu-id="e27a8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e27a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3506

{
  "value": {
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
    "minimumWipeOsVersion": "Minimum Wipe Os Version value",
    "minimumWipeAppVersion": "Minimum Wipe App Version value",
    "appActionIfDeviceComplianceRequired": "wipe",
    "appActionIfMaximumPinRetriesExceeded": "wipe",
    "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
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
    "exemptedAppProtocols": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "exemptedAppPackages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "faceIdBlocked": true,
    "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
    "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
    "allowedIosDeviceModels": "Allowed Ios Device Models value",
    "appActionIfIosDeviceModelNotAllowed": "wipe",
    "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
    "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
    "thirdPartyKeyboardsBlocked": true,
    "filterOpenInToOnlyManagedApps": true,
    "disableProtectionOfManagedOutboundOpenInData": true,
    "protectInboundDataFromUnknownSources": true
  }
}
```





