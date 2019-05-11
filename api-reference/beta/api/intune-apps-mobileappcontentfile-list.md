---
title: Перечисление объектов mobileAppContentFile
description: Список свойств и связей объектов mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b9116a0eafd6cb8dca6268a2c09e3707838e833
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935169"
---
# <a name="list-mobileappcontentfiles"></a><span data-ttu-id="d0765-103">Перечисление объектов mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d0765-103">List mobileAppContentFiles</span></span>

> <span data-ttu-id="d0765-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0765-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0765-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0765-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0765-106">Список свойств и связей объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="d0765-106">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0765-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d0765-107">Prerequisites</span></span>
<span data-ttu-id="d0765-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0765-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0765-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0765-110">Permission type</span></span>|<span data-ttu-id="d0765-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0765-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0765-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0765-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0765-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0765-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d0765-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0765-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0765-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0765-115">Not supported.</span></span>|
|<span data-ttu-id="d0765-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0765-116">Application</span></span>|<span data-ttu-id="d0765-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0765-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0765-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0765-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="d0765-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0765-119">Request headers</span></span>
|<span data-ttu-id="d0765-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0765-120">Header</span></span>|<span data-ttu-id="d0765-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d0765-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0765-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0765-122">Authorization</span></span>|<span data-ttu-id="d0765-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0765-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0765-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d0765-124">Accept</span></span>|<span data-ttu-id="d0765-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0765-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0765-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d0765-126">Request body</span></span>
<span data-ttu-id="d0765-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d0765-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0765-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0765-128">Response</span></span>
<span data-ttu-id="d0765-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d0765-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0765-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d0765-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0765-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0765-131">Request</span></span>
<span data-ttu-id="d0765-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0765-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

### <a name="response"></a><span data-ttu-id="d0765-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0765-133">Response</span></span>
<span data-ttu-id="d0765-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0765-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 588

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
      "uploadState": "transientError",
      "isFrameworkFile": true,
      "isDependency": true
    }
  ]
}
```




