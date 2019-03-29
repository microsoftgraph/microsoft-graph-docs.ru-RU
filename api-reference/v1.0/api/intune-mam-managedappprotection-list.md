---
title: Перечисление объектов managedAppProtection
description: Список свойств и связей объектов managedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8fd9809293db8d0c1875ec1e4d0b4f35807e0821
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959693"
---
# <a name="list-managedappprotections"></a><span data-ttu-id="7a941-103">Перечисление объектов managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="7a941-103">List managedAppProtections</span></span>

> <span data-ttu-id="7a941-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a941-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a941-105">Список свойств и связей объектов [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7a941-105">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a941-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7a941-106">Prerequisites</span></span>
<span data-ttu-id="7a941-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a941-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a941-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a941-109">Permission type</span></span>|<span data-ttu-id="7a941-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a941-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a941-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a941-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7a941-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a941-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7a941-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a941-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a941-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a941-114">Not supported.</span></span>|
|<span data-ttu-id="7a941-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a941-115">Application</span></span>|<span data-ttu-id="7a941-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a941-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a941-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a941-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="7a941-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a941-118">Request headers</span></span>
|<span data-ttu-id="7a941-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a941-119">Header</span></span>|<span data-ttu-id="7a941-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7a941-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a941-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a941-121">Authorization</span></span>|<span data-ttu-id="7a941-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a941-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a941-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7a941-123">Accept</span></span>|<span data-ttu-id="7a941-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7a941-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a941-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a941-125">Request body</span></span>
<span data-ttu-id="7a941-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7a941-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a941-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a941-127">Response</span></span>
<span data-ttu-id="7a941-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppProtection](../resources/intune-mam-managedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7a941-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a941-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7a941-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a941-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a941-130">Request</span></span>
<span data-ttu-id="7a941-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a941-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="7a941-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a941-132">Response</span></span>
<span data-ttu-id="7a941-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a941-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1715

{
  "value": [
    {
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
  ]
}
```



