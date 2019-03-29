---
title: Перечисление объектов iosManagedAppProtection
description: Перечисление свойств и связей объектов iosManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b1b0793de7ec7086354abe51f691d80c801fba4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984501"
---
# <a name="list-iosmanagedappprotections"></a><span data-ttu-id="4ab46-103">Перечисление объектов iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="4ab46-103">List iosManagedAppProtections</span></span>

> <span data-ttu-id="4ab46-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ab46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ab46-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ab46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ab46-106">Перечисление свойств и связей объектов [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4ab46-106">List properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ab46-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4ab46-107">Prerequisites</span></span>
<span data-ttu-id="4ab46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ab46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ab46-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ab46-110">Permission type</span></span>|<span data-ttu-id="4ab46-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ab46-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ab46-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ab46-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ab46-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ab46-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4ab46-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ab46-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ab46-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ab46-115">Not supported.</span></span>|
|<span data-ttu-id="4ab46-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ab46-116">Application</span></span>|<span data-ttu-id="4ab46-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ab46-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ab46-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ab46-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="4ab46-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ab46-119">Request headers</span></span>
|<span data-ttu-id="4ab46-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ab46-120">Header</span></span>|<span data-ttu-id="4ab46-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4ab46-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ab46-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ab46-122">Authorization</span></span>|<span data-ttu-id="4ab46-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ab46-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ab46-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4ab46-124">Accept</span></span>|<span data-ttu-id="4ab46-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ab46-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ab46-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ab46-126">Request body</span></span>
<span data-ttu-id="4ab46-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ab46-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ab46-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ab46-128">Response</span></span>
<span data-ttu-id="4ab46-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4ab46-129">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ab46-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4ab46-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ab46-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ab46-131">Request</span></span>
<span data-ttu-id="4ab46-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ab46-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="4ab46-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ab46-133">Response</span></span>
<span data-ttu-id="4ab46-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ab46-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3005

{
  "value": [
    {
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




