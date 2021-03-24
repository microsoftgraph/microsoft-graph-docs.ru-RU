---
title: Список configManagerCollections
description: Список свойств и связей объектов configManagerCollection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 31f3ece6b40e2dc420b39627abca20a3c5b9edae
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125438"
---
# <a name="list-configmanagercollections"></a><span data-ttu-id="bef33-103">Список configManagerCollections</span><span class="sxs-lookup"><span data-stu-id="bef33-103">List configManagerCollections</span></span>

<span data-ttu-id="bef33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bef33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bef33-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bef33-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bef33-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bef33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bef33-107">Список свойств и связей объектов [configManagerCollection.](../resources/intune-partnerintegration-configmanagercollection.md)</span><span class="sxs-lookup"><span data-stu-id="bef33-107">List properties and relationships of the [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bef33-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bef33-108">Prerequisites</span></span>
<span data-ttu-id="bef33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bef33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bef33-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bef33-111">Permission type</span></span>|<span data-ttu-id="bef33-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bef33-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bef33-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bef33-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bef33-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bef33-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bef33-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bef33-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bef33-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bef33-116">Not supported.</span></span>|
|<span data-ttu-id="bef33-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bef33-117">Application</span></span>|<span data-ttu-id="bef33-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bef33-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bef33-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bef33-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configManagerCollections
```

## <a name="request-headers"></a><span data-ttu-id="bef33-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bef33-120">Request headers</span></span>
|<span data-ttu-id="bef33-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bef33-121">Header</span></span>|<span data-ttu-id="bef33-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bef33-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bef33-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bef33-123">Authorization</span></span>|<span data-ttu-id="bef33-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bef33-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bef33-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bef33-125">Accept</span></span>|<span data-ttu-id="bef33-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bef33-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bef33-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bef33-127">Request body</span></span>
<span data-ttu-id="bef33-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bef33-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bef33-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bef33-129">Response</span></span>
<span data-ttu-id="bef33-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bef33-130">If successful, this method returns a `200 OK` response code and a collection of [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bef33-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bef33-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bef33-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bef33-132">Request</span></span>
<span data-ttu-id="bef33-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bef33-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configManagerCollections
```

### <a name="response"></a><span data-ttu-id="bef33-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bef33-134">Response</span></span>
<span data-ttu-id="bef33-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bef33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 500

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.configManagerCollection",
      "id": "5f9d1d76-1d76-5f9d-761d-9d5f761d9d5f",
      "displayName": "Display Name value",
      "collectionIdentifier": "Collection Identifier value",
      "hierarchyName": "Hierarchy Name value",
      "hierarchyIdentifier": "Hierarchy Identifier value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




