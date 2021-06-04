---
title: Перечисление объектов managedAppProtection
description: Список свойств и связей объектов managedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9ff9173889078fe89fc2966906d391e65bbf2dc9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753521"
---
# <a name="list-managedappprotections"></a><span data-ttu-id="5f638-103">Перечисление объектов managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="5f638-103">List managedAppProtections</span></span>

<span data-ttu-id="5f638-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f638-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f638-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f638-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f638-106">Список свойств и связей объектов [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="5f638-106">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f638-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5f638-107">Prerequisites</span></span>
<span data-ttu-id="5f638-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f638-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f638-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f638-110">Permission type</span></span>|<span data-ttu-id="5f638-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f638-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f638-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f638-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f638-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f638-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5f638-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f638-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f638-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f638-115">Not supported.</span></span>|
|<span data-ttu-id="5f638-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5f638-116">Application</span></span>|<span data-ttu-id="5f638-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f638-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f638-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f638-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="5f638-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5f638-119">Request headers</span></span>
|<span data-ttu-id="5f638-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f638-120">Header</span></span>|<span data-ttu-id="5f638-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5f638-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f638-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f638-122">Authorization</span></span>|<span data-ttu-id="5f638-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f638-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f638-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5f638-124">Accept</span></span>|<span data-ttu-id="5f638-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5f638-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f638-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f638-126">Request body</span></span>
<span data-ttu-id="5f638-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f638-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f638-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f638-128">Response</span></span>
<span data-ttu-id="5f638-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppProtection](../resources/intune-mam-managedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5f638-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f638-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5f638-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f638-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f638-131">Request</span></span>
<span data-ttu-id="5f638-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f638-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="5f638-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f638-133">Response</span></span>
<span data-ttu-id="5f638-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f638-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1757

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
      "minimumWarningAppVersion": "Minimum Warning App Version value",
      "managedBrowser": "microsoftEdge"
    }
  ]
}
```




