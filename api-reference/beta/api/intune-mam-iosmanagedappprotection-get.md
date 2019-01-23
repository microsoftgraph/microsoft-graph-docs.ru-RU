---
title: Получение объекта iosManagedAppProtection
description: Чтение свойств и связей объекта iosManagedAppProtection.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6d39d28ceb4f207e6ae93e7f941878f3a484f971
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420257"
---
# <a name="get-iosmanagedappprotection"></a><span data-ttu-id="b69fb-103">Получение объекта iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="b69fb-103">Get iosManagedAppProtection</span></span>

> <span data-ttu-id="b69fb-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b69fb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b69fb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b69fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b69fb-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b69fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b69fb-107">Чтение свойств и связей объекта [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b69fb-107">Read properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b69fb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b69fb-108">Prerequisites</span></span>
<span data-ttu-id="b69fb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b69fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b69fb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b69fb-111">Permission type</span></span>|<span data-ttu-id="b69fb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b69fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b69fb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b69fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b69fb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b69fb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b69fb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b69fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b69fb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b69fb-116">Not supported.</span></span>|
|<span data-ttu-id="b69fb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b69fb-117">Application</span></span>|<span data-ttu-id="b69fb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b69fb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b69fb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b69fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b69fb-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b69fb-120">Optional query parameters</span></span>
<span data-ttu-id="b69fb-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b69fb-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b69fb-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b69fb-122">Request headers</span></span>
|<span data-ttu-id="b69fb-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b69fb-123">Header</span></span>|<span data-ttu-id="b69fb-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b69fb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b69fb-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b69fb-125">Authorization</span></span>|<span data-ttu-id="b69fb-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b69fb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b69fb-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b69fb-127">Accept</span></span>|<span data-ttu-id="b69fb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b69fb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b69fb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b69fb-129">Request body</span></span>
<span data-ttu-id="b69fb-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b69fb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b69fb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b69fb-131">Response</span></span>
<span data-ttu-id="b69fb-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b69fb-132">If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b69fb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b69fb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b69fb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b69fb-134">Request</span></span>
<span data-ttu-id="b69fb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b69fb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="b69fb-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b69fb-136">Response</span></span>
<span data-ttu-id="b69fb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b69fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2804

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
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




