---
title: Get mobileAppContentFile
description: Чтение свойств и связей объекта mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9ecbdfac8335e777c4c104f732e378ebf2d07f17
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932142"
---
# <a name="get-mobileappcontentfile"></a><span data-ttu-id="6f3ca-103">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="6f3ca-103">Get mobileAppContentFile</span></span>

> <span data-ttu-id="6f3ca-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f3ca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f3ca-105">Чтение свойств и связей объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="6f3ca-105">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f3ca-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6f3ca-106">Prerequisites</span></span>
<span data-ttu-id="6f3ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f3ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f3ca-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f3ca-109">Permission type</span></span>|<span data-ttu-id="6f3ca-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f3ca-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f3ca-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f3ca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6f3ca-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f3ca-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6f3ca-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f3ca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f3ca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f3ca-114">Not supported.</span></span>|
|<span data-ttu-id="6f3ca-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f3ca-115">Application</span></span>|<span data-ttu-id="6f3ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f3ca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f3ca-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f3ca-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f3ca-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6f3ca-118">Optional query parameters</span></span>
<span data-ttu-id="6f3ca-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6f3ca-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6f3ca-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f3ca-120">Request headers</span></span>
|<span data-ttu-id="6f3ca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f3ca-121">Header</span></span>|<span data-ttu-id="6f3ca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6f3ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f3ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f3ca-123">Authorization</span></span>|<span data-ttu-id="6f3ca-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6f3ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f3ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f3ca-125">Accept</span></span>|<span data-ttu-id="6f3ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f3ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f3ca-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f3ca-127">Request body</span></span>
<span data-ttu-id="6f3ca-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f3ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f3ca-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f3ca-129">Response</span></span>
<span data-ttu-id="6f3ca-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6f3ca-130">If successful, this method returns a `200 OK` response code and [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f3ca-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6f3ca-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f3ca-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f3ca-132">Request</span></span>
<span data-ttu-id="6f3ca-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f3ca-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

### <a name="response"></a><span data-ttu-id="6f3ca-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f3ca-134">Response</span></span>
<span data-ttu-id="6f3ca-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6f3ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



