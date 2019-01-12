---
title: Перечисление объектов managedAppProtection
description: Список свойств и связей объектов managedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a1c6d4462ae015af1e1c5b625feb7bbeec05aa5f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942873"
---
# <a name="list-managedappprotections"></a><span data-ttu-id="19a8a-103">Перечисление объектов managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="19a8a-103">List managedAppProtections</span></span>

> <span data-ttu-id="19a8a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="19a8a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19a8a-105">Список свойств и связей объектов [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="19a8a-105">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="19a8a-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="19a8a-106">Prerequisites</span></span>
<span data-ttu-id="19a8a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19a8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19a8a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19a8a-109">Permission type</span></span>|<span data-ttu-id="19a8a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19a8a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19a8a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19a8a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="19a8a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="19a8a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="19a8a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19a8a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19a8a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19a8a-114">Not supported.</span></span>|
|<span data-ttu-id="19a8a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19a8a-115">Application</span></span>|<span data-ttu-id="19a8a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19a8a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19a8a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19a8a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="19a8a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19a8a-118">Request headers</span></span>
|<span data-ttu-id="19a8a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19a8a-119">Header</span></span>|<span data-ttu-id="19a8a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="19a8a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19a8a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="19a8a-121">Authorization</span></span>|<span data-ttu-id="19a8a-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="19a8a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19a8a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="19a8a-123">Accept</span></span>|<span data-ttu-id="19a8a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="19a8a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19a8a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19a8a-125">Request body</span></span>
<span data-ttu-id="19a8a-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19a8a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19a8a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="19a8a-127">Response</span></span>
<span data-ttu-id="19a8a-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppProtection](../resources/intune-mam-managedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="19a8a-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19a8a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="19a8a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="19a8a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="19a8a-130">Request</span></span>
<span data-ttu-id="19a8a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19a8a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="19a8a-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="19a8a-132">Response</span></span>
<span data-ttu-id="19a8a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="19a8a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



