---
title: Get managedIOSLobApp
description: Чтение свойств и связей объекта managedIOSLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca17d00e65092aae61a2def6568b7d2f32439476
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974596"
---
# <a name="get-managedioslobapp"></a><span data-ttu-id="fb9da-103">Get managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="fb9da-103">Get managedIOSLobApp</span></span>

> <span data-ttu-id="fb9da-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb9da-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb9da-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb9da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb9da-106">Чтение свойств и связей объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb9da-106">Read properties and relationships of the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb9da-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fb9da-107">Prerequisites</span></span>
<span data-ttu-id="fb9da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb9da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb9da-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb9da-110">Permission type</span></span>|<span data-ttu-id="fb9da-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb9da-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb9da-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb9da-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fb9da-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb9da-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fb9da-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb9da-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb9da-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb9da-115">Not supported.</span></span>|
|<span data-ttu-id="fb9da-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb9da-116">Application</span></span>|<span data-ttu-id="fb9da-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb9da-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb9da-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb9da-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb9da-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fb9da-119">Optional query parameters</span></span>
<span data-ttu-id="fb9da-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fb9da-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb9da-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb9da-121">Request headers</span></span>
|<span data-ttu-id="fb9da-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb9da-122">Header</span></span>|<span data-ttu-id="fb9da-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fb9da-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb9da-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb9da-124">Authorization</span></span>|<span data-ttu-id="fb9da-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb9da-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb9da-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fb9da-126">Accept</span></span>|<span data-ttu-id="fb9da-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fb9da-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb9da-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fb9da-128">Request body</span></span>
<span data-ttu-id="fb9da-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb9da-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb9da-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb9da-130">Response</span></span>
<span data-ttu-id="fb9da-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fb9da-131">If successful, this method returns a `200 OK` response code and [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb9da-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fb9da-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb9da-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb9da-133">Request</span></span>
<span data-ttu-id="fb9da-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb9da-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="fb9da-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb9da-135">Response</span></span>
<span data-ttu-id="fb9da-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb9da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1756

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
      "v12_0": true
    },
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "versionNumber": "Version Number value",
    "buildNumber": "Build Number value",
    "identityVersion": "Identity Version value"
  }
}
```





