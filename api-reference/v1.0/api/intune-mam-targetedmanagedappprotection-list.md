---
title: Перечисление объектов targetedManagedAppProtection
description: Перечисление свойств и связей объектов targetedManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 48fef12c16e01c3f05167abb21e7829c83c57b3e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825468"
---
# <a name="list-targetedmanagedappprotections"></a><span data-ttu-id="87f48-103">Перечисление объектов targetedManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="87f48-103">List targetedManagedAppProtections</span></span>

> <span data-ttu-id="87f48-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="87f48-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87f48-105">Перечисление свойств и связей объектов [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87f48-105">List properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87f48-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="87f48-106">Prerequisites</span></span>
<span data-ttu-id="87f48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87f48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87f48-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87f48-109">Permission type</span></span>|<span data-ttu-id="87f48-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87f48-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87f48-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87f48-111">Delegated (work or school account)</span></span>|<span data-ttu-id="87f48-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="87f48-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="87f48-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87f48-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87f48-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87f48-114">Not supported.</span></span>|
|<span data-ttu-id="87f48-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87f48-115">Application</span></span>|<span data-ttu-id="87f48-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87f48-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87f48-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87f48-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="87f48-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87f48-118">Request headers</span></span>
|<span data-ttu-id="87f48-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87f48-119">Header</span></span>|<span data-ttu-id="87f48-120">Значение</span><span class="sxs-lookup"><span data-stu-id="87f48-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87f48-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="87f48-121">Authorization</span></span>|<span data-ttu-id="87f48-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="87f48-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87f48-123">Accept</span><span class="sxs-lookup"><span data-stu-id="87f48-123">Accept</span></span>|<span data-ttu-id="87f48-124">application/json</span><span class="sxs-lookup"><span data-stu-id="87f48-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87f48-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="87f48-125">Request body</span></span>
<span data-ttu-id="87f48-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87f48-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87f48-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="87f48-127">Response</span></span>
<span data-ttu-id="87f48-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="87f48-128">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87f48-129">Пример</span><span class="sxs-lookup"><span data-stu-id="87f48-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="87f48-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="87f48-130">Request</span></span>
<span data-ttu-id="87f48-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87f48-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="87f48-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="87f48-132">Response</span></span>
<span data-ttu-id="87f48-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="87f48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1750

{
  "value": [
    {
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
  ]
}
```



