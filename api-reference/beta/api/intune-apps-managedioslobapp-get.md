---
title: Get managedIOSLobApp
description: Чтение свойств и связей объекта managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d86e47c4c372e6ca9059041cf130b09e4c71ad0b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157255"
---
# <a name="get-managedioslobapp"></a><span data-ttu-id="2f4ca-103">Get managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="2f4ca-103">Get managedIOSLobApp</span></span>

<span data-ttu-id="2f4ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f4ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f4ca-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f4ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f4ca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f4ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f4ca-107">Чтение свойств и связей объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f4ca-107">Read properties and relationships of the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f4ca-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2f4ca-108">Prerequisites</span></span>
<span data-ttu-id="2f4ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f4ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f4ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f4ca-111">Permission type</span></span>|<span data-ttu-id="2f4ca-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f4ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f4ca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f4ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f4ca-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f4ca-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2f4ca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f4ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f4ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f4ca-116">Not supported.</span></span>|
|<span data-ttu-id="2f4ca-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f4ca-117">Application</span></span>|<span data-ttu-id="2f4ca-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f4ca-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f4ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f4ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f4ca-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2f4ca-120">Optional query parameters</span></span>
<span data-ttu-id="2f4ca-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2f4ca-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f4ca-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f4ca-122">Request headers</span></span>
|<span data-ttu-id="2f4ca-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f4ca-123">Header</span></span>|<span data-ttu-id="2f4ca-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2f4ca-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f4ca-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f4ca-125">Authorization</span></span>|<span data-ttu-id="2f4ca-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f4ca-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f4ca-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2f4ca-127">Accept</span></span>|<span data-ttu-id="2f4ca-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2f4ca-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f4ca-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f4ca-129">Request body</span></span>
<span data-ttu-id="2f4ca-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f4ca-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f4ca-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f4ca-131">Response</span></span>
<span data-ttu-id="2f4ca-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2f4ca-132">If successful, this method returns a `200 OK` response code and [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f4ca-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2f4ca-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f4ca-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f4ca-134">Request</span></span>
<span data-ttu-id="2f4ca-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f4ca-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="2f4ca-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f4ca-136">Response</span></span>
<span data-ttu-id="2f4ca-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f4ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1861

{
  "value": {
    "@odata.type": "#microsoft.graph.managedIOSLobApp",
    "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
      "v13_0": true,
      "v14_0": true
    },
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "versionNumber": "Version Number value",
    "buildNumber": "Build Number value",
    "identityVersion": "Identity Version value"
  }
}
```




