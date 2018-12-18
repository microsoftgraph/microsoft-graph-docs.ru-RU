---
title: Get mobileAppContentFile
description: Чтение свойств и связей объекта mobileAppContentFile.
author: tfitzmac
ms.openlocfilehash: 0494b834c6817c08eac750859138f673a793d02a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301094"
---
# <a name="get-mobileappcontentfile"></a><span data-ttu-id="f135b-103">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="f135b-103">Get mobileAppContentFile</span></span>

> <span data-ttu-id="f135b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f135b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f135b-105">Чтение свойств и связей объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="f135b-105">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f135b-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f135b-106">Prerequisites</span></span>
<span data-ttu-id="f135b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f135b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f135b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f135b-109">Permission type</span></span>|<span data-ttu-id="f135b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f135b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f135b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f135b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f135b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f135b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f135b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f135b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f135b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f135b-114">Not supported.</span></span>|
|<span data-ttu-id="f135b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f135b-115">Application</span></span>|<span data-ttu-id="f135b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f135b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f135b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f135b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f135b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f135b-118">Optional query parameters</span></span>
<span data-ttu-id="f135b-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f135b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f135b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f135b-120">Request headers</span></span>
|<span data-ttu-id="f135b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f135b-121">Header</span></span>|<span data-ttu-id="f135b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f135b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f135b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f135b-123">Authorization</span></span>|<span data-ttu-id="f135b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f135b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f135b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f135b-125">Accept</span></span>|<span data-ttu-id="f135b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f135b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f135b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f135b-127">Request body</span></span>
<span data-ttu-id="f135b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f135b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f135b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f135b-129">Response</span></span>
<span data-ttu-id="f135b-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f135b-130">If successful, this method returns a `200 OK` response code and [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f135b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f135b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f135b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f135b-132">Request</span></span>
<span data-ttu-id="f135b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f135b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

### <a name="response"></a><span data-ttu-id="f135b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f135b-134">Response</span></span>
<span data-ttu-id="f135b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f135b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 491

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppContentFile",
    "azureStorageUri": "Azure Storage Uri value",
    "isCommitted": true,
    "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "name": "Name value",
    "size": 4,
    "sizeEncrypted": 13,
    "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
    "manifest": "bWFuaWZlc3Q=",
    "uploadState": "transientError"
  }
}
```



