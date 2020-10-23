---
title: Get iosLobApp
description: Чтение свойств и связей объекта iosLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 50f69d4974d903483a66cedd3b1857066c3e4048
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700404"
---
# <a name="get-ioslobapp"></a><span data-ttu-id="42c06-103">Get iosLobApp</span><span class="sxs-lookup"><span data-stu-id="42c06-103">Get iosLobApp</span></span>

<span data-ttu-id="42c06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42c06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42c06-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42c06-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42c06-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42c06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42c06-107">Чтение свойств и связей объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="42c06-107">Read properties and relationships of the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42c06-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="42c06-108">Prerequisites</span></span>
<span data-ttu-id="42c06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42c06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42c06-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42c06-111">Permission type</span></span>|<span data-ttu-id="42c06-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42c06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42c06-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42c06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42c06-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="42c06-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="42c06-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42c06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42c06-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42c06-116">Not supported.</span></span>|
|<span data-ttu-id="42c06-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42c06-117">Application</span></span>|<span data-ttu-id="42c06-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="42c06-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42c06-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42c06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42c06-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="42c06-120">Optional query parameters</span></span>
<span data-ttu-id="42c06-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="42c06-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42c06-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42c06-122">Request headers</span></span>
|<span data-ttu-id="42c06-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42c06-123">Header</span></span>|<span data-ttu-id="42c06-124">Значение</span><span class="sxs-lookup"><span data-stu-id="42c06-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42c06-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42c06-125">Authorization</span></span>|<span data-ttu-id="42c06-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42c06-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42c06-127">Accept</span><span class="sxs-lookup"><span data-stu-id="42c06-127">Accept</span></span>|<span data-ttu-id="42c06-128">application/json</span><span class="sxs-lookup"><span data-stu-id="42c06-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42c06-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="42c06-129">Request body</span></span>
<span data-ttu-id="42c06-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42c06-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42c06-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="42c06-131">Response</span></span>
<span data-ttu-id="42c06-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosLobApp](../resources/intune-apps-ioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="42c06-132">If successful, this method returns a `200 OK` response code and [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42c06-133">Пример</span><span class="sxs-lookup"><span data-stu-id="42c06-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="42c06-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="42c06-134">Request</span></span>
<span data-ttu-id="42c06-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42c06-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="42c06-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="42c06-136">Response</span></span>
<span data-ttu-id="42c06-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42c06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1757

{
  "value": {
    "@odata.type": "#microsoft.graph.iosLobApp",
    "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "bundleId": "Bundle Id value",
    "applicableDeviceType": {
      "@odata.type": "microsoft.graph.iosDeviceType",
      "iPad": true,
      "iPhoneAndIPod": true
    },
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
      "v8_0": true,
      "v9_0": true,
      "v10_0": true,
      "v11_0": true,
      "v12_0": true,
      "v13_0": true
    },
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "versionNumber": "Version Number value",
    "buildNumber": "Build Number value",
    "identityVersion": "Identity Version value"
  }
}
```





