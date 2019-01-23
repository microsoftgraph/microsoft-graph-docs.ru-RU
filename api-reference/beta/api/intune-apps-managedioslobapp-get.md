---
title: Get managedIOSLobApp
description: Чтение свойств и связей объекта managedIOSLobApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 557caa7ca87a415dd5da6959883818321d19b6a0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424135"
---
# <a name="get-managedioslobapp"></a><span data-ttu-id="b9909-103">Get managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="b9909-103">Get managedIOSLobApp</span></span>

> <span data-ttu-id="b9909-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9909-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b9909-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9909-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9909-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9909-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9909-107">Чтение свойств и связей объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9909-107">Read properties and relationships of the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9909-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b9909-108">Prerequisites</span></span>
<span data-ttu-id="b9909-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b9909-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b9909-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9909-111">Permission type</span></span>|<span data-ttu-id="b9909-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9909-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9909-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9909-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9909-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9909-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b9909-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9909-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9909-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9909-116">Not supported.</span></span>|
|<span data-ttu-id="b9909-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9909-117">Application</span></span>|<span data-ttu-id="b9909-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9909-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9909-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9909-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9909-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b9909-120">Optional query parameters</span></span>
<span data-ttu-id="b9909-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b9909-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9909-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9909-122">Request headers</span></span>
|<span data-ttu-id="b9909-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9909-123">Header</span></span>|<span data-ttu-id="b9909-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b9909-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9909-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9909-125">Authorization</span></span>|<span data-ttu-id="b9909-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b9909-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9909-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b9909-127">Accept</span></span>|<span data-ttu-id="b9909-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b9909-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9909-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9909-129">Request body</span></span>
<span data-ttu-id="b9909-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9909-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9909-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9909-131">Response</span></span>
<span data-ttu-id="b9909-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b9909-132">If successful, this method returns a `200 OK` response code and [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9909-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b9909-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9909-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9909-134">Request</span></span>
<span data-ttu-id="b9909-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9909-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="b9909-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9909-136">Response</span></span>
<span data-ttu-id="b9909-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b9909-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1727

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




