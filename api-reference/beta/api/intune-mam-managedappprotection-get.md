---
title: Get managedAppProtection
description: Чтение свойств и связей объекта managedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 787d593da91fecd2f3d8d7c88dbc4849a3843c7d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33903553"
---
# <a name="get-managedappprotection"></a><span data-ttu-id="5c7ef-103">Get managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="5c7ef-103">Get managedAppProtection</span></span>

> <span data-ttu-id="5c7ef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c7ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c7ef-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c7ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c7ef-106">Чтение свойств и связей объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="5c7ef-106">Read properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c7ef-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5c7ef-107">Prerequisites</span></span>
<span data-ttu-id="5c7ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c7ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c7ef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c7ef-110">Permission type</span></span>|<span data-ttu-id="5c7ef-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c7ef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c7ef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c7ef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c7ef-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c7ef-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5c7ef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c7ef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c7ef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c7ef-115">Not supported.</span></span>|
|<span data-ttu-id="5c7ef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c7ef-116">Application</span></span>|<span data-ttu-id="5c7ef-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c7ef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c7ef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c7ef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c7ef-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c7ef-119">Optional query parameters</span></span>
<span data-ttu-id="5c7ef-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5c7ef-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c7ef-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c7ef-121">Request headers</span></span>
|<span data-ttu-id="5c7ef-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c7ef-122">Header</span></span>|<span data-ttu-id="5c7ef-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5c7ef-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c7ef-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c7ef-124">Authorization</span></span>|<span data-ttu-id="5c7ef-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c7ef-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c7ef-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5c7ef-126">Accept</span></span>|<span data-ttu-id="5c7ef-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5c7ef-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c7ef-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c7ef-128">Request body</span></span>
<span data-ttu-id="5c7ef-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c7ef-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c7ef-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c7ef-130">Response</span></span>
<span data-ttu-id="5c7ef-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppProtection](../resources/intune-mam-managedappprotection.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5c7ef-131">If successful, this method returns a `200 OK` response code and [managedAppProtection](../resources/intune-mam-managedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c7ef-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5c7ef-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c7ef-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c7ef-133">Request</span></span>
<span data-ttu-id="5c7ef-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c7ef-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="5c7ef-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c7ef-135">Response</span></span>
<span data-ttu-id="5c7ef-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c7ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2053

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
    "minimumRequiredOsVersion": "Minimum Required Os Version value",
    "minimumWarningOsVersion": "Minimum Warning Os Version value",
    "minimumRequiredAppVersion": "Minimum Required App Version value",
    "minimumWarningAppVersion": "Minimum Warning App Version value",
    "minimumWipeOsVersion": "Minimum Wipe Os Version value",
    "minimumWipeAppVersion": "Minimum Wipe App Version value",
    "appActionIfDeviceComplianceRequired": "wipe",
    "appActionIfMaximumPinRetriesExceeded": "wipe",
    "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
    "allowedOutboundClipboardSharingExceptionLength": 14
  }
}
```




