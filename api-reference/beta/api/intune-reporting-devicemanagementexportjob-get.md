---
title: Get deviceManagementExportJob
description: Чтение свойств и связей объекта deviceManagementExportJob.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 92ae0a5a2703b8650463abf853bfc792f9206238
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443813"
---
# <a name="get-devicemanagementexportjob"></a><span data-ttu-id="43cf0-103">Get deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="43cf0-103">Get deviceManagementExportJob</span></span>

<span data-ttu-id="43cf0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43cf0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43cf0-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43cf0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43cf0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43cf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43cf0-107">Чтение свойств и связей [объекта deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)</span><span class="sxs-lookup"><span data-stu-id="43cf0-107">Read properties and relationships of the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43cf0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="43cf0-108">Prerequisites</span></span>
<span data-ttu-id="43cf0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43cf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43cf0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43cf0-111">Permission type</span></span>|<span data-ttu-id="43cf0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43cf0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43cf0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43cf0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43cf0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="43cf0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="43cf0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43cf0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43cf0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43cf0-116">Not supported.</span></span>|
|<span data-ttu-id="43cf0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="43cf0-117">Application</span></span>|<span data-ttu-id="43cf0-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="43cf0-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43cf0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43cf0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43cf0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="43cf0-120">Optional query parameters</span></span>
<span data-ttu-id="43cf0-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="43cf0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43cf0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43cf0-122">Request headers</span></span>
|<span data-ttu-id="43cf0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43cf0-123">Header</span></span>|<span data-ttu-id="43cf0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="43cf0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43cf0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="43cf0-125">Authorization</span></span>|<span data-ttu-id="43cf0-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43cf0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43cf0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="43cf0-127">Accept</span></span>|<span data-ttu-id="43cf0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="43cf0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43cf0-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="43cf0-129">Request body</span></span>
<span data-ttu-id="43cf0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43cf0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43cf0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="43cf0-131">Response</span></span>
<span data-ttu-id="43cf0-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="43cf0-132">If successful, this method returns a `200 OK` response code and [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43cf0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="43cf0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="43cf0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="43cf0-134">Request</span></span>
<span data-ttu-id="43cf0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43cf0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

### <a name="response"></a><span data-ttu-id="43cf0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="43cf0-136">Response</span></span>
<span data-ttu-id="43cf0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43cf0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




