---
title: Get windowsUpdateCatalogItem
description: Чтение свойств и связей объекта WindowsUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d2e3bbf0ec6ce092ea133862732c45421037d0b6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156102"
---
# <a name="get-windowsupdatecatalogitem"></a><span data-ttu-id="7d902-103">Get windowsUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="7d902-103">Get windowsUpdateCatalogItem</span></span>

<span data-ttu-id="7d902-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d902-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d902-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d902-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d902-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d902-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d902-107">Чтение свойств и связей [объекта WindowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="7d902-107">Read properties and relationships of the [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d902-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7d902-108">Prerequisites</span></span>
<span data-ttu-id="7d902-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d902-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d902-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d902-111">Permission type</span></span>|<span data-ttu-id="7d902-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d902-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d902-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d902-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d902-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d902-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d902-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d902-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d902-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d902-116">Not supported.</span></span>|
|<span data-ttu-id="7d902-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7d902-117">Application</span></span>|<span data-ttu-id="7d902-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d902-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d902-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d902-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d902-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7d902-120">Optional query parameters</span></span>
<span data-ttu-id="7d902-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7d902-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d902-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d902-122">Request headers</span></span>
|<span data-ttu-id="7d902-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d902-123">Header</span></span>|<span data-ttu-id="7d902-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7d902-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d902-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d902-125">Authorization</span></span>|<span data-ttu-id="7d902-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d902-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d902-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7d902-127">Accept</span></span>|<span data-ttu-id="7d902-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7d902-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d902-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d902-129">Request body</span></span>
<span data-ttu-id="7d902-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d902-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d902-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d902-131">Response</span></span>
<span data-ttu-id="7d902-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект WindowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7d902-132">If successful, this method returns a `200 OK` response code and [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d902-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7d902-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d902-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d902-134">Request</span></span>
<span data-ttu-id="7d902-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d902-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

### <a name="response"></a><span data-ttu-id="7d902-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d902-136">Response</span></span>
<span data-ttu-id="7d902-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d902-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 241

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdateCatalogItem",
    "id": "e887145d-145d-e887-5d14-87e85d1487e8",
    "displayName": "Display Name value",
    "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00"
  }
}
```




