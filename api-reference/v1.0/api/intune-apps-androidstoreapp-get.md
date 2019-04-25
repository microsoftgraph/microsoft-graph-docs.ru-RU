---
title: Get androidStoreApp
description: Чтение свойств и связей объекта androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d508c75ebce8184ab993a5473fe43ccff5b9ae7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577492"
---
# <a name="get-androidstoreapp"></a><span data-ttu-id="87371-103">Get androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="87371-103">Get androidStoreApp</span></span>

> <span data-ttu-id="87371-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87371-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87371-105">Чтение свойств и связей объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="87371-105">Read properties and relationships of the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87371-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="87371-106">Prerequisites</span></span>
<span data-ttu-id="87371-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87371-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87371-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87371-109">Permission type</span></span>|<span data-ttu-id="87371-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87371-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87371-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87371-111">Delegated (work or school account)</span></span>|<span data-ttu-id="87371-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="87371-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="87371-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87371-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87371-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87371-114">Not supported.</span></span>|
|<span data-ttu-id="87371-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87371-115">Application</span></span>|<span data-ttu-id="87371-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87371-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87371-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87371-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87371-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="87371-118">Optional query parameters</span></span>
<span data-ttu-id="87371-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="87371-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87371-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87371-120">Request headers</span></span>
|<span data-ttu-id="87371-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87371-121">Header</span></span>|<span data-ttu-id="87371-122">Значение</span><span class="sxs-lookup"><span data-stu-id="87371-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87371-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87371-123">Authorization</span></span>|<span data-ttu-id="87371-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87371-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87371-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87371-125">Accept</span></span>|<span data-ttu-id="87371-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87371-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87371-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87371-127">Request body</span></span>
<span data-ttu-id="87371-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87371-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87371-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="87371-129">Response</span></span>
<span data-ttu-id="87371-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="87371-130">If successful, this method returns a `200 OK` response code and [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87371-131">Пример</span><span class="sxs-lookup"><span data-stu-id="87371-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="87371-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="87371-132">Request</span></span>
<span data-ttu-id="87371-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87371-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="87371-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="87371-134">Response</span></span>
<span data-ttu-id="87371-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="87371-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1193

{
  "value": {
    "@odata.type": "#microsoft.graph.androidStoreApp",
    "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
    "packageId": "Package Id value",
    "appStoreUrl": "https://example.com/appStoreUrl/",
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
    }
  }
}
```



