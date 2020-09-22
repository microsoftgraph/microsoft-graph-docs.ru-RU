---
title: Получение объекта iosManagedAppProtection
description: Чтение свойств и связей объекта iosManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 52f6c82f454621918d48b953ae8a53dd3a0a8c2f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031937"
---
# <a name="get-iosmanagedappprotection"></a><span data-ttu-id="47f2d-103">Получение объекта iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="47f2d-103">Get iosManagedAppProtection</span></span>

<span data-ttu-id="47f2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47f2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47f2d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47f2d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47f2d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47f2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47f2d-107">Чтение свойств и связей объекта [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="47f2d-107">Read properties and relationships of the [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47f2d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="47f2d-108">Prerequisites</span></span>
<span data-ttu-id="47f2d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47f2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47f2d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47f2d-111">Permission type</span></span>|<span data-ttu-id="47f2d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47f2d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47f2d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47f2d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="47f2d-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="47f2d-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="47f2d-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="47f2d-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="47f2d-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="47f2d-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="47f2d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="47f2d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="47f2d-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47f2d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47f2d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47f2d-119">Not supported.</span></span>|
|<span data-ttu-id="47f2d-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47f2d-120">Application</span></span>||
| <span data-ttu-id="47f2d-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="47f2d-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="47f2d-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="47f2d-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="47f2d-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="47f2d-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="47f2d-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="47f2d-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47f2d-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47f2d-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47f2d-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="47f2d-126">Optional query parameters</span></span>
<span data-ttu-id="47f2d-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="47f2d-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47f2d-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47f2d-128">Request headers</span></span>
|<span data-ttu-id="47f2d-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47f2d-129">Header</span></span>|<span data-ttu-id="47f2d-130">Значение</span><span class="sxs-lookup"><span data-stu-id="47f2d-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47f2d-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="47f2d-131">Authorization</span></span>|<span data-ttu-id="47f2d-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47f2d-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47f2d-133">Accept</span><span class="sxs-lookup"><span data-stu-id="47f2d-133">Accept</span></span>|<span data-ttu-id="47f2d-134">application/json</span><span class="sxs-lookup"><span data-stu-id="47f2d-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47f2d-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47f2d-135">Request body</span></span>
<span data-ttu-id="47f2d-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47f2d-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47f2d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="47f2d-137">Response</span></span>
<span data-ttu-id="47f2d-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="47f2d-138">If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47f2d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="47f2d-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="47f2d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="47f2d-140">Request</span></span>
<span data-ttu-id="47f2d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47f2d-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="47f2d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="47f2d-142">Response</span></span>
<span data-ttu-id="47f2d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47f2d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2944

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
    "allowedOutboundClipboardSharingExceptionLength": 14,
    "notificationRestriction": "blockOrganizationalData",
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
    "filterOpenInToOnlyManagedApps": true,
    "disableProtectionOfManagedOutboundOpenInData": true,
    "protectInboundDataFromUnknownSources": true,
    "customBrowserProtocol": "Custom Browser Protocol value"
  }
}
```









