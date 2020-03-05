---
title: Перечисление объектов mobileAppContentFile
description: Список свойств и связей объектов mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73e8d6a69219bb483d467def5a42d29252ffd586
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450743"
---
# <a name="list-mobileappcontentfiles"></a><span data-ttu-id="cf2fc-103">Перечисление объектов mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cf2fc-103">List mobileAppContentFiles</span></span>

<span data-ttu-id="cf2fc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cf2fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf2fc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf2fc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf2fc-107">Список свойств и связей объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="cf2fc-107">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf2fc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cf2fc-108">Prerequisites</span></span>
<span data-ttu-id="cf2fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf2fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf2fc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf2fc-111">Permission type</span></span>|<span data-ttu-id="cf2fc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf2fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf2fc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf2fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf2fc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf2fc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cf2fc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf2fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf2fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-116">Not supported.</span></span>|
|<span data-ttu-id="cf2fc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf2fc-117">Application</span></span>|<span data-ttu-id="cf2fc-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf2fc-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf2fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf2fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="cf2fc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cf2fc-120">Request headers</span></span>
|<span data-ttu-id="cf2fc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf2fc-121">Header</span></span>|<span data-ttu-id="cf2fc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cf2fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf2fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf2fc-123">Authorization</span></span>|<span data-ttu-id="cf2fc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf2fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf2fc-125">Accept</span></span>|<span data-ttu-id="cf2fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf2fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf2fc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf2fc-127">Request body</span></span>
<span data-ttu-id="cf2fc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf2fc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf2fc-129">Response</span></span>
<span data-ttu-id="cf2fc-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf2fc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cf2fc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf2fc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf2fc-132">Request</span></span>
<span data-ttu-id="cf2fc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

### <a name="response"></a><span data-ttu-id="cf2fc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf2fc-134">Response</span></span>
<span data-ttu-id="cf2fc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf2fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





