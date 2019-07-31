---
title: Get mobileAppContentFile
description: Чтение свойств и связей объекта mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 16f6c51b41851022e1bd038ec29672da5fdc9e69
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960841"
---
# <a name="get-mobileappcontentfile"></a><span data-ttu-id="2a123-103">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="2a123-103">Get mobileAppContentFile</span></span>

> <span data-ttu-id="2a123-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a123-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a123-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a123-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a123-106">Чтение свойств и связей объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="2a123-106">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a123-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2a123-107">Prerequisites</span></span>
<span data-ttu-id="2a123-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a123-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a123-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a123-110">Permission type</span></span>|<span data-ttu-id="2a123-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a123-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a123-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a123-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a123-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a123-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2a123-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a123-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a123-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a123-115">Not supported.</span></span>|
|<span data-ttu-id="2a123-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a123-116">Application</span></span>|<span data-ttu-id="2a123-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a123-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a123-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a123-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a123-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2a123-119">Optional query parameters</span></span>
<span data-ttu-id="2a123-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2a123-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a123-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a123-121">Request headers</span></span>
|<span data-ttu-id="2a123-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a123-122">Header</span></span>|<span data-ttu-id="2a123-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2a123-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a123-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a123-124">Authorization</span></span>|<span data-ttu-id="2a123-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a123-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a123-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2a123-126">Accept</span></span>|<span data-ttu-id="2a123-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2a123-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a123-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a123-128">Request body</span></span>
<span data-ttu-id="2a123-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a123-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a123-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a123-130">Response</span></span>
<span data-ttu-id="2a123-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2a123-131">If successful, this method returns a `200 OK` response code and [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a123-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2a123-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a123-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a123-133">Request</span></span>
<span data-ttu-id="2a123-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a123-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

### <a name="response"></a><span data-ttu-id="2a123-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a123-135">Response</span></span>
<span data-ttu-id="2a123-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a123-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 548

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
    "uploadState": "transientError",
    "isFrameworkFile": true,
    "isDependency": true
  }
}
```





