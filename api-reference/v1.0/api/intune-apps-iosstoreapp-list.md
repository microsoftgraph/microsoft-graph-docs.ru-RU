---
title: Перечисление объектов iosStoreApp
description: Список свойств и связей объектов iosStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c25a1a46864dc1e605a9c7f7624d8b3f9fd70be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070137"
---
# <a name="list-iosstoreapps"></a><span data-ttu-id="bf6d5-103">Перечисление объектов iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="bf6d5-103">List iosStoreApps</span></span>

<span data-ttu-id="bf6d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf6d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf6d5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf6d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf6d5-106">Список свойств и связей объектов [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="bf6d5-106">List properties and relationships of the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf6d5-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bf6d5-107">Prerequisites</span></span>
<span data-ttu-id="bf6d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bf6d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bf6d5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf6d5-110">Permission type</span></span>|<span data-ttu-id="bf6d5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf6d5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf6d5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf6d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf6d5-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf6d5-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bf6d5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf6d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf6d5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf6d5-115">Not supported.</span></span>|
|<span data-ttu-id="bf6d5-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="bf6d5-116">Application</span></span>|<span data-ttu-id="bf6d5-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf6d5-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf6d5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf6d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bf6d5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bf6d5-119">Request headers</span></span>
|<span data-ttu-id="bf6d5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf6d5-120">Header</span></span>|<span data-ttu-id="bf6d5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bf6d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf6d5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf6d5-122">Authorization</span></span>|<span data-ttu-id="bf6d5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf6d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf6d5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bf6d5-124">Accept</span></span>|<span data-ttu-id="bf6d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf6d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf6d5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf6d5-126">Request body</span></span>
<span data-ttu-id="bf6d5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf6d5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf6d5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf6d5-128">Response</span></span>
<span data-ttu-id="bf6d5-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bf6d5-129">If successful, this method returns a `200 OK` response code and a collection of [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf6d5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bf6d5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf6d5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf6d5-131">Request</span></span>
<span data-ttu-id="bf6d5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf6d5-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="bf6d5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf6d5-133">Response</span></span>
<span data-ttu-id="bf6d5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf6d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1371

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosStoreApp",
      "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
      "bundleId": "Bundle Id value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
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
      }
    }
  ]
}
```









