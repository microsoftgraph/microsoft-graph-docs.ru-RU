---
title: Get mobileApp
description: Чтение свойств и связей объекта mobileApp.
author: tfitzmac
ms.openlocfilehash: 65ed02218e28b64d3749834d4eee5d57a05e8d74
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323578"
---
# <a name="get-mobileapp"></a><span data-ttu-id="85144-103">Get mobileApp</span><span class="sxs-lookup"><span data-stu-id="85144-103">Get mobileApp</span></span>

> <span data-ttu-id="85144-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="85144-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85144-105">Чтение свойств и связей объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85144-105">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85144-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="85144-106">Prerequisites</span></span>
<span data-ttu-id="85144-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85144-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85144-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85144-109">Permission type</span></span>|<span data-ttu-id="85144-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85144-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85144-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85144-111">Delegated (work or school account)</span></span>|<span data-ttu-id="85144-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="85144-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="85144-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85144-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85144-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85144-114">Not supported.</span></span>|
|<span data-ttu-id="85144-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85144-115">Application</span></span>|<span data-ttu-id="85144-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85144-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85144-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85144-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="85144-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="85144-118">Optional query parameters</span></span>
<span data-ttu-id="85144-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="85144-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="85144-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85144-120">Request headers</span></span>
|<span data-ttu-id="85144-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85144-121">Header</span></span>|<span data-ttu-id="85144-122">Значение</span><span class="sxs-lookup"><span data-stu-id="85144-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85144-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85144-123">Authorization</span></span>|<span data-ttu-id="85144-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="85144-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85144-125">Accept</span><span class="sxs-lookup"><span data-stu-id="85144-125">Accept</span></span>|<span data-ttu-id="85144-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85144-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85144-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85144-127">Request body</span></span>
<span data-ttu-id="85144-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85144-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85144-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="85144-129">Response</span></span>
<span data-ttu-id="85144-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileApp](../resources/intune-apps-mobileapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="85144-130">If successful, this method returns a `200 OK` response code and [mobileApp](../resources/intune-apps-mobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85144-131">Пример</span><span class="sxs-lookup"><span data-stu-id="85144-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="85144-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="85144-132">Request</span></span>
<span data-ttu-id="85144-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85144-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="85144-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="85144-134">Response</span></span>
<span data-ttu-id="85144-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="85144-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 803

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileApp",
    "id": "0177548a-548a-0177-8a54-77018a547701",
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
    "publishingState": "processing"
  }
}
```



