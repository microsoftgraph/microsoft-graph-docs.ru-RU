---
title: Список мобильных устройствAppRelationships
description: Список свойств и связей объектов mobileAppRelationship.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 463b8218ba913ffb1af6c1cd718340f12c1c32e1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139608"
---
# <a name="list-mobileapprelationships"></a><span data-ttu-id="21a10-103">Список мобильных устройствAppRelationships</span><span class="sxs-lookup"><span data-stu-id="21a10-103">List mobileAppRelationships</span></span>

<span data-ttu-id="21a10-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21a10-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21a10-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21a10-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21a10-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21a10-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21a10-107">Список свойств и связей объектов [mobileAppRelationship.](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="21a10-107">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21a10-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="21a10-108">Prerequisites</span></span>
<span data-ttu-id="21a10-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21a10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21a10-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21a10-111">Permission type</span></span>|<span data-ttu-id="21a10-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21a10-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21a10-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21a10-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21a10-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21a10-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="21a10-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21a10-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21a10-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21a10-116">Not supported.</span></span>|
|<span data-ttu-id="21a10-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="21a10-117">Application</span></span>|<span data-ttu-id="21a10-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21a10-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21a10-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21a10-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="21a10-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="21a10-120">Request headers</span></span>
|<span data-ttu-id="21a10-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21a10-121">Header</span></span>|<span data-ttu-id="21a10-122">Значение</span><span class="sxs-lookup"><span data-stu-id="21a10-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21a10-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21a10-123">Authorization</span></span>|<span data-ttu-id="21a10-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21a10-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21a10-125">Accept</span><span class="sxs-lookup"><span data-stu-id="21a10-125">Accept</span></span>|<span data-ttu-id="21a10-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21a10-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21a10-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21a10-127">Request body</span></span>
<span data-ttu-id="21a10-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21a10-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21a10-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="21a10-129">Response</span></span>
<span data-ttu-id="21a10-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="21a10-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21a10-131">Пример</span><span class="sxs-lookup"><span data-stu-id="21a10-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="21a10-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="21a10-132">Request</span></span>
<span data-ttu-id="21a10-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21a10-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

### <a name="response"></a><span data-ttu-id="21a10-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="21a10-134">Response</span></span>
<span data-ttu-id="21a10-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21a10-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppRelationship",
      "id": "7b4b5b14-5b14-7b4b-145b-4b7b145b4b7b",
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value",
      "targetDisplayVersion": "Target Display Version value",
      "targetPublisher": "Target Publisher value",
      "targetType": "parent"
    }
  ]
}
```




