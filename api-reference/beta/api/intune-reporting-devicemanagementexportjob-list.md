---
title: Список Девицеманажементекспортжобс
description: Список свойств и связей объектов Девицеманажементекспортжоб.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e738277d9a7647132400196afea9c34a7c51805e
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538310"
---
# <a name="list-devicemanagementexportjobs"></a><span data-ttu-id="d771c-103">Список Девицеманажементекспортжобс</span><span class="sxs-lookup"><span data-stu-id="d771c-103">List deviceManagementExportJobs</span></span>

> <span data-ttu-id="d771c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d771c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d771c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d771c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d771c-106">Список свойств и связей объектов [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) .</span><span class="sxs-lookup"><span data-stu-id="d771c-106">List properties and relationships of the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d771c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d771c-107">Prerequisites</span></span>
<span data-ttu-id="d771c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d771c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d771c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d771c-110">Permission type</span></span>|<span data-ttu-id="d771c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d771c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d771c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d771c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d771c-113">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="d771c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d771c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d771c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d771c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d771c-115">Not supported.</span></span>|
|<span data-ttu-id="d771c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d771c-116">Application</span></span>|<span data-ttu-id="d771c-117">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="d771c-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d771c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d771c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/exportJobs
```

## <a name="request-headers"></a><span data-ttu-id="d771c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d771c-119">Request headers</span></span>
|<span data-ttu-id="d771c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d771c-120">Header</span></span>|<span data-ttu-id="d771c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d771c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d771c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d771c-122">Authorization</span></span>|<span data-ttu-id="d771c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d771c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d771c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d771c-124">Accept</span></span>|<span data-ttu-id="d771c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d771c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d771c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d771c-126">Request body</span></span>
<span data-ttu-id="d771c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d771c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d771c-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d771c-128">Response</span></span>
<span data-ttu-id="d771c-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d771c-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d771c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d771c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d771c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d771c-131">Request</span></span>
<span data-ttu-id="d771c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d771c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs
```

### <a name="response"></a><span data-ttu-id="d771c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d771c-133">Response</span></span>
<span data-ttu-id="d771c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d771c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 594

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementExportJob",
      "id": "9ddfb995-b995-9ddf-95b9-df9d95b9df9d",
      "reportName": "Report Name value",
      "filter": "Filter value",
      "select": [
        "Select value"
      ],
      "orderBy": [
        "Order By value"
      ],
      "format": "pdf",
      "snapshotId": "Snapshot Id value",
      "status": "notStarted",
      "url": "Url value",
      "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
    }
  ]
}
```






