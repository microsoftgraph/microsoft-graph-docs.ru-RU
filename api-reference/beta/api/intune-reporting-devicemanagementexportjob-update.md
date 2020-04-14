---
title: Обновление Девицеманажементекспортжоб
description: Обновление свойств объекта Девицеманажементекспортжоб.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2609727b57fb4242169d135e3eb7a205db10ef03
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454405"
---
# <a name="update-devicemanagementexportjob"></a><span data-ttu-id="c50b7-103">Обновление Девицеманажементекспортжоб</span><span class="sxs-lookup"><span data-stu-id="c50b7-103">Update deviceManagementExportJob</span></span>

<span data-ttu-id="c50b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c50b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c50b7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c50b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c50b7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c50b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c50b7-107">Обновление свойств объекта [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) .</span><span class="sxs-lookup"><span data-stu-id="c50b7-107">Update the properties of a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c50b7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c50b7-108">Prerequisites</span></span>
<span data-ttu-id="c50b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c50b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c50b7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c50b7-111">Permission type</span></span>|<span data-ttu-id="c50b7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c50b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c50b7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c50b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c50b7-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c50b7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c50b7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c50b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c50b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c50b7-116">Not supported.</span></span>|
|<span data-ttu-id="c50b7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c50b7-117">Application</span></span>|<span data-ttu-id="c50b7-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c50b7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c50b7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c50b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## <a name="request-headers"></a><span data-ttu-id="c50b7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c50b7-120">Request headers</span></span>
|<span data-ttu-id="c50b7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c50b7-121">Header</span></span>|<span data-ttu-id="c50b7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c50b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c50b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c50b7-123">Authorization</span></span>|<span data-ttu-id="c50b7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c50b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c50b7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c50b7-125">Accept</span></span>|<span data-ttu-id="c50b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c50b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c50b7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c50b7-127">Request body</span></span>
<span data-ttu-id="c50b7-128">В тексте запроса добавьте представление объекта [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c50b7-128">In the request body, supply a JSON representation for the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

<span data-ttu-id="c50b7-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md).</span><span class="sxs-lookup"><span data-stu-id="c50b7-129">The following table shows the properties that are required when you create the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span></span>

|<span data-ttu-id="c50b7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c50b7-130">Property</span></span>|<span data-ttu-id="c50b7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c50b7-131">Type</span></span>|<span data-ttu-id="c50b7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c50b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c50b7-133">id</span><span class="sxs-lookup"><span data-stu-id="c50b7-133">id</span></span>|<span data-ttu-id="c50b7-134">String</span><span class="sxs-lookup"><span data-stu-id="c50b7-134">String</span></span>|<span data-ttu-id="c50b7-135">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="c50b7-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="c50b7-136">репортнаме</span><span class="sxs-lookup"><span data-stu-id="c50b7-136">reportName</span></span>|<span data-ttu-id="c50b7-137">String</span><span class="sxs-lookup"><span data-stu-id="c50b7-137">String</span></span>|<span data-ttu-id="c50b7-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="c50b7-138">Name of the report</span></span>|
|<span data-ttu-id="c50b7-139">filter</span><span class="sxs-lookup"><span data-stu-id="c50b7-139">filter</span></span>|<span data-ttu-id="c50b7-140">String</span><span class="sxs-lookup"><span data-stu-id="c50b7-140">String</span></span>|<span data-ttu-id="c50b7-141">Фильтры, примененные к отчету</span><span class="sxs-lookup"><span data-stu-id="c50b7-141">Filters applied on the report</span></span>|
|<span data-ttu-id="c50b7-142">select</span><span class="sxs-lookup"><span data-stu-id="c50b7-142">select</span></span>|<span data-ttu-id="c50b7-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c50b7-143">String collection</span></span>|<span data-ttu-id="c50b7-144">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="c50b7-144">Columns selected from the report</span></span>|
|<span data-ttu-id="c50b7-145">format</span><span class="sxs-lookup"><span data-stu-id="c50b7-145">format</span></span>|[<span data-ttu-id="c50b7-146">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="c50b7-146">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="c50b7-147">Формат экспортированного отчета.</span><span class="sxs-lookup"><span data-stu-id="c50b7-147">Format of the exported report.</span></span> <span data-ttu-id="c50b7-148">Возможные значения: `csv`, `pdf`.</span><span class="sxs-lookup"><span data-stu-id="c50b7-148">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="c50b7-149">снапшотид</span><span class="sxs-lookup"><span data-stu-id="c50b7-149">snapshotId</span></span>|<span data-ttu-id="c50b7-150">String</span><span class="sxs-lookup"><span data-stu-id="c50b7-150">String</span></span>|<span data-ttu-id="c50b7-151">Моментальный снимок является идентифицируемым подмножеством набора данных, представленным Репортнаме.</span><span class="sxs-lookup"><span data-stu-id="c50b7-151">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="c50b7-152">Здесь можно использовать идентификатор sessionId или Качедрепортконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="c50b7-152">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="c50b7-153">Если указан идентификатор sessionId, фильтрация, выбор и OrderBy применяются к данным, представленным в sessionId.</span><span class="sxs-lookup"><span data-stu-id="c50b7-153">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="c50b7-154">Filter, SELECT и OrderBy не могут указываться вместе с идентификатором Качедрепортконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="c50b7-154">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="c50b7-155">status</span><span class="sxs-lookup"><span data-stu-id="c50b7-155">status</span></span>|[<span data-ttu-id="c50b7-156">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="c50b7-156">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="c50b7-157">Состояние задания экспорта.</span><span class="sxs-lookup"><span data-stu-id="c50b7-157">Status of the export job.</span></span> <span data-ttu-id="c50b7-158">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="c50b7-158">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="c50b7-159">url</span><span class="sxs-lookup"><span data-stu-id="c50b7-159">url</span></span>|<span data-ttu-id="c50b7-160">String</span><span class="sxs-lookup"><span data-stu-id="c50b7-160">String</span></span>|<span data-ttu-id="c50b7-161">Временное расположение экспортируемого отчета</span><span class="sxs-lookup"><span data-stu-id="c50b7-161">Temporary location of the exported report</span></span>|
|<span data-ttu-id="c50b7-162">рекуестдатетиме</span><span class="sxs-lookup"><span data-stu-id="c50b7-162">requestDateTime</span></span>|<span data-ttu-id="c50b7-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c50b7-163">DateTimeOffset</span></span>|<span data-ttu-id="c50b7-164">Время запроса экспорта отчета</span><span class="sxs-lookup"><span data-stu-id="c50b7-164">Time that the exported report was requested</span></span>|
|<span data-ttu-id="c50b7-165">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c50b7-165">expirationDateTime</span></span>|<span data-ttu-id="c50b7-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c50b7-166">DateTimeOffset</span></span>|<span data-ttu-id="c50b7-167">Время истечения срока действия экспортированного отчета</span><span class="sxs-lookup"><span data-stu-id="c50b7-167">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="c50b7-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="c50b7-168">Response</span></span>
<span data-ttu-id="c50b7-169">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c50b7-169">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c50b7-170">Пример</span><span class="sxs-lookup"><span data-stu-id="c50b7-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="c50b7-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="c50b7-171">Request</span></span>
<span data-ttu-id="c50b7-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c50b7-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
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
```

### <a name="response"></a><span data-ttu-id="c50b7-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="c50b7-173">Response</span></span>
<span data-ttu-id="c50b7-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c50b7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 453

{
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
```



