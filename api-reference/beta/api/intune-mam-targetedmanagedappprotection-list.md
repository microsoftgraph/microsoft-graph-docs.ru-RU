---
title: Перечисление объектов targetedManagedAppProtection
description: Перечисление свойств и связей объектов targetedManagedAppProtection.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d266d7648cd584ebe37d1857a823da4824e56569
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411437"
---
# <a name="list-targetedmanagedappprotections"></a><span data-ttu-id="ba133-103">Перечисление объектов targetedManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="ba133-103">List targetedManagedAppProtections</span></span>

> <span data-ttu-id="ba133-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ba133-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ba133-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba133-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba133-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba133-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba133-107">Перечисление свойств и связей объектов [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="ba133-107">List properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba133-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ba133-108">Prerequisites</span></span>
<span data-ttu-id="ba133-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ba133-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ba133-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba133-111">Permission type</span></span>|<span data-ttu-id="ba133-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba133-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba133-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba133-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba133-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba133-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ba133-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba133-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba133-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba133-116">Not supported.</span></span>|
|<span data-ttu-id="ba133-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba133-117">Application</span></span>|<span data-ttu-id="ba133-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba133-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba133-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba133-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="ba133-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba133-120">Request headers</span></span>
|<span data-ttu-id="ba133-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba133-121">Header</span></span>|<span data-ttu-id="ba133-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ba133-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba133-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba133-123">Authorization</span></span>|<span data-ttu-id="ba133-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ba133-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba133-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ba133-125">Accept</span></span>|<span data-ttu-id="ba133-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba133-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba133-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba133-127">Request body</span></span>
<span data-ttu-id="ba133-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba133-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba133-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba133-129">Response</span></span>
<span data-ttu-id="ba133-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ba133-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba133-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ba133-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba133-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba133-132">Request</span></span>
<span data-ttu-id="ba133-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba133-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="ba133-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba133-134">Response</span></span>
<span data-ttu-id="ba133-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ba133-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2180

{
  "value": [
    {
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
      "isAssigned": true,
      "targetedAppManagementLevels": "unmanaged"
    }
  ]
}
```




