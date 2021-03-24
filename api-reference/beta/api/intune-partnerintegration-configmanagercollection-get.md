---
title: Get configManagerCollection
description: Чтение свойств и связей объекта configManagerCollection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6c61668935c8db5d084078399f8cfddcaef1cce8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145266"
---
# <a name="get-configmanagercollection"></a><span data-ttu-id="d8aaf-103">Get configManagerCollection</span><span class="sxs-lookup"><span data-stu-id="d8aaf-103">Get configManagerCollection</span></span>

<span data-ttu-id="d8aaf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8aaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8aaf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8aaf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8aaf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8aaf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8aaf-107">Чтение свойств и связей объекта [configManagerCollection.](../resources/intune-partnerintegration-configmanagercollection.md)</span><span class="sxs-lookup"><span data-stu-id="d8aaf-107">Read properties and relationships of the [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8aaf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d8aaf-108">Prerequisites</span></span>
<span data-ttu-id="d8aaf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8aaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8aaf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8aaf-111">Permission type</span></span>|<span data-ttu-id="d8aaf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8aaf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8aaf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8aaf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8aaf-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8aaf-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d8aaf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8aaf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8aaf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8aaf-116">Not supported.</span></span>|
|<span data-ttu-id="d8aaf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d8aaf-117">Application</span></span>|<span data-ttu-id="d8aaf-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8aaf-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8aaf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8aaf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configManagerCollections/{configManagerCollectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d8aaf-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d8aaf-120">Optional query parameters</span></span>
<span data-ttu-id="d8aaf-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d8aaf-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8aaf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8aaf-122">Request headers</span></span>
|<span data-ttu-id="d8aaf-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8aaf-123">Header</span></span>|<span data-ttu-id="d8aaf-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d8aaf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8aaf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8aaf-125">Authorization</span></span>|<span data-ttu-id="d8aaf-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8aaf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8aaf-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d8aaf-127">Accept</span></span>|<span data-ttu-id="d8aaf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d8aaf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8aaf-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8aaf-129">Request body</span></span>
<span data-ttu-id="d8aaf-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8aaf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8aaf-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8aaf-131">Response</span></span>
<span data-ttu-id="d8aaf-132">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d8aaf-132">If successful, this method returns a `200 OK` response code and [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8aaf-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d8aaf-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8aaf-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8aaf-134">Request</span></span>
<span data-ttu-id="d8aaf-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8aaf-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configManagerCollections/{configManagerCollectionId}
```

### <a name="response"></a><span data-ttu-id="d8aaf-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8aaf-136">Response</span></span>
<span data-ttu-id="d8aaf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8aaf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 470

{
  "value": {
    "@odata.type": "#microsoft.graph.configManagerCollection",
    "id": "5f9d1d76-1d76-5f9d-761d-9d5f761d9d5f",
    "displayName": "Display Name value",
    "collectionIdentifier": "Collection Identifier value",
    "hierarchyName": "Hierarchy Name value",
    "hierarchyIdentifier": "Hierarchy Identifier value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```




