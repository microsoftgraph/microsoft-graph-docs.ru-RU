---
title: Создание Девицеманажементекспортжоб
description: Создание нового объекта Девицеманажементекспортжоб.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dc8ab860820f3f8c8df6b374924bb0bd07e087ee
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698276"
---
# <a name="create-devicemanagementexportjob"></a><span data-ttu-id="69ee7-103">Создание Девицеманажементекспортжоб</span><span class="sxs-lookup"><span data-stu-id="69ee7-103">Create deviceManagementExportJob</span></span>

<span data-ttu-id="69ee7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69ee7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69ee7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69ee7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69ee7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69ee7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69ee7-107">Создание нового объекта [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) .</span><span class="sxs-lookup"><span data-stu-id="69ee7-107">Create a new [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69ee7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="69ee7-108">Prerequisites</span></span>
<span data-ttu-id="69ee7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69ee7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69ee7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69ee7-111">Permission type</span></span>|<span data-ttu-id="69ee7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69ee7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69ee7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69ee7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69ee7-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="69ee7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="69ee7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69ee7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69ee7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69ee7-116">Not supported.</span></span>|
|<span data-ttu-id="69ee7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69ee7-117">Application</span></span>|<span data-ttu-id="69ee7-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="69ee7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69ee7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69ee7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/exportJobs
```

## <a name="request-headers"></a><span data-ttu-id="69ee7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="69ee7-120">Request headers</span></span>
|<span data-ttu-id="69ee7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69ee7-121">Header</span></span>|<span data-ttu-id="69ee7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="69ee7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69ee7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69ee7-123">Authorization</span></span>|<span data-ttu-id="69ee7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69ee7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69ee7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="69ee7-125">Accept</span></span>|<span data-ttu-id="69ee7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69ee7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69ee7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69ee7-127">Request body</span></span>
<span data-ttu-id="69ee7-128">В тексте запроса добавьте представление объекта Девицеманажементекспортжоб в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69ee7-128">In the request body, supply a JSON representation for the deviceManagementExportJob object.</span></span>

<span data-ttu-id="69ee7-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементекспортжоб.</span><span class="sxs-lookup"><span data-stu-id="69ee7-129">The following table shows the properties that are required when you create the deviceManagementExportJob.</span></span>

|<span data-ttu-id="69ee7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="69ee7-130">Property</span></span>|<span data-ttu-id="69ee7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="69ee7-131">Type</span></span>|<span data-ttu-id="69ee7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="69ee7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69ee7-133">id</span><span class="sxs-lookup"><span data-stu-id="69ee7-133">id</span></span>|<span data-ttu-id="69ee7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="69ee7-134">String</span></span>|<span data-ttu-id="69ee7-135">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="69ee7-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="69ee7-136">репортнаме</span><span class="sxs-lookup"><span data-stu-id="69ee7-136">reportName</span></span>|<span data-ttu-id="69ee7-137">Строка</span><span class="sxs-lookup"><span data-stu-id="69ee7-137">String</span></span>|<span data-ttu-id="69ee7-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="69ee7-138">Name of the report</span></span>|
|<span data-ttu-id="69ee7-139">filter</span><span class="sxs-lookup"><span data-stu-id="69ee7-139">filter</span></span>|<span data-ttu-id="69ee7-140">Строка</span><span class="sxs-lookup"><span data-stu-id="69ee7-140">String</span></span>|<span data-ttu-id="69ee7-141">Фильтры, примененные к отчету</span><span class="sxs-lookup"><span data-stu-id="69ee7-141">Filters applied on the report</span></span>|
|<span data-ttu-id="69ee7-142">select</span><span class="sxs-lookup"><span data-stu-id="69ee7-142">select</span></span>|<span data-ttu-id="69ee7-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="69ee7-143">String collection</span></span>|<span data-ttu-id="69ee7-144">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="69ee7-144">Columns selected from the report</span></span>|
|<span data-ttu-id="69ee7-145">format</span><span class="sxs-lookup"><span data-stu-id="69ee7-145">format</span></span>|[<span data-ttu-id="69ee7-146">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="69ee7-146">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="69ee7-147">Формат экспортированного отчета.</span><span class="sxs-lookup"><span data-stu-id="69ee7-147">Format of the exported report.</span></span> <span data-ttu-id="69ee7-148">Возможные значения: `csv`, `pdf`.</span><span class="sxs-lookup"><span data-stu-id="69ee7-148">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="69ee7-149">снапшотид</span><span class="sxs-lookup"><span data-stu-id="69ee7-149">snapshotId</span></span>|<span data-ttu-id="69ee7-150">Строка</span><span class="sxs-lookup"><span data-stu-id="69ee7-150">String</span></span>|<span data-ttu-id="69ee7-151">Моментальный снимок является идентифицируемым подмножеством набора данных, представленным Репортнаме.</span><span class="sxs-lookup"><span data-stu-id="69ee7-151">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="69ee7-152">Здесь можно использовать идентификатор sessionId или Качедрепортконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="69ee7-152">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="69ee7-153">Если указан идентификатор sessionId, фильтрация, выбор и OrderBy применяются к данным, представленным в sessionId.</span><span class="sxs-lookup"><span data-stu-id="69ee7-153">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="69ee7-154">Filter, SELECT и OrderBy не могут указываться вместе с идентификатором Качедрепортконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="69ee7-154">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="69ee7-155">status</span><span class="sxs-lookup"><span data-stu-id="69ee7-155">status</span></span>|[<span data-ttu-id="69ee7-156">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="69ee7-156">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="69ee7-157">Состояние задания экспорта.</span><span class="sxs-lookup"><span data-stu-id="69ee7-157">Status of the export job.</span></span> <span data-ttu-id="69ee7-158">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="69ee7-158">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="69ee7-159">url</span><span class="sxs-lookup"><span data-stu-id="69ee7-159">url</span></span>|<span data-ttu-id="69ee7-160">String</span><span class="sxs-lookup"><span data-stu-id="69ee7-160">String</span></span>|<span data-ttu-id="69ee7-161">Временное расположение экспортируемого отчета</span><span class="sxs-lookup"><span data-stu-id="69ee7-161">Temporary location of the exported report</span></span>|
|<span data-ttu-id="69ee7-162">рекуестдатетиме</span><span class="sxs-lookup"><span data-stu-id="69ee7-162">requestDateTime</span></span>|<span data-ttu-id="69ee7-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69ee7-163">DateTimeOffset</span></span>|<span data-ttu-id="69ee7-164">Время запроса экспорта отчета</span><span class="sxs-lookup"><span data-stu-id="69ee7-164">Time that the exported report was requested</span></span>|
|<span data-ttu-id="69ee7-165">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="69ee7-165">expirationDateTime</span></span>|<span data-ttu-id="69ee7-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69ee7-166">DateTimeOffset</span></span>|<span data-ttu-id="69ee7-167">Время истечения срока действия экспортированного отчета</span><span class="sxs-lookup"><span data-stu-id="69ee7-167">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="69ee7-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="69ee7-168">Response</span></span>
<span data-ttu-id="69ee7-169">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементекспортжоб](../resources/intune-reporting-devicemanagementexportjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69ee7-169">If successful, this method returns a `201 Created` response code and a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69ee7-170">Пример</span><span class="sxs-lookup"><span data-stu-id="69ee7-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="69ee7-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="69ee7-171">Request</span></span>
<span data-ttu-id="69ee7-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69ee7-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs
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

### <a name="response"></a><span data-ttu-id="69ee7-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="69ee7-173">Response</span></span>
<span data-ttu-id="69ee7-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69ee7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





