---
title: Перечисление объектов managedAppProtection
description: Список свойств и связей объектов managedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b26a35635f9cba39ae7c6fa1c1528f5b88f664a5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463379"
---
# <a name="list-managedappprotections"></a><span data-ttu-id="06d4e-103">Перечисление объектов managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="06d4e-103">List managedAppProtections</span></span>

<span data-ttu-id="06d4e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="06d4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06d4e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06d4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06d4e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06d4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06d4e-107">Список свойств и связей объектов [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06d4e-107">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06d4e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="06d4e-108">Prerequisites</span></span>
<span data-ttu-id="06d4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06d4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06d4e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06d4e-111">Permission type</span></span>|<span data-ttu-id="06d4e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06d4e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06d4e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06d4e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06d4e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="06d4e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="06d4e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06d4e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06d4e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06d4e-116">Not supported.</span></span>|
|<span data-ttu-id="06d4e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06d4e-117">Application</span></span>|<span data-ttu-id="06d4e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="06d4e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06d4e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06d4e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="06d4e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="06d4e-120">Request headers</span></span>
|<span data-ttu-id="06d4e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06d4e-121">Header</span></span>|<span data-ttu-id="06d4e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="06d4e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06d4e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06d4e-123">Authorization</span></span>|<span data-ttu-id="06d4e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06d4e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06d4e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="06d4e-125">Accept</span></span>|<span data-ttu-id="06d4e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06d4e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06d4e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06d4e-127">Request body</span></span>
<span data-ttu-id="06d4e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06d4e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06d4e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="06d4e-129">Response</span></span>
<span data-ttu-id="06d4e-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppProtection](../resources/intune-mam-managedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="06d4e-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06d4e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="06d4e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="06d4e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d4e-132">Request</span></span>
<span data-ttu-id="06d4e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06d4e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="06d4e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d4e-134">Response</span></span>
<span data-ttu-id="06d4e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06d4e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2589

{
  "value": [
    {
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
      "appActionIfUnableToAuthenticateUser": "wipe"
    }
  ]
}
```





