---
title: Получение объекта targetedManagedAppProtection
description: Чтение свойств и связей объекта targetedManagedAppProtection.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 781de6dc65e29f06dadb642b15a2005af7f7dec5
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363117"
---
# <a name="get-targetedmanagedappprotection"></a><span data-ttu-id="6966e-103">Получение объекта targetedManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="6966e-103">Get targetedManagedAppProtection</span></span>

> <span data-ttu-id="6966e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6966e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6966e-105">Чтение свойств и связей объекта [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="6966e-105">Read properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6966e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6966e-106">Prerequisites</span></span>
<span data-ttu-id="6966e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6966e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6966e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6966e-109">Permission type</span></span>|<span data-ttu-id="6966e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6966e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6966e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6966e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6966e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6966e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6966e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6966e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6966e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6966e-114">Not supported.</span></span>|
|<span data-ttu-id="6966e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6966e-115">Application</span></span>|<span data-ttu-id="6966e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6966e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6966e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6966e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6966e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6966e-118">Optional query parameters</span></span>
<span data-ttu-id="6966e-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6966e-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6966e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6966e-120">Request headers</span></span>
|<span data-ttu-id="6966e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6966e-121">Header</span></span>|<span data-ttu-id="6966e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6966e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6966e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6966e-123">Authorization</span></span>|<span data-ttu-id="6966e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6966e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6966e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6966e-125">Accept</span></span>|<span data-ttu-id="6966e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6966e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6966e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6966e-127">Request body</span></span>
<span data-ttu-id="6966e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6966e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6966e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6966e-129">Response</span></span>
<span data-ttu-id="6966e-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6966e-130">If successful, this method returns a `200 OK` response code and [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6966e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6966e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6966e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6966e-132">Request</span></span>
<span data-ttu-id="6966e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6966e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="6966e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6966e-134">Response</span></span>
<span data-ttu-id="6966e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6966e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1664

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
    "isAssigned": true
  }
}
```




