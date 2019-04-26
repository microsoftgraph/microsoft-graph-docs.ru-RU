---
title: Перечисление объектов mobileAppContentFile
description: Список свойств и связей объектов mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a02a97afe42bb7e2816bd093ac73f70496d7e4b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554795"
---
# <a name="list-mobileappcontentfiles"></a><span data-ttu-id="c2b46-103">Перечисление объектов mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="c2b46-103">List mobileAppContentFiles</span></span>

> <span data-ttu-id="c2b46-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2b46-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2b46-105">Список свойств и связей объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="c2b46-105">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2b46-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c2b46-106">Prerequisites</span></span>
<span data-ttu-id="c2b46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2b46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2b46-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2b46-109">Permission type</span></span>|<span data-ttu-id="c2b46-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2b46-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2b46-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2b46-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c2b46-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b46-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c2b46-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2b46-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2b46-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2b46-114">Not supported.</span></span>|
|<span data-ttu-id="c2b46-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2b46-115">Application</span></span>|<span data-ttu-id="c2b46-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2b46-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2b46-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2b46-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="c2b46-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2b46-118">Request headers</span></span>
|<span data-ttu-id="c2b46-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2b46-119">Header</span></span>|<span data-ttu-id="c2b46-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c2b46-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2b46-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2b46-121">Authorization</span></span>|<span data-ttu-id="c2b46-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2b46-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2b46-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c2b46-123">Accept</span></span>|<span data-ttu-id="c2b46-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c2b46-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2b46-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2b46-125">Request body</span></span>
<span data-ttu-id="c2b46-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2b46-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2b46-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2b46-127">Response</span></span>
<span data-ttu-id="c2b46-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2b46-128">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2b46-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c2b46-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2b46-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2b46-130">Request</span></span>
<span data-ttu-id="c2b46-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2b46-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

### <a name="response"></a><span data-ttu-id="c2b46-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2b46-132">Response</span></span>
<span data-ttu-id="c2b46-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2b46-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



