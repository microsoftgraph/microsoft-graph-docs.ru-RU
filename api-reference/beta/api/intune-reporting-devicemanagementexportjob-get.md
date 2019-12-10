---
title: Получение Девицеманажементекспортжоб
description: Чтение свойств и связей объекта Девицеманажементекспортжоб.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b9a887a141b02bbff7d29453627e66b66e322dad
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940336"
---
# <a name="get-devicemanagementexportjob"></a><span data-ttu-id="404df-103">Получение Девицеманажементекспортжоб</span><span class="sxs-lookup"><span data-stu-id="404df-103">Get deviceManagementExportJob</span></span>

> <span data-ttu-id="404df-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="404df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="404df-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="404df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="404df-106">Чтение свойств и связей объекта [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) .</span><span class="sxs-lookup"><span data-stu-id="404df-106">Read properties and relationships of the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="404df-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="404df-107">Prerequisites</span></span>
<span data-ttu-id="404df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="404df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="404df-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="404df-110">Permission type</span></span>|<span data-ttu-id="404df-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="404df-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="404df-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="404df-112">Delegated (work or school account)</span></span>|<span data-ttu-id="404df-113">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="404df-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="404df-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="404df-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="404df-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="404df-115">Not supported.</span></span>|
|<span data-ttu-id="404df-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="404df-116">Application</span></span>|<span data-ttu-id="404df-117">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="404df-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="404df-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="404df-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="404df-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="404df-119">Optional query parameters</span></span>
<span data-ttu-id="404df-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="404df-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="404df-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="404df-121">Request headers</span></span>
|<span data-ttu-id="404df-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="404df-122">Header</span></span>|<span data-ttu-id="404df-123">Значение</span><span class="sxs-lookup"><span data-stu-id="404df-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="404df-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="404df-124">Authorization</span></span>|<span data-ttu-id="404df-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="404df-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="404df-126">Accept</span><span class="sxs-lookup"><span data-stu-id="404df-126">Accept</span></span>|<span data-ttu-id="404df-127">application/json</span><span class="sxs-lookup"><span data-stu-id="404df-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="404df-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="404df-128">Request body</span></span>
<span data-ttu-id="404df-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="404df-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="404df-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="404df-130">Response</span></span>
<span data-ttu-id="404df-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="404df-131">If successful, this method returns a `200 OK` response code and [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="404df-132">Пример</span><span class="sxs-lookup"><span data-stu-id="404df-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="404df-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="404df-133">Request</span></span>
<span data-ttu-id="404df-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="404df-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

### <a name="response"></a><span data-ttu-id="404df-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="404df-135">Response</span></span>
<span data-ttu-id="404df-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="404df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 498

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
    "status": "notStarted",
    "url": "Url value",
    "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
  }
}
```





