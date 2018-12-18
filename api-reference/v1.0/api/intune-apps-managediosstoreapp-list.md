---
title: Перечисление объектов managedIOSStoreApp
description: Список свойств и связей объектов managedIOSStoreApp.
author: tfitzmac
ms.openlocfilehash: c5d8f0153f7c28f92578b92fbd0f4b0aac0ff885
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324115"
---
# <a name="list-managediosstoreapps"></a><span data-ttu-id="decf3-103">Перечисление объектов managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="decf3-103">List managedIOSStoreApps</span></span>

> <span data-ttu-id="decf3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="decf3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="decf3-105">Список свойств и связей объектов [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="decf3-105">List properties and relationships of the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="decf3-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="decf3-106">Prerequisites</span></span>
<span data-ttu-id="decf3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="decf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="decf3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="decf3-109">Permission type</span></span>|<span data-ttu-id="decf3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="decf3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="decf3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="decf3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="decf3-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="decf3-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="decf3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="decf3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="decf3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="decf3-114">Not supported.</span></span>|
|<span data-ttu-id="decf3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="decf3-115">Application</span></span>|<span data-ttu-id="decf3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="decf3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="decf3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="decf3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="decf3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="decf3-118">Request headers</span></span>
|<span data-ttu-id="decf3-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="decf3-119">Header</span></span>|<span data-ttu-id="decf3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="decf3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="decf3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="decf3-121">Authorization</span></span>|<span data-ttu-id="decf3-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="decf3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="decf3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="decf3-123">Accept</span></span>|<span data-ttu-id="decf3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="decf3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="decf3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="decf3-125">Request body</span></span>
<span data-ttu-id="decf3-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="decf3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="decf3-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="decf3-127">Response</span></span>
<span data-ttu-id="decf3-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="decf3-128">If successful, this method returns a `200 OK` response code and a collection of [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="decf3-129">Пример</span><span class="sxs-lookup"><span data-stu-id="decf3-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="decf3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="decf3-130">Request</span></span>
<span data-ttu-id="decf3-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="decf3-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="decf3-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="decf3-132">Response</span></span>
<span data-ttu-id="decf3-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="decf3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1433

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
        "v12_0": true
      }
    }
  ]
}
```



