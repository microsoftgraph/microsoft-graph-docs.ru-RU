---
title: Get managedIOSStoreApp
description: Чтение свойств и связей объекта managedIOSStoreApp.
author: tfitzmac
ms.openlocfilehash: cebe7a431b7b41f3f1cb05e4464e932118322516
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351543"
---
# <a name="get-managediosstoreapp"></a><span data-ttu-id="c2e62-103">Get managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="c2e62-103">Get managedIOSStoreApp</span></span>

> <span data-ttu-id="c2e62-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c2e62-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2e62-105">Чтение свойств и связей объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2e62-105">Read properties and relationships of the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2e62-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c2e62-106">Prerequisites</span></span>
<span data-ttu-id="c2e62-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2e62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2e62-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2e62-109">Permission type</span></span>|<span data-ttu-id="c2e62-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2e62-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2e62-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2e62-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c2e62-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2e62-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c2e62-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2e62-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2e62-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2e62-114">Not supported.</span></span>|
|<span data-ttu-id="c2e62-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2e62-115">Application</span></span>|<span data-ttu-id="c2e62-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2e62-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2e62-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2e62-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2e62-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2e62-118">Optional query parameters</span></span>
<span data-ttu-id="c2e62-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c2e62-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c2e62-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2e62-120">Request headers</span></span>
|<span data-ttu-id="c2e62-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2e62-121">Header</span></span>|<span data-ttu-id="c2e62-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2e62-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2e62-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2e62-123">Authorization</span></span>|<span data-ttu-id="c2e62-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c2e62-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2e62-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2e62-125">Accept</span></span>|<span data-ttu-id="c2e62-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2e62-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2e62-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2e62-127">Request body</span></span>
<span data-ttu-id="c2e62-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2e62-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2e62-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2e62-129">Response</span></span>
<span data-ttu-id="c2e62-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c2e62-130">If successful, this method returns a `200 OK` response code and [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2e62-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c2e62-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2e62-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2e62-132">Request</span></span>
<span data-ttu-id="c2e62-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2e62-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="c2e62-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2e62-134">Response</span></span>
<span data-ttu-id="c2e62-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c2e62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1347

{
  "value": {
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
}
```



