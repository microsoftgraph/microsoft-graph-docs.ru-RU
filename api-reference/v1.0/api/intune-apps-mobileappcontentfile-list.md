---
title: Перечисление объектов mobileAppContentFile
description: Список свойств и связей объектов mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 76c985ba272231ed7ba68d93b310bfddb3fde7b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016022"
---
# <a name="list-mobileappcontentfiles"></a><span data-ttu-id="67ee7-103">Перечисление объектов mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="67ee7-103">List mobileAppContentFiles</span></span>

> <span data-ttu-id="67ee7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="67ee7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67ee7-105">Список свойств и связей объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="67ee7-105">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67ee7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="67ee7-106">Prerequisites</span></span>
<span data-ttu-id="67ee7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67ee7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67ee7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67ee7-109">Permission type</span></span>|<span data-ttu-id="67ee7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="67ee7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67ee7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67ee7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="67ee7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="67ee7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="67ee7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67ee7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67ee7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67ee7-114">Not supported.</span></span>|
|<span data-ttu-id="67ee7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67ee7-115">Application</span></span>|<span data-ttu-id="67ee7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67ee7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67ee7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67ee7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="67ee7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67ee7-118">Request headers</span></span>
|<span data-ttu-id="67ee7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="67ee7-119">Header</span></span>|<span data-ttu-id="67ee7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="67ee7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67ee7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67ee7-121">Authorization</span></span>|<span data-ttu-id="67ee7-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67ee7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67ee7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="67ee7-123">Accept</span></span>|<span data-ttu-id="67ee7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="67ee7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67ee7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="67ee7-125">Request body</span></span>
<span data-ttu-id="67ee7-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="67ee7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67ee7-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="67ee7-127">Response</span></span>
<span data-ttu-id="67ee7-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="67ee7-128">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67ee7-129">Пример</span><span class="sxs-lookup"><span data-stu-id="67ee7-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="67ee7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="67ee7-130">Request</span></span>
<span data-ttu-id="67ee7-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67ee7-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

### <a name="response"></a><span data-ttu-id="67ee7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="67ee7-132">Response</span></span>
<span data-ttu-id="67ee7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67ee7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



