---
title: Перечисление объектов mobileAppContentFile
description: Список свойств и связей объектов mobileAppContentFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d69d131ac34d6518c4bc81a13b3d11d86b4bdaf8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515913"
---
# <a name="list-mobileappcontentfiles"></a><span data-ttu-id="bf4ad-103">Перечисление объектов mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="bf4ad-103">List mobileAppContentFiles</span></span>

<span data-ttu-id="bf4ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf4ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf4ad-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf4ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf4ad-106">Список свойств и связей объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="bf4ad-106">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf4ad-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bf4ad-107">Prerequisites</span></span>
<span data-ttu-id="bf4ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf4ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf4ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf4ad-110">Permission type</span></span>|<span data-ttu-id="bf4ad-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf4ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf4ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf4ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf4ad-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf4ad-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bf4ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf4ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf4ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf4ad-115">Not supported.</span></span>|
|<span data-ttu-id="bf4ad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf4ad-116">Application</span></span>|<span data-ttu-id="bf4ad-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf4ad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf4ad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf4ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="bf4ad-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bf4ad-119">Request headers</span></span>
|<span data-ttu-id="bf4ad-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf4ad-120">Header</span></span>|<span data-ttu-id="bf4ad-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bf4ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf4ad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf4ad-122">Authorization</span></span>|<span data-ttu-id="bf4ad-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf4ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf4ad-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bf4ad-124">Accept</span></span>|<span data-ttu-id="bf4ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf4ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf4ad-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf4ad-126">Request body</span></span>
<span data-ttu-id="bf4ad-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf4ad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf4ad-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf4ad-128">Response</span></span>
<span data-ttu-id="bf4ad-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bf4ad-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf4ad-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bf4ad-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf4ad-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf4ad-131">Request</span></span>
<span data-ttu-id="bf4ad-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf4ad-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

### <a name="response"></a><span data-ttu-id="bf4ad-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf4ad-133">Response</span></span>
<span data-ttu-id="bf4ad-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf4ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




