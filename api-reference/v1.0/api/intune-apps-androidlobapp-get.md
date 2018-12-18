---
title: Get androidLobApp
description: Чтение свойств и связей объекта androidLobApp.
author: tfitzmac
ms.openlocfilehash: 16773d162232e01296c7859acd626a6ff281027b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331964"
---
# <a name="get-androidlobapp"></a><span data-ttu-id="53708-103">Get androidLobApp</span><span class="sxs-lookup"><span data-stu-id="53708-103">Get androidLobApp</span></span>

> <span data-ttu-id="53708-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="53708-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53708-105">Чтение свойств и связей объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="53708-105">Read properties and relationships of the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53708-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="53708-106">Prerequisites</span></span>
<span data-ttu-id="53708-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53708-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53708-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53708-109">Permission type</span></span>|<span data-ttu-id="53708-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53708-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53708-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53708-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53708-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="53708-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="53708-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53708-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53708-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53708-114">Not supported.</span></span>|
|<span data-ttu-id="53708-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53708-115">Application</span></span>|<span data-ttu-id="53708-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53708-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53708-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53708-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53708-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="53708-118">Optional query parameters</span></span>
<span data-ttu-id="53708-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="53708-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="53708-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53708-120">Request headers</span></span>
|<span data-ttu-id="53708-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53708-121">Header</span></span>|<span data-ttu-id="53708-122">Значение</span><span class="sxs-lookup"><span data-stu-id="53708-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53708-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53708-123">Authorization</span></span>|<span data-ttu-id="53708-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="53708-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53708-125">Accept</span><span class="sxs-lookup"><span data-stu-id="53708-125">Accept</span></span>|<span data-ttu-id="53708-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53708-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53708-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53708-127">Request body</span></span>
<span data-ttu-id="53708-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53708-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53708-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="53708-129">Response</span></span>
<span data-ttu-id="53708-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidLobApp](../resources/intune-apps-androidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="53708-130">If successful, this method returns a `200 OK` response code and [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53708-131">Пример</span><span class="sxs-lookup"><span data-stu-id="53708-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="53708-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="53708-132">Request</span></span>
<span data-ttu-id="53708-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53708-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="53708-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="53708-134">Response</span></span>
<span data-ttu-id="53708-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="53708-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1338

{
  "value": {
    "@odata.type": "#microsoft.graph.androidLobApp",
    "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "packageId": "Package Id value",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
      "v4_0": true,
      "v4_0_3": true,
      "v4_1": true,
      "v4_2": true,
      "v4_3": true,
      "v4_4": true,
      "v5_0": true,
      "v5_1": true
    },
    "versionName": "Version Name value",
    "versionCode": "Version Code value"
  }
}
```



