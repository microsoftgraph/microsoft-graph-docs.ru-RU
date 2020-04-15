---
title: Перечисление объектов targetedManagedAppProtection
description: Перечисление свойств и связей объектов targetedManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ee1fd79ac9ed858363c55959c1fdae549e8ec6ad
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43397727"
---
# <a name="list-targetedmanagedappprotections"></a><span data-ttu-id="eac30-103">Перечисление объектов targetedManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="eac30-103">List targetedManagedAppProtections</span></span>

<span data-ttu-id="eac30-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eac30-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eac30-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eac30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eac30-106">Перечисление свойств и связей объектов [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="eac30-106">List properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eac30-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="eac30-107">Prerequisites</span></span>
<span data-ttu-id="eac30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eac30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eac30-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eac30-110">Permission type</span></span>|<span data-ttu-id="eac30-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eac30-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eac30-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eac30-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eac30-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eac30-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="eac30-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eac30-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eac30-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eac30-115">Not supported.</span></span>|
|<span data-ttu-id="eac30-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eac30-116">Application</span></span>|<span data-ttu-id="eac30-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eac30-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eac30-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eac30-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="eac30-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eac30-119">Request headers</span></span>
|<span data-ttu-id="eac30-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eac30-120">Header</span></span>|<span data-ttu-id="eac30-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eac30-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eac30-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eac30-122">Authorization</span></span>|<span data-ttu-id="eac30-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eac30-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eac30-124">Accept</span><span class="sxs-lookup"><span data-stu-id="eac30-124">Accept</span></span>|<span data-ttu-id="eac30-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eac30-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eac30-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eac30-126">Request body</span></span>
<span data-ttu-id="eac30-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eac30-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eac30-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="eac30-128">Response</span></span>
<span data-ttu-id="eac30-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eac30-129">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eac30-130">Пример</span><span class="sxs-lookup"><span data-stu-id="eac30-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="eac30-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="eac30-131">Request</span></span>
<span data-ttu-id="eac30-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eac30-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="eac30-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="eac30-133">Response</span></span>
<span data-ttu-id="eac30-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eac30-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






