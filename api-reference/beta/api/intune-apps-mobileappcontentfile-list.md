---
title: Перечисление объектов mobileAppContentFile
description: Список свойств и связей объектов mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 48cc498a7b923cb844e0fe01447a1dafe2e7eca3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695938"
---
# <a name="list-mobileappcontentfiles"></a><span data-ttu-id="dd652-103">Перечисление объектов mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="dd652-103">List mobileAppContentFiles</span></span>

<span data-ttu-id="dd652-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd652-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd652-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd652-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd652-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd652-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd652-107">Список свойств и связей объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="dd652-107">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd652-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dd652-108">Prerequisites</span></span>
<span data-ttu-id="dd652-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd652-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd652-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd652-111">Permission type</span></span>|<span data-ttu-id="dd652-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd652-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd652-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd652-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd652-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd652-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dd652-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd652-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd652-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd652-116">Not supported.</span></span>|
|<span data-ttu-id="dd652-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd652-117">Application</span></span>|<span data-ttu-id="dd652-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd652-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd652-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd652-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="dd652-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dd652-120">Request headers</span></span>
|<span data-ttu-id="dd652-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd652-121">Header</span></span>|<span data-ttu-id="dd652-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dd652-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd652-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd652-123">Authorization</span></span>|<span data-ttu-id="dd652-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd652-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd652-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dd652-125">Accept</span></span>|<span data-ttu-id="dd652-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd652-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd652-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd652-127">Request body</span></span>
<span data-ttu-id="dd652-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd652-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd652-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd652-129">Response</span></span>
<span data-ttu-id="dd652-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd652-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd652-131">Пример</span><span class="sxs-lookup"><span data-stu-id="dd652-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd652-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd652-132">Request</span></span>
<span data-ttu-id="dd652-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd652-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

### <a name="response"></a><span data-ttu-id="dd652-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd652-134">Response</span></span>
<span data-ttu-id="dd652-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd652-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





