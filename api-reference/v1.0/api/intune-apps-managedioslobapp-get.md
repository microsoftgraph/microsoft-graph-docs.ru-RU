---
title: Get managedIOSLobApp
description: Чтение свойств и связей объекта managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f1cbf7f0989e1bc1c9058d7a84cee84c88c6d7a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025845"
---
# <a name="get-managedioslobapp"></a><span data-ttu-id="0f4ac-103">Get managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="0f4ac-103">Get managedIOSLobApp</span></span>

<span data-ttu-id="0f4ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f4ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f4ac-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f4ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f4ac-106">Чтение свойств и связей объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f4ac-106">Read properties and relationships of the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f4ac-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0f4ac-107">Prerequisites</span></span>
<span data-ttu-id="0f4ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0f4ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0f4ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f4ac-110">Permission type</span></span>|<span data-ttu-id="0f4ac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f4ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f4ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f4ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f4ac-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f4ac-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0f4ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f4ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f4ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f4ac-115">Not supported.</span></span>|
|<span data-ttu-id="0f4ac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f4ac-116">Application</span></span>|<span data-ttu-id="0f4ac-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f4ac-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f4ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f4ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0f4ac-119">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="0f4ac-119">Optional query parameters</span></span>
<span data-ttu-id="0f4ac-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0f4ac-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f4ac-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f4ac-121">Request headers</span></span>
|<span data-ttu-id="0f4ac-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f4ac-122">Header</span></span>|<span data-ttu-id="0f4ac-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0f4ac-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f4ac-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f4ac-124">Authorization</span></span>|<span data-ttu-id="0f4ac-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f4ac-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f4ac-126">Accept</span><span class="sxs-lookup"><span data-stu-id="0f4ac-126">Accept</span></span>|<span data-ttu-id="0f4ac-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0f4ac-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f4ac-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0f4ac-128">Request body</span></span>
<span data-ttu-id="0f4ac-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f4ac-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f4ac-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f4ac-130">Response</span></span>
<span data-ttu-id="0f4ac-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0f4ac-131">If successful, this method returns a `200 OK` response code and [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f4ac-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0f4ac-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f4ac-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f4ac-133">Request</span></span>
<span data-ttu-id="0f4ac-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f4ac-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="0f4ac-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f4ac-135">Response</span></span>
<span data-ttu-id="0f4ac-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f4ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1582

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
    "publishingState": "processing",
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
      "v13_0": true
    },
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "versionNumber": "Version Number value",
    "buildNumber": "Build Number value"
  }
}
```









