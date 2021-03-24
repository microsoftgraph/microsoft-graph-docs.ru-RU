---
title: Get managedAndroidLobApp
description: Чтение свойств и связей объекта managedAndroidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 44a6cda8d145d31dbc94600b65b307a56eca7061
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143740"
---
# <a name="get-managedandroidlobapp"></a><span data-ttu-id="61851-103">Get managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="61851-103">Get managedAndroidLobApp</span></span>

<span data-ttu-id="61851-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61851-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61851-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61851-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61851-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="61851-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61851-107">Чтение свойств и связей объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="61851-107">Read properties and relationships of the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61851-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="61851-108">Prerequisites</span></span>
<span data-ttu-id="61851-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61851-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61851-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61851-111">Permission type</span></span>|<span data-ttu-id="61851-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61851-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61851-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61851-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61851-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61851-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="61851-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61851-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61851-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61851-116">Not supported.</span></span>|
|<span data-ttu-id="61851-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="61851-117">Application</span></span>|<span data-ttu-id="61851-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61851-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61851-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61851-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61851-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="61851-120">Optional query parameters</span></span>
<span data-ttu-id="61851-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="61851-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61851-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61851-122">Request headers</span></span>
|<span data-ttu-id="61851-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="61851-123">Header</span></span>|<span data-ttu-id="61851-124">Значение</span><span class="sxs-lookup"><span data-stu-id="61851-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61851-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="61851-125">Authorization</span></span>|<span data-ttu-id="61851-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61851-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61851-127">Accept</span><span class="sxs-lookup"><span data-stu-id="61851-127">Accept</span></span>|<span data-ttu-id="61851-128">application/json</span><span class="sxs-lookup"><span data-stu-id="61851-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61851-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61851-129">Request body</span></span>
<span data-ttu-id="61851-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="61851-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61851-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="61851-131">Response</span></span>
<span data-ttu-id="61851-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="61851-132">If successful, this method returns a `200 OK` response code and [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61851-133">Пример</span><span class="sxs-lookup"><span data-stu-id="61851-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="61851-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="61851-134">Request</span></span>
<span data-ttu-id="61851-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61851-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="61851-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="61851-136">Response</span></span>
<span data-ttu-id="61851-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="61851-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1891

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAndroidLobApp",
    "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "uploadState": 11,
    "publishingState": "processing",
    "isAssigned": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "dependentAppCount": 1,
    "supersedingAppCount": 3,
    "supersededAppCount": 2,
    "appAvailability": "lineOfBusiness",
    "version": "Version value",
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "packageId": "Package Id value",
    "identityName": "Identity Name value",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
      "v4_0": true,
      "v4_0_3": true,
      "v4_1": true,
      "v4_2": true,
      "v4_3": true,
      "v4_4": true,
      "v5_0": true,
      "v5_1": true,
      "v6_0": true,
      "v7_0": true,
      "v7_1": true,
      "v8_0": true,
      "v8_1": true,
      "v9_0": true,
      "v10_0": true,
      "v11_0": true
    },
    "versionName": "Version Name value",
    "versionCode": "Version Code value",
    "identityVersion": "Identity Version value"
  }
}
```




