---
title: Get managedAppProtection
description: Чтение свойств и связей объекта managedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d84ddd7a842e251aed7a8c23ca8b507ae3b420c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149158"
---
# <a name="get-managedappprotection"></a><span data-ttu-id="8f939-103">Get managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="8f939-103">Get managedAppProtection</span></span>

<span data-ttu-id="8f939-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f939-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f939-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f939-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f939-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f939-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f939-107">Чтение свойств и связей объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8f939-107">Read properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f939-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8f939-108">Prerequisites</span></span>
<span data-ttu-id="8f939-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f939-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f939-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f939-111">Permission type</span></span>|<span data-ttu-id="8f939-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f939-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f939-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f939-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f939-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f939-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8f939-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f939-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f939-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f939-116">Not supported.</span></span>|
|<span data-ttu-id="8f939-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8f939-117">Application</span></span>|<span data-ttu-id="8f939-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f939-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f939-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f939-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f939-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8f939-120">Optional query parameters</span></span>
<span data-ttu-id="8f939-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8f939-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f939-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f939-122">Request headers</span></span>
|<span data-ttu-id="8f939-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f939-123">Header</span></span>|<span data-ttu-id="8f939-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8f939-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f939-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f939-125">Authorization</span></span>|<span data-ttu-id="8f939-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f939-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f939-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8f939-127">Accept</span></span>|<span data-ttu-id="8f939-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8f939-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f939-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f939-129">Request body</span></span>
<span data-ttu-id="8f939-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f939-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f939-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f939-131">Response</span></span>
<span data-ttu-id="8f939-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppProtection](../resources/intune-mam-managedappprotection.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8f939-132">If successful, this method returns a `200 OK` response code and [managedAppProtection](../resources/intune-mam-managedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f939-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8f939-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f939-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f939-134">Request</span></span>
<span data-ttu-id="8f939-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f939-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="8f939-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f939-136">Response</span></span>
<span data-ttu-id="8f939-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f939-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2713

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "a6c064ce-64ce-a6c0-ce64-c0a6ce64c0a6",
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
    "maximumRequiredOsVersion": "Maximum Required Os Version value",
    "maximumWarningOsVersion": "Maximum Warning Os Version value",
    "maximumWipeOsVersion": "Maximum Wipe Os Version value",
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
    "appActionIfUnableToAuthenticateUser": "wipe",
    "dialerRestrictionLevel": "managedApps"
  }
}
```




