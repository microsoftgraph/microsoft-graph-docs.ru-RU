---
title: Обновление Девицеманажементекспортжоб
description: Обновление свойств объекта Девицеманажементекспортжоб.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5617d7896b90919d902e9ad72129c2e5f738c1c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940322"
---
# <a name="update-devicemanagementexportjob"></a><span data-ttu-id="988e0-103">Обновление Девицеманажементекспортжоб</span><span class="sxs-lookup"><span data-stu-id="988e0-103">Update deviceManagementExportJob</span></span>

> <span data-ttu-id="988e0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="988e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="988e0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="988e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="988e0-106">Обновление свойств объекта [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) .</span><span class="sxs-lookup"><span data-stu-id="988e0-106">Update the properties of a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="988e0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="988e0-107">Prerequisites</span></span>
<span data-ttu-id="988e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="988e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="988e0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="988e0-110">Permission type</span></span>|<span data-ttu-id="988e0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="988e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="988e0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="988e0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="988e0-113">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="988e0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="988e0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="988e0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="988e0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="988e0-115">Not supported.</span></span>|
|<span data-ttu-id="988e0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="988e0-116">Application</span></span>|<span data-ttu-id="988e0-117">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="988e0-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="988e0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="988e0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## <a name="request-headers"></a><span data-ttu-id="988e0-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="988e0-119">Request headers</span></span>
|<span data-ttu-id="988e0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="988e0-120">Header</span></span>|<span data-ttu-id="988e0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="988e0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="988e0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="988e0-122">Authorization</span></span>|<span data-ttu-id="988e0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="988e0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="988e0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="988e0-124">Accept</span></span>|<span data-ttu-id="988e0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="988e0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="988e0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="988e0-126">Request body</span></span>
<span data-ttu-id="988e0-127">В тексте запроса добавьте представление объекта [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="988e0-127">In the request body, supply a JSON representation for the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

<span data-ttu-id="988e0-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md).</span><span class="sxs-lookup"><span data-stu-id="988e0-128">The following table shows the properties that are required when you create the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span></span>

|<span data-ttu-id="988e0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="988e0-129">Property</span></span>|<span data-ttu-id="988e0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="988e0-130">Type</span></span>|<span data-ttu-id="988e0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="988e0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="988e0-132">id</span><span class="sxs-lookup"><span data-stu-id="988e0-132">id</span></span>|<span data-ttu-id="988e0-133">Строка</span><span class="sxs-lookup"><span data-stu-id="988e0-133">String</span></span>|<span data-ttu-id="988e0-134">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="988e0-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="988e0-135">репортнаме</span><span class="sxs-lookup"><span data-stu-id="988e0-135">reportName</span></span>|<span data-ttu-id="988e0-136">Строка</span><span class="sxs-lookup"><span data-stu-id="988e0-136">String</span></span>|<span data-ttu-id="988e0-137">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="988e0-137">Name of the report</span></span>|
|<span data-ttu-id="988e0-138">filter</span><span class="sxs-lookup"><span data-stu-id="988e0-138">filter</span></span>|<span data-ttu-id="988e0-139">Строка</span><span class="sxs-lookup"><span data-stu-id="988e0-139">String</span></span>|<span data-ttu-id="988e0-140">Фильтры, примененные к отчету</span><span class="sxs-lookup"><span data-stu-id="988e0-140">Filters applied on the report</span></span>|
|<span data-ttu-id="988e0-141">select</span><span class="sxs-lookup"><span data-stu-id="988e0-141">select</span></span>|<span data-ttu-id="988e0-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="988e0-142">String collection</span></span>|<span data-ttu-id="988e0-143">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="988e0-143">Columns selected from the report</span></span>|
|<span data-ttu-id="988e0-144">format</span><span class="sxs-lookup"><span data-stu-id="988e0-144">format</span></span>|[<span data-ttu-id="988e0-145">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="988e0-145">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="988e0-146">Формат экспортированного отчета.</span><span class="sxs-lookup"><span data-stu-id="988e0-146">Format of the exported report.</span></span> <span data-ttu-id="988e0-147">Возможные значения: `csv`, `pdf`.</span><span class="sxs-lookup"><span data-stu-id="988e0-147">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="988e0-148">снапшотид</span><span class="sxs-lookup"><span data-stu-id="988e0-148">snapshotId</span></span>|<span data-ttu-id="988e0-149">Строка</span><span class="sxs-lookup"><span data-stu-id="988e0-149">String</span></span>|<span data-ttu-id="988e0-150">Моментальный снимок является идентифицируемым подмножеством набора данных, представленным Репортнаме.</span><span class="sxs-lookup"><span data-stu-id="988e0-150">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="988e0-151">Здесь можно использовать идентификатор sessionId или Качедрепортконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="988e0-151">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="988e0-152">Если указан идентификатор sessionId, фильтрация, выбор и OrderBy применяются к данным, представленным в sessionId.</span><span class="sxs-lookup"><span data-stu-id="988e0-152">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="988e0-153">Filter, SELECT и OrderBy не могут указываться вместе с идентификатором Качедрепортконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="988e0-153">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="988e0-154">status</span><span class="sxs-lookup"><span data-stu-id="988e0-154">status</span></span>|[<span data-ttu-id="988e0-155">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="988e0-155">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="988e0-156">Состояние задания экспорта.</span><span class="sxs-lookup"><span data-stu-id="988e0-156">Status of the export job.</span></span> <span data-ttu-id="988e0-157">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="988e0-157">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="988e0-158">url</span><span class="sxs-lookup"><span data-stu-id="988e0-158">url</span></span>|<span data-ttu-id="988e0-159">String</span><span class="sxs-lookup"><span data-stu-id="988e0-159">String</span></span>|<span data-ttu-id="988e0-160">Временное расположение экспортируемого отчета</span><span class="sxs-lookup"><span data-stu-id="988e0-160">Temporary location of the exported report</span></span>|
|<span data-ttu-id="988e0-161">рекуестдатетиме</span><span class="sxs-lookup"><span data-stu-id="988e0-161">requestDateTime</span></span>|<span data-ttu-id="988e0-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="988e0-162">DateTimeOffset</span></span>|<span data-ttu-id="988e0-163">Время запроса экспорта отчета</span><span class="sxs-lookup"><span data-stu-id="988e0-163">Time that the exported report was requested</span></span>|
|<span data-ttu-id="988e0-164">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="988e0-164">expirationDateTime</span></span>|<span data-ttu-id="988e0-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="988e0-165">DateTimeOffset</span></span>|<span data-ttu-id="988e0-166">Время истечения срока действия экспортированного отчета</span><span class="sxs-lookup"><span data-stu-id="988e0-166">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="988e0-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="988e0-167">Response</span></span>
<span data-ttu-id="988e0-168">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="988e0-168">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="988e0-169">Пример</span><span class="sxs-lookup"><span data-stu-id="988e0-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="988e0-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="988e0-170">Request</span></span>
<span data-ttu-id="988e0-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="988e0-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="988e0-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="988e0-172">Response</span></span>
<span data-ttu-id="988e0-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="988e0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





