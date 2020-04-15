---
title: Перечисление объектов managedIOSStoreApp
description: Список свойств и связей объектов managedIOSStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2eef6884d580afc1b501e5b5b2ccd9e1609427a4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442508"
---
# <a name="list-managediosstoreapps"></a><span data-ttu-id="0daa8-103">Перечисление объектов managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="0daa8-103">List managedIOSStoreApps</span></span>

<span data-ttu-id="0daa8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0daa8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0daa8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0daa8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0daa8-106">Список свойств и связей объектов [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="0daa8-106">List properties and relationships of the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0daa8-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0daa8-107">Prerequisites</span></span>
<span data-ttu-id="0daa8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0daa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0daa8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0daa8-110">Permission type</span></span>|<span data-ttu-id="0daa8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0daa8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0daa8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0daa8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0daa8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0daa8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0daa8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0daa8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0daa8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0daa8-115">Not supported.</span></span>|
|<span data-ttu-id="0daa8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0daa8-116">Application</span></span>|<span data-ttu-id="0daa8-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0daa8-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0daa8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0daa8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0daa8-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0daa8-119">Request headers</span></span>
|<span data-ttu-id="0daa8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0daa8-120">Header</span></span>|<span data-ttu-id="0daa8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0daa8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0daa8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0daa8-122">Authorization</span></span>|<span data-ttu-id="0daa8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0daa8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0daa8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0daa8-124">Accept</span></span>|<span data-ttu-id="0daa8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0daa8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0daa8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0daa8-126">Request body</span></span>
<span data-ttu-id="0daa8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0daa8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0daa8-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0daa8-128">Response</span></span>
<span data-ttu-id="0daa8-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0daa8-129">If successful, this method returns a `200 OK` response code and a collection of [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0daa8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0daa8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0daa8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0daa8-131">Request</span></span>
<span data-ttu-id="0daa8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0daa8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="0daa8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0daa8-133">Response</span></span>
<span data-ttu-id="0daa8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0daa8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1457

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedIOSStoreApp",
      "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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






