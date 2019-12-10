---
title: Получение объекта targetedManagedAppProtection
description: Чтение свойств и связей объекта targetedManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e88ee1539af667ab2fde5ee4cd4f90ccbbbf0109
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942214"
---
# <a name="get-targetedmanagedappprotection"></a><span data-ttu-id="ddb85-103">Получение объекта targetedManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="ddb85-103">Get targetedManagedAppProtection</span></span>

> <span data-ttu-id="ddb85-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddb85-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddb85-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ddb85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddb85-106">Чтение свойств и связей объекта [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="ddb85-106">Read properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddb85-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ddb85-107">Prerequisites</span></span>
<span data-ttu-id="ddb85-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddb85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddb85-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddb85-110">Permission type</span></span>|<span data-ttu-id="ddb85-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddb85-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddb85-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddb85-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ddb85-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddb85-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ddb85-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddb85-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddb85-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddb85-115">Not supported.</span></span>|
|<span data-ttu-id="ddb85-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddb85-116">Application</span></span>|<span data-ttu-id="ddb85-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddb85-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddb85-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddb85-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddb85-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ddb85-119">Optional query parameters</span></span>
<span data-ttu-id="ddb85-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ddb85-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddb85-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddb85-121">Request headers</span></span>
|<span data-ttu-id="ddb85-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ddb85-122">Header</span></span>|<span data-ttu-id="ddb85-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ddb85-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddb85-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ddb85-124">Authorization</span></span>|<span data-ttu-id="ddb85-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddb85-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddb85-126">Accept</span><span class="sxs-lookup"><span data-stu-id="ddb85-126">Accept</span></span>|<span data-ttu-id="ddb85-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ddb85-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddb85-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ddb85-128">Request body</span></span>
<span data-ttu-id="ddb85-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ddb85-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddb85-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ddb85-130">Response</span></span>
<span data-ttu-id="ddb85-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ddb85-131">If successful, this method returns a `200 OK` response code and [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddb85-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ddb85-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddb85-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddb85-133">Request</span></span>
<span data-ttu-id="ddb85-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddb85-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="ddb85-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddb85-135">Response</span></span>
<span data-ttu-id="ddb85-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ddb85-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2497

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "b6b92266-2266-b6b9-6622-b9b66622b9b6",
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
    "previousPinBlockCount": 5,
    "managedBrowser": "microsoftEdge",
    "maximumAllowedDeviceThreatLevel": "secured",
    "mobileThreatDefenseRemediationAction": "wipe",
    "blockDataIngestionIntoOrganizationDocuments": true,
    "allowedDataIngestionLocations": [
      "sharePoint"
    ],
    "isAssigned": true,
    "targetedAppManagementLevels": "unmanaged"
  }
}
```





