---
title: Get mobileAppContentFile
description: Чтение свойств и связей объекта mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 44ad144cc6646eb26be035db1d309adfed92410f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139792"
---
# <a name="get-mobileappcontentfile"></a><span data-ttu-id="c31df-103">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="c31df-103">Get mobileAppContentFile</span></span>

<span data-ttu-id="c31df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c31df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c31df-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c31df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c31df-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c31df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c31df-107">Чтение свойств и связей объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="c31df-107">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c31df-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c31df-108">Prerequisites</span></span>
<span data-ttu-id="c31df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c31df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c31df-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c31df-111">Permission type</span></span>|<span data-ttu-id="c31df-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c31df-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c31df-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c31df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c31df-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c31df-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c31df-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c31df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c31df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c31df-116">Not supported.</span></span>|
|<span data-ttu-id="c31df-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c31df-117">Application</span></span>|<span data-ttu-id="c31df-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c31df-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c31df-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c31df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c31df-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c31df-120">Optional query parameters</span></span>
<span data-ttu-id="c31df-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c31df-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c31df-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c31df-122">Request headers</span></span>
|<span data-ttu-id="c31df-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c31df-123">Header</span></span>|<span data-ttu-id="c31df-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c31df-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c31df-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c31df-125">Authorization</span></span>|<span data-ttu-id="c31df-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c31df-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c31df-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c31df-127">Accept</span></span>|<span data-ttu-id="c31df-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c31df-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c31df-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c31df-129">Request body</span></span>
<span data-ttu-id="c31df-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c31df-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c31df-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c31df-131">Response</span></span>
<span data-ttu-id="c31df-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c31df-132">If successful, this method returns a `200 OK` response code and [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c31df-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c31df-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c31df-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c31df-134">Request</span></span>
<span data-ttu-id="c31df-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c31df-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

### <a name="response"></a><span data-ttu-id="c31df-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c31df-136">Response</span></span>
<span data-ttu-id="c31df-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c31df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




