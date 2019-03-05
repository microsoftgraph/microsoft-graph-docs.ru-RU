---
title: Get managedAppProtection
description: Чтение свойств и связей объекта managedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0a4e04162a6ce235a9a84f5677f65bb0caa2a15e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252345"
---
# <a name="get-managedappprotection"></a><span data-ttu-id="18525-103">Get managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="18525-103">Get managedAppProtection</span></span>

> <span data-ttu-id="18525-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18525-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18525-105">Чтение свойств и связей объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="18525-105">Read properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18525-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="18525-106">Prerequisites</span></span>
<span data-ttu-id="18525-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="18525-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="18525-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18525-109">Permission type</span></span>|<span data-ttu-id="18525-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18525-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18525-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18525-111">Delegated (work or school account)</span></span>|<span data-ttu-id="18525-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="18525-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="18525-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18525-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18525-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18525-114">Not supported.</span></span>|
|<span data-ttu-id="18525-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18525-115">Application</span></span>|<span data-ttu-id="18525-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18525-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18525-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18525-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18525-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="18525-118">Optional query parameters</span></span>
<span data-ttu-id="18525-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="18525-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18525-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18525-120">Request headers</span></span>
|<span data-ttu-id="18525-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18525-121">Header</span></span>|<span data-ttu-id="18525-122">Значение</span><span class="sxs-lookup"><span data-stu-id="18525-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18525-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18525-123">Authorization</span></span>|<span data-ttu-id="18525-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="18525-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18525-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18525-125">Accept</span></span>|<span data-ttu-id="18525-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18525-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18525-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18525-127">Request body</span></span>
<span data-ttu-id="18525-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18525-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18525-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="18525-129">Response</span></span>
<span data-ttu-id="18525-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppProtection](../resources/intune-mam-managedappprotection.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="18525-130">If successful, this method returns a `200 OK` response code and [managedAppProtection](../resources/intune-mam-managedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18525-131">Пример</span><span class="sxs-lookup"><span data-stu-id="18525-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="18525-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="18525-132">Request</span></span>
<span data-ttu-id="18525-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18525-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="18525-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="18525-134">Response</span></span>
<span data-ttu-id="18525-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18525-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1631

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
    "minimumWarningAppVersion": "Minimum Warning App Version value"
  }
}
```



