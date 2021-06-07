---
title: Get deviceManagementExportJob
description: Чтение свойств и связей объекта deviceManagementExportJob.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 21b54572b501197e31c3c460ee9d1377b191451e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755473"
---
# <a name="get-devicemanagementexportjob"></a><span data-ttu-id="36f5a-103">Get deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="36f5a-103">Get deviceManagementExportJob</span></span>

<span data-ttu-id="36f5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36f5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36f5a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36f5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36f5a-106">Чтение свойств и связей [объекта deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)</span><span class="sxs-lookup"><span data-stu-id="36f5a-106">Read properties and relationships of the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36f5a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="36f5a-107">Prerequisites</span></span>
<span data-ttu-id="36f5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36f5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36f5a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36f5a-110">Permission type</span></span>|<span data-ttu-id="36f5a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36f5a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36f5a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36f5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36f5a-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36f5a-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="36f5a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36f5a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36f5a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36f5a-115">Not supported.</span></span>|
|<span data-ttu-id="36f5a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="36f5a-116">Application</span></span>|<span data-ttu-id="36f5a-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36f5a-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36f5a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36f5a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36f5a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="36f5a-119">Optional query parameters</span></span>
<span data-ttu-id="36f5a-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="36f5a-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36f5a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36f5a-121">Request headers</span></span>
|<span data-ttu-id="36f5a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36f5a-122">Header</span></span>|<span data-ttu-id="36f5a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="36f5a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36f5a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="36f5a-124">Authorization</span></span>|<span data-ttu-id="36f5a-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36f5a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36f5a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="36f5a-126">Accept</span></span>|<span data-ttu-id="36f5a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="36f5a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36f5a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36f5a-128">Request body</span></span>
<span data-ttu-id="36f5a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36f5a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36f5a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="36f5a-130">Response</span></span>
<span data-ttu-id="36f5a-131">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="36f5a-131">If successful, this method returns a `200 OK` response code and [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36f5a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="36f5a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="36f5a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="36f5a-133">Request</span></span>
<span data-ttu-id="36f5a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36f5a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

### <a name="response"></a><span data-ttu-id="36f5a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="36f5a-135">Response</span></span>
<span data-ttu-id="36f5a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36f5a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 551

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementExportJob",
    "id": "9ddfb995-b995-9ddf-95b9-df9d95b9df9d",
    "reportName": "Report Name value",
    "filter": "Filter value",
    "select": [
      "Select value"
    ],
    "format": "pdf",
    "snapshotId": "Snapshot Id value",
    "localizationType": "replaceLocalizableValues",
    "status": "notStarted",
    "url": "Url value",
    "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
  }
}
```




