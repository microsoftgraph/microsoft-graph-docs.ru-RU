---
title: Перечисление объектов mobileAppContentFile
description: Список свойств и связей объектов mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: be0c1fef3792bb3787127f16385273e880e984ee
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754058"
---
# <a name="list-mobileappcontentfiles"></a><span data-ttu-id="64b11-103">Перечисление объектов mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="64b11-103">List mobileAppContentFiles</span></span>

<span data-ttu-id="64b11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64b11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64b11-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64b11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64b11-106">Список свойств и связей объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="64b11-106">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64b11-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="64b11-107">Prerequisites</span></span>
<span data-ttu-id="64b11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64b11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64b11-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64b11-110">Permission type</span></span>|<span data-ttu-id="64b11-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64b11-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64b11-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64b11-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64b11-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64b11-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="64b11-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64b11-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64b11-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64b11-115">Not supported.</span></span>|
|<span data-ttu-id="64b11-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="64b11-116">Application</span></span>|<span data-ttu-id="64b11-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64b11-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64b11-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64b11-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="64b11-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="64b11-119">Request headers</span></span>
|<span data-ttu-id="64b11-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64b11-120">Header</span></span>|<span data-ttu-id="64b11-121">Значение</span><span class="sxs-lookup"><span data-stu-id="64b11-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64b11-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="64b11-122">Authorization</span></span>|<span data-ttu-id="64b11-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64b11-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64b11-124">Accept</span><span class="sxs-lookup"><span data-stu-id="64b11-124">Accept</span></span>|<span data-ttu-id="64b11-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64b11-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64b11-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64b11-126">Request body</span></span>
<span data-ttu-id="64b11-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64b11-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64b11-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="64b11-128">Response</span></span>
<span data-ttu-id="64b11-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64b11-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64b11-130">Пример</span><span class="sxs-lookup"><span data-stu-id="64b11-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="64b11-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="64b11-131">Request</span></span>
<span data-ttu-id="64b11-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64b11-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

### <a name="response"></a><span data-ttu-id="64b11-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="64b11-133">Response</span></span>
<span data-ttu-id="64b11-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64b11-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 527

{
  "value": [
    {
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
  ]
}
```




